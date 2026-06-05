---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen von XD-Zeichenflächen als Dokumente in Workfront
description: Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in Adobe Workfront zu speichern.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/WZAXsygXZTnW7VeLoNH-3vVTIwluZuCaf2iQrEjs6UE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 533
ht-degree: 8%

---

# Hochladen [!DNL XD] Zeichenflächen als Dokumente in [!DNL Workfront]

Sie können Ihre Zeichenflächen als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in [!DNL Adobe Workfront] zu speichern.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
    <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr>
  -->
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Workfront] über eine [!DNL Adobe Creative Cloud]-Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf [!UICONTROL -Dokumente] bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] Zugriff oder höher auf das Objekt, in das Sie ein Dokument hochladen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
      <td>Die Zeichenflächen werden als JPG in die Registerkarte [!UICONTROL -Dokumente] des Arbeitselements in [!DNL Workfront] hochgeladen. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenflächen werden als SVG in die Registerkarte [!UICONTROL -Dokumente] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Wählen Sie aus, ob die ausgewählten Zeichenflächen als <strong>Einzelne PDF-Datei</strong> oder <strong>Mehrere PDF-Dateien</strong> hochgeladen werden sollen. Die Zeichenflächen werden als PDF in die Registerkarte [!UICONTROL Documents] des Arbeitselements in [!DNL Workfront] hochgeladen.</td>
     </tr>
    </tbody>
   </table>


1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
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
   >Wenn Sie eine neue Version eines SVG, PNG oder JPG hochladen möchten, können Sie nur eine einzige Zeichenfläche hochladen.

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
      <td>Die Zeichenfläche wird in [!DNL Workfront] als JPG in die Registerkarte [!UICONTROL -Dokumente] des Arbeitselements hochgeladen. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Die Zeichenfläche wird als SVG in die Registerkarte [!UICONTROL -Dokumente] des Arbeitselements in [!DNL Workfront] hochgeladen. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Die Zeichenflächen werden als PDF in die Registerkarte [!UICONTROL -Dokumente] des Arbeitselements in [!DNL Workfront] hochgeladen.</p>
      <p><strong>Hinweis</strong>: Für eine neue Dokumentversion kann nur eine Zeichenfläche hochgeladen werden.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.
