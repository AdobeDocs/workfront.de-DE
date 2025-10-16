---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Hochladen von Testsendungen aus InDesign
description: Sie können Ihre Grafiktafeln als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in Adobe Workfront zu speichern.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Hochladen von Testsendungen aus [!DNL InDesign]

Sie können Ihre Grafiktafeln als Korrekturabzüge direkt in [!DNL Adobe Workfront] hochladen, um sie gründlich zu prüfen und zu genehmigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td>Beliebig </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Standard</p> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Adobe Creative Cloud] über eine [!DNL Workfront]-Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>[!UICONTROL Manager] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf [!UICONTROL -Dokumente] bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Voraussetzungen

* Sie müssen das [!DNL Adobe Workfront for design and video]-Plug-in installieren, bevor Sie Korrekturabzüge von [!DNL InDesign] hochladen können.

  Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Hochladen eines einfachen Korrekturabzugs

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie einen Korrekturabzug hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument](assets/documents.png) in der Navigationsleiste.
1. Klicken Sie **[!UICONTROL Neue Datei]** unten im Plug-in.
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
   Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.


## Hochladen eines automatisierten Korrekturabzugs

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, in das Sie einen Korrekturabzug hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie **[!UICONTROL Neue Datei]** unten im Plug-in.
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
Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.

## Hochladen einer neuen Korrekturabzugsversion

Sie können eine neue Version eines Korrekturabzugs hochladen. Das Plug-in speichert den Korrekturabzugs-Workflow, der für die vorherige Version festgelegt wurde. Sie können dies jedoch bei Bedarf ändern.

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wechseln Sie zu dem Arbeitselement, auf das Sie ein Dokument hochladen möchten.
1. Klicken Sie auf das **[!UICONTROL Dokument]**-Symbol ![Dokument-Symbol](assets/documents.png) in der Navigationsleiste.

1. Klicken Sie **[!UICONTROL Neue Version]** am unteren Rand des Plug-ins.
1. Aktivieren Sie den **[!UICONTROL Korrekturabzug erstellen]**.

1. Wählen Sie im Abschnitt *[!UICONTROL *Korrekturabzugsgenehmigungen]* die Option **[!UICONTROL Standard]** oder **[!UICONTROL Automated]**.

1. Fügen Sie **[!UICONTROL Prüfer]** oder eine **[!UICONTROL Workflow-Vorlage]** basierend auf dem in Schritt 7 ausgewählten Validierungstyp hinzu.

1. (Optional) Geben Sie einen Kommentar im Bereich **[!UICONTROL Aktualisierungen]** ein.
1. Wählen Sie **[!UICONTROL Asset-Typ]** aus dem Dropdown-Menü aus.
1. Klicken Sie **[!UICONTROL Hochladen]** und konfigurieren Sie dann alle gewünschten Exportoptionen basierend auf dem oben ausgewählten Asset-Typ.
Das Dokument wird im Bereich [!UICONTROL Dokumente] im Plug-in und im Desktop-Programm angezeigt.
