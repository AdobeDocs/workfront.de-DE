---
title: Aktivieren einer Workfront Planning Workspace in GenStudio for Performance Marketing
description: Wenn Sie bereits über einen Arbeitsbereich in Adobe Workfront Planning verfügen, können Sie ihn für GenStudio for Performance Marketing aktivieren, anstatt Ihre Daten neu zu erstellen.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# Aktivieren eines Workfront Planning Workspace für GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
Wenn Ihr Unternehmen auch Adobe GenStudio for Performance Marketing erworben hat, ist neben Workfront Planning auch der GenStudio-Arbeitsbereich in Adobe Workfront Planning verfügbar, wenn Ihre Workfront-Instanz in die GenStudio-Instanz Ihres Unternehmens integriert ist.

Wenn Sie bereits über einen Arbeitsbereich in Workfront Planning verfügen, können Sie ihn für GenStudio aktivieren, anstatt Ihre Daten neu zu erstellen.

Durch Aktivierung eines Arbeitsbereichs wird dieser mit einem Adobe-Speicherprojekt verknüpft und seine Datensatztypen und -felder werden dem GenStudio Workspace-Schema zugeordnet. Nachdem Sie die Konfiguration abgeschlossen haben, können Sie die Datensätze des Arbeitsbereichs in GenStudio öffnen.

Beachten Sie Folgendes:

* Sie müssen Zugriff auf Workfront Planning und GenStudio for Performance Marketing haben.
* Sie müssen über ein Adobe-Cloud-Speicherprojekt verfügen, um eine Verknüpfung mit dem Arbeitsbereich herstellen zu können. Ein Organisations-Admin kann in der Adobe Admin Console eine erstellen.

  Weitere Informationen finden Sie unter [Verwalten von Adobe-](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)<!--ensure this site still works-->


## Aktivieren eines Workfront Planning Workspace für GenStudio

1. Öffnen Sie in Workfront Planning den Arbeitsbereich, den Sie aktivieren möchten.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Workspace-Namen und klicken Sie dann auf **GenStudio aktivieren**.

   Das Feld **Make Workspace GenStudio** aktiviert“ wird mit den folgenden Schritten geöffnet:

   1. **ACPC-Projekt**: Wählen Sie das **ACPC-Projekt** (Adobe-Cloud-Speicherprojekt) aus, das Sie mit diesem Arbeitsbereich synchronisieren möchten, und klicken Sie dann auf **Weiter**. Benutzende greifen über dieses Projekt auf den Arbeitsbereich in GenStudio zu.

      ![GenStudio Workspace aktivieren - ACPC-Projektschritt](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Datensatztypen**: Ordnen Sie die Datensatztypen des Arbeitsbereichs den sechs Datensatztypen zu, die für GenStudio erforderlich sind:

      * Kampagnen
      * Produkte
      * Personas
      * Kanäle
      * Regionen
      * Aktivierungen

      Öffnen Sie für jeden Datensatz die Liste und wählen Sie den entsprechenden Planungs-Datensatztyp aus, oder wählen Sie **Neu hinzufügen** aus, um ihn zu erstellen, und klicken Sie dann auf **Weiter**.

      ![GenStudio Workspace aktivieren - Schritt Datensatztypen](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Felder**: Ordnen Sie die Felder für jeden Datensatztyp zu. Verwenden Sie die Registerkarten oben im Dialogfeld, um zwischen Datensatztypen zu wechseln. Wählen Sie für jedes Feld das entsprechende Feld Planung aus oder wählen Sie **Neu hinzufügen**, um es zu erstellen.

      Wiederholen Sie die Feldeinrichtung für alle Datensatztypen.

      ![Arbeitsbereich für GenStudio aktivieren - Schritt „Felder“](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Überprüfen und beseitigen Sie etwaige Warnungen.

      Ein neues Feld kann beispielsweise das primäre Feld für den Datensatztyp werden oder ein bereits verwendeter Feldalias wird umbenannt (wenn Sie bereits ein Feld mit dem Namen „Regionen“ haben, könnte das importierte in „Regionen 2“ umbenannt werden).

      Durch Zuordnen **Felds** Status“ werden die erforderlichen Optionen hinzugefügt.

   1. Klicken Sie auf **Veröffentlichen**.

      Wenn der Arbeitsbereich aktiviert ist, wird eine Bestätigungsmeldung angezeigt. Zugeordnete Datensatztypen sind im Arbeitsbereich markiert.

      Die Datensatztypen, denen zugeordnet ist, damit sie über GenStudio zugänglich sind, haben ein neues **Adobe**-Symbol auf ihren Karten.

      ![Kampagnen-Datensatztyp mit Adobe-Symbol](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Öffnen Sie GenStudio, wählen Sie **Kampagnen** und klicken Sie dann auf das **ACPC-Projekt** das Sie ursprünglich für dieses Setup konfiguriert haben, in der unteren linken Ecke des Bildschirms. Überprüfen Sie die importierten Datensatztypen und -felder.

   >[!TIP]
   >
   >Es werden nur die Datensätze angezeigt, die durch Ihre ACPC-Projektmitgliedschaft zulässig sind.
