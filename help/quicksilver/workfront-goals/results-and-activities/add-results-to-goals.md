---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen
description: Ergebnisse messen den Fortschritt eines Ziels. Ohne die Zuordnung von Ergebnissen, Aktivitäten oder aufeinander abgestimmten Zielen zu einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 3%

---

# Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen

Ergebnisse messen den Fortschritt eines Ziels. Ohne die Zuordnung von Ergebnissen, Aktivitäten oder aufeinander abgestimmten Zielen zu einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitarbeiter oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderungen, eine der folgenden: </p>
<ul>
<li>Ein Select- oder Prime-Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderungen: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Zugriffsebene</p></td>
 <td> <p>Zugriff auf Ziele bearbeiten</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
  <p>Berechtigungen für das Ziel verwalten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.
* Ein vorhandenes Ziel.

  Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Ein Ziel darf nicht mehr als 1000 Aktivitäten, Ergebnisse, Projekte oder aufeinander abgestimmte Ziele haben.

## Hinzufügen eines Ergebnisses zu einem Ziel

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

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

1. Klicken Sie auf das Hauptmenü ![](assets/main-menu-icon.png), dann **Ziele**.

1. Aus dem **Zielliste** klicken Sie auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicks **Fortschrittsanzeigen** im linken Bereich.
1. Erweitern Sie die **Neuer Fortschrittsanzeiger** Dropdown-Menü, und klicken Sie auf **Ergebnis erstellen**.

   Das Feld Neues Ergebnis wird geöffnet.

   ![](assets/new-result-box-unshimmed.png)

1. Geben Sie einen Namen für das Ergebnis im **Ergebnisname** -Feld. Dies ist ein Pflichtfeld.
1. (Optional) Entfernen Sie Ihren Namen aus dem **Ergebniseigentümer** ein, wenn Sie das Ergebnis einem anderen Benutzer zuweisen möchten. Standardmäßig sind Sie Eigentümer einer von Ihnen erstellten Aktivität.

   >[!NOTE]
   >
   >Sie können kein Team, keine Gruppe oder das Unternehmen als Ergebniseigentümer zuweisen.

1. Im **Wie wollen Sie Ihr Ergebnis messen?** -Bereich, geben Sie die folgenden Informationen an:
   * **Werttyp**: Zeigt an, wie Sie den Fortschritt am Ergebnis messen möchten. Sie können den Fortschritt numerisch, mit einem Prozentwert oder mit einem Währungsbetrag messen.

     Wählen Sie einen Werttyp aus den in der folgenden Tabelle aufgeführten Optionen aus:

     | Werttyp | Beschreibung |
     |---------------------------------------------------------|------------------|
     | Zahl | Zahlenwert |
     | % | Prozentwert |
     | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Währungswerte |

   * **Anfangswert**: Der Wert, den das Ergebnis am Anfang hat, bevor ein Fortschritt aufgezeichnet wurde.
   * **Zielwert**: Der Wert, den das Ergebnis erzielen soll, wenn es als abgeschlossen betrachtet wird.
1. Klicks **Ergebnis erstellen**.

   Das Ergebnis wird im Abschnitt Fortschrittsindikatoren der Zielseite unter der Ergebnisgruppierung angezeigt.

   Nachdem Sie das Ziel aktiviert haben, wird der Fortschritt des Ziels automatisch aktualisiert, wenn Sie den Fortschritt eines Ergebnisses aktualisieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Ziele in Adobe Workfront aktivieren](../goal-management/activate-goals.md).
