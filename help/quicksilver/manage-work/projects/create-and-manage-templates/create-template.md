---
product-area: templates
navigation-topic: templates-navigation-topic
title: Erstellen einer Projektvorlage
description: Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und alle Informationen für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann an das Projekt übertragen, wenn Sie sie aus der Vorlage erstellen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Erstellen einer Projektvorlage

Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und alle Informationen für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann an das Projekt übertragen, wenn Sie sie aus der Vorlage erstellen.

>[!NOTE]
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem Zeitpunkt, zu dem das zukünftige Projekt beginnen kann) eine Aufgabe beginnen kann und an welchem Tag die Aufgabe möglicherweise abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte die tatsächlichen Daten. Weitere Informationen finden Sie unter [Projekt erstellen](../create-projects/create-project.md).


Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf, wie in diesem Artikel beschrieben.
* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.

  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Projekt als Vorlage speichern](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* durch Kopieren aus einer anderen Vorlage.

  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Wenn Sie Workfront-Administrator sind, können Sie Vorlagen durch Importieren von Blueprints erstellen. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Systemadministrator für den Import von Vorlagen aus Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie verfügen standardmäßig über Verwaltungsberechtigungen für die erstellten Vorlagen.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen einer Vorlage

1. Aus dem **Hauptmenü** ![](assets/main-menu-icon.png) click **Vorlagen**.

1. Klicken **Neue Vorlage**.

   Die Vorlage hat keinen Titel.

   ![Neue Vorlage](assets/create-template-nwe-2022-350x102.png)

1. Geben Sie einen Namen für die neue Vorlage in der Vorlagenkopfzeile ein und drücken Sie dann die Eingabetaste **Geben Sie ein.**
1. Klicken Sie auf **Vorlagenaufgaben** im linken Bereich.
1. Klicken **Beginnen mit dem Hinzufügen von Vorlagenaufgaben**.

   Oder

   Klicken **Neue Vorlagenaufgabe** , um Ihrer Vorlage Aufgaben hinzuzufügen.

   Das Hinzufügen von Vorlagenaufgaben zu einer Vorlage entspricht dem Hinzufügen von Aufgaben zu einem Projekt.

   Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Sie können wiederkehrende Aufgaben nicht zu einer Vorlage hinzufügen.

1. (Optional) Klicken Sie auf die **Gantt-Diagramm** in der oberen rechten Ecke der Aufgabenliste ein, um eine visuelle Darstellung der Aufgabenliste der Vorlage anzuzeigen.

   >[!TIP]
   >
   >Aufgaben können nicht direkt über dieses Gantt-Diagramm bearbeitet werden.

1. Um Informationen zu Ihrer neuen Vorlage hinzuzufügen, klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten**.

   Informationen zum Bearbeiten einer Vorlage finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Klicken **Änderungen speichern**.
1. (Optional) Wenn Sie der Vorlage weitere Elemente hinzufügen möchten, lesen Sie den Abschnitt . [Hinzufügen zusätzlicher Elemente zu einer Vorlage](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) im Artikel [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Vorlageneinstellungen, die von der Gruppenzuordnung bestimmt werden

Die Verknüpfung einer Projektvorlage mit einer Gruppe (oder deren Fehlen) beeinflusst, wie Projekt-, Aufgaben- und Problemeinstellungen bestimmte Einstellungen in der Vorlage bestimmen. Weitere Informationen finden Sie im Abschnitt . [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) im Artikel [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
