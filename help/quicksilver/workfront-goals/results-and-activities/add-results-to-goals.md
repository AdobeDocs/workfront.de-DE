---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals
description: Die Ergebnisse messen den Fortschritt eines Ziels. Ohne die Verknüpfung von Ergebnissen, Aktivitäten oder abgestimmten Zielen mit einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 3%

---

# Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Die Ergebnisse messen den Fortschritt eines Ziels. Ohne die Verknüpfung von Ergebnissen, Aktivitäten oder abgestimmten Zielen mit einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.

## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-Paket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Mitwirkender oder höher</p>
<p>Anfrage oder höher</p></td>
 </tr>
  <tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Systemadministratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.
* Ein vorhandenes Ziel.

  Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Ein Ziel kann nicht mehr als insgesamt 1000 Aktivitäten, Ergebnisse, Projekte oder abgestimmte Ziele haben.

## Hinzufügen eines Ergebnisses zu einem Ziel

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Klicken Sie auf das Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png), dann **Ziele**.

1. Klicken Sie in **Zielliste** auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Erweitern Sie das **Neue Fortschrittsanzeige** Dropdown-Menü und klicken Sie auf **Ergebnis erstellen**.

   Das Feld Neues Ergebnis wird geöffnet.

   ![Neues Ergebnisfeld](assets/new-result-box-unshimmed.png)

1. Geben Sie einen Namen für das Ergebnis in das Feld **Ergebnisname** ein. Dies ist ein Pflichtfeld.
1. (Optional) Entfernen Sie Ihren Namen aus dem Feld **Ergebnisbesitzer**, wenn Sie das Ergebnis einem anderen Benutzer zuweisen möchten. Standardmäßig sind Sie der Eigentümer einer von Ihnen erstellten Aktivität.

   >[!NOTE]
   >
   >Es ist nicht möglich, ein Team, eine Gruppe oder die Firma als Ergebnisinhaber zuzuweisen.

1. Im **Wie möchten Sie Ihr Ergebnis messen?Geben Sie** Bereich die folgenden Informationen an:
   * **Werttyp**: Dies gibt an, wie Sie den Fortschritt beim Ergebnis messen möchten. Sie können den Fortschritt numerisch, mit einem Prozentwert oder unter Verwendung eines Währungsbetrags messen.

     Wählen Sie einen Werttyp aus den in der folgenden Tabelle aufgelisteten Optionen aus:

     | Werttyp | Beschreibung |
     |---------------------------------------------------------|------------------|
     | Zahl | Zahlenwert |
     | % | Prozentwert |
     | CN,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Währungswerte |

   * **Ausgangswert** Der Wert, den das Ergebnis am Anfang hat, bevor ein Fortschritt aufgezeichnet wurde.
   * **Zielwert**: Der Wert, den das Ergebnis erreichen soll, wenn es als abgeschlossen gilt.
1. Klicken Sie **Ergebnis erstellen**.

   Das Ergebnis wird im Bereich Fortschrittsanzeigen auf der Zielseite unter der Gruppierung Ergebnis angezeigt.

   Nachdem Sie das Ziel aktiviert haben, wird der Fortschritt des Ziels automatisch aktualisiert, wenn Sie den Fortschritt eines Ergebnisses aktualisieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../goal-management/activate-goals.md).
