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
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 949907d7d4c37fa6541a021b458f84f1ebff2896
workflow-type: tm+mt
source-wordcount: '2412'
ht-degree: 3%

---

# Objekte von einem Objekt verschieben [!DNL Workfront] Umgebung zu einer anderen

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] Plan</td> 
   <td> <p>Enterprise, Prime oder Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] Lizenz</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Objektberechtigungen</p> </td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support-Paket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] oder [!UICONTROL Enterprise]</p> <p>Das standardmäßige Support-Paket hat keinen Zugriff auf die Sandbox Benutzerdefinierte Aktualisierung, aber es hat Zugriff auf die Vorschau-Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Der Endpunkt &quot;Promotion Package erstellen&quot;setzt voraus, dass Sie die Quellumgebung bereits konfiguriert haben. Dieser API-Aufruf erfordert das manuelle Erstellen einer Objektzuordnung von [!DNL Workfront] objCodes und Objektkennungen. Die spezifische Struktur dieser Karte wird nachfolgend beschrieben.

## Unterstützte Objekte für die Umgebungsförderung

Die Funktion zur Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Die Möglichkeit zum Verschieben von Transaktionsobjekten wird nicht unterstützt (mit eingeschränkten Ausnahmen).

* [Arbeitsobjekte](#work-objects)
* [Reporting-Objekte](#reporting-objects)
* [Benutzerdefinierte Datenobjekte](#custom-data-objects)
* [Organisationsobjekte](#organization-objects)
* [Andere Konfigurationsobjekte](#other-configuration-objects)


### Arbeitsobjekte

| Förderbares Objekt | Einbezogene förderfähige Unterobjekte |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Aufgabe<br>Zuweisung<br>Vorgänger<br>Firma<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nichtarbeitstag<br>Warteschlangendefinition<br>Themengruppe &quot;Warteschlange&quot;<br>Warteschlangenthema<br>Routing-Regel<br>Milestone-Pfad<br>Milestone<br>Stündentyp<br>Ressourcenpool<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Vorlage (TMPL) | Vorlage<br>Vorlagenaufgabe<br>Vorlagenaufgaben zuweisen<br>VorlagenTask-Vorgänger<br>Firma<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nichtarbeitstag<br>Warteschlangendefinition<br>Themengruppe &quot;Warteschlange&quot;<br>Warteschlangenthema<br>Routing-Regel<br>Milestone-Pfad<br>Milestone<br>Stündentyp<br>Ressourcenpool<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Reporting-Objekte

| Förderbares Objekt | Einbezogene förderfähige Unterobjekte |
| --- | --- |
| Layout Template (UITMPL) | Layout-Vorlage<br>Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Dashboard (PTLTAB) | Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Kalender (CALEND) | Kalender<br>Kalenderabschnitt |
| Externe Seite (EXTSEC) | Externe Seite |
| Bericht (PTLSEC) | Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Gruppierung (UIGB) | Gruppierung<br>Parameter |
| Anzeigen (UIVW) | Ansicht<br>Parameter |

### Benutzerdefinierte Datenobjekte

| Förderbares Objekt | Einbezogene förderfähige Unterobjekte |
| --- | --- |
| Kategorie (KG) | Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik<br>Gruppe |
| Parameter (PARAM) | Parameter<br>Parameteroption |
| Parametergruppe (PGRP) | Parametergruppe |

### Organisationsobjekte

| Förderbares Objekt | Einbezogene förderfähige Unterobjekte |
| --- | --- |
| Gruppe (GRUPPE) | Gruppe <br>Untergruppen (bis zu 5 Ebenen)<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Rolle (ROLE) | Funktion |
| Team (TEAM) | Team<br>Gruppe |
| Unternehmen (CMPY) | Firma<br>Überschreibungsrate<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameter <br>Kategorieanzeigelogik<br>Gruppe |
| Portfolio (HAFEN) | Portfolio<br>Programm<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Programm (PRGM) | Programm<br>Portfolio<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Andere Konfigurationsobjekte

| Förderbares Objekt | Einbezogene förderfähige Unterobjekte |
| --- | --- |
| Genehmigungsverfahren (ARVVR) | Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Rolle<br>Team<br>Gruppe |
| Zeitplan (SCHED) | Zeitplan<br>Nichtarbeitstag<br>Gruppe |
| Meilensteinpfad (MPATH) | Milestone-Pfad<br>Milestone |
| Datenblatt-Profil (TSPRO) | Datenblatt-Profil<br>Stündentyp |
| Stundentyp (STUNDE) | Stundentyp |
| Ausgabentyp (EXPTYP) | Ausgabentyp |
| Risikotyp (RSKTYP) | Risikotyp |
| Ressourcen-Pool (RSPL) | Ressourcenpool |

## Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff auf das Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID oder eines API-Schlüssels, der mit der folgenden Methode gegeben werden kann:

### Authentifizierung des Anforderungsheaders

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anforderungsheader namens SessionID zu übergeben, der das Sitzungstoken enthält. Das hat den Vorteil, dass man vor [Cross-Site Request Forgery (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) greift zu und stört nicht den URI zum Zwischenspeichern.

Im Folgenden finden Sie ein Beispiel für eine Anfrage-Kopfzeile:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-Endpunkte

* [Package erstellen](#create-a-package)
* [Eine Liste von Paketen abrufen](#get-a-list-of-packages)
* [Paket nach ID abrufen](#get-a-package-by-id)
* [Konfigurationsdefinition eines Pakets abrufen](#get-a-packages-configuration-definition)
* [Ersetzen von Paketdetails und Definition](#replace-package-details-and-definition)
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

Der zweite Schritt verwendet die `objectCollections` -Array, das im Hauptteil der POST bereitgestellt wird, um die angeforderten Datensätze aus Workfront zusammenzustellen. Dieser Schritt kann je nach der Anzahl der angeforderten Datensätze und Ihrer Workfront-Konfiguration mehrere Minuten dauern. Am Ende dieses Prozesses wird das leere Promotion-Paket mit dem `packageEntities` und der Status automatisch auf &quot;ENTWURF&quot;gesetzt wird.


>[!NOTE]
>
>Beachten Sie die Struktur der `objectCollections`  Array.
>
>Jedes Element im Array enthält eine `objCode` -Schlüssel, der dem im Workfront API Explorer dokumentierten Objektcode entspricht.
>
>Jedes Element enthält auch `entities` -Sammlung. Dies erwartet die `ID` -Feld. Es kann auch eine optionale `name` -Attribut, um die `ID` darstellt.
>
>Für die Liste der zulässigen Objektcodes, die im Abschnitt `objectCollections` Liste, siehe [Unterstützte Objekte für die Umgebungsförderung](#supported-objects-for-environment-promotion) in diesem Artikel beschrieben.

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
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
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
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

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
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

### Konfigurationsdefinition eines Pakets abrufen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
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

#### Antwort

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Ersetzen von Paketdetails und Definition

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Dieser Aufruf ersetzt alle Inhalte des Promotionpakets.

Die Anfrage erwartet, dass alle bearbeitbaren Felder bereitgestellt werden.

Die bearbeitbaren Attribute sind:

1. name (string)
1. description (string)
1. source (Zeichenfolge mit URL-Validierung)
1. status (Zeichenfolge mit Wertvalidierung)
1. version (integer)
1. packageEntities (collection)

Zu den Statusoptionen gehören:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>Dieser Status wird automatisch zugewiesen, während Objekte assembliert werden.</p><p>Dieser Status kann nicht direkt von einem Kunden festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ENTWURF</td> 
   <td><p>Dieser Status wird beim Abschluss eines Assemblyprozesses oder beim Erstellen eines leeren Promotion-Pakets zugewiesen.</p><p>Es ist möglich, dass ein Kunde das Promotion-Paket zurück in diesen Status verschiebt.</p><p>Während in diesem Status das Promotion-Paket in keiner Umgebung installiert werden kann.</p></td> 
  </tr> 
  <tr> 
   <td>TESTEN</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in jeder Vorschau- oder benutzerdefinierten Aktualisierungs-Sandbox. Während in diesem Status kann das Paket nicht in der Produktion installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in einer beliebigen Umgebung, einschließlich der Produktion.</p><p>Wenn ein Paketstatus auf "ACTIVE"gesetzt ist, wird die <code>publishedAt</code> Datum wird automatisch auf den aktuellen Zeitstempel der Anforderung gesetzt.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Dieser Status wird verwendet, um zuvor verwendete Promotionspakete auszublenden, die in Zukunft in keiner Umgebung installiert werden.</p><p>Wenn ein Paket diesen Status aufweist, kann es in keiner Umgebung installiert werden.</p><p>Wenn ein Paketstatus auf DEAKTIVIERT gesetzt ist, wird die <code>retiredAt</code> Datum wird automatisch auf den aktuellen Zeitstempel der Anforderung gesetzt.</p><p>Die Verwendung dieses Status wird empfohlen, da die<code>DELETE /package</code> -Endpunkt, da er abgerufen werden kann und der Installationsverlauf für alle Implementierungen, die mit diesem Paket vorgenommen werden, beibehalten wird.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Wenn die ASSEMBLING-Phase fehlschlägt, wird das Promotionpaket automatisch in diesen Status versetzt.</p><p>Um das Package in die Phase der ASSEMBLING zurückzusetzen, müssen Sie den Extraktionsvorgang erneut Trigger haben.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopfzeilen

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

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
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
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
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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
1. source (Zeichenfolge mit URL-Validierung)
1. status (Zeichenfolge mit Wertvalidierung)
1. version (integer)
1. packageEntities (collection)

   oder

   objectCollections (Array)

Stellen Sie die `packageEntities` aktualisiert das Promotion-Paket mit der angegebenen Konfigurationsdefinition.

Stellen Sie die `objectCollections` wird eine Neuextraktion von der `source` Umgebung, die mit dem Promotion-Paket verknüpft ist. Die `source` -Feld muss angegeben werden, wenn die `objectCollections` bereitgestellt wird.

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
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
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

#### Antwort

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

Für jedes Promotion-Objekt eine der folgenden Optionen `actions`  festgelegt wird:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ERSTELLEN</td> 
   <td><p>Wenn ein entsprechender Datensatz nicht in der Zielumgebung gefunden werden kann, ist die Aktion auf CREATE gesetzt.</p><p>Wenn diese Aktion in der <code>translationmap</code> , die dem <code>/install</code> -Endpunkt verwenden, erstellt der Installationsdienst den Datensatz.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISCH</td> 
   <td><p>Wenn ein entsprechender Datensatz in der Zielumgebung gefunden wird, wird die Aktion auf USEXISTING gesetzt und eine <code>targetId</code> wird auch im <code>translationmap</code>.</p><p>Wenn diese Aktion in der <code>translationmap</code> , die dem <code>/install</code> -Endpunkt verwenden, erstellt der Installationsdienst den Datensatz nicht. Sie verwendet jedoch die <code>targetId</code> im Zuordnungseintrag für andere Objekte enthalten, die möglicherweise einen Verweis auf diesen Datensatz enthalten.</p><p>Beispielsweise kann eine "Standardgruppe"in der Zielumgebung gefunden werden, in der ein Paket bereitgestellt wird. Es ist nicht möglich, zwei Standardgruppendatensätze zu verwenden. Daher verwendet der Installationsdienst die GUID für die bestehende Gruppe in allen anderen Aktionen zur Objekterstellung, die einen Verweis auf die "Standardgruppe"enthalten, z. B. in einem Projekt, einem Formular oder einer anderen Entität, die mit dieser Gruppe verbunden ist.</p><p><b>Notiz:</b> <ul><li><p>Wenn die Aktion USEXISTING zugewiesen wird, wird der vorhandene Datensatz in der Zielumgebung nicht geändert. </p><p>Wenn sich beispielsweise die Beschreibung für die "Standardgruppe"in der Sandbox geändert hat, aus der das Paket erstellt wurde, und der Beschreibungswert in der Zielumgebung unterschiedlich ist, bleibt der Wert nach einer Installation mit dieser unverändert. <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Diese Aktion wird nicht automatisch festgelegt.</p><p>Es bietet die Möglichkeit, eine zugewiesene CREATE- oder USEEXISTING-Aktion manuell zu überschreiben, bevor die <code>/install</code> aufrufen.</p><p><b>Notizen: </b><ul><li><p>Wenn ein Datensatz, der ursprünglich auf CREATE gesetzt wurde, auf IGNORE festgelegt ist, sollten alle untergeordneten Datensätze ebenfalls auf IGNORE gesetzt werden.</p><p>Wenn beispielsweise ein Vorlagendatensatz einer CREATE-Aktion zugeordnet wurde und der Installations-Benutzer ihn von der Bereitstellung ausschließen möchte, kann er die Aktion der Vorlage auf IGNORE setzen.</p><p>In diesem Fall führt die Bereitstellung zu einem fehlgeschlagenen Installationsversuch, wenn der Benutzer nicht auch die Vorlagenaufgaben, Vorlagenaufgaben, Vorlagenaufgaben, Vorlagenaufgaben, Warteschlangendefinition, Warteschlangenthemen, Routing-Regeln usw. auf IGNORE setzt.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf USEEXISTING gesetzt wurde, auf IGNORE gesetzt ist, kann es während des Installationsprozesses zu einigen negativen Auswirkungen kommen.</p><p>Wenn beispielsweise ein Gruppendatensatz der Aktion USEXISTING zugeordnet wurde und der Installations-Benutzer die Aktion zu IGNORE ändert, wird für Objekte, die eine Gruppe erfordern (z. B. ein Projekt kann nicht ohne zugewiesene Gruppe existieren), diesem Projekt die Systemstandardgruppe zugewiesen.</p></li><li><p>Wenn ein Datensatz, der ursprünglich auf USEEXISTING festgelegt war, auf CREATE gesetzt ist, kann es während des Installationsprozesses zu einigen negativen Auswirkungen kommen, da viele Workfront-Entitäten über eindeutige Namensbeschränkungen verfügen.</p><p>Wenn beispielsweise ein Eintrag "Standardgruppe"der Aktion USEXISTING zugeordnet wurde und der Installations-Benutzer die Aktion in CREATE ändert, da bereits eine "Standardgruppe"vorhanden ist, schlägt der Installationsprozess fehl, alle Schritte abzuschließen. Gruppennamen müssen eindeutig sein.</p><p>Einige Entitäten haben keine individuelle Namensbeschränkung. Bei diesen Objekten führt diese Änderung zu zwei identischen Datensätzen. Beispielsweise erfordern Vorlagen, Projekte, Ansichten, Filter, Gruppierungen, Berichte und Dashboards keine eindeutigen Namensbeschränkungen. Es empfiehlt sich, eindeutige Namen für diese Datensätze zu verwenden, diese werden jedoch nicht erzwungen.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Es wird derzeit kein UPDATE unterstützt `action` in den Alpha-Funktionen dieses Dienstes. Die Option zum Zulassen einer UPDATE `action` ist etwas, das wir untersuchen.

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
>Die ID, die Sie zum Ausführen der Installation benötigen, ist die `id` -Feld. In diesem Beispiel wird die `id` -Feld ist der dritte von oben und hat einen Wert, der mit `c0bc79bd`.

### Ausführen einer Installation

>[!IMPORTANT]
>
>Bevor Sie eine Installation ausführen können, müssen Sie eine Vorab-Ausführung ausführen. Sie verwenden die ID, die aus der Vorab-Ausführung generiert wurde, wenn Sie die Installation ausführen.
>
>Wenn Änderungen an der Zielumgebung (der Umgebung, in der das Paket bereitgestellt wird) nach der Ausführung der Vorab-Ausführung vorgenommen wurden, empfehlen wir, die Vorab-Ausführung erneut auszuführen. Wenn Sie die Vorab-Ausführung nicht erneut ausführen, ist die Ausführung möglicherweise nicht ordnungsgemäß abgeschlossen oder die Installation schlägt möglicherweise fehl.
>
>Anweisungen zum Ausführen einer Vorab-Ausführung finden Sie unter [Ausführen einer Vorab-Ausführung](#execute-a-pre-run).

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

#### Antwort

```
200
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
        "status": "COMPLETED",
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

Dieser Aufruf gibt die endgültige `translationMap` von der Installationsdienststelle für eine bestimmte Anlage erzeugt werden.

Jeder Datensatz gibt an, was die `action` war und ob diese Aktion erfolgreich war oder nicht.

Für Datensätze mit CREATE `action` die `targetId` wird mit dem Wert des neu erstellten Datensatzes im Zielsystem festgelegt. Darüber hinaus wird die `installationStatus` wird auf INSTALLIERT gesetzt.

Für Datensätze mit USEEXISTING `action` die `targetId` wird ebenfalls festgelegt, und die `installationStatus` wird auf REGISTRIERT gesetzt. Dies bedeutet, dass der Zuordnungsprozess abgeschlossen ist und der Installationsdienst bestätigt, dass er den Datensatz ausgewertet hat und dass nichts zu tun ist.

Wenn der Datensatz ein CREATE aufweist `action` aber der Datensatz nicht erfolgreich erstellt werden kann, wird die `installationStatus` auf FEHLGESCHLAGEN gesetzt und der Grund für den Fehler wird ebenfalls angegeben.

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
    "status": "COMPLETED",
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
