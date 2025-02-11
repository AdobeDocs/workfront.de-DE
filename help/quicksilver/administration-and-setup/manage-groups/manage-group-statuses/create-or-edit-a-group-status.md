---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Gruppenstatus erstellen oder bearbeiten
description: Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe erstellen. Dies hilft, die Notwendigkeit für Dutzende von unternehmensweiten benutzerdefinierten Status zu vermeiden, und ermöglicht mehr Autonomie in Ihren Gruppenhierarchien.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 1%

---

# Erstellen oder Bearbeiten eines Gruppenstatus

Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe erstellen. Dies hilft, die Notwendigkeit für Dutzende von unternehmensweiten benutzerdefinierten Status zu vermeiden, und ermöglicht mehr Autonomie in Ihren Gruppenhierarchien.

Sie können auch einen Status auf Systemebene für eine von Ihnen verwaltete Gruppe bearbeiten, wenn ein Workfront-Administrator den Status entsperrt hat. Weitere Informationen finden Sie unter [Gesperrte und entsperrte Status auf Systemebene](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>Benutzerdefinierte Gruppenstatus können nicht in einem Projekt angezeigt werden, wenn das Projekt in einer Agile-Ansicht angezeigt wird. Beim Anzeigen eines Projekts in einer Agile-Ansicht sind nur standardmäßige und benutzerdefinierte gesperrte Status sichtbar. Informationen zum Anpassen einer Agile-Ansicht für ein Projekt finden Sie im Abschnitt [Erstellen oder Anpassen einer Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) im Artikel [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Allgemeine Informationen zu Status finden Sie unter [Status - Übersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen oder Bearbeiten eines Status für eine Gruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, in der Sie Status erstellen oder anpassen möchten.
1. Klicken Sie im linken Bedienfeld auf **Status**.

   Wenn es sich bei der angezeigten Gruppe um eine Gruppe auf oberster Ebene handelt, enthält die angezeigte Liste Folgendes:

   * Gesperrte Status auf Systemebene.
   * Benutzerdefinierte Status wurden bereits für die Gruppe erstellt.

   Wenn die angezeigte Gruppe eine Untergruppe ist, enthält die Liste außerdem:

   * Gesperrte Status, die zu den Gruppen oberhalb der Untergruppe gehören.
   * Entsperrte Status, die zu den Gruppen oberhalb der Untergruppe gehörten, als diese erstellt wurde.

     Nachdem eine Untergruppe erstellt wurde, werden entsperrte Status, die in den darüber liegenden Gruppen erstellt wurden, nicht in die Statusliste der Untergruppe aufgenommen. Wenn jedoch jemand eine von ihnen später sperrt, wird sie in die Statusliste der Untergruppe aufgenommen. Weitere Informationen finden Sie unter [So erben Gruppen Status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgaben** oder **Probleme**) aus, den Sie mit dem Status verknüpfen möchten.

1. (Bedingt) Wenn der Status ein Problemstatus ist, stellen Sie sicher, dass **Masterliste** ausgewählt ist.

   ![Hauptliste](assets/master-list.png)

   Informationen zum Anpassen der anderen Problemtypen (Fehlerbericht, Änderungsanforderung, Problem, Anfrage) finden Sie unter [Anpassen von standardmäßigen Problemtypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Bedingt) Um einen neuen Status zu erstellen, klicken Sie auf **Neuen Status hinzufügen**.

   Oder

   Um einen vorhandenen Status zu bearbeiten, bewegen Sie den Mauszeiger über den Status, den Sie bearbeiten möchten, und klicken Sie dann auf die **Bearbeiten** Option, die ganz rechts angezeigt wird.

   ![Gruppenstatus](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Sie können einen Status für Ihre Gruppe nur bearbeiten, wenn Sie:
   >      
   >* Sie verwalten die Gruppe, für die der Status erstellt wurde
   >* Ein Workfront-Administrator hat den Status auf Systemebene entsperrt
   >* Ein Gruppenadministrator einer Gruppe über Ihrer Gruppe hat den Status entsperrt
   >      
   >      
   >Wenn Sie einen vorhandenen Status bearbeiten, können Sie nur dessen Namen, Beschreibung und Farbe ändern.
   >
   >Wenn Sie einen gesperrten Status bearbeiten, wirken sich Ihre Änderungen auf alle Untergruppen aus, die den Status von Ihrer Gruppe übernommen haben.
   >   
   >Umgekehrt wirkt sich die Bearbeitung eines entsperrten Status nicht auf die Untergruppen aus, die den Status von Ihrer Gruppe übernommen haben.

1. Geben Sie die folgenden Informationen an.

   Wenn Sie einen Status bearbeiten, können nur die ersten drei Einstellungen geändert werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusname</td> 
      <td> <p>Geben Sie einen Namen für den Status ein. Dies ist ein Pflichtfeld.</p> <p>Beachten Sie beim Erstellen eines Statusnamens, dass andere Benutzer im System einen Status mit demselben Namen erstellen können. Es wird empfohlen, einen eindeutigen Namen zu verwenden, um Verwirrungen bei der Auswahl von Status in Workfront zu vermeiden.</p><p>Wenn doppelte Status vorhanden sind, sollte der Gruppenadministrator die Namen aktualisieren, um zwischen ihnen zu unterscheiden. Der einzige Eindeutigkeitsindikator im System ist der Statusschlüssel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>(Optional) Geben Sie eine Beschreibung des Status ein. Dies kommuniziert seinen Zweck an diejenigen, die es verwenden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Passen Sie die Farbe des Status an, indem Sie auf das Farbfeld klicken und eine Farbe aus dem Farbfeld auswählen. Sie können auch eine Hexadezimalzahl in das Feld eingeben.</p> <p>Die Statusfarbe wird in der rechten oberen Ecke von Workfront angezeigt, wenn ein(e) Benutzende(r) das Objekt aufruft.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entspricht</td> 
      <td> <p>Wählen Sie eine der Optionen aus der Liste aus, die die Funktion des Status am besten beschreibt. Wenn der Statusname beispielsweise „Fertig“ lautet, sollte die entsprechende Option „Fertig“ sein.</p> <p>Jeder Status muss mit einer dieser Optionen übereinstimmen, da dies bestimmt, wie der Status funktioniert.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schlüssel</td> 
      <td> <p>Wenn Sie einen neuen Status erstellen, geben Sie einen Code oder eine Abkürzung für den Status ein oder verwenden Sie die für Sie generierte Abkürzung. Dieser Schlüssel muss in Workfront eindeutig sein, da er zu Berichtszwecken verwendet werden kann. Wenn Sie versuchen, einen Schlüssel anzugeben, der bereits im System verwendet wird, wird das Feld rot.</p> <p>Es kann nützlich sein, eine Abkürzung zu verwenden, die für diejenigen erkennbar ist, die sie verwenden werden.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> <p>Sie können den Schlüssel-Code für die Status „Planung“, „Aktuell“ und „Abgeschlossen“ nicht ändern. Dies ist wichtig, wenn Sie einen Bericht im Textmodus erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status ausblenden</td> 
      <td> <p>(Nur Projekt- und Aufgabenstatus)</p> <p>Aktivieren Sie diese Option, wenn der Status vor Benutzern ausgeblendet werden soll. Wenn sie deaktiviert ist (Standardeinstellung), können alle Untergruppen unter der Gruppe den Status verwenden.</p> <p>Tipp: Sie können den Status eines Problems ausblenden, indem Sie alle vier Problemtypen deaktivieren (Fehlerbericht, Änderungsanforderung, Problem, Anfrage).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für alle Gruppen sperren</td> 
      <td> 
       <p>Wenn Sie diese Option aktiviert lassen, können die Benutzenden in Ihrer Gruppe und ihren Untergruppen den Status sehen und verwenden und Gruppenadministratoren können ihn nicht für niedrigere Untergruppen anpassen.</p> 
       <p>Wenn diese Option deaktiviert ist, können Gruppenadministratoren den Status für niedrigere Untergruppen anpassen.</p> 
       <p><b>HINWEIS</b>: Sie können in einem Gruppengenehmigungsprozess sowohl gesperrte als auch entsperrte Status verwenden. Wenn Sie einen Gruppengenehmigungsprozess mit einem nicht gesperrten Gruppenstatus erstellen, können Benutzer den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem anhängen, das mit der Gruppe verknüpft ist.</p> 
       <p>Weitere Informationen zum Sperrstatus finden Sie unter <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Gesperrte und entsperrte Gruppenstatus</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Der Status ist jetzt für alle Projekte verfügbar, die mit Ihrer Gruppe oder Untergruppe verknüpft sind. Wenn Sie ihn gesperrt haben, ist er für alle niedrigeren Untergruppen verfügbar.

   Sie können den Status als Standardstatus für die Gruppe konfigurieren. Weitere Informationen finden Sie unter [Verwenden eines benutzerdefinierten Status als Standardstatus für eine Gruppe](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Erstellen eines benutzerdefinierten Status für mehrere Gruppen

Wenn Sie Workfront-Administrator sind, können Sie einen benutzerdefinierten Status für mehrere Gruppen erstellen, indem Sie einen systemweiten Status erstellen und diesen dann für alle Gruppen ausblenden, die ihn nicht benötigen.

Wenn Sie Gruppenadministrator (oder Workfront-Administrator) sind, können Sie einen benutzerdefinierten Status für mehrere Untergruppen innerhalb einer von Ihnen verwalteten Gruppenhierarchie erstellen, indem Sie einen Status für eine Gruppe auf höherer Ebene erstellen und diesen Status dann für alle niedrigeren Untergruppen ausblenden, die ihn nicht benötigen.

1. Wenn Sie ein Workfront-Administrator sind, erstellen Sie einen systemweiten entsperrten Status, wie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) beschrieben.
1. Löschen Sie in dem Feld oben rechts **Systemstatus**, geben Sie den Namen einer Gruppe ein, in der Sie den Status ausblenden möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.
1. Bewegen Sie den Mauszeiger über den Status, den Sie aus der Gruppe ausblenden möchten, und klicken Sie dann auf **Bearbeiten** wenn er angezeigt wird.

   ![Status bearbeiten](assets/hover-click-edit.jpg)

1. Aktivieren Sie die **Status ausblenden** Option, die angezeigt wird.

   ![Status ausblenden](assets/hide-group-status.png)

1. Klicken Sie auf **Speichern**.

   Der Status ist abgeblendet und nicht mehr für alle Benutzenden in dieser Gruppe sichtbar.

1. Wiederholen Sie die Schritte 3 bis 5, um den benutzerdefinierten Status vor allen anderen Gruppen auszublenden, die ihn nicht benötigen.

