---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objekte von einer Umgebung in eine andere verschieben
description: Die Funktion zur Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Die Möglichkeit zum Verschieben von Transaktionsobjekten wird nicht unterstützt (mit eingeschränkten Ausnahmen).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '2095'
ht-degree: 2%

---

# Verschieben von Objekten zwischen [!DNL Workfront]-Umgebungen mithilfe der [!DNL Workfront] Umgebungsförderungs-API

Mit der Umgebungsförderungsfunktion können Sie konfigurationsbezogene Objekte von einer Umgebung in eine andere verschieben. Sie können diese Objekte mithilfe der Workfront-API verschieben, wie in diesem Artikel beschrieben.

Anweisungen zum Verschieben von Objekten zwischen Umgebungen mithilfe der Workfront-Anwendung finden Sie unter:

* [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime oder Ultimate (nur neue Pläne)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenses</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationen auf Zugriffsebene
   </td>
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Der Endpunkt &quot;Promotion Package erstellen&quot;setzt voraus, dass Sie die Quellumgebung bereits konfiguriert haben. Dieser API-Aufruf erfordert das manuelle Erstellen einer Objektzuordnung von [!DNL Workfront] objCodes und Objekt-GUIDs. Die spezifische Struktur dieser Karte wird nachfolgend beschrieben.

## Unterstützte Objekte für die Umgebungsförderung

Die Funktion zur Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Die Möglichkeit zum Verschieben von Transaktionsobjekten wird nicht unterstützt (mit eingeschränkten Ausnahmen).

Eine Liste der förderfähigen Objekte und der zugehörigen förderfähigen Unterobjekte finden Sie unter [Unterstützte Objekte für die Umgebungsförderung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) im Artikel [Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff auf das Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID oder eines API-Schlüssels, der mit der folgenden Methode gegeben werden kann:

### Authentifizierung des Anforderungsheaders

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anforderungsheader namens SessionID zu übergeben, der das Sitzungstoken enthält. Dies hat den Vorteil, dass sie vor [Cross-Site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) -Angriffen geschützt sind und den URI nicht zum Zwischenspeichern stören.

Im Folgenden finden Sie ein Beispiel für eine Anfrage-Kopfzeile:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-Endpunkte

* [Package erstellen](#create-a-package)
* [Eine Liste von Paketen abrufen](#get-a-list-of-packages)
* [Paket nach ID abrufen](#get-a-package-by-id)
* [Aktualisieren bestimmter Eigenschaften eines Pakets](#update-specific-properties-of-a-package)
* [Löschen eines Pakets](#delete-a-package)
* [Ausführen einer Vorab-Ausführung](#execute-a-pre-run)
* [Ausführen einer Installation](#execute-an-installation)
* [Liste der Installationen für ein bestimmtes Paket abrufen](#get-a-list-of-installations-for-a-specific-package)
* [Installationsdetails für eine Installation abrufen](#get-the-installation-details-for-an-installation)

### Package erstellen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf führt einen mehrstufigen Prozess aus.

Der erste Schritt führt zur Erstellung eines leeren Promotionpakets im Status &quot;ASSEMBLING&quot;.

Der zweite Schritt verwendet das im Hauptteil der POST bereitgestellte Array `objectCollections` , um die angeforderten Datensätze aus Workfront zusammenzustellen. Dieser Schritt kann je nach der Anzahl der angeforderten Datensätze und Ihrer Workfront-Konfiguration mehrere Minuten dauern. Am Ende dieses Prozesses wird das leere Promotion-Paket mit dem Wert `packageEntities` aktualisiert und der Status wird automatisch auf &quot;ENTWURF&quot;gesetzt.


>[!NOTE]
>
>Beachten Sie die Struktur des `objectCollections` -Arrays.
>
>Jedes Element im Array enthält einen `objCode` -Schlüssel, der dem im Workfront API Explorer dokumentierten Objektcode entspricht.
>
>Jedes Element enthält auch eine `entities` -Sammlung. Dadurch wird das `ID` -Feld erwartet. Es kann auch ein optionales `name` -Attribut akzeptieren, um leichter zu erkennen, was das `ID` darstellt.
>
>Eine Liste der zulässigen Objektcodes, die in der Liste `objectCollections` angefordert werden sollen, finden Sie im Abschnitt [Unterstützte Objekte für die Umgebungsförderung](#supported-objects-for-environment-promotion) in diesem Artikel.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Kopfzeilen

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oder

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Text

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Reaktion

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### Eine Liste von Paketen abrufen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt eine ungefilterte Liste von Promotion-Paketen zurück, die zum Kunden gehören.

Die Antwort umfasst alle Pakete, die aus einer der Sandboxes, Vorschauen oder Produktionsinstanzen des Kunden von Workfront erstellt wurden.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Kopfzeilen

```json
{
    "apikey": "**********"
}
```

Oder

```json
{
    "sessionID": "*****************"
}
```

#### Text

_Empty_

#### Reaktion

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Überprüfen Sie den obigen &quot;Status&quot;— wurde er hinzugefügt?—>

### Paket nach ID abrufen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt die Details eines angeforderten Promotion-Pakets zurück.

Die Anfrage kann unabhängig von der ursprünglichen Quelle des Promotion-Pakets über jede Umgebung gesendet werden.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopfzeilen

```json
{
    "apikey": "**********"
}
```

Oder

```json
{
    "sessionID": "*****************"
}
```

#### Text

_Empty_

#### Reaktion

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Aktualisieren bestimmter Eigenschaften eines Pakets

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf aktualisiert alle Inhalte des Promotion-Pakets, die im PATCH-Textkörper bereitgestellt werden.

Die bearbeitbaren Attribute sind:

1. name (string)
1. description (string)
1. status (Zeichenfolge mit Wertvalidierung)

Eine ausführliche Beschreibung der verfügbaren Status finden Sie unter [Status der Umgebungsförderung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) im Artikel [Überblick über das Verschieben von Objekten zwischen Workfront-Umgebungen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Kopfzeilen

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oder

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Text

```json
{
    "status": "ACTIVE"
}
```

#### Reaktion

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Löschen eines Pakets

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Durch diesen Aufruf wird der Datensatz des Promotion-Pakets gelöscht. Diese Aktion ist unumkehrbar.

>[!NOTE]
>
>Im Gegensatz zum Löschen eines Promotion-Pakets wird empfohlen, den Status des Pakets in DEAKTIVIERT zu ändern. Dadurch kann das Paket abgerufen werden und der Installationsverlauf der Bereitstellung wird beibehalten.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopfzeilen

```json
{
    "apikey": "**********"
}
```

Oder

```json
{
    "sessionID": "*****************"
}
```

#### Text

_Empty_

#### Reaktion

```
200
```

```
Deleted
```

### Ausführen einer Vorab-Ausführung

>[!IMPORTANT]
>
>Bevor Sie eine Installation ausführen können, müssen Sie diese Vorab-Ausführung ausführen. Sie verwenden die von diesem Aufruf generierte ID, wenn Sie die Installation ausführen.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf führt einen Vergleich zwischen der Package-Definition und der in der URL angegebenen Zielumgebung durch.

Das Ergebnis ist ein JSON-Hauptteil, der angibt, ob ein Promotion-Objekt in der Zielumgebung gefunden wurde oder nicht.

Für jedes Promotion-Objekt wird einer der folgenden `actions` festgelegt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ERSTELLEN</td> 
   <td><p>Wenn ein entsprechender Datensatz nicht in der Zielumgebung gefunden werden kann, ist die Aktion auf CREATE gesetzt.</p><p>Wenn diese Aktion in dem <code>translationmap</code> festgelegt ist, der für den <code>/install</code> -Endpunkt bereitgestellt wird, erstellt der Installationsdienst den Datensatz.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISCH</td> 
   <td><p>Wenn ein entsprechender Datensatz in der Zielumgebung gefunden wird, wird die Aktion auf USEXISTING gesetzt und eine <code>targetId</code> wird auch in der <code>translationmap</code> erfasst.</p><p>Wenn diese Aktion in dem <code>translationmap</code> festgelegt ist, der für den <code>/install</code> -Endpunkt bereitgestellt wird, erstellt der Installationsdienst den Datensatz nicht. Sie verwendet jedoch die im Zuordnungseintrag enthaltene <code>targetId</code> für andere Objekte, die möglicherweise einen Verweis auf diesen Datensatz enthalten.</p><p>Beispielsweise kann eine "Standardgruppe"in der Zielumgebung gefunden werden, in der ein Paket bereitgestellt wird. Es ist nicht möglich, zwei Standardgruppendatensätze zu verwenden. Daher verwendet der Installationsdienst die GUID für die bestehende Gruppe in allen anderen Aktionen zur Objekterstellung, die einen Verweis auf die "Standardgruppe"enthalten, z. B. in einem Projekt, einem Formular oder einer anderen Entität, die mit dieser Gruppe verbunden ist.</p><p><b>Hinweis:</b> <ul><li><p>Wenn die Aktion USEXISTING zugewiesen wird, wird der vorhandene Datensatz in der Zielumgebung nicht geändert. </p><p>Wenn sich beispielsweise die Beschreibung für die "Standardgruppe"in der Sandbox geändert hat, aus der das Paket erstellt wurde, und der Beschreibungswert in der Zielumgebung unterschiedlich ist, bleibt der Wert nach einer Installation mit dem Wert <code>translationmap</code> unverändert.</li></ul></td> 
  </tr> 
  <tr> 
   <td>ÜBERSCHREIBUNG</td> 
   <td><p>Diese Aktion wird nicht automatisch festgelegt.</p><p>Diese Aktion bietet die Möglichkeit, ein Objekt zu aktualisieren, das in der Zielumgebung vorhanden ist. Es bietet die Möglichkeit, eine zugewiesene CREATE - oder USEEXISTING -Aktion manuell zu überschreiben, bevor der <code>/install</code> -Aufruf ausgeführt wird.<ul><li>Ein Benutzer kann ein Objekt in der Testumgebung aktualisieren und dann mithilfe der Aktion ÜBERSCHREIBEN dieses Objekt in der Zielumgebung aktualisieren.</p></li><li><p>Wenn der Benutzer zunächst ein Promotion-Paket installiert und dann in Zukunft ein neues (oder aktualisiertes) Paket Änderungen an Objekten im ursprünglichen Paket enthält, kann der Benutzer mithilfe von OVERWRITING zuvor installierte Objekte ersetzen (überschreiben). </p><p>Weitere Informationen zum Überschreiben finden Sie im Abschnitt [Überschreiben](#overwriting) in diesem Artikel.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Diese Aktion wird nicht automatisch festgelegt.</p><p>Es bietet die Möglichkeit, eine zugewiesene CREATE - oder USEEXISTING -Aktion manuell zu überschreiben, bevor der <code>/install</code> -Aufruf ausgeführt wird.</p><p><b>Hinweise: </b><ul><li><p>Wenn ein Datensatz, der ursprünglich auf CREATE gesetzt wurde, auf IGNORE festgelegt ist, sollten alle untergeordneten Datensätze ebenfalls auf IGNORE gesetzt werden.</p><p>Wenn beispielsweise ein Vorlagendatensatz einer CREATE-Aktion zugeordnet wurde und der Installations-Benutzer ihn von der Bereitstellung ausschließen möchte, kann er die Aktion der Vorlage auf IGNORE setzen.</p><p>In diesem Fall führt die Bereitstellung zu einem fehlgeschlagenen Installationsversuch, wenn der Benutzer nicht auch die Vorlagenaufgaben, Vorlagenaufgaben, Vorlagenaufgaben, Vorlagenaufgaben, Warteschlangendefinition, Warteschlangenthemen, Routing-Regeln usw. auf IGNORE setzt.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf USEEXISTING gesetzt wurde, auf IGNORE gesetzt ist, kann es während des Installationsprozesses zu einigen negativen Auswirkungen kommen.</p><p>Wenn beispielsweise ein Gruppendatensatz der Aktion USEXISTING zugeordnet wurde und der Installations-Benutzer die Aktion zu IGNORE ändert, wird für Objekte, die eine Gruppe erfordern (z. B. ein Projekt kann nicht ohne zugewiesene Gruppe existieren), diesem Projekt die Systemstandardgruppe zugewiesen.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf USEEXISTING festgelegt war, auf CREATE gesetzt ist, kann es während des Installationsprozesses zu einigen negativen Auswirkungen kommen, da viele Workfront-Entitäten über eindeutige Namensbeschränkungen verfügen.</p><p>Wenn beispielsweise ein Eintrag "Standardgruppe"der Aktion USEXISTING zugeordnet wurde und der Installations-Benutzer die Aktion in CREATE ändert, da bereits eine "Standardgruppe"vorhanden ist, schlägt der Installationsprozess fehl, alle Schritte abzuschließen. Gruppennamen müssen eindeutig sein.</p><p>Einige Entitäten haben keine individuelle Namensbeschränkung. Bei diesen Objekten führt diese Änderung zu zwei identischen Datensätzen. Beispielsweise erfordern Vorlagen, Projekte, Ansichten, Filter, Gruppierungen, Berichte und Dashboards keine eindeutigen Namensbeschränkungen. Es empfiehlt sich, eindeutige Namen für diese Datensätze zu verwenden, diese werden jedoch nicht erzwungen.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Es gibt derzeit keine Unterstützung für ein UPDATE `action` in den Alpha-Funktionen dieses Dienstes. Die Option, ein UPDATE `action` zuzulassen, ist etwas, das wir untersuchen.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Kopfzeilen

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oder

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Text

```json
{}
```

#### Reaktion

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>Die ID, die Sie zum Ausführen der Installation benötigen, ist das Feld `id` . In diesem Beispiel ist das Feld `id` das dritte Feld von oben und hat einen Wert, der mit `c0bc79bd` beginnt.

### Ausführen einer Installation

>[!IMPORTANT]
>
>Bevor Sie eine Installation ausführen können, müssen Sie eine Vorab-Ausführung ausführen. Sie verwenden die ID, die aus der Vorab-Ausführung generiert wurde, wenn Sie die Installation ausführen.
>
>Wenn Änderungen an der Zielumgebung (der Umgebung, in der das Paket bereitgestellt wird) nach der Ausführung der Vorab-Ausführung vorgenommen wurden, empfehlen wir, die Vorab-Ausführung erneut auszuführen. Wenn Sie die Vorab-Ausführung nicht erneut ausführen, ist die Ausführung möglicherweise nicht ordnungsgemäß abgeschlossen oder die Installation schlägt möglicherweise fehl.
>
>Anweisungen zum Ausführen einer Vorab-Ausführung finden Sie unter [Ausführen einer Vorab-Ausführung ausführen](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf startet einen Installationsversuch eines Promotion-Pakets in der in der POST-URL angegebenen Zielumgebung.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Kopfzeilen

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oder

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Text

```json
{
}
```

#### Reaktion

```
202
```


```json
{}
```

### Liste der Installationen für ein bestimmtes Paket abrufen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Die Ergebnisse umfassen Installationsereignisse aus allen Umgebungen, in denen das Paket bereitgestellt wurde. Sie beschränken sich nicht auf die Anlagen für die Umgebung, über die die Anfrage gestellt wird. Auf diese Weise können Sie ermitteln, welche Umgebungen dieses Paket erhalten haben.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Kopfzeilen

```json
{
    "apikey": "**********"
}
```

Oder

```json
{
    "sessionID": "*****************"
}
```

#### Text

_Empty_

#### Reaktion

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Installationsdetails für eine Installation abrufen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt die finale `translationMap` zurück, die vom Installationsdienst für eine bestimmte Installation erzeugt wurde.

Jeder Datensatz gibt an, was die verschriebene `action` war und ob diese Aktion erfolgreich war oder nicht.

Für Datensätze mit CREATE `action` wird das Feld `targetId` mit dem Wert des neu erstellten Datensatzes im Zielsystem festgelegt. Außerdem wird für das Feld `installationStatus` der Wert INSTALLIERT festgelegt.

Für Datensätze mit dem USEXISTING `action` wird auch das Feld `targetId` festgelegt und das Feld `installationStatus` auf REGISTRIERT. Dies bedeutet, dass der Zuordnungsprozess abgeschlossen ist und der Installationsdienst bestätigt, dass er den Datensatz ausgewertet hat und dass nichts zu tun ist.

Wenn der Datensatz einen CREATE `action` -Wert hat, der Datensatz jedoch nicht erfolgreich erstellt werden kann, wird der `installationStatus` auf FEHLGESCHLAGEN gesetzt und der Grund für den Fehler wird ebenfalls angegeben.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Kopfzeilen

```json
{
    "apikey": "**********"
}
```

Oder

```json
{
    "sessionID": "*****************"
}
```

#### Text

_Empty_

#### Reaktion

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```

## Überschreiben

Dies ist ein dreistufiger Prozess.

1. Erstellen Sie eine Übersetzungszuordnung (entspricht der Phase &quot;Installation vorbereiten&quot;).
1. Bearbeiten Sie die generierte Übersetzungszuordnung und legen Sie die Felder `action` und `targetId` für jedes Objekt fest, das überschrieben werden soll. Die Aktion sollte `OVERWRITING` lauten und die `targetId` sollte die UUID des Objekts sein, das überschrieben werden soll
1. Führen Sie die Installation aus.

* [Schritt 1: Erstellen einer Übersetzungskarte](#step-1---create-a-translation-map)
* [Schritt 2: Ändern der Übersetzungskarte](#step-2---modify-the-translation-map)
* [Schritt 3: Installieren](#step-3---install)

### **Schritt 1: Erstellen einer Übersetzungskarte**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Text

Keine

#### Reaktion

Eine Übersetzungszuordnung mit dem Status `202 - OK`

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Beispiel

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Schritt 2: Ändern der Übersetzungskarte

Für diesen Schritt gibt es keinen Endpunkt.

1. Überprüfen Sie in der Übersetzungszuordnung, die in [Schritt 1 - Erstellen einer Übersetzungszuordnung](#step-1---create-a-translation-map) zurückgegeben wird, die Liste der zu installierenden Objekte.
1. Aktualisieren Sie das Aktionsfeld für jedes Objekt auf die gewünschte Installationsaktion.
1. Validieren Sie die `targetId` für jedes Objekt. Wenn die festgelegte Aktion `USEEXISTING` oder `OVERWRITING` ist, sollte für die `targetId` die UUID des Zielobjekts in der Zielumgebung festgelegt werden. Bei jeder anderen Aktion sollte targetId eine leere Zeichenfolge sein.

   >[!NOTE]
   >
   >Die `targetId` ist bereits ausgefüllt, wenn eine Kollision erkannt wurde.

### **Schritt 3 - Installieren**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Text

Dies ist ein Objekt mit einem einzelnen Feld `translationMap`, das der geänderten Übersetzungszuordnung aus [Schritt 2 - Übersetzungszuordnung ändern](#step-2---modify-the-translation-map) entsprechen sollte.

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Beispiel

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Reaktion

Die Antwort enthält den Status `{uuid of the created installation}` und `202 - ACCEPTED`.

Beispiel: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
