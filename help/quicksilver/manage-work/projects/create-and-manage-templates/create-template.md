---
product-area: templates
navigation-topic: templates-navigation-topic
title: Erstellen einer Projektvorlage
description: Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/JqR-bwIq1AVMOMz3aTWIKoiPep1VQ6IaONbbuDJ1AiA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: b91c0848-76c4-4da4-8b81-3aade0518dd0id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 790
ht-degree: 9%

---

# Erstellen einer Projektvorlage

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

Sie können Vorlagen im Bereich Vorlagen erstellen und löschen. Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.

>[!NOTE]
>
>Eine Vorlage und ihre Aufgaben haben keine tatsächlichen Daten, sondern einen Hinweis darauf, an welchem Tag (ab dem das zukünftige Projekt beginnen könnte) eine Aufgabe beginnen könnte und an welchem Tag sie abgeschlossen werden muss. Wenn Sie Vorlagen zur Erstellung künftiger Projekte verwenden, erhalten die Projekte tatsächliche Termine. Weitere Informationen finden Sie unter [Erstellen eines Projekts](../create-projects/create-project.md).


Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf neu, wie in diesem Artikel beschrieben.
* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.

  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Speichern eines Projekts als Vorlage](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Durch Kopieren aus einer anderen Vorlage.

  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer ](../../../manage-work/projects/create-and-manage-templates/copy-template.md)).

* Durch den Import von Blueprints. Sie müssen Workfront-Administrator sein, um Blueprints importieren zu können. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
</table>
-->

## Erstellen einer Vorlage

{{step1-to-templates}}

1. Klicken Sie auf **Neue Vorlage**.

1. (Bedingt) Klicken Sie je nachdem, welchen Dokumentspeicher Ihr Unternehmen verwendet, auf eine der folgenden Optionen:

   * **Neue Vorlage**, wenn der Workfront-Administrator entweder **Adobe Cloud-Speicher** oder **Legacy-Workfront** auswählt und die Einstellung **Dem Benutzer die Auswahl des Speicheranbieters erlauben** ausgewählt hat oder nicht.
   * **Neue Vorlage (Legacy-Speicher)** Wenn der Workfront-Administrator entweder **Adobe-Cloud-** oder **Legacy-Workfront** auswählt und außerdem die Einstellung **Auswahl des Speicheranbieters durch den Benutzer zulassen** ausgewählt hat.

     Diese Option wird nur angezeigt, wenn **Einstellung „Auswahl des Speicheranbieters durch den Benutzer zulassen** im Bereich „Setup“ ausgewählt ist.

     Weitere Informationen finden Sie unter [Aktivieren von Adobe-Cloud-Speicher für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

     Eine Vorlage wird erstellt. Ihr Standardname folgt den folgenden Mustern, je nachdem, welcher Speicher Workfront für Dokumente verwendet:

      * **Unbenannte Vorlage** für eine Workfront-Speichervorlage.

        Bei einer Legacy-Workfront-Speichervorlage wird neben dem Namen das Symbol **Legacy** Workfront-Speicher![ Legacy-](assets/legacy-storage-project-icon.png)-Projekt) angezeigt.

      * **Nicht benannte Vorlage - &lt; Tag Monat, Jahr, Stunde.Minute.Sekunde >** für eine Adobe Cloud-Speichervorlage

        >[!IMPORTANT]
        >
        >Vorlagen, die den Adobe-Speicher verwenden, müssen eindeutige Namen haben.

   ![Neue Vorlage](assets/create-template-nwe-2022-350x102.png)

1. Geben Sie in der Vorlagenkopfzeile einen Namen für die neue Vorlage ein und drücken Sie dann die **Eingabetaste.**
1. Klicken Sie auf **Abschnitt** Vorlagenaufgaben“ im linken Bedienfeld.
1. Klicken Sie **Vorlagenaufgaben hinzufügen**, um Aufgaben inline hinzuzufügen

   ODER

   Klicken Sie auf **Neue Vorlagenaufgabe**, um Ihrer Vorlage im Feld **Neue Vorlagenaufgabe** Aufgaben hinzuzufügen.

   Das **Vorlagenaufgabe erstellen** wird geöffnet, wenn Sie auf **Neue Vorlagenaufgabe** klicken.

   ![Neues Erlebnis für neue Vorlagenaufgabe](assets/new-template-task-box-unshimmed.png)

1. (Bedingt) Aktualisieren Sie Informationen in den folgenden Bereichen im Feld **Vorlagenaufgabe erstellen**:

   * Name der Vorlagenaufgabe
   * Übersicht
   * Arbeitsaufträge
   * Finanzielle Details
   * Benutzerdefinierte Formulare
   * Dokumente
   * Einstellungen

   Das Aktualisieren von Informationen für eine Vorlagenaufgabe ähnelt dem Bearbeiten von Vorlagenaufgaben.

   Weitere Informationen finden Sie unter [Vorlagenaufgaben bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-template-task.md).

   >[!NOTE]
   >
   >Sie können einer Vorlage keine wiederkehrenden Aufgaben hinzufügen.

1. Klicken Sie **Vorlagenaufgabe erstellen**.

1. (Optional) Klicken Sie nach dem Hinzufügen der Vorlagenaufgaben im **Vorlagenaufgaben** auf das **Gantt-Diagramm**-Symbol ![Gantt-Symbol](assets/gantt-icon.png) in der oberen rechten Ecke der Aufgabenliste, um eine visuelle Darstellung der Aufgabenliste der Vorlage anzuzeigen.

   >[!TIP]
   >
   >Sie können Aufgaben nicht direkt über ein Gantt-Diagramm für Vorlagenaufgaben bearbeiten.

1. Um Informationen zu Ihrer neuen Vorlage hinzuzufügen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-icon.png) rechts neben dem Vorlagennamen in der Kopfzeile und klicken dann auf **Bearbeiten**.

   Informationen zum Bearbeiten einer Vorlage finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >Die Zuordnung einer Projektvorlage zu einer Gruppe (oder das Fehlen einer Gruppe) wirkt sich darauf aus, wie die Voreinstellungen für Projekte, Aufgaben und Probleme bestimmte Einstellungen in der Vorlage bestimmen.
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

   Weitere Informationen finden Sie im Abschnitt „Hinzufügen weiterer Elemente zu einer Vorlage“ im Artikel &quot;[ bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




