---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen XD Zeichenflächen als Dokumente in Workfront
description: Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in Adobe Workfront zu speichern.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# [!DNL XD] Zeichenflächen als Dokumente in [!DNL Workfront] hochladen

Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in [!DNL Adobe Workfront] zu speichern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Workfront] -Lizenz über eine [!DNL Adobe Creative Cloud] -Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf [!UICONTROL Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf die [!UICONTROL Ansicht] oder höher auf das Objekt, in das Sie ein Dokument hochladen möchten.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

* Sie müssen das Plug-in [!DNL Adobe Workfront for XD] installieren, bevor Sie XD Artboards als Dokumente in Workfront hochladen können.

Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Neues Dokument hinzufügen

1. Klicken Sie oben rechts auf das Symbol **[!UICONTROL Menü]** und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Wechseln Sie zum Arbeitselement, in das Sie ein Dokument hochladen möchten.
1. Klicken Sie in der Navigationsleiste auf das Symbol **[!UICONTROL Dokument]** ![](assets/documents.png) .

1. Klicken Sie unten im Plug-in auf **[!UICONTROL Neue Datei]** .
1. Wählen Sie die Zeichenfläche aus, die Sie hochladen möchten.

   >[!TIP]
   >
   >Um mehr als eine Zeichenfläche auszuwählen, klicken Sie auf die gewünschte Zeichenfläche und ziehen Sie die Maus darüber.
1. (Optional) Geben Sie einen Kommentar in den Bereich **[!UICONTROL Aktualisierungen]** ein.
1. Wählen Sie den **[!UICONTROL Asset-Typ]** aus dem Dropdownmenü aus:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Exportformat]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Die Zeichenflächen laden als PNG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Die Zeichenflächen laden als JPG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenflächen laden als SVG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Wählen Sie aus, ob die ausgewählten Zeichenflächen als <strong>einzelne PDF-Datei</strong> oder als <strong>Mehrere PDF-Dateien</strong> hochgeladen werden sollen. Die Zeichenflächen werden als PDF auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hochgeladen.</td>
     </tr>
    </tbody>
   </table>


1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.

## Hinzufügen einer neuen Version

1. Klicken Sie oben rechts auf das Symbol **[!UICONTROL Menü]** und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Wechseln Sie zum Arbeitselement, in das Sie ein Dokument hochladen möchten.
1. Klicken Sie in der Navigationsleiste auf das Symbol **[!UICONTROL Dokument]** ![](assets/documents.png) .

1. Klicken Sie auf das Dokument, dem Sie eine neue Version hinzufügen möchten.
1. Klicken Sie unten im Plug-in auf **[!UICONTROL Neue Version]** .
1. Wählen Sie die hochzuladenden Zeichenflächen aus.

   >[!NOTE]
   >
   >Wenn Sie eine neue SVG-, PNG- oder JPG-Version hochladen möchten, können Sie nur eine Zeichenfläche hochladen.

1. (Optional) Geben Sie einen Kommentar in den Bereich **[!UICONTROL Aktualisierungen]** ein.

1. Wählen Sie den **[!UICONTROL Asset-Typ]** aus dem Dropdownmenü aus:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Exportformat</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Die Zeichenfläche lädt als PNG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Die Zeichenfläche lädt als JPG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenfläche lädt als SVG auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Die Zeichenflächen laden als PDF auf die Registerkarte [!UICONTROL Dokumente] des Arbeitselements in [!DNL Workfront] hoch.</p>
      <p><strong>Hinweis</strong>: Sie können nur eine Zeichenfläche für eine neue Dokumentversion hochladen.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.
