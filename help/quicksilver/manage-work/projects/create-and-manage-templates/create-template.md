---
product-area: templates
navigation-topic: templates-navigation-topic
title: Erstellen einer Projektvorlage
description: Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann an jedes Projekt übertragen, das Sie aus der Vorlage erstellen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 2%

---

# Erstellen einer Projektvorlage

<!-- Audited: 1/2024 -->

Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann an jedes Projekt übertragen, das Sie aus der Vorlage erstellen.

>[!NOTE]
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem Zeitpunkt, zu dem das zukünftige Projekt beginnen kann) eine Aufgabe beginnen kann und an welchem Tag die Aufgabe möglicherweise abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte die tatsächlichen Daten. Weitere Informationen finden Sie unter [Erstellen eines Projekts](../create-projects/create-project.md).


Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf, wie in diesem Artikel beschrieben.
* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.

  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Projekt als Vorlage speichern](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* durch Kopieren aus einer anderen Vorlage.

  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* durch Import von Blueprints. Sie müssen ein Workfront-Administrator sein, um Blueprints zu importieren. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard </p><p>Oder </p><p>Aktuell: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Sie müssen Systemadministrator sein, um Vorlagen aus Blueprints zu importieren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie verfügen standardmäßig über Verwaltungsberechtigungen für die erstellten Vorlagen.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Vorlage

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Vorlagen**.

1. Klicken Sie auf **Neue Vorlage**.

   Die Vorlage hat keinen Titel.

   ![Neue Vorlage](assets/create-template-nwe-2022-350x102.png)

1. Geben Sie einen Namen für die neue Vorlage in der Vorlagenkopfzeile ein und drücken Sie dann die Eingabetaste **1}.**
1. Klicken Sie im linken Bereich auf den Abschnitt **Vorlagenaufgaben** .
1. Klicken Sie auf **Hinzufügen von Vorlagenaufgaben beginnen**.

   Oder

   Klicken Sie auf **Neue Vorlagenaufgabe** , um Ihrer Vorlage Aufgaben hinzuzufügen.

   Das Hinzufügen von Vorlagenaufgaben zu einer Vorlage entspricht dem Hinzufügen von Aufgaben zu einem Projekt.

   Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Sie können wiederkehrende Aufgaben nicht zu einer Vorlage hinzufügen.

1. (Optional) Klicken Sie oben rechts in der Aufgabenliste auf das Symbol **Gantt-Diagramm** , um eine visuelle Darstellung der Aufgabenliste der Vorlage anzuzeigen.

   >[!TIP]
   >
   >Aufgaben können nicht direkt über dieses Gantt-Diagramm bearbeitet werden.

1. Um Ihrer neuen Vorlage Informationen hinzuzufügen, klicken Sie auf das Menü **Mehr** und anschließend auf **Bearbeiten**.![](assets/more-icon.png)

   Weitere Informationen zum Bearbeiten einer Vorlage finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Klicken Sie auf **Änderungen speichern**.
1. (Optional) Wenn Sie zusätzliche Elemente zur Vorlage hinzufügen möchten, lesen Sie den Abschnitt &quot;[Zusätzliche Elemente zu einer Vorlage hinzufügen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template)&quot;im Artikel &quot;[Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)&quot;.

## Vorlageneinstellungen, die von der Gruppenzuordnung bestimmt werden

Die Zuordnung einer Projektvorlage zu einer Gruppe (oder das Fehlen einer Gruppe) beeinflusst, wie Projekt-, Aufgaben- und Problemeinstellungen bestimmte Einstellungen in der Vorlage bestimmen. Weitere Informationen finden Sie im Abschnitt [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
