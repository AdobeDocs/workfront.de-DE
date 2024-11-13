---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Arbeiten mit großen Dateien in Adobe Workfront Fusion
description: Große Dateiunterstützung ist derzeit für die Workfront- und HTTP-Connectoren verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: e0be458c-a5f4-48e4-a8fb-afd5d072b6ff
source-git-commit: 5e32c0dd3378fc49f8687668f11daa5dc838c587
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Arbeiten mit großen Dateien in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Die Funktion &quot;Große Dateien&quot;ist nur für Kunden von Workfront Ultimate verfügbar und wird schrittweise eingeführt. Alle Fusion-Organisationen mit einem Workfront Ultimate-Plan werden bis Januar 2025 über eine große Dateikapazität verfügen.

In Workfront Fusion stehen nun erweiterte Funktionen zur Datenübertragung zur Verfügung, mit denen Szenarien erheblich größere Dateien verarbeiten können.

Um größere Dateien zu verarbeiten, müssen Ihre Szenarien aktualisiert werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>
   <td> <p>Neu: Ultmatat</p> <p>Oder</p> <p>Aktuell: Nicht verfügbar</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: Nicht verfügbar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu: [!DNL Workfront Fusion] ist im Ultimate Workfront-Plan enthalten.</p> <p>Oder</p>
   <p>Aktuell: Nicht verfügbar</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Connectoren, die große Dateien unterstützen

In der ersten Version unterstützen die folgenden Connectoren große Dateien.

* Workfront > Dokument hochladen
* Adobe Experience Manager Assets > Dokument hochladen
* HTTP

Andere Connectoren werden in zukünftigen Versionen unterstützt.

## Aktualisieren Sie Ihre Szenarien für die Verarbeitung großer Dateien

Das Modul Workfront > Dokument hochladen wurde geändert, um größere Dateien zu verarbeiten. Die frühere Version dieses Moduls zeigt nun &quot;`(Legacy)`&quot; an, das an den Modulnamen angehängt ist. In den meisten Fällen funktioniert das alte Modul weiterhin.

Wenn Sie mit größeren Dateien arbeiten möchten, empfehlen wir, das alte Modul durch das neue Modul Dokument hochladen zu ersetzen. Das neue Modul Dokument hochladen verhindert Timeouts und andere Fehler.

![Dokument hochladen](assets/new-upload-document.png)

## FAQs

### Was ist die neue Dateigrößenbeschränkung?

Benutzer können jetzt Dateien verarbeiten, die die vorherige 1 GB-Grenze überschreiten, was Effizienz und Produktivität steigert.  Obwohl die Plattform einzelne Dateien mit einer einzigen Aktion von bis zu 15 GB unterstützen kann (z. B. das Hochladen einer Datei), gibt es andere Faktoren, die sich auf die Datenübertragung auswirken. Die Dateigrößenbeschränkung für einzelne Aktionen hängt letztendlich vom Webdienst ab, mit dem Fusion eine Verbindung herstellt. Die Datenübertragung ist die Gesamtverarbeitung für eine einzelne Ausführung. Das bedeutet, dass mehrere Aktionen in einer Ausführung zur gesamten Datenübertragung beitragen.

Fusion verarbeitet Dateien, bis die Ausführungsgrenze von 40 Minuten erreicht ist. Große Dateien können in Ihrem Fusion-Szenario einige Zeit in Anspruch nehmen, um sie hochzuladen, herunterzuladen oder zu verarbeiten. Die Größe einzelner Dateien ist zwar nicht beschränkt, die Ausführungszeit eines Szenarios ist jedoch auf 40 Minuten begrenzt. Wenn daher große Dateien dazu führen, dass die Ausführung länger als 40 Minuten dauert, schlägt das Szenario fehl. Die Ausführungszeit eines Szenarios kann auch durch die Größe des Szenarios, die Komplexität des Moduls und die Netzwerkgeschwindigkeit beeinflusst werden. Daher empfehlen wir, diese Aspekte Ihrer Szenarien bei der Verwendung großer Dateien zu berücksichtigen.

### Wie funktioniert die neue Dateiübertragung von Fusion?

Bei der Verarbeitung von Dateien durch Fusion werden größere Dateien zu persistentem Speicher hinzugefügt (S3-Behälter oder Azure-Blob-Speicher). Wenn ein Fusion-Modul eine Dateiaktion wie den Upload oder Download ausführt, verwendet Fusion die Datei im persistenten Speicher als Quelle anstelle des aktiven Speichers.

### Kann ich mit größeren Dateien mit unvollständigen Ausführungen arbeiten?

Ja, Fusion unterstützt unvollständige Ausführungen mit größeren Dateien. Beachten Sie, dass unvollständige Ausführungen für eine Organisation begrenzt sind und aktiv verwaltet werden sollten.

### Kann ich größere Dateien mit einem beliebigen Connector verwenden?

Jeder Fusion-Connector muss aktualisiert werden, um größere Dateien zu unterstützen. Zu den unterstützten Connectoren gehören Workfront, HTTP und AEM Assets. Fusion-Connectoren sind weiterhin durch die vom Webdienst unterstützte Dateigröße begrenzt. Dateigrößenbeschränkungen sind normalerweise in der API-Dokumentation für Webdienst-Endpunkte enthalten, die Dateien herunterladen und hochladen.

### Hat dies Auswirkungen auf Vorgänge?

Nein, die Anzahl der von einem Modul ausgeführten Vorgänge ist identisch.

### Wann wird die Benutzeroberfläche von Fusion aktualisiert, um Dateiübertragungsdaten anzuzeigen?

Wir arbeiten aktiv an Aktualisierungen der Fusion-Benutzeroberfläche für die Dateiübertragung auf der Dashboard- und Szenario-Ausführungs-Detailseite mit einer gezielten Version im 1. Quartal 2025.

### Welche Möglichkeiten gibt es, über die neuen Dateiverarbeitungsbeschränkungen nachzudenken, die mir beim Entwerfen von Szenarien helfen?

Die Erstellung eines Szenarios, das innerhalb der Ausführungsgrenze von 40 Minuten funktioniert, kann kompliziert erscheinen. Es wird empfohlen, bei der Erstellung eines Szenarios Folgendes zu beachten:

* **Grundlegendes zu Ihren Geschäftsanforderungen für die Ausführungszeit**: Die Plattform-Beschränkung von Fusion für die Ausführungszeit beträgt 40 Minuten, aber die meisten Automatisierungen von Geschäftsprozessen werden voraussichtlich viel schneller ausgeführt. Beispielsweise wird erwartet, dass vom Benutzer initiierte Automatisierungen mit ergebnisabhängiger Kontinuität deutlich unter der 40-Minuten-Grenze abgeschlossen werden.
* **Berücksichtigen Sie die Ausführungszeit beim Entwerfen von**: Beim Entwerfen Ihres Szenarios ist es wichtig, die Ausführungszeit des Moduls für einzelne Dateiaktionen wie Uploads und Downloads zu verstehen. Dieses Wissen hilft Ihnen bei der Planung von Szenarien, die mehrere Dateiaktionen beinhalten.  Um die Genauigkeit in Ihrem Design sicherzustellen, empfehlen wir, die Ausführungszeit des Moduls so zu runden, dass ein Puffer eingefügt wird.
Wenn Fusion beispielsweise ein Dokument in 144 Sekunden (2,4 Minuten) herunterlädt, können Sie davon ausgehen, dass eine einzelne Ausführung ähnliche Aktionen mehrmals ausführen kann. In diesem Beispiel dauert die Ausführung des Moduls 144 Sekunden, und Sie sollten eine Ausführungsdauer von 3 Minuten für den Download planen. Wenn Ihre Anforderungen sowohl einen Upload als auch einen Download beinhalten, beträgt die erwartete Ausführungszeit ca. 6 Minuten. Beachten Sie, dass die Ausführungszeiten von Fusion auf 40 Minuten begrenzt sind.

* **Zusammenfassen von Dateiaktionen**: Das häufigste Beispiel für Dateiaktionen in einem Fusion-Szenario ist ein Download und ein Upload. Die meisten Szenarien mit nur diesen beiden Aktionen werden in wenigen Minuten ausgeführt. Wenn möglich, sollten Fusion-Designer ihre Szenarien auf einen Download und einen Upload beschränken.

* **Berechnen der Größe mithilfe des Zuordnungsbedienfelds**: Workfront und andere Webdienste schließen die Dateigröße einer Datei in die Ausgabe des Download-Moduls ein. Sie können diese Daten verwenden, um Dateien herauszufiltern, die für einen Modul-Upload zu groß oder für die Ausführungszeit des Szenarios zu groß sind.

* **Isolieren Sie Dateiaktionen in ihrem eigenen Szenario beim Arbeiten mit mehreren Dateien**: Fusion-Designer sollten erwägen, Dateiaktionen in separaten Szenarien zu isolieren. Beispielsweise kann ein Fusion-Szenario, das durch eine neue Workfront-Anfrage mit mehreren angehängten Dateien ausgelöst wird, bis zu 30 Dateien aufnehmen. Da das Hochladen und Herunterladen jeder Datei bis zu 3 Minuten dauern kann, würde die Verarbeitung aller Dateien in einer einzigen Ausführung die Ausführungsgrenze von 40 Minuten von Fusion überschreiten. Die Lösung besteht darin, ein Dateiaktionsszenario zu erstellen, das dem Upload und Download einzelner Dateien gewidmet ist. Das durch eine Anfrage ausgelöste Szenario würde durch die angehängten Dateien navigieren und das Dateiaktionsszenario für jede Datei mit dem HTTP-Modul aufrufen. Dadurch wird sichergestellt, dass jede Datei innerhalb der Ausführungszeiträume verarbeitet wird.

<!--
## Connectors that do not support large files

Some Fusion connectors do not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

The following connectors do **not** support large files. 

* Archive
* Box
* Convert
* CSV
* Datastores
* Flow control
* FTP
* JSON
* JWT
* Markdown
* Math
* Microsoft Word templates
* MIME
* Microsoft SQL
* SFTP
* Adobe Acrobat Sign
* SOAP
* Tools
* XML

If a connector is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.-->






<!--## Connectors that support large files

The following connectors support large files.

Workfront
HTTP
Webhooks
Salesforce
Microsoft Email
Workfront Proof
AEM Assets
Email
Slack
Jira
Microsoft Excel
SharePoint
Frame.io
Adobe PDF Services
Marketo
Azure Devops 
Google Email
Jira Server
Google Sheets
Microsoft OneDrive
ServiceNow 
AWS S3
Bynder
OneDrive Business
Adobe Authenticator
Google Drive
Microsoft Dynamics
Google Docs
NetSuite
Airtable
Azure AD
QuickBase 
Adobe Target
Adobe Campaign Classic
Microsoft Calendar
Workfront Planning
HubSpot CRM  
DropBox
Cloud Convert
Egnyte
Adobe Firefly
OpenAI / Chat GPT
Allocadia
Cvent
GitLab 
Google Team Drive
Google Calendar
Workfront SDL Managed Translation
Widen
Workfront Boards
Google Slides
Qualtrics
Microsoft Power BI
Adobe Photoshop
Anaplan
DocuSign 
MariaDB
Adobe Creative Cloud Libraries
Figma
AEM Forms
Datadog
GitHub 
Google Forms
Adobe I/O Events
Trello
Workday
Adobe Journey Optimizer
Adobe Lightroom


If a file is not on this list, it does not support large files. For these connectors, Fusion's total processing capacity for files is **1 GB**. 

This limit is based on a total memory cost. Every operation contributes to that cost. If a single file of 400 MB is downloaded and uploaded then the total cost to the file capacity would be 800 MB.

-->
