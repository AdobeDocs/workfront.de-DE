---
title: Erstellen und Anpassen von Prioritäten
description: Im Einrichtungsbereich von Workfront können Sie die Prioritäten für Projekte, Aufgaben und Probleme festlegen. Prioritäten geben Ihren Projekten, Aufgaben oder Problemen in Adobe Workfront Priorität.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Erstellen und Anpassen von Prioritäten

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Im Einrichtungsbereich von Workfront können Sie die Prioritäten für Projekte, Aufgaben und Probleme festlegen. Prioritäten geben Ihren Projekten, Aufgaben oder Problemen in Adobe Workfront Priorität.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassung vorhandener Prioritäten

Als Workfront-Administrator können Sie die folgenden Änderungen an den in Workfront bereitgestellten Standardprioritäten vornehmen:

* Umbenennen von Prioritäten.
* Neuordnung der Prioritäten.

  Weitere Informationen zum Neuanordnen von Prioritäten finden Sie unter [Erstellen einer Priorität für eine Projektaufgabe oder Problem](#create-a-priority-for-a-project-task-or-issue).

* Ändern Sie die Standardpriorität.

  Weitere Informationen zur Funktion zum Ändern der Standardpriorität finden Sie unter [Erstellen einer Priorität für eine Projektaufgabe oder Problem](#create-a-priority-for-a-project-task-or-issue).

* Bearbeiten Sie die Beschreibung der Prioritäten.
* Legen Sie für jede Priorität eine Farbe fest.

  Die Farbe der Priorität wird in Diagrammberichten verwendet, wenn Sie Ihre Ergebnisse nach **Priorität** gruppieren.

  Weitere Informationen zu Diagrammberichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Löschen von Prioritäten.

  Wenn Sie eine vorhandene Priorität löschen, müssen Sie eine Ersatzpriorität auswählen.

* Ausblenden von Prioritäten.

  Weitere Informationen zur Funktion zum Ausblenden von Prioritäten finden Sie unter [Erstellen einer Priorität für eine Projektaufgabe oder Problem](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Sie müssen für jedes Objekt mindestens eine Priorität in Ihrem Workfront-Konto haben.

Die standardmäßig für jeden Objekttyp (Projekt, Aufgabe und Problem) bereitgestellten Prioritäten sind identisch:

* Keine
* Niedrig
* Normal
* Hoch
* Dringend

## Erstellen einer Priorität für eine Projektaufgabe oder ein Problem {#create-a-priority-for-a-project-task-or-issue}

Zusätzlich zu den Standardprioritäten, die in Workfront bereitgestellt werden, können Sie Ihre eigenen Prioritäten hinzufügen, um die Anforderungen Ihres Unternehmens zu berücksichtigen.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Projekteinstellungen** > **Prioritäten**.

1. Klicken Sie auf die Registerkarte für den Objekttyp, für den Sie eine Priorität erstellen möchten (**Projekt**, **Aufgabe** oder **Problem**).
1. Klicken Sie auf **Neue Priorität hinzufügen**.
1. Geben Sie die folgenden Informationen für die neue Priorität an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name der Priorität</td> 
      <td>Geben Sie einen Namen für Ihre Priorität ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wichtigkeit</td> 
      <td> <p>Beim Hinzufügen einer neuen Priorität wird ihr standardmäßig eine Zahl zugewiesen. Bearbeiten Sie diese Zahl, wenn sie nicht Ihren Anforderungen entspricht.</p> <p>Die Nummer <strong>Wichtigkeit</strong> für jede Priorität muss für das ausgewählte Objekt eindeutig sein.<br>Die Prioritätsnummer spiegelt die Wichtigkeit des Projekts, der Aufgabe oder des Problems wider: Die höchste Zahl entspricht der höchsten Priorität.</p> <p><b>HINWEIS</b>: Sie können die Wichtigkeitsnummer nach dem Speichern der Priorität nicht bearbeiten. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Wählen Sie eine Farbe für Ihre Priorität aus.</p> <p>Die Farbe der Priorität wird in Diagrammberichten und Agile Team Settings verwendet. Weitere Informationen zu Diagrammberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Hinzufügen eines Diagramms zu einem Bericht</a>.</p> <p>Weitere Informationen zu den Agile-Team-Einstellungen finden Sie unter .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardpriorität</td> 
      <td> <p>Entscheiden Sie, ob dies eine Standardpriorität sein soll, indem Sie das Optionsfeld auswählen.</p> <p>Wenn eine Priorität als <strong>Standardpriorität</strong> festgelegt ist, wird sie automatisch für alle Projekte, Aufgaben oder Probleme in Workfront ausgewählt. <strong>Normal</strong> ist die Standardpriorität für alle Objekte in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Fügen Sie eine Beschreibung für Ihre Priorität hinzu, um ihre Funktion zu erläutern.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausblenden</td> 
      <td> <p>Aktivieren Sie dieses Kontrollkästchen, wenn Sie die Priorität ausblenden möchten.</p><p>Wenn Sie die Option <b>Ausblenden</b> auswählen, wird die Priorität nirgendwo in Workfront angezeigt und die Benutzer können sie nicht für ihre Projekte, Aufgaben und Probleme auswählen.</p> 
      <p><b>WICHTIG</b>: Wir empfehlen, die Prioritäten, die Sie nicht mehr verwenden möchten, auszublenden, anstatt sie zu löschen. Wenn Sie sie ausblenden, behalten Sie immer noch alle historischen Daten von Objekten, die mit dieser Priorität ausgefüllt wurden, und verhindern gleichzeitig, dass Menschen diese Priorität in Zukunft wählen. </p>
      <p>Optional können Sie die Reihenfolge der Prioritäten ändern, indem Sie sie in die gewünschte Reihenfolge ziehen und dort ablegen. Dadurch wird die Reihenfolge geändert, in der sie für Projekte, Aufgaben und Probleme angezeigt werden. Die Zahl <b>Wichtigkeit</b> wird dadurch nicht geändert. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

Anweisungen zur Anwendung von Prioritäten auf Projekte, Aufgaben und Probleme finden Sie in den folgenden Artikeln:

* [Grundlegendes zu und Aktualisieren von Projektprioritäten](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Aufgabenpriorität aktualisieren](../../../manage-work/tasks/task-information/task-priority.md)
* [Priorität von Problemen aktualisieren](../../../manage-work/issues/issue-information/update-issue-priority.md)
