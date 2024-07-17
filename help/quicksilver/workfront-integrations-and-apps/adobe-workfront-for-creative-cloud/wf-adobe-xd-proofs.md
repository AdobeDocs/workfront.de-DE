---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Hochladen von XD Artboards als Testsendungen in Workfront
description: Sie können Ihre Zeichenflächen als Testsendungen direkt in Adobe Workfront hochladen, um eine gründliche Überprüfung und Genehmigung zu erhalten.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d5255968a96452d9501a285408f67be7da10d933
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL XD] Zeichenflächen als Testsendungen in [!DNL Workfront] hochladen

Sie können Ihre Zeichenflächen direkt als Testsendungen in [!DNL Adobe Workfront] hochladen, um eine gründliche Überprüfung und Genehmigung zu erhalten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Aktueller Plan: [!UICONTROL Pro] oder höher</p> <p>oder</p> <p>Veralteter Plan: [!UICONTROL Premium]</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Aktueller Plan: [!UICONTROL Work] oder [!UICONTROL Proof]</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Workfront] -Lizenz über eine [!DNL Adobe Creative Cloud] -Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>[!UICONTROL Manager] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf [!UICONTROL Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] - oder [!DNL Workfront Proof] -Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Berechtigung zum Testen haben.

## Voraussetzungen

* Sie müssen das Plug-in [!DNL Adobe Workfront for XD] installieren, bevor Sie Testsendungen in [!DNL Adobe XD] hochladen können.

  Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Hochladen eines statischen Testversands

1. Klicken Sie oben rechts auf das Symbol **[!UICONTROL Menü]** und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen statischen Testversand hochladen möchten.
1. Klicken Sie in der Navigationsleiste auf das Symbol **[!UICONTROL Dokument]** ![](assets/documents.png) .

1. Klicken Sie unten im Plug-in auf **[!UICONTROL Neue Datei]** .
1. Wählen Sie die hochzuladenden Zeichenflächen aus.

   >[!TIP]
   >
   >* Die Zeichenflächen werden im Testversand in der Reihenfolge angezeigt, in der sie ausgewählt wurden. Die erste ausgewählte Zeichenfläche ist die erste Seite im Testversand usw.
   >* Um schnell mehr als eine Zeichenfläche auszuwählen, klicken Sie auf und ziehen Sie die Maus über die gewünschten Zeichenflächen. Auf diese Weise können Sie die Reihenfolge der Zeichenflächen im Testversand nicht steuern.

1. Aktivieren Sie **[!UICONTROL Erstellen eines Testversands]**.

1. Nennen Sie den Testversand.

1. Wählen Sie den gewünschten Typ der Testversandvalidierung aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Grundlegende Genehmigungsprozesse sind Ad-hoc-Prozesse und können bei Bedarf verschiedene Validierungsverantwortliche umfassen: </p> 
       <ul> 
        <li> <p>(Optional) Fügen Sie <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Überblick über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optional) Geben Sie einen Kommentar in den Bereich **[!UICONTROL Aktualisierungen]** ein.

   ![](assets/proof-approvals-xd-350x396.png)

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Asset-Typ]** das Exportformat aus.


1. (Optional) Wenn Sie PDF als Asset-Typ auswählen und mehr als eine Zeichenfläche ausgewählt haben, wählen Sie aus, ob Sie Ihre Zeichenflächen als **[!UICONTROL Einzelne PDF-Datei]s** oder als **M[!UICONTROL mehrere PDF-Dateien]** exportieren möchten.

1. (Optional) Benennen Sie die PDF.

   ![](assets/pdf-options.png)

1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.

## Hochladen eines interaktiven Testversands {#upload-an-interactive-proof}

Mit dem Plug-in [!DNL Workfront for Adobe] können Sie einen interaktiven Testversand für Ihre Zeichenflächen erstellen. Es handelt sich um einen zweistufigen Prozess. Zunächst müssen Sie einen interaktiven Link erstellen und dann den Testversand in ein Arbeitselement hochladen.

### Interaktiven Link für die Zeichenfläche erstellen  {#create-an-interactive-link-for-your-art-board}

1. Öffnen Sie die Zeichenfläche und klicken Sie dann im linken oberen Bereich des Bildschirms auf **[!UICONTROL Freigabe]** .
1. Geben Sie die Link-Einstellungen an:

   1. Benennen Sie den Link.
   1. Wählen Sie eine Anzeigeeinstellung aus.
   1. Stellen Sie im Abschnitt **[!UICONTROL Link-Zugriff]** sicher, dass **[!UICONTROL Jeder, der über diesen Link verfügt]** ausgewählt ist.

      Sie müssen diese Art von Zugriff aktivieren, um einen interaktiven Testversand zu erzeugen.

   1. Klicken Sie auf **[!UICONTROL Link erstellen]**.

1. Klicken Sie im linken oberen Bereich des Bildschirms wieder auf **[!UICONTROL Design]** . Fahren Sie mit dem Abschnitt [Hochladen eines interaktiven Testversands](#upload-an-interactive-proof) weiter unten fort.

   >[!NOTE]
   >
   >Möglicherweise müssen Sie das Plug-in-Bedienfeld in der linken unteren Ecke des Bildschirms erneut öffnen.

### Hochladen eines interaktiven Testversands

1. Klicken Sie oben rechts auf das Symbol **[!UICONTROL Menü]** und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen interaktiven Testversand hochladen möchten.
1. Klicken Sie in der Navigationsleiste auf das Symbol **[!UICONTROL Dokument]** ![](assets/documents.png) .

1. Klicken Sie unten im Plug-in auf **[!UICONTROL Neue Datei]** .
1. Aktivieren Sie **[!UICONTROL Erstellen eines Testversands]**.

1. Wählen Sie den gewünschten Typ der Testversandvalidierung aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Grundlegende Genehmigungsprozesse sind Ad-hoc-Prozesse und können bei Bedarf verschiedene Validierungsverantwortliche umfassen: </p> 
       <ul> 
        <li> <p>(Optional) Fügen Sie <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Überblick über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optional) Geben Sie einen Kommentar in den Bereich **[!UICONTROL Aktualisierungen]** ein.

   ![](assets/proof-approvals-xd-350x396.png)

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Asset-Typ]** den soeben erstellten Link auf der Registerkarte **Freigegebene Links** aus. Weitere Informationen finden Sie unter [Interaktiven Link für Ihre Zeichenfläche erstellen](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Klicken Sie auf **[!UICONTROL Hochladen]**.

   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.

   >[!IMPORTANT]
   >
   >Benutzer müssen Zugriff auf den [!UICONTROL Desktop Proofing Viewer] haben, um interaktive Testsendungen zu überprüfen und zu genehmigen. Weitere Informationen finden Sie unter [Installieren des [!UICONTROL Desktop-Proofing-Viewers]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Eine neue Testversion hochladen

Sie können eine neue Version eines Testversands hochladen. Das Plug-in speichert den in der vorherigen Version festgelegten Testversand-Workflow, kann diesen jedoch bei Bedarf ändern.

1. Klicken Sie oben rechts auf das Symbol **[!UICONTROL Menü]** und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie ein Dokument hochladen müssen.
1. Klicken Sie in der Navigationsleiste auf das Symbol **[!UICONTROL Dokument]** ![](assets/documents.png) .

1. Klicken Sie unten im Plug-in auf **[!UICONTROL Neue Version]** .
1. Aktivieren Sie **[!UICONTROL Erstellen eines Testversands]**.
1. Wählen Sie die hochzuladenden Zeichenflächen aus.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version von .svg, .png oder .jpg hochladen möchten, können Sie nur eine Zeichenfläche hochladen.

1. Wählen Sie den gewünschten Typ der Testversandvalidierung aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Grundlegende Genehmigungsprozesse sind Ad-hoc-Prozesse und können bei Bedarf verschiedene Validierungsverantwortliche umfassen: </p> 
       <ul> 
        <li> <p>(Optional) Fügen Sie <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Überblick über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Asset-Typ]** das Exportformat aus.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Optional) Geben Sie einen Kommentar in den Bereich **[!UICONTROL Aktualisierungen]** ein.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Optional) Wenn Sie PDF als Asset-Typ auswählen und mehr als eine Zeichenfläche ausgewählt haben, wählen Sie aus, ob Sie Ihre Zeichenflächen als **[!UICONTROL Einzelne PDF-Datei]s** oder als **M[!UICONTROL mehrere PDF-Dateien]** exportieren möchten.

1. (Optional) Benennen Sie die PDF.

   ![](assets/pdf-options.png)

1. Klicken Sie auf **[!UICONTROL Hochladen]**.\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.
