---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: connections-annd-webhooks
title: Erstellen Sie Verbindungen in [!DNL Adobe Workfront Fusion]
description: Eine Verbindung muss den Anforderungen entsprechen, die von der API der App oder des Webservices festgelegt werden, mit der bzw. dem sie eine Verbindung herstellt. Aus diesem Grund variieren die Anweisungen zum Einrichten einer Verbindung je nach App oder Webservice. Dieser Artikel kann Ihnen dabei helfen, die Anweisungen zum Verbinden von mit  [!DNL Adobe Workfront Fusion]  ausgewählten App oder dem ausgewählten Webservice zu identifizieren und zu finden.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# Erstellen von Verbindungen in [!DNL Adobe Workfront Fusion]

<!-- Audited: 3/2024-->

Eine Verbindung muss den Anforderungen entsprechen, die von der API der App oder des Webservices festgelegt werden, mit der bzw. dem sie eine Verbindung herstellt. Aus diesem Grund variieren die Anweisungen zum Einrichten einer Verbindung je nach App oder Webservice. Dieser Artikel kann Ihnen dabei helfen, die Anweisungen zum Verbinden von [!DNL Adobe Workfront Fusion] mit der ausgewählten App oder dem ausgewählten Webservice zu identifizieren und zu finden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Beliebig</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p> 
   <p>Oder</p> 
   <p>Legacy: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Herstellen einer Verbindung zu einer Anwendung oder einem Webdienst, für die/den keine Konfiguration erforderlich ist

In den meisten Fällen können Sie das Modul verwenden, um eine Verbindung mit wenigen oder keinen zusätzlichen Informationen zu erstellen. [!DNL Workfront Fusion] verarbeitet die Authentifizierung automatisch.

Anweisungen zum Erstellen einer Verbindung ohne besondere Überlegungen finden Sie unter [Verbindung herstellen mit [!DNL Adobe Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Herstellen einer Verbindung zu einer [!DNL Microsoft] App oder einem Webdienst

Die meisten [!DNL Microsoft]-Apps in [!DNL Workfront Fusion] ermöglichen es Ihnen, eine Verbindung ohne zusätzliche Informationen zu erstellen.

Die folgenden Umstände erfordern beim Erstellen einer Verbindung zusätzliche Schritte:

* Verwenden von [!DNL Microsoft Dynamics 365].

  Anweisungen finden Sie unter [[!DNL Microsoft Dynamics 365] Module](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Herstellen einer Verbindung zum [!DNL Microsoft Graph API] über ein [!UICONTROL HTTP]-Modul

  Anweisungen finden Sie unter [Aufrufen der  [!DNL MS Graph REST API]  über das  [!DNL Adobe Workfront Fusion] [!UICONTROL -] > [!UICONTROL OAuth 2.0-Anfrage ])](../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Herstellen einer Verbindung zu einer [!DNL Google] App oder einem Webdienst

Der Prozess zum Herstellen einer Verbindung zu [!DNL Google] Apps kann je nach Art des von Ihnen verwendeten [!DNL Google]-Kontos unterschiedlich sein. Darüber hinaus müssen [!DNL Google] Sicherheitsmaßnahmen möglicherweise zusätzlich konfiguriert werden, wenn Sie eine Verbindung zu [!DNL Workfront Fusion] herstellen.

Weitere Informationen finden Sie unter:

* [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Verbindung  [!DNL Adobe Workfront Fusion] / [!DNL Google Services]  mit aktualisierten Sicherheitsmaßnahmen](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Andere Apps, für die eine zusätzliche Konfiguration erforderlich ist

Die folgenden Apps folgen nicht der Basiskonfiguration für [!DNL Workfront Fusion]. Anweisungen zum Verbinden dieser Apps finden Sie im Artikel zu dieser App.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App/Web-Service</th> 
   <th>Zusätzliche Informationen zu Verbindungen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Adobe Workfront] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Allocadia] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] Modulen</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Verbinden von [!DNL AWS] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Verbinden von [!DNL CloudConvert] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] Modulen</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Datadog] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Verbinden von [!DNL DocuSign] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-Mail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Verbinden Sie Ihre E-Mail mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL E-Mail]-Modulen</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Jira Cloud] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Verbinden von [!DNL Jira Server] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Verbinden von [!DNL MariaDB] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Marketo] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Verbinden von [!DNL Qualtrics] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Verbinden von [!DNL ServiceNow] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP]-Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Verbinden von [!DNL SharePoint] mit [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] Modulen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Verbreitern</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] Modulen</a></td> 
  </tr> 
 </tbody> 
</table>
