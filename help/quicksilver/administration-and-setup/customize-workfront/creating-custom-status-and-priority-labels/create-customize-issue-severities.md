---
title: Erstellen oder Anpassen von Problemschwerpunkten
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Ihre Benutzer können Prioritätsstufen verwenden, um festzulegen, wie schwerwiegend ein Problem ist. Sie können einen der fünf Standardabstufungen in Adobe Workfront anpassen oder einen neuen Schweregrad für Ihre Benutzer erstellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# Erstellen oder Anpassen von Problemschwerpunkten

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Ihre Benutzer können Prioritätsstufen verwenden, um festzulegen, wie schwerwiegend ein Problem ist. Sie können einen der fünf Standardabstufungen in Adobe Workfront anpassen oder einen neuen Schweregrad für Ihre Benutzer erstellen.

>[!NOTE]
>
>Aufgaben und Projekte haben keine Schwerpunkte.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Integrierte Problembereiche

Workfront verfügt über fünf integrierte Problemschwerpunkte:

* Kosmetisch
* Verwirrend
* Programmfehler mit Umgehungslösung
* Programmfehler ohne Umgehungslösung
* Schwerer Fehler

<p>Sie können für diese Prioritätsstufen Folgendes bearbeiten:</p>

* Name
* Farbe

   Die Farbe eines Schweregrads wird in einem Diagrammbericht beibehalten, wenn Sie Ihre Ergebnisse nach Schweregrad des Problems gruppieren. Informationen zu Diagrammberichten finden Sie unter [Diagramm zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Welche Schweregrad ist die Standardeinstellung?

   Weitere Informationen zu Standardabstufungen finden Sie unter [Erstellen oder Bearbeiten eines Schweregrads eines Problems](#create-or-edit-an-issue-severity) in diesem Artikel.
* Beschreibung
* Ob ein Schweregrad in Workfront ausgeblendet wird

   Weitere Informationen zum Ausblenden eines Schweregrads finden Sie unter [Erstellen oder Bearbeiten eines Schweregrads eines Problems](#create-or-edit-an-issue-severity")

* Schweregrad löschen

   In diesem Fall müssen Sie einen Ersatzschwerpunkt auswählen.

## Erstellen oder Bearbeiten eines Schweregrads eines Problems {#create-or-edit-an-issue-severity}

Als Workfront-Administrator können Sie Problemabstufungen entsprechend den Anforderungen Ihrer Benutzer erstellen und bearbeiten.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Projektvoreinstellungen** > **Schweregrad**.

1. Wenn Sie einen neuen Schweregrad erstellen, klicken Sie auf **Neuen Schweregrad hinzufügen**.
1. Konfigurieren Sie die folgenden Optionen für den neuen Schweregrad oder bearbeiten Sie sie für einen vorhandenen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name des Schweregrads</td> 
      <td>Geben Sie einen Namen für den Schweregrad ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wichtigkeit</td> 
      <td>Erhöhen oder verringern Sie den Schweregrad, der ursprünglich von Workfront zugewiesen wurde.
      <p>Die Wichtigkeitsnummer für jeden Schweregrad muss eindeutig sein. Die höchste Zahl entspricht dem höchsten Schweregrad.</p> <p>Sie können diese Zahl nach dem Speichern der Prioritätsstufe nicht mehr bearbeiten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Wählen Sie eine Farbe für den Schweregrad.</p> 
      <p>Die Farbe des Schweregrads wird in Diagrammberichten verwendet, wenn Sie Ihre Ergebnisse nach Schweregrad des Problems gruppieren. Informationen zu Diagrammberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Diagramm zu einem Bericht hinzufügen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardschweregrad</td> 
      <td>Wählen Sie den Schweregrad aus, den Workfront automatisch für alle neu erstellten Probleme auswählen soll.</p>
      <p>Kosmetik ist der Standardschwerpunkt bei Problemen in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für den Schweregrad ein, um dessen Funktion zu erläutern.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausblenden</td> 
      <td> Verbergen Sie einen Schweregrad, der nicht mehr benötigt wird. 
      <p>In Workfront wird kein verborgener Schweregrad angezeigt, sodass Benutzer ihn nicht für ihre Probleme auswählen können.</p> 
      <p><b>WICHTIG</b>: Anstatt Prioritätsstufen zu löschen, die Sie nicht mehr verwenden möchten, empfehlen wir, diese zu verbergen. Auf diese Weise bewahren Sie alle historischen Daten zu Objekten auf, die bereits mit der Schwere ausgefüllt sind, und verhindern gleichzeitig, dass Menschen den Schweregrad in Zukunft verwenden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Ändern Sie die Listenreihenfolge Ihrer Prioritätsstufen, indem Sie sie in die gewünschte Reihenfolge ziehen und dort ablegen.

   Dadurch wird die Reihenfolge geändert, in der sie für Probleme angezeigt werden. Die **Wichtigkeit** Zahl.

1. Klicken Sie auf **Speichern**.

Weitere Informationen zur Verwendung von Prioritätsstufen bei der Arbeit mit Problemen finden Sie unter [Schweregrad des Problems aktualisieren](../../../manage-work/issues/issue-information/update-issue-severity.md).
