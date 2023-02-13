---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen
description: Ergebnisse messen den Fortschritt eines Ziels. Ohne die Zuordnung von Ergebnissen, Aktivitäten oder aufeinander abgestimmten Zielen zu einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---

# Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen

Ergebnisse messen den Fortschritt eines Ziels. Ohne die Zuordnung von Ergebnissen, Aktivitäten oder aufeinander abgestimmten Zielen zu einem Ziel können Sie das Ziel nicht aktivieren und den Fortschritt nicht aufzeichnen.

## Zugriffsanforderungen

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die Adobe Workfront Goals erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele bearbeiten</p> <p><b>NOTIZ</b>

<p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Berechtigungen für das Ziel verwalten</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.
* Ein vorhandenes Ziel.

   Informationen zum Erstellen von Zielen finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Ein Ziel darf nicht mehr als 1000 Aktivitäten, Ergebnisse, Projekte oder aufeinander abgestimmte Ziele haben.

## Ergebnis zu einem Ziel hinzufügen

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
1. Klicken **Fortschrittsanzeigen** im linken Bereich.
1. Erweitern Sie die **Neuer Fortschrittsanzeiger** Dropdown-Menü, und klicken Sie auf **Ergebnis erstellen**.

   Das Feld Neues Ergebnis wird geöffnet.

   ![](assets/new-result-box-unshimmed.png)

1. Geben Sie im Feld **Ergebnisname** -Feld. Dies ist ein Pflichtfeld.
1. (Optional) Entfernen Sie Ihren Namen aus dem **Ergebniseigentümer** ein, wenn Sie das Ergebnis einem anderen Benutzer zuweisen möchten. Standardmäßig sind Sie Eigentümer einer von Ihnen erstellten Aktivität.

   >[!NOTE]
   >
   >Sie können kein Team, keine Gruppe oder das Unternehmen als Ergebniseigentümer zuweisen.

1. Im **Wie wollen Sie Ihr Ergebnis messen?** -Bereich, geben Sie die folgenden Informationen an:
   * **Werttyp**: Dies zeigt an, wie Sie den Fortschritt am Ergebnis messen möchten. Sie können den Fortschritt numerisch, mit einem Prozentwert oder mit einem Währungsbetrag messen.

      Wählen Sie einen Werttyp aus den in der folgenden Tabelle aufgeführten Optionen aus:

      | Werttyp | Beschreibung |
      |---------------------------------------------------------|------------------|
      | Zahl | Zahlenwert |
      | % | Prozentwert |
      | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Währungswerte |

   * **Anfangswert**: Der Wert, den das Ergebnis am Anfang hat, bevor der Fortschritt aufgezeichnet wurde.
   * **Zielwert**: Der Wert, den das Ergebnis erreichen soll, wenn es als abgeschlossen betrachtet wird.
1. Klicken **Ergebnis erstellen**.

   Das Ergebnis wird im Abschnitt Fortschrittsindikatoren der Zielseite unter der Ergebnisgruppierung angezeigt.

   Nachdem Sie das Ziel aktiviert haben, wird der Fortschritt des Ziels automatisch aktualisiert, wenn Sie den Fortschritt eines Ergebnisses aktualisieren. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront-Zielen](../goal-management/activate-goals.md).
