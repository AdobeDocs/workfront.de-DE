---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Verschieben von Objekten von einer Umgebung in eine andere
description: Die Funktion Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Das Verschieben von Transaktionsobjekten wird nicht unterstützt (mit wenigen Ausnahmen).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 2%

---

# Verschieben von Objekten zwischen [!DNL Workfront] Umgebungen mithilfe der [!DNL Workfront] Environment Promotion API

Mit der Funktion Umgebungsförderung können Sie konfigurationsbezogene Objekte von einer Umgebung in eine andere verschieben. Sie können diese Objekte mithilfe der Workfront-API verschieben, wie in diesem Artikel beschrieben.

Anweisungen zum Verschieben von Objekten zwischen Umgebungen mithilfe des Workfront-Programms finden Sie unter:

* [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installieren eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront-Lizenzen</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td><p>Sie müssen ein Workfront-Administrator sein.</p>
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Der Endpunkt Erstellen eines Weiterleitungspakets setzt voraus, dass Sie die Quellumgebung bereits konfiguriert haben. Dieser API-Aufruf erfordert die manuelle Erstellung einer Objektzuordnung mit [!DNL Workfront] objCodes und Objekt-GUIDs. Die spezifische Struktur dieser Zuordnung wird nachfolgend beschrieben.

## Unterstützte Objekte für die Umgebungs-Promotion

Die Funktion Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Das Verschieben von Transaktionsobjekten wird nicht unterstützt (mit wenigen Ausnahmen).

Eine Liste der Promotable-Objekte und der darin enthaltenen Promotable-Unterobjekte finden Sie unter [Unterstützte Objekte für die ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)) im Artikel [Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff zum Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID oder eines API-Schlüssels, die mithilfe der folgenden Methode erteilt werden können:

### Authentifizierung beim Anforderungsheader

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anfrage-Header mit dem Namen SessionID zu übergeben, der das Sitzungs-Token enthält. Dies hat den Vorteil, dass es vor [Cross-Site Request Forgery (CSRF)-Angriffen ](https://en.wikipedia.org/wiki/Cross-site_request_forgery) ist und den URI zu Caching-Zwecken nicht beeinträchtigt.

Im Folgenden finden Sie ein Beispiel für einen Anfrage-Header:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-Endpunkte

* [Erstellen eines Pakets](#create-a-package)
* [Abrufen einer Liste von Paketen](#get-a-list-of-packages)
* [Abrufen eines Pakets nach ID](#get-a-package-by-id)
* [Aktualisieren spezifischer Eigenschaften eines Pakets](#update-specific-properties-of-a-package)
* [Löschen eines Pakets](#delete-a-package)
* [Ausführen eines Vorlaufs](#execute-a-pre-run)
* [Ausführen einer Installation](#execute-an-installation)
* [Abrufen einer Liste von Installationen für ein bestimmtes Paket](#get-a-list-of-installations-for-a-specific-package)
* [Abrufen der Installationsdetails für eine Installation](#get-the-installation-details-for-an-installation)

### Erstellen eines Pakets

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf führt einen mehrstufigen Prozess aus.

Der erste Schritt führt zur Erstellung eines leeren Promotion-Pakets im Status „ASSEMBLING“.

Im zweiten Schritt werden die von Workfront angeforderten Datensätze mithilfe des `objectCollections`-Arrays zusammengestellt, das im POST-Hauptteil bereitgestellt wird. Dieser Schritt kann je nach der Anzahl der angeforderten Datensätze und Ihrer Workfront-Konfiguration mehrere Minuten dauern. Am Ende dieses Prozesses wird das leere Promotion-Paket mit dem `packageEntities` aktualisiert und der Status wird automatisch auf „ENTWURF“ gesetzt.


>[!NOTE]
>
>Beachten Sie die Struktur des `objectCollections`-Arrays.
>
>Jedes Element im -Array enthält einen `objCode`, der dem im Workfront-API-Explorer dokumentierten Objekt-Code entspricht.
>
>Jedes Element enthält auch eine `entities`. Dies erwartet das `ID` Feld. Er kann auch ein optionales `name`-Attribut akzeptieren, um das Erkennen der `ID` zu vereinfachen.
>
>Die Liste der zulässigen Objekt-Codes, die in der `objectCollections` angefordert werden dürfen, finden Sie im Abschnitt [Unterstützte Objekte für die ](#supported-objects-for-environment-promotion)) in diesem Artikel.

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

#### Textkörper

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

#### Antwort

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

### Abrufen einer Liste von Paketen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt eine ungefilterte Liste von Promotion-Paketen zurück, die zum Kunden gehören.

Die Antwort enthält alle Pakete, die aus einer der Sandbox-, Vorschau- oder Produktionsinstanzen des Kunden von Workfront erstellt wurden.

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

#### Textkörper

_leer_

#### Antwort

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

&lt;!—Überprüfen Sie oben „status“—wurde sie hinzugefügt?—>

### Abrufen eines Pakets nach ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt die Details eines angeforderten Promotion-Pakets zurück.

Die Anfrage kann über jede Umgebung unabhängig von der ursprünglichen Quelle des Promotion-Pakets erfolgen.

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

#### Textkörper

_leer_

#### Antwort

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

### Aktualisieren spezifischer Eigenschaften eines Pakets

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf aktualisiert alle Inhalte des Promotion-Pakets, die im PATCH-Hauptteil bereitgestellt werden.

Die bearbeitbaren Attribute sind:

1. Name (Zeichenfolge)
1. description (String)
1. Status (Zeichenfolge mit Wertvalidierung)

Eine ausführliche Beschreibung der verfügbaren Status finden Sie unter [Umgebungsförderungsstatus](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) im Artikel „Übersicht [ Verschieben von Objekten zwischen Workfront-Umgebungen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


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

#### Textkörper

```json
{
    "status": "ACTIVE"
}
```

#### Antwort

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

Dieser Aufruf löscht den Datensatz des Promotion-Pakets. Diese Aktion kann nicht rückgängig gemacht werden.

>[!NOTE]
>
>Anstatt ein Promotion-Paket zu löschen, wird empfohlen, den Status des Pakets in DEAKTIVIERT zu ändern. Dadurch kann das Paket abgerufen werden und der Installationsverlauf wird dort gespeichert, wo es bereitgestellt wurde.

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

#### Textkörper

_leer_

#### Antwort

```
200
```

```
Deleted
```

### Ausführen eines Vorlaufs

>[!IMPORTANT]
>
>Bevor Sie eine Installation ausführen können, müssen Sie diesen Pre-Run ausführen. Sie verwenden die bei diesem Aufruf generierte ID, wenn Sie die Installation ausführen.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf führt einen Vergleich zwischen der Paketdefinition und der in der URL identifizierten Zielumgebung durch.

Das Ergebnis ist ein JSON-Text, der angibt, ob ein Weiterleitungsobjekt in der Zielumgebung gefunden wurde oder nicht.

Für jedes Promotion-Objekt wird eine der folgenden `actions` festgelegt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ERSTELLEN</td> 
   <td><p>Wenn in der Zielumgebung kein entsprechender Datensatz gefunden werden kann, wird die Aktion auf ERSTELLEN gesetzt.</p><p>Wenn diese Aktion in der <code>translationmap</code> festgelegt wird, die dem <code>/install</code>-Endpunkt bereitgestellt wird, erstellt der Installations-Service den Datensatz.</p></td> 
  </tr> 
  <tr> 
   <td>VORHANDENE VERWENDEN</td> 
   <td><p>Wenn ein entsprechender Datensatz in der Zielumgebung gefunden wird, wird die Aktion auf „USEEXISTING“ festgelegt und ein <code>targetId</code> wird ebenfalls in der <code>translationmap</code> erfasst.</p><p>Wenn diese Aktion in der <code>translationmap</code> festgelegt ist, die dem <code>/install</code>-Endpunkt bereitgestellt wird, erstellt der Installations-Service den Datensatz nicht. Sie verwendet jedoch die im Zuordnungseintrag enthaltenen <code>targetId</code> für andere Objekte, die möglicherweise auf diesen Datensatz verweisen.</p><p>Beispielsweise kann sich eine „Standardgruppe“ in der Zielumgebung befinden, in der ein Paket bereitgestellt wird. Es ist nicht möglich, zwei „Standardgruppen“-Datensätze zu verwenden. Daher verwendet der Installations-Service die GUID für die bestehende Gruppe bei allen anderen Objekterstellungsaktionen, die einen Verweis auf die „Standardgruppe“ enthalten, z. B. ein Projekt, ein Formular oder eine andere Entität, die mit dieser Gruppe verbunden ist.</p><p><b>Hinweis:</b> <ul><li><p>Wenn die Aktion „VORHANDEN VERWENDEN“ zugewiesen wird, wird der vorhandene Datensatz in der Zielumgebung nicht geändert. </p><p>Wenn sich beispielsweise die Beschreibung für die „Standardgruppe“ in der Sandbox geändert hat, aus der das Paket erstellt wurde, und der Wert der Beschreibung in der Zielumgebung anders ist, bleibt der Wert nach einer Installation mit dieser <code>translationmap</code> unverändert.</li></ul></td> 
  </tr> 
  <tr> 
   <td>ÜBERSCHREIBEN</td> 
   <td><p>Diese Aktion wird nicht automatisch festgelegt.</p><p>Diese Aktion bietet die Möglichkeit, ein Objekt zu aktualisieren, das in der Zielumgebung vorhanden ist. Es bietet die Möglichkeit, eine zugewiesene CREATE- oder USEEXISTING-Aktion manuell zu überschreiben, bevor der <code>/install</code>-Aufruf ausgeführt wird.<ul><li>Ein Benutzer kann ein Objekt in der Testumgebung aktualisieren und dann die Aktion „ÜBERSCHREIBEN“ verwenden, um dieses Objekt in der Zielumgebung zu aktualisieren.</p></li><li><p>Wenn der Benutzer ein Promotion-Paket anfänglich installiert und dann ein neues (oder aktualisiertes) Paket in der Zukunft Änderungen an Objekten im ursprünglichen Paket enthält, kann der Benutzer OVERWRITING verwenden, um zuvor installierte Objekte zu ersetzen (zu überschreiben). </p><p>Weitere Informationen zum Überschreiben finden Sie im Abschnitt [Überschreiben](#overwriting) in diesem Artikel.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORIEREN</td> 
   <td><p>Diese Aktion wird nicht automatisch festgelegt.</p><p>Es bietet die Möglichkeit, eine zugewiesene CREATE- oder USEEXISTING-Aktion manuell zu überschreiben, bevor der <code>/install</code>-Aufruf ausgeführt wird.</p><p><b>Hinweise: </b><ul><li><p>Wenn ein Datensatz, der ursprünglich auf ERSTELLEN festgelegt war, auf IGNORIEREN festgelegt ist, sollten auch alle untergeordneten Datensätze auf IGNORIEREN festgelegt werden.</p><p>Wenn beispielsweise ein Vorlagendatensatz einer CREATE-Aktion zugeordnet wurde und die installierenden Benutzenden ihn aus der Bereitstellung ausschließen möchten, können sie die Vorlagenaktion auf IGNORIEREN setzen.</p><p>Wenn der installierende Benutzer in diesem Fall nicht auch die Vorlagenaufgaben, Vorlagenaufgabenzuweisungen, Vorlagenaufgabenvorgänger, Warteschlangendefinition, Warteschlangenthemen, Routing-Regeln usw. auf IGNORIEREN festlegt, führt die Bereitstellung zu einem fehlgeschlagenen Installationsversuch.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf „VORHANDEN VERWENDEN“ festgelegt war, auf „IGNORIEREN“ gesetzt wurde, kann es während des Installationsprozesses zu einigen nachteiligen Auswirkungen kommen.</p><p>Wenn beispielsweise der Aktion „USEEXISTING“ ein Gruppeneintrag zugeordnet wurde und die installierende Person die Aktion in „IGNORE“ ändert, wird diesem Projekt bei Objekten, für die eine Gruppe erforderlich ist (z. B. wenn ein Projekt ohne zugewiesene Gruppe nicht vorhanden sein kann) die Standardgruppe zugewiesen.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf „USEEXISTING“ festgelegt war, auf „CREATE“ gesetzt ist, kann es während des Installationsprozesses zu unerwünschten Effekten kommen, da viele Workfront-Entitäten über Einschränkungen hinsichtlich eindeutiger Namen verfügen.</p><p>Wenn beispielsweise der Aktion USEEXISTING ein Eintrag „Standardgruppe“ zugeordnet wurde und der installierende Benutzer die Aktion in CREATE ändert, da bereits eine „Standardgruppe“ vorhanden ist, können bei der Installation nicht alle Schritte ausgeführt werden. Gruppennamen müssen eindeutig sein.</p><p>Einige Entitäten verfügen nicht über eine eindeutige Namensbeschränkung. Für diese Objekte führt diese Änderung zu zwei identisch benannten Datensätzen. Für Vorlagen, Projekte, Ansichten, Filter, Gruppierungen, Berichte und Dashboards sind beispielsweise keine Beschränkungen für eindeutige Namen erforderlich. Es empfiehlt sich, eindeutige Namen für diese Datensätze zu haben. Dies wird jedoch nicht erzwungen.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

In den Alpha-Funktionen dieses Service wird derzeit kein UPDATE-`action` unterstützt. Wir forschen an der Option, eine UPDATE-`action` zuzulassen.

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

#### Textkörper

```json
{}
```

#### Antwort

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
>Die ID, die Sie für die Installation benötigen, ist das Feld `id` . In diesem Beispiel ist das `id` Feld ein drittes von oben und hat einen Wert, der mit `c0bc79bd` beginnt.

### Ausführen einer Installation

>[!IMPORTANT]
>
>Bevor Sie eine Installation ausführen können, müssen Sie einen Pre-Run ausführen. Sie verwenden die ID, die aus der Vorabausführung generiert wurde, wenn Sie die Installation ausführen.
>
>Wenn nach dem Ausführen der Vorabausführung Änderungen an der Zielumgebung (der Umgebung, in der das Paket bereitgestellt wird) vorgenommen wurden, empfehlen wir, die Vorabausführung erneut auszuführen. Wenn Sie die Vorabausführung nicht erneut ausführen, wird die Ausführung möglicherweise nicht korrekt abgeschlossen oder die Installation schlägt fehl.
>
>Anweisungen zum Ausführen eines Vorlaufs finden Sie unter [Ausführen eines Vorlaufs](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf startet einen Installationsversuch eines Promotion-Pakets in die Zielumgebung, die in der POST-URL angegeben ist.

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

#### Textkörper

```json
{
}
```

#### Antwort

```
202
```


```json
{}
```

### Abrufen einer Liste von Installationen für ein bestimmtes Paket

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Die Ergebnisse umfassen Installationsereignisse aus allen Umgebungen, in denen das Paket bereitgestellt wurde. Sie beschränken sich nicht auf die Anlagen für die Umgebung, über die die Anforderung erfolgt. Auf diese Weise können Sie feststellen, welche Umgebungen dieses Paket erhalten haben.

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

#### Textkörper

_leer_

#### Antwort

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

### Abrufen der Installationsdetails für eine Installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf gibt die endgültigen `translationMap` zurück, die vom Installationsdienst für eine bestimmte Installation erzeugt wurden.

In jedem Datensatz wird angegeben, was die vorgeschriebene `action` war und ob diese Aktion erfolgreich war oder nicht.

Bei Datensätzen mit der `action` ERSTELLEN wird das Feld `targetId` mit dem Wert des neu erstellten Datensatzes im Zielsystem festgelegt. Darüber hinaus wird das Feld `installationStatus` auf INSTALLIERT gesetzt.

Bei Datensätzen mit der `action` USEEXISTING wird auch das Feld `targetId` festgelegt und das Feld `installationStatus` wird auf REGISTRIERT gesetzt. Dies bedeutet, dass der Zuordnungsprozess abgeschlossen war und der Installations-Service bestätigt, dass er den Datensatz ausgewertet hat und es keine Maßnahmen gibt.

Wenn der Datensatz eine CREATE-`action` hat, aber nicht erfolgreich erstellt werden kann, wird die `installationStatus` auf FAILED gesetzt und der Grund für den Fehler wird ebenfalls angegeben.

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

#### Textkörper

_leer_

#### Antwort

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

1. Erstellen eines Übersetzungsdiagramms (analog zur Phase „Installation vorbereiten„)
1. Bearbeiten Sie die generierte Übersetzungszuordnung und legen Sie die `action`- und `targetId` für alle Objekte fest, die sie überschreiben möchten. Die Aktion sollte `OVERWRITING` sein und der `targetId` sollte die UUID des Objekts sein, das überschrieben werden soll
1. Führen Sie die Installation aus.

* [Schritt 1: Erstellen einer Übersetzungskarte](#step-1---create-a-translation-map)
* [Schritt 2: Ändern der Übersetzungszuordnung](#step-2---modify-the-translation-map)
* [Schritt 3: Installieren](#step-3---install)

### **Schritt 1: Erstellen einer Übersetzungskarte**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Textkörper

Keine

#### Antwort

Eine Übersetzungskarte mit einem `202 - OK` Status

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

### Schritt 2: Ändern der Übersetzungszuordnung

Für diesen Schritt gibt es keinen Endpunkt.

1. Überprüfen Sie in der Übersetzungszuordnung[ die in Schritt 1 - Erstellen einer ](#step-1---create-a-translation-map) zurückgegeben wird, die Liste der zu installierenden Objekte.
1. Aktualisieren Sie das Aktionsfeld auf jedem Objekt, um die gewünschte Installationsaktion durchzuführen.
1. Überprüfen Sie die `targetId` für jedes Objekt. Wenn die Aktion „Festlegen“ `USEEXISTING` oder `OVERWRITING` ist, sollte die `targetId` auf die UUID des Zielobjekts in der Zielumgebung festgelegt werden. Für jede andere Aktion sollte die targetId eine leere Zeichenfolge sein.

   >[!NOTE]
   >
   >Der `targetId` wird bereits ausgefüllt, wenn eine Kollision erkannt wurde.

### **Schritt 3: Installieren**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Textkörper

Dies ist ein Objekt mit einem einzelnen `translationMap`, das der geänderten Übersetzungszuordnung aus [Schritt 2 - Übersetzungszuordnung ändern](#step-2---modify-the-translation-map) entsprechen sollte.

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

#### Antwort

Die Antwort enthält die `{uuid of the created installation}` und einen `202 - ACCEPTED`.

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
