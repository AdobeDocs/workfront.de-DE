---
product-previous: workfront-goals
navigation-topic: goal-management
title: Schließen und Erneutes Öffnen von Zielen in Adobe Workfront
description: Sie können ein Ziel schließen, wenn Sie anzeigen möchten, dass Sie es abgeschlossen haben oder nicht mehr daran arbeiten, da es veraltet ist.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 2%

---

# Schließen und erneutes Öffnen von Zielen in Adobe Workfront-Zielen

<!--Audited for P&P only: 4/2025-->

Sie können ein Ziel schließen, wenn Sie Folgendes angeben möchten:

* Das Ziel ist erreicht, weil Sie es erreicht haben oder weil die Zeit verstrichen ist.
* Sie arbeiten nicht mehr daran und planen dies auch nicht in naher Zukunft.

Sie können geschlossene Ziele erneut öffnen, wenn sie wieder relevant werden.

## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

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
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Mitwirkender oder höher</p>
 <p>Anfrage oder höher</p></td>
 </tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr>
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
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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

## Überlegungen beim Schließen oder erneuten Öffnen von Zielen

* Sie müssen Zugriff auf „Ziele bearbeiten“ in Ihrer Zugriffsebene haben, bevor Sie Ziele schließen und erneut öffnen können. Informationen zum Gewähren des Zugriffs auf Ziele finden Sie unter [Gewähren des Zugriffs auf Adobe Workfront-Ziele](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Sie können nur aktive Ziele schließen. Ziele mit dem Status Entwurf können nicht geschlossen werden.

  Informationen zum Zielstatus finden Sie unter [Zielstatusübersicht in Adobe Workfront-](../../workfront-goals/goal-management/goal-status-overview.md).

* Das Schließen von Zielen blockiert den Fortschritt und ermöglicht es Ihnen zu bewerten, wie gut Sie dabei waren.

  >[!CAUTION]
  >
  >Beim Schließen eines Ziels, das aktive beitragende Ziele hat, ändert sich sein Fortschritt nach dem Schließen, um den Fortschritt der aktiven beitragenden Ziele anzugeben. Informationen zum Ausrichten von Zielen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-Zielen](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Aktualisieren Sie die Fortschrittsanzeigen des Ziels, bevor Sie das Ziel schließen, um sicherzustellen, dass das Ziel mit einem genauen Fortschrittswert geschlossen wird. Wenn alle Fortschrittsindikatoren erreicht wurden, sollte das Ziel in Prozent abgeschlossen 100 % betragen und das Ziel wurde erreicht. Informationen zum Aktualisieren Ihrer Produktziele finden Sie unter [Aktualisieren des Zielfortschritts in Adobe Workfront-Produktzielen](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Hinterlassen Sie alle abschließenden Kommentare als Aktualisierung der Ziele, die Sie schließen. Informationen zum Hinzufügen von Kommentaren zu Zielen finden Sie unter [Verwalten von Zielkommentaren in Adobe Workfront-](../../workfront-goals/goal-management/manage-goal-comments.md).
* Sie können den Fortschritt der Ergebnisse und Aktivitäten für ein Ziel, das Sie schließen, nicht mehr aktualisieren.
* Sie können ein geschlossenes Ziel erneut öffnen, wenn Sie es weiter bearbeiten möchten.
* Wenn das Ziel nicht erreicht wurde, kopieren Sie die meisten seiner Informationen in den nächsten Zeitraum (Quartal oder Jahr). Dies ist eine großartige Option für Ziele, die von einem Zeitraum zum nächsten gleich sind, oder für Ziele, an deren Erreichung Sie möglicherweise noch im nächsten Zeitrahmen arbeiten müssen. Informationen zum Kopieren von Zielen finden Sie unter [Kopieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/copy-goals.md). Sie können auch den Zeitraum im Ziel aktualisieren, anstatt ihn in einen anderen Zeitraum zu kopieren.
* Workfront löscht die Kommentare eines geschlossenen Ziels, wenn es erneut geöffnet wird. Wenn Sie die Kommentare beibehalten müssen, empfehlen wir, das geschlossene Ziel einschließlich der damit verbundenen Ergebnisse zu kopieren, anstatt es erneut zu öffnen.


## Ziele schließen

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![Closing goals with active aligned goals](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

{{step1-to-goals}}

Die Liste „Ziel“ wird geöffnet.

1. (Optional) Ändern Sie Ihre Filter, um nur aktive Ziele anzuzeigen.

   Informationen zum Filtern von Informationen in Workfront Goals finden Sie unter [Filtern von Informationen in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Klicken Sie auf ein aktives Ziel.

   Die Zielseite wird geöffnet.

   ![Zielseite](assets/goal-page-unshimmed.png)
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Zielnamen und dann auf **Schließen**.

   Das Ziel wird geschlossen und Sie erhalten eine Bestätigung in der oberen rechten Ecke des Bildschirms.

   ![Bestätigung zum Schließen des Ziels](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Optional) Klicken Sie im Bestätigungsfeld auf **Abschließende Anmerkungen hinzufügen**, um Kommentare zu diesem Ziel hinzuzufügen und zu erklären, warum Sie es schließen müssen.
1. Fügen Sie abschließende Anmerkungen hinzu und klicken Sie dann auf **Anmerkungen hinzufügen**.

   ![Endnotenfeld hinzufügen](assets/add-closing-notes-box-unshimmed.png)

   Die Kommentare werden im Abschnitt „Zieldetails“ der Zielseite im Bereich „Abschließende Anmerkungen“ angezeigt.

   >[!NOTE]
   >
   >Workfront löscht die Schlussnotizen, wenn Sie später ein geschlossenes Ziel erneut öffnen.


## Ziele erneut öffnen

Sie können geschlossene Ziele erneut öffnen, wenn Sie feststellen, dass sie wieder relevant geworden sind und Sie ihren Fortschritt weiterhin aktualisieren müssen.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

{{step1-to-goals}}

Die Liste „Ziel“ wird geöffnet.

1. (Optional) Ändern Sie Ihre Filter, um nur Ziele anzuzeigen, die geschlossen sind.

   Informationen zum Filtern von Informationen in Workfront Goals finden Sie unter [Filtern von Informationen in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).
1. Klicken Sie auf den Namen eines geschlossenen Ziels.

   Die Zielseite wird geöffnet.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Zielnamen und dann **Erneut öffnen** > **Erneut öffnen**.

   Folgendes geschieht:
   * Das Ziel ist jetzt offen und hat den Status Aktiv .
   * Der Fortschritt des Ziels wird ab dem aktuellen Datum neu berechnet.
   * Alle abschließenden Anmerkungen werden von der Seite mit den Zieldetails gelöscht. Gelöschte Abschlussnotizen können nicht wiederhergestellt werden.

1. (Optional) Ändern Sie Ihre Filter erneut, um nur aktive Ziele anzuzeigen.

   Die von Ihnen geöffneten Ziele werden auf dem Bildschirm angezeigt.

