---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Hochladen von XD Artboards als Testsendungen in Workfront
description: Sie können Ihre Zeichenflächen als Testsendungen direkt in Adobe Workfront hochladen, um eine gründliche Überprüfung und Genehmigung zu erhalten.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4a7fb18674b399b138fd981907f3a9da8e0bb30e
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Hochladen [!DNL XD] Zeichenflächen als Testsendungen für [!DNL Workfront]

Sie können Ihre Zeichenflächen als Testsendungen direkt in [!DNL Adobe Workfront] für eine gründliche Überprüfung und Genehmigung.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Aktueller Plan: [!UICONTROL Pro] oder höher</p> <p>oder</p> <p>Veralteter Plan: [!UICONTROL Premium]</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Aktueller Plan: [!UICONTROL Work] oder [!UICONTROL Proof]</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über eine [!DNL Adobe Creative Cloud] zusätzlich zu einer [!DNL Workfront] Lizenz.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>[!UICONTROL Manager] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf [!UICONTROL Dokumente bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] oder [!DNL Workfront Proof] Administrator.

## Voraussetzungen

* Sie müssen die [!DNL Adobe Workfront for XD] Plug-in, bevor Sie Testsendungen in hochladen können [!DNL Adobe XD].

   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Hochladen eines statischen Testversands

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen statischen Testversand hochladen möchten.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste.

1. Klicken **[!UICONTROL Neue Datei]** im unteren Bereich des Plug-ins.
1. Wählen Sie die gewünschten Zeichenflächen aus.

   >[!TIP]
   >
   >Um mehr als eine Zeichenfläche auszuwählen, klicken Sie auf die gewünschte Zeichenfläche und ziehen Sie die Maus darüber.

1. Aktivieren **[!UICONTROL Erstellen eines Testversands]**.

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
        <li> <p>(Optional) Hinzufügen <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Übersicht über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Geben Sie einen Kommentar in das Feld **[!UICONTROL Updates]** Bereich.

   ![](assets/proof-approvals-xd-350x396.png)

1. Wählen Sie das Exportformat aus dem **[!UICONTROL Asset-Typ]** Dropdown-Menü.


1. (Optional) Wenn Sie als Asset-Typ PDF auswählen und mehr als eine Zeichenfläche ausgewählt haben, wählen Sie aus, ob Sie Ihre Zeichenflächen als **[!UICONTROL Einzelne PDF-Datei]s** oder **M[!UICONTROL Mehrere PDF-Dateien]**.

1. (Optional) Benennen Sie die PDF.

   ![](assets/pdf-options.png)

1. Klicken **[!UICONTROL Hochladen]**.\
   Das Dokument wird im [!UICONTROL Dokumente] -Bereich im Plug-in und im Desktop-Programm.

## Hochladen eines interaktiven Testversands {#upload-an-interactive-proof}

Sie können einen interaktiven Testversand für Ihre Zeichenflächen mit dem [!DNL Workfront for Adobe] Plug-in. Es handelt sich um einen zweistufigen Prozess. Zunächst müssen Sie einen interaktiven Link erstellen und dann den Testversand in ein Arbeitselement hochladen.

### Interaktiven Link für die Zeichenfläche erstellen  {#create-an-interactive-link-for-your-art-board}

1. Öffnen Sie die Zeichenfläche und klicken Sie auf **[!UICONTROL Freigeben]** im linken oberen Bereich des Bildschirms.
1. Geben Sie die Link-Einstellungen an:

   1. Benennen Sie den Link.
   1. Wählen Sie eine Ansichtseinstellung aus.
   1. Im **[!UICONTROL Link-Zugriff]** Abschnitt **[!UICONTROL Jeder mit diesem Link]** ausgewählt ist.

      Sie müssen diese Art von Zugriff aktivieren, um einen interaktiven Testversand zu erzeugen.

   1. Klicken **[!UICONTROL Link erstellen]**.

1. Klicken Sie zurück zu **[!UICONTROL Design]** im linken oberen Bereich des Bildschirms. Fahren Sie mit dem [Hochladen eines interaktiven Testversands](#upload-an-interactive-proof) unten.

   >[!NOTE]
   >
   >Möglicherweise müssen Sie das Plug-in-Bedienfeld in der linken unteren Ecke des Bildschirms erneut öffnen.

### Hochladen eines interaktiven Testversands

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen interaktiven Testversand hochladen möchten.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste.

1. Klicken **[!UICONTROL Neue Datei]** im unteren Bereich des Plug-ins.
1. Aktivieren **[!UICONTROL Erstellen eines Testversands]**.

1. Wählen Sie den gewünschten Typ der Testversandvalidierung aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>Grundlegende Genehmigungsprozesse sind Ad-hoc-Prozesse und können bei Bedarf verschiedene Validierungsverantwortliche umfassen: </p> 
       <ul> 
        <li> <p>(Optional) Hinzufügen <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Übersicht über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Geben Sie einen Kommentar in das Feld **[!UICONTROL Updates]** Bereich.

   ![](assets/proof-approvals-xd-350x396.png)

1. Im **[!UICONTROL Asset-Typ]** im Dropdown-Menü den soeben erstellten Link unter **Freigegebene Links** Registerkarte. Weitere Informationen finden Sie unter [Interaktiven Link für die Zeichenfläche erstellen](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Klicken **[!UICONTROL Hochladen]**.

   Das Dokument wird im [!UICONTROL Dokumente] -Bereich im Plug-in und im Desktop-Programm.

   >[!IMPORTANT]
   >
   >Benutzer müssen Zugriff auf die [!UICONTROL Desktop Proofing Viewer] um interaktive Testsendungen zu überprüfen und zu genehmigen. Weitere Informationen finden Sie unter [Installieren Sie die [!UICONTROL Desktop Proofing Viewer]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Eine neue Testversion hochladen

Sie können eine neue Version eines Testversands hochladen. Das Plug-in speichert den in der vorherigen Version festgelegten Testversand-Workflow, kann diesen jedoch bei Bedarf ändern.

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/menu-350x440.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie ein Dokument hochladen müssen.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png)in der Navigationsleiste.

1. Klicken **[!UICONTROL Neue Version]** im unteren Bereich des Plug-ins.
1. Aktivieren **[!UICONTROL Erstellen eines Testversands]**.
1. Wählen Sie die gewünschten Zeichenflächen aus.

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
        <li> <p>(Optional) Hinzufügen <strong>Genehmiger</strong> in das Feld ein.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Die automatisierten Genehmigungsprozesse werden von Administratoren vorkonfiguriert und umfassen spezifische Validierer und Phasen. Weitere Informationen finden Sie unter <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Übersicht über den automatisierten Workflow</a>.</p> 
       <ul> 
        <li> <p>Wählen Sie eine [!UICONTROL Workflow-Vorlage] aus dem Dropdown-Menü aus.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wählen Sie das Exportformat aus dem **[!UICONTROL Asset-Typ]** Dropdown-Menü.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Optional) Geben Sie einen Kommentar in das Feld **[!UICONTROL Updates]** Bereich.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Optional) Wenn Sie als Asset-Typ PDF auswählen und mehr als eine Zeichenfläche ausgewählt haben, wählen Sie aus, ob Sie Ihre Zeichenflächen als **[!UICONTROL Einzelne PDF-Datei]s** oder **M[!UICONTROL Mehrere PDF-Dateien]**.

1. (Optional) Benennen Sie die PDF.

   ![](assets/pdf-options.png)

1. Klicken **[!UICONTROL Hochladen]**.\
   Das Dokument wird im [!UICONTROL Dokumente] -Bereich im Plug-in und im Desktop-Programm.
