---
product-area: templates
navigation-topic: templates-navigation-topic
title: Erstellen einer Projektvorlage
description: Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 5%

---

# Erstellen einer Projektvorlage

<!-- Audited: 10/2025 -->

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

{{step1-to-templates}}

1. Klicken Sie auf **Neue Vorlage**.

   Die Vorlage hat keinen Titel.

   ![Neue Vorlage](assets/create-template-nwe-2022-350x102.png)

1. Geben Sie in der Vorlagenkopfzeile einen Namen für die neue Vorlage ein und drücken Sie dann die **Eingabetaste.**
1. Klicken Sie auf **Abschnitt** Vorlagenaufgaben“ im linken Bedienfeld.
1. Klicken Sie **Vorlagenaufgaben hinzufügen**, um Aufgaben inline hinzuzufügen

   Oder

   Klicken Sie auf **Neue Vorlagenaufgabe**, um Ihrer Vorlage im Feld **Neue Vorlagenaufgabe** Aufgaben hinzuzufügen.

   ![Feld „Neue Vorlagenaufgabe“](assets/new-template-task-box.png)

1. Aktualisieren Sie Informationen in den folgenden Bereichen:

   * Übersicht
   * Finanzielle Details
   * Einstellungen
   * Arbeitsaufträge
   * Benutzerdefinierte Formulare
   * Dokument anfügen

     Das Aktualisieren von Informationen für eine Vorlagenaufgabe ähnelt dem Bearbeiten von Aufgaben in einem Projekt. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Sie können einer Vorlage keine wiederkehrenden Aufgaben hinzufügen.

1. Klicken Sie auf eine der folgenden Optionen:

   * **Vorlagenaufgabe speichern** speichert die aktuelle Vorlagenaufgabe und schließt das Feld Neue Vorlagenaufgabe.
   * **Vorlagenaufgabe speichern und eine andere**, um die aktuelle Vorlagenaufgabe zu speichern und ein weiteres Feld Neue Vorlagenaufgabe zu öffnen, um eine weitere Aufgabe hinzuzufügen.
   * **Abbrechen**, um das Feld zu schließen, ohne die Vorlagenaufgabe zu speichern.
1. (Optional) Klicken Sie nach dem Hinzufügen der Vorlagenaufgaben im Abschnitt Vorlagenaufgaben auf das **Gantt-Diagramm**-Symbol in der rechten oberen Ecke der Aufgabenliste, um eine visuelle Darstellung der Aufgabenliste der Vorlage anzuzeigen.

   >[!TIP]
   >
   >Aufgaben können nicht direkt über dieses Gantt-Diagramm bearbeitet werden.

1. Um Informationen zu Ihrer neuen Vorlage hinzuzufügen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-icon.png) links neben dem Vorlagennamen in der Kopfzeile und klicken dann auf **Bearbeiten**.

   Informationen zum Bearbeiten einer Vorlage finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >   Die Zuordnung einer Projektvorlage zu einer Gruppe (oder das Fehlen einer Gruppe) wirkt sich darauf aus, wie die Voreinstellungen für Projekte, Aufgaben und Probleme bestimmte Einstellungen in der Vorlage bestimmen.
   >
   >Weitere Informationen finden Sie im Abschnitt „Wie Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet werden“ im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Klicken Sie auf **Speichern**.
1. (Optional) Fügen Sie der Vorlage die folgenden Elemente hinzu

   * Dokumente
   * Risiken
   * Genehmigungsprozesse
   * Abrechnungssätze
   * Ausgaben
   * Warteschlangendetails
   * Themengruppen und Warteschlangenthemen

1. (Optional) Fügen Sie den Aufgaben in der Vorlage die folgenden Elemente hinzu:

   * Dokumente
   * Ausgaben
   * Genehmigungen

   Weitere Informationen finden Sie im Abschnitt „Hinzufügen weiterer Elemente zu einer Vorlage“ im Artikel &quot;[&#x200B; bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




