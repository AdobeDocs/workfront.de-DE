---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen von XD-Zeichenflächen als Dokumente in Workfront
description: Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in Adobe Workfront zu speichern.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 1%

---


# Hochladen [!DNL XD] Zeichenflächen als Dokumente in [!DNL Workfront]

Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in [!DNL Adobe Workfront] zu speichern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td>Sie müssen zusätzlich zu einer [!DNL Workfront] über eine [!DNL Adobe Creative Cloud]-Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf [!UICONTROL -Dokumente] bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] Zugriff oder höher auf das Objekt, in das Sie ein Dokument hochladen möchten.</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

* Sie müssen das [!DNL Adobe Workfront for XD]-Plug-in installieren, bevor Sie XD-Artboards als Dokumente in Workfront hochladen können.

Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Neues Dokument hinzufügen

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Menüsymbol](assets/menu-350x440.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie ein Dokument hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie **[!UICONTROL Neue Datei]** unten im Plug-in.
1. Wählen Sie die Zeichenfläche aus, die Sie hochladen möchten.

   >[!TIP]
   >
   >Um mehrere Zeichenflächen auszuwählen, klicken Sie auf die gewünschten Zeichenflächen und ziehen Sie die Maus darüber.
1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.
1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Exportformat]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Die Zeichenflächen werden als PNG in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Die Zeichenflächen werden als JPG in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenflächen werden als SVG in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Wählen Sie aus, ob die ausgewählten Zeichenflächen als <strong>Einzelne PDF-Datei</strong> oder <strong>Mehrere PDF-Dateien</strong> hochgeladen werden sollen. Die Zeichenflächen werden als PDF auf die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen.</td>
     </tr>
    </tbody>
   </table>


1. Klicken Sie **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.

## Neue Version hinzufügen

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Menüsymbol](assets/menu-350x440.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie ein Dokument hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument-Symbol](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie auf das Dokument, dem Sie eine neue Version hinzufügen möchten.
1. Klicken Sie **[!UICONTROL Neue Version]** am unteren Rand des Plug-ins.
1. Wählen Sie die Zeichenflächen aus, die Sie hochladen möchten.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version einer SVG, PNG oder JPG hochladen möchten, können Sie nur eine Zeichenfläche hochladen.

1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.

1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Exportformat</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Die Zeichenfläche wird als PNG in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Die Zeichenfläche wird als JPG auf die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenfläche wird als SVG auf die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Die Zeichenflächen werden als PDF in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen.</p>
      <p><strong>Hinweis</strong>: Für eine neue Dokumentversion kann nur eine Zeichenfläche hochgeladen werden.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.
