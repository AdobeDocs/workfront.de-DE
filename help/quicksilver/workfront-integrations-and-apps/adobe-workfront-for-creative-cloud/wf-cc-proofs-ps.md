---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen von Testsendungen aus Adobe Photoshop
description: Sie können Fotodokumentvorgaben als Korrekturabzüge direkt in hochladen [!DNL Adobe Workfront]  um eine gründliche Überprüfung und Genehmigung zu erhalten.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
TQID: https://experienceleague.adobe.com/gV7TwIUpXsu4wBBb31QE2ADnvZ6vWXtwQBvFGPYt73Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 625
ht-degree: 5%

---

# Hochladen von Testsendungen aus [!DNL Photoshop]

Sie können bestimmte Photoshop-Dokumentvorgabentypen als Korrekturabzüge direkt in [!DNL Adobe Workfront] hochladen, um sie gründlich zu überprüfen und zu genehmigen.

>[!IMPORTANT]
>
>Bei der Datei muss es sich um eine Fotodokumentvorgabe handeln, wie unter [Vorlagen und Vorgaben in Photoshop](https://helpx.adobe.com/de/photoshop/using/create-documents.html) beschrieben.



## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td> Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Standard</p>
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Workfront] über eine [!DNL Adobe Creative Cloud]-Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturabzug-Berechtigungsprofil </td> 
   <td>[!UICONTROL Manager] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf [!UICONTROL -Dokumente] bearbeiten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

* Sie müssen [!DNL Adobe Workfront for Photoshop] installieren, bevor Sie Korrekturabzüge von [!DNL Adobe Photoshop] hochladen können.

  Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Hochladen eines einfachen Korrekturabzugs

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie einen Korrekturabzug hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument](assets/documents.png) in der Navigationsleiste.
1. Klicken Sie **[!UICONTROL Neue Datei]** am unteren Rand des [!DNL Workfront] Bedienfelds.
1. Aktivieren Sie den **[!UICONTROL Korrekturabzug erstellen]**.
1. (Optional) Geben Sie einen Namen für den Korrekturabzug in das Textfeld **[!UICONTROL Korrekturabzugsname]** ein.
1. Wählen Sie im **[!UICONTROL Korrekturabzugsgenehmigungen]** die Option **[!UICONTROL Standard]** aus.
1. (Optional) Fügen Sie genehmigende Personen hinzu.
1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.

   ![Kommentar hinzufügen](assets/add-comment.png)

1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus.

1. (Optional) Wählen Sie **[!UICONTROL Externe Datei hinzufügen]**, um eine Datei von Ihrem Computer hinzuzufügen.
1. Klicken Sie **[!UICONTROL Hochladen]** und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.

   ![Dateien im Plug-in](assets/plugin-files-350x307.png)\
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im [!DNL Workfront] in [!DNL Photoshop] und im [!DNL Workfront]-Desktop-Programm angezeigt.


## Hochladen eines automatisierten Korrekturabzugs

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie einen Korrekturabzug hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie **[!UICONTROL Neue Datei]** am unteren Rand des [!DNL Workfront] Bedienfelds.
1. Aktivieren Sie den **[!UICONTROL Korrekturabzug erstellen]**.
1. (Optional) Geben Sie einen Namen für den Korrekturabzug in das Textfeld **[!UICONTROL Korrekturabzugsname]** ein.
1. Wählen Sie im **[!UICONTROL Korrekturabzugsgenehmigungen]** die Option **[!UICONTROL Automated]** aus.
1. (Optional) Geben Sie in das Feld **[!UICONTROL Workflow]** Vorlage) den Namen einer Workflow-Vorlage für Korrekturabzüge ein.

{{adjust-proof-settings}}

>[!NOTE]
>
> Wenn die Workflow-Vorlage leere Pflichtfelder enthält, werden die Einstellungen für automatisierte Korrekturabzüge automatisch geöffnet. Diese Felder müssen ausgefüllt werden, damit der Korrekturabzug hochgeladen werden kann.


1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.

   ![Kommentar hinzufügen - automatisierte Genehmigung](assets/add-comment-automated-approval.png)

1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus.
1. (Optional) Wählen Sie **[!UICONTROL Externe Datei hinzufügen]**, um eine Datei von Ihrem Computer hinzuzufügen.
1. Klicken Sie **[!UICONTROL Hochladen]** und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.
Das Dokument wird im Bereich [!UICONTROL Dokumente] im [!DNL Workfront] in [!DNL Photoshop] und im [!DNL Workfront]-Desktop-Programm angezeigt.

## Hochladen einer neuen Korrekturabzugsversion

Sie können eine neue Version eines Korrekturabzugs hochladen. Das Plug-in speichert den Korrekturabzugs-Workflow, der für die vorherige Version festgelegt wurde. Sie können dies jedoch bei Bedarf ändern.

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, auf das Sie ein Dokument hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument-Symbol](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie **[!UICONTROL Neue Version]** am unteren Rand des [!DNL Workfront] Bedienfelds.
1. Aktivieren Sie den **[!UICONTROL Korrekturabzug erstellen]**.

1. Wählen Sie im Abschnitt *[!UICONTROL *Korrekturabzugsgenehmigungen]* die Option **[!UICONTROL Standard]** oder **[!UICONTROL Automated]**.

1. Fügen Sie **[!UICONTROL Prüfer]** oder eine **[!UICONTROL Workflow-Vorlage]** basierend auf dem in Schritt 7 ausgewählten Validierungstyp hinzu.

1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.
1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus.
1. Klicken Sie **[!UICONTROL Hochladen]** und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.
Das Dokument wird im Bereich [!UICONTROL Dokumente] im [!DNL Workfront] in [!DNL Photoshop] und im [!DNL Workfront]-Desktop-Programm angezeigt.
