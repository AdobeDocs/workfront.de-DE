---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen von Testsendungen aus Adobe Photoshop
description: Sie können Ihre Kunstboards direkt als Testsendungen in Adobe Workfront hochladen, um eine gründliche Überprüfung und Genehmigung zu erhalten.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 66186bb8af14e7ce86b3fb5e8bb1b07fe32dca7a
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Hochladen von Testsendungen aus [!DNL Photoshop]

Sie können Ihre Kunstboards direkt als Testsendungen in [!DNL Adobe Workfront] für eine gründliche Überprüfung und Genehmigung.

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
   <td> <p>Aktueller Plan: [!UICONTROL Work] oder [!UICONTROL Proof]</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über eine [!DNL Adobe Creative Cloud] zusätzlich zu einer [!DNL Workfront] -Lizenz.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>[!UICONTROL Manager] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf [!UICONTROL Dokumente bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Voraussetzungen

* Sie müssen installieren [!DNL Adobe Workfront for Photoshop] vor dem Hochladen von Testsendungen aus [!DNL Adobe Photoshop].

  Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Hochladen eines einfachen Testversands

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen Testversand hochladen möchten.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste.
1. Klicks **[!UICONTROL Neue Datei]** unten im [!DNL Workfront] Bedienfeld.
1. Aktivieren Sie die **[!UICONTROL Erstellen eines Testversands]** umschalten.
1. (Optional) Geben Sie einen Namen für den Testversand im **[!UICONTROL Testname]** Textfeld.
1. Im **[!UICONTROL Testgenehmigungen]** Bereich, wählen Sie **[!UICONTROL Allgemein]**.
1. (Optional) Fügen Sie Genehmiger hinzu.
1. (Optional) Geben Sie einen Kommentar in die **[!UICONTROL Updates]** Bereich.

   ![](assets/add-comment.png)

1. Wählen Sie die **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü.

1. (Optional) Wählen Sie **[!UICONTROL Externe Datei hinzufügen]** , um eine Datei von Ihrem Computer hinzuzufügen.
1. Klicks **[!UICONTROL Hochladen]** und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.

   ![](assets/plugin-files-350x307.png)\
   Das Dokument wird im [!UICONTROL Dokumente] -Gebiet [!DNL Workfront] Bedienfeld in [!DNL Photoshop] und im [!DNL Workfront] Desktop-Programm.


## Hochladen eines automatisierten Testversands

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Gehen Sie zum Arbeitselement, in das Sie einen Testversand hochladen möchten.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste.

1. Klicks **[!UICONTROL Neue Datei]** unten im [!DNL Workfront] Bedienfeld.
1. Aktivieren Sie die **[!UICONTROL Erstellen eines Testversands]** umschalten.
1. (Optional) Geben Sie einen Namen für den Testversand im **[!UICONTROL Testname]** Textfeld.
1. Im **[!UICONTROL Testgenehmigungen]** Bereich, wählen Sie **[!UICONTROL Automatisiert]**.
1. (Optional) Im **[!UICONTROL Workflow-Vorlage]** Geben Sie den Namen einer Testversand-Workflow-Vorlage ein.

{{adjust-proof-settings}}

>[!NOTE]
>
> Wenn die Workflow-Vorlage leere erforderliche Felder enthält, werden die automatisierten Testversandeinstellungen automatisch geöffnet. Sie müssen diese Felder ausfüllen, um den Testversand hochzuladen.


1. (Optional) Geben Sie einen Kommentar in die **[!UICONTROL Updates]** Bereich.

   ![](assets/add-comment-automated-approval.png)

1. Wählen Sie die **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü.
1. (Optional) Wählen Sie **[!UICONTROL Externe Datei hinzufügen]** , um eine Datei von Ihrem Computer hinzuzufügen.
1. Klicks **[!UICONTROL Hochladen]**und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.
Das Dokument wird im [!UICONTROL Dokumente] -Gebiet [!DNL Workfront] Bedienfeld in [!DNL Photoshop] und im [!DNL Workfront] Desktop-Programm.

## Eine neue Testversion hochladen

Sie können eine neue Version eines Testversands hochladen. Das Plug-in speichert den in der vorherigen Version festgelegten Testversand-Workflow, kann diesen jedoch bei Bedarf ändern.

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie ein Dokument hochladen müssen.
1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png)in der Navigationsleiste.

1. Klicks **[!UICONTROL Neue Version]** unten im [!DNL Workfront] Bedienfeld.
1. Aktivieren Sie die **[!UICONTROL Erstellen eines Testversands]** umschalten.

1. Im *[!UICONTROL *Testversandgenehmigungen]** Abschnitt, wählen Sie **[!UICONTROL Allgemein]** oder **[!UICONTROL Automatisiert]**.

1. Hinzufügen **[!UICONTROL Überprüfer]** oder **[!UICONTROL Workflow-Vorlage]** basierend auf dem in Schritt 7 ausgewählten Validierungstyp.

1. (Optional) Geben Sie einen Kommentar in die **[!UICONTROL Updates]** Bereich.
1. Wählen Sie die **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü.
1. Klicks **[!UICONTROL Hochladen]**und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.
Das Dokument wird im [!UICONTROL Dokumente] -Gebiet [!DNL Workfront] Bedienfeld in [!DNL Photoshop] und im [!DNL Workfront] Desktop-Programm.
