---
product-area: templates
navigation-topic: templates-navigation-topic
title: Erstellen einer Projektvorlage
description: Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 3%

---

# Erstellen einer Projektvorlage

<!-- Audited: 1/2024 -->

Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.

>[!NOTE]
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem das zukünftige Projekt beginnen könnte) eine Aufgabe beginnen könnte und an welchem Tag sie abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte tatsächliche Termine. Weitere Informationen finden Sie unter [Erstellen eines Projekts](../create-projects/create-project.md).


Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf neu, wie in diesem Artikel beschrieben.
* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.

  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Speichern eines Projekts als Vorlage](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Durch Kopieren aus einer anderen Vorlage.

  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer &#x200B;](../../../manage-work/projects/create-and-manage-templates/copy-template.md)).

* Durch den Import von Blueprints. Sie müssen Workfront-Administrator sein, um Blueprints importieren zu können. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard </p><p>Plan</p> <p>Sie müssen Systemadministrator sein, um Vorlagen aus Blueprints importieren zu können</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie haben standardmäßig Verwaltungsberechtigungen für die von Ihnen erstellten Vorlagen</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Erstellen einer Vorlage

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Vorlagen**.

1. Klicken Sie auf **Neue Vorlage**.

   Die Vorlage hat keinen Titel.

   ![Neue Vorlage](assets/create-template-nwe-2022-350x102.png)

1. Geben Sie in der Vorlagenkopfzeile einen Namen für die neue Vorlage ein und drücken Sie dann die **Eingabetaste.**
1. Klicken Sie auf **Abschnitt** Vorlagenaufgaben“ im linken Bedienfeld.
1. Klicken Sie **Vorlagenaufgaben hinzufügen**.

   Oder

   Klicken Sie auf **Neue Vorlagenaufgabe**, um Ihrer Vorlage Aufgaben hinzuzufügen.

   Das Hinzufügen von Vorlagenaufgaben zu einer Vorlage entspricht dem Hinzufügen von Aufgaben zu einem Projekt.

   Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Sie können einer Vorlage keine wiederkehrenden Aufgaben hinzufügen.

1. (Optional) Klicken Sie auf **Gantt** Diagramm) in der rechten oberen Ecke der Aufgabenliste, um eine visuelle Darstellung der Aufgabenliste der Vorlage anzuzeigen.

   >[!TIP]
   >
   >Aufgaben können nicht direkt über dieses Gantt-Diagramm bearbeitet werden.

1. Um Informationen zu Ihrer neuen Vorlage hinzuzufügen, klicken Sie auf das Menü **Mehr** ![Mehr-Symbol](assets/more-icon.png) und dann auf **Bearbeiten**.

   Informationen zum Bearbeiten einer Vorlage finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Klicken Sie auf **Änderungen speichern**.
1. (Optional) Wenn Sie zusätzliche Elemente zu einer Vorlage hinzufügen möchten, finden Sie weitere Informationen im Abschnitt [Hinzufügen zusätzlicher Elemente zu einer Vorlage](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) im Artikel [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Vorlageneinstellungen durch Gruppenzuordnung bestimmt

Die Zuordnung einer Projektvorlage zu einer Gruppe (oder das Fehlen einer Gruppe) wirkt sich darauf aus, wie die Voreinstellungen für Projekte, Aufgaben und Probleme bestimmte Einstellungen in der Vorlage bestimmen. Weitere Informationen finden Sie im Abschnitt [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
