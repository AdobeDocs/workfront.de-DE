---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Arbeiten mit großen Dateien in Adobe Workfront Fusion
description: Große Dateiunterstützung ist derzeit für die Workfront- und HTTP-Connectoren verfügbar.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 630467ca64281df0b257dae8cc5c6edc55ae56ad
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Arbeiten mit großen Dateien in Adobe Workfront Fusion

Einige Fusion-Connectoren unterstützen Dateien mit einer Größe von mehr als 1 GB.

## Connectoren, die große Dateien unterstützen

Die Unterstützung großer Dateien ist derzeit für die folgenden Connectoren verfügbar:

* Workfront
* HTTP

## Auswirkungen auf die große Dateigröße auf die Ausführungszeit eines Szenarios

Große Dateien können in Ihrem Fusion-Szenario einige Zeit in Anspruch nehmen, um sie hochzuladen, herunterzuladen oder zu verarbeiten. Die Dateigröße ist zwar nicht begrenzt, die Ausführungszeit eines Szenarios ist jedoch auf 40 Minuten begrenzt. Wenn daher große Dateien dazu führen, dass die Ausführung länger als 40 Minuten dauert, schlägt das Szenario fehl.

Die Ausführungszeit eines Szenarios kann auch durch die Größe des Szenarios, die Komplexität des Moduls und die Netzwerkgeschwindigkeit beeinflusst werden. Daher empfehlen wir, diese Aspekte Ihrer Szenarien bei der Verwendung großer Dateien zu berücksichtigen.


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