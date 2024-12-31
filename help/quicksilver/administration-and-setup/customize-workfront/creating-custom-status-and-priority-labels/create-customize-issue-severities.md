---
title: Anfrageschweregrade erstellen oder anpassen
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Mithilfe von Schweregraden können Sie festlegen, wie ernst ein Problem ist. Sie können einen der fünf in Adobe Workfront vorhandenen Standardschweregrade anpassen oder einen neuen Schweregrad für Ihre Benutzerinnen und Benutzer erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 5%

---

# Problemschweregrade erstellen oder anpassen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Mithilfe von Schweregraden können Sie festlegen, wie ernst ein Problem ist. Sie können einen der fünf in Adobe Workfront vorhandenen Standardschweregrade anpassen oder einen neuen Schweregrad für Ihre Benutzerinnen und Benutzer erstellen.

>[!NOTE]
>
>Aufgaben und Projekte haben keinen Schweregrad.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
     <p>Neu: Standard</p>
     <p>oder</p>
     <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrierte Problemschweregrade

Workfront verfügt über fünf integrierte Problemschweregrade:

* Kosmetisch
* Verwirrend
* Programmfehler mit Umgehungslösung
* Programmfehler ohne Umgehungslösung
* Schwerer Fehler

<p>Für diese Schweregrade können Sie Folgendes bearbeiten:</p>

* Name
* Farbe

  Die Farbe des Schweregrads wird in einem Diagrammbericht beibehalten, wenn Sie die Ergebnisse nach Problemschweregrad gruppieren. Informationen zu Diagrammberichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Welcher Schweregrad der Standard ist

  Weitere Informationen zu Standardschweregraden finden Sie unter [Erstellen oder Bearbeiten eines Problemschweregrads](#create-or-edit-an-issue-severity) in diesem Artikel.
* Beschreibung
* Ob ein Schweregrad in Workfront ausgeblendet ist

  Weitere Informationen zum Ausblenden eines Schweregrads finden Sie unter [Erstellen oder Bearbeiten eines Schweregrads des Problems](#create-or-edit-an-issue-severity")

* Löschen eines Schweregrads

  In diesem Fall müssen Sie einen Ersatzschweregrad auswählen.

## Erstellen oder Bearbeiten eines Problemschweregrads {#create-or-edit-an-issue-severity}

Als Workfront-Admin können Sie Problemschweregrade erstellen und bearbeiten, um sie an die Anforderungen Ihrer Benutzenden anzupassen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** > **Schweregrade**.

1. Wenn Sie einen neuen Schweregrad erstellen, klicken Sie auf &quot;**Schweregrad hinzufügen**.
1. Konfigurieren Sie die folgenden Optionen für den neuen Schweregrad oder bearbeiten Sie sie für einen vorhandenen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name des Schweregrads</td> 
      <td>Geben Sie einen Namen für den Schweregrad ein</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wichtigkeit</td> 
      <td>Erhöhen oder verringern Sie den Schweregrad der ursprünglich von Workfront zugewiesenen Schwere.
      <p>Die Wichtigkeitsnummer für jeden Schweregrad muss eindeutig sein. Die höchste Zahl entspricht dem höchsten Schweregrad.</p> <p>Sie können diese Zahl nicht mehr bearbeiten, nachdem Sie den Schweregrad gespeichert haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Wählen Sie eine Farbe für den Schweregrad.</p> 
      <p>Die Farbe des Schweregrads wird in Diagrammberichten verwendet, wenn Sie Ihre Ergebnisse nach Problemschweregrad gruppieren. Informationen zu Diagrammberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Hinzufügen eines Diagramms zu einem Bericht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardschweregrad</td> 
      <td>Wählen Sie den Schweregrad aus, für den Workfront automatisch alle neu erstellten Probleme auswählen soll.</p>
      <p>Kosmetik ist der Standardschweregrad für Probleme in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für den Schweregrad ein, um dessen Funktion zu erklären.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausblenden</td> 
      <td> Ausblenden eines nicht mehr benötigten Schweregrads. 
      <p>Ein ausgeblendeter Schweregrad wird nirgends in Workfront angezeigt, sodass Benutzende ihn nicht für ihre Probleme auswählen können.</p> 
      <p><b>WICHTIG</b>: Anstatt Schweregrade zu löschen, die Sie nicht mehr verwenden möchten, empfehlen wir, sie auszublenden. Auf diese Weise behalten Sie alle historischen Daten zu Objekten, die bereits mit dem Schweregrad abgeschlossen wurden, und verhindern gleichzeitig, dass Benutzer den Schweregrad in Zukunft verwenden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Ändern Sie die Auflistungsreihenfolge Ihrer Schweregrade, indem Sie sie in die gewünschte Reihenfolge ziehen und ablegen.

   Dadurch wird die Reihenfolge geändert, in der Probleme angezeigt werden. Die Zahl „Wichtigkeit **wird** geändert.

1. Klicken Sie auf **Speichern**.

Weitere Informationen zur Verwendung von Schweregraden bei der Arbeit mit Problemen finden Sie unter [Aktualisieren des Problemschweregrads](../../../manage-work/issues/issue-information/update-issue-severity.md).
