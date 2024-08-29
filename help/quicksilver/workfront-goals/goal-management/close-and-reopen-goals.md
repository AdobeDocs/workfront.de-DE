---
product-previous: workfront-goals
navigation-topic: goal-management
title: Ziele in Adobe Workfront schließen und erneut öffnen
description: Sie können ein Ziel schließen, wenn Sie angeben möchten, dass Sie es abgeschlossen haben oder dass Sie nicht mehr daran arbeiten, weil es veraltet wurde.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Ziele in Adobe Workfront schließen und erneut öffnen

Sie können ein Ziel schließen, wenn Sie Folgendes angeben möchten:

* Das Ziel wird erreicht, entweder weil Sie es erreicht haben oder weil der Zeitraum abgelaufen ist.
* Du arbeitest nicht mehr daran, noch hast du vor, dies in nächster Zukunft zu tun.

Sie können Ziele, die geschlossen wurden, wenn sie wieder relevant werden, erneut öffnen.

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
  <ul><li>Ein ultimativer Plan </li></ul>
   </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
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
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Schließen oder erneuten Öffnen von Zielen

* Sie müssen Zugriff auf die Option Ziele bearbeiten in Ihrer Zugriffsebene haben, bevor Sie Ziele schließen und erneut öffnen können. Informationen zur Gewährung des Zugriffs auf Ziele finden Sie unter [Gewähren des Zugriffs auf Adobe Workfront-Ziele](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* Sie können nur aktive Ziele schließen. Ziele, die sich im Status Entwurf befinden, können nicht geschlossen werden.

  Informationen zu den Zielstatus finden Sie unter [Zielstatusübersicht in Adobe Workfront-Zielen](../../workfront-goals/goal-management/goal-status-overview.md).

* Das Schließen von Zielen hängt in seinem Fortschritt ab und ermöglicht es Ihnen, zu beurteilen, wie gut Sie es bei der Erreichung des Ziels gemacht haben.

  >[!CAUTION]
  >
  >Beim Schließen eines Ziels mit aktiven Beitragszielen ändert sich der Fortschritt nach dem Schließen, um den Fortschritt der beitragenden aktiven Ziele anzuzeigen. Informationen zum Ausrichten von Zielen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Aktualisieren Sie die Fortschrittsanzeigen des Ziels, bevor Sie das Ziel schließen, um sicherzustellen, dass das Ziel mit einem genauen Fortschrittswert geschlossen wird. Wenn alle Fortschrittsindikatoren erreicht wurden, sollte der Zielprozentsatz vollständig erreicht werden und Ihr Ziel wurde erreicht. Informationen zum Aktualisieren Ihrer Ziele finden Sie unter [Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Lassen Sie alle endgültigen Kommentare als Update zu den Zielen, die Sie schließen. Informationen zum Hinzufügen von Kommentaren zu Zielen finden Sie unter [Zielkommentare in Adobe Workfront-Zielen verwalten](../../workfront-goals/goal-management/manage-goal-comments.md).
* Sie können den Fortschritt von Ergebnissen und Aktivitäten bei einem Ziel, das Sie schließen, nicht mehr aktualisieren.
* Sie können ein geschlossenes Ziel erneut öffnen, wenn Sie weiterhin daran arbeiten möchten.
* Wenn das Ziel nicht erreicht wurde, sollten Sie erwägen, die meisten Informationen in den nächsten Zeitraum (Quartal oder Jahr) zu kopieren. Dies ist eine großartige Option für Ziele, die von einem Zeitraum zum nächsten identisch sind, oder für Ziele, an denen Sie möglicherweise noch im nächsten Zeitrahmen arbeiten müssen. Informationen zum Kopieren von Zielen finden Sie unter [Kopieren von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/copy-goals.md). Sie können den Zeitraum für das Ziel auch aktualisieren, anstatt ihn in einen anderen Zeitraum zu kopieren.
* Workfront löscht die Kommentare zu einem geschlossenen Ziel, wenn Sie es erneut öffnen. Wenn Sie die Kommentare beibehalten müssen, empfehlen wir, das geschlossene Ziel einschließlich der damit verbundenen Ergebnisse zu kopieren, anstatt es erneut zu öffnen.


## Ziele schließen

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Klicken Sie oben rechts auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) > **Ziele** .

   Die Zielliste wird geöffnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Ändern Sie Ihre Filter so, dass nur aktive Ziele angezeigt werden.

   Informationen zum Filtern von Informationen in Workfront-Zielen finden Sie unter [Filtern von Informationen in Adobe Workfront-Zielen](../goal-management/filter-information-wf-goals.md).
1. Klicken Sie auf ein aktives Ziel.

   Die Zielseite wird geöffnet.

   ![](assets/goal-page-unshimmed.png)
1. Klicken Sie auf das Menü **Mehr** rechts neben dem Zielnamen und dann auf **Schließen**.![](assets/more-icon.png)

   Das Ziel wird geschlossen und Sie erhalten eine Bestätigung in der rechten oberen Ecke des Bildschirms.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Optional) Klicken Sie im Bestätigungsfeld auf **Notizen zum Schließen hinzufügen** , um Kommentare zu diesem Ziel und dazu hinzuzufügen, warum Sie es schließen müssen.
1. Fügen Sie schließende Notizen hinzu und klicken Sie dann auf **Notizen hinzufügen**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   Die Kommentare werden im Abschnitt &quot;Zieldetails&quot;der Zielseite im Bereich &quot;Notizen schließen&quot;angezeigt.

   >[!NOTE]
   >
   >Workfront löscht die schließenden Notizen, wenn Sie ein geschlossenes Ziel später erneut öffnen.


## Ziele erneut öffnen

Sie können geschlossene Ziele erneut öffnen, wenn Sie sich dafür entscheiden, dass sie erneut relevant geworden sind und dass Sie den Fortschritt der Ziele weiter aktualisieren müssen.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Klicken Sie oben rechts auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png)> **Ziele** .

   Die Zielliste wird geöffnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optional) Ändern Sie Ihre Filter so, dass nur geschlossene Ziele angezeigt werden.

   Informationen zum Filtern von Informationen in Workfront-Zielen finden Sie unter [Filtern von Informationen in Adobe Workfront-Zielen](../goal-management/filter-information-wf-goals.md).
1. Klicken Sie auf den Namen eines geschlossenen Ziels.

   Die Zielseite wird geöffnet.
1. Klicken Sie auf das Menü **Mehr** rechts neben dem Zielnamen und dann auf **Neu öffnen** > **Erneut öffnen**.![](assets/more-icon.png)

   Folgendes geschieht:
   * Das Ziel ist jetzt geöffnet und hat den Status Aktiv .
   * Der Fortschritt des Ziels wird ab dem aktuellen Datum neu berechnet.
   * Alle abschließenden Hinweise werden von der Seite mit den Zieldetails gelöscht. Gelöschte Schlussnotizen können nicht wiederhergestellt werden.

1. (Optional) Ändern Sie Ihre Filter erneut, sodass nur aktive Ziele angezeigt werden.

   Die von Ihnen geöffneten Ziele werden auf dem Bildschirm angezeigt.

