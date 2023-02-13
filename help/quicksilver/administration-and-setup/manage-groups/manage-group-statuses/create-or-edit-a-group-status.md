---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Erstellen oder Bearbeiten eines Gruppenstatus
description: Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe erstellen. Dadurch wird die Notwendigkeit von Dutzenden von unternehmensweiten benutzerdefinierten Status beseitigt und eine größere Autonomie in Ihren Gruppenhierarchien ermöglicht.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# Erstellen oder Bearbeiten eines Gruppenstatus

Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe erstellen. Dadurch wird die Notwendigkeit von Dutzenden von unternehmensweiten benutzerdefinierten Status beseitigt und eine größere Autonomie in Ihren Gruppenhierarchien ermöglicht.

Sie können auch den Status auf Systemebene für eine von Ihnen verwaltete Gruppe bearbeiten, wenn ein Workfront-Administrator den Status entsperrt hat. Weitere Informationen finden Sie unter [Status auf Systemebene gesperrt und entsperrt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>Benutzerdefinierte Gruppenstatus können in einem Projekt nicht angezeigt werden, wenn das Projekt in einer agilen Ansicht angezeigt wird. Beim Anzeigen eines Projekts in einer agilen Ansicht sind nur die standardmäßigen und benutzerdefinierten gesperrten Status sichtbar. Informationen zum Anpassen einer agilen Ansicht für ein Projekt finden Sie im Abschnitt [Erstellen oder Anpassen einer Agile-Ansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Allgemeine Informationen zum Status finden Sie unter [Statusübersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Erstellen oder Bearbeiten eines Status für eine Gruppe

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, in der Sie Status erstellen oder anpassen möchten.
1. Klicken Sie im linken Bereich auf **Status**.

   Wenn es sich bei der angezeigten Gruppe um eine Gruppe der obersten Ebene handelt, enthält die angezeigte Liste Folgendes:

   * Sperrstatus auf Systemebene.
   * Benutzerdefinierte Status, die bereits für die Gruppe erstellt wurden.

   Wenn es sich bei der angezeigten Gruppe um eine Untergruppe handelt, enthält die Liste außerdem:

   * Gesperrte Status, die zu den Gruppen über der Untergruppe gehören.
   * Entsperrte Status, die zu den Gruppen über der Untergruppe gehörten, als sie erstellt wurde.

      Nach der Erstellung einer Untergruppe werden entsperrte Status, die in den oben stehenden Gruppen erstellt werden, nicht in die Statusliste der Untergruppe aufgenommen. Wenn jedoch einer von ihnen später gesperrt wird, wird er in die Statusliste der Untergruppe aufgenommen. Weitere Informationen finden Sie unter [Vererben von Status durch Gruppen](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgaben** oder **Probleme**), die Sie mit dem Status verknüpfen möchten.

1. (Bedingt) Wenn der Status ein Problemstatus ist, stellen Sie sicher, dass **Übergeordnete Liste** ausgewählt ist.

   ![](assets/master-list.png)

   Informationen zum Anpassen der anderen Problemtypen (Fehlerbericht, Reihenfolge ändern, Problem, Anforderung) finden Sie unter [Anpassen von Standardausgabetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Bedingt) Um einen neuen Status zu erstellen, klicken Sie auf **Neuen Status hinzufügen**.

   Oder

   Um einen vorhandenen Status zu bearbeiten, bewegen Sie den Mauszeiger über den Status, den Sie bearbeiten möchten, und klicken Sie dann auf **Bearbeiten** -Option, die ganz rechts angezeigt wird.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Sie können einen Status für Ihre Gruppe nur bearbeiten, wenn:
   >      
   >* Sie verwalten die Gruppe, für die der Status erstellt wurde
   >* Ein Workfront-Administrator entsperrt den Status auf Systemebene
   >* Gruppenadministrator einer Gruppe oberhalb Ihrer Gruppe entsperrt den Status

   >      
   >      
   >Wenn Sie einen vorhandenen Status bearbeiten, können Sie nur dessen Namen, Beschreibung und Farbe ändern.
   >
   >Wenn Sie einen gesperrten Status bearbeiten, wirken sich Ihre Änderungen auf alle Untergruppen aus, die den Status von Ihrer Gruppe übernommen haben.
   >   
   >Die Bearbeitung eines entsperrten Status wirkt sich dagegen nicht auf die Untergruppen aus, die den Status von Ihrer Gruppe übernommen haben.

1. Geben Sie die folgenden Informationen an.

   Wenn Sie einen Status bearbeiten, können nur die ersten drei Einstellungen geändert werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusname</td> 
      <td> <p>Geben Sie einen Namen für den Status ein. Dies ist ein Pflichtfeld.</p> <p>Beachten Sie beim Erstellen eines Statusnamens, dass andere Benutzer im System einen Status mit demselben Namen erstellen können. Es wird empfohlen, einen eindeutigen Namen zu verwenden, um Verwirrung bei der Auswahl von Status in Workfront zu vermeiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>(Optional) Geben Sie eine Beschreibung des Status ein. Dieser kommuniziert seinen Zweck mit denen, die ihn verwenden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Passen Sie die Farbe des Status an, indem Sie auf das Farbfeld klicken und eine Farbe aus dem Farbfeldbedienfeld auswählen. Sie können auch eine Hexadezimalzahl in das Feld eingeben.</p> <p>Die Statusfarbe wird oben rechts in Workfront angezeigt, wenn ein Benutzer das Objekt anzeigt.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entspricht</td> 
      <td> <p>Wählen Sie eine der Optionen aus der Liste aus, die die Funktion des Status am besten beschreibt. Wenn der Statusname beispielsweise Fertig lautet, sollte die Option, mit der er übereinstimmt, "Fertig"lauten.</p> <p>Jeder Status muss mit einer dieser Optionen übereinstimmen, da dies bestimmt, wie der Status funktioniert.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schlüssel</td> 
      <td> <p>Wenn Sie einen neuen Status erstellen, geben Sie einen Code oder eine Abkürzung für den Status ein oder verwenden Sie den für Sie generierten Status. Dieser Schlüssel muss in Workfront eindeutig sein, da er zu Berichtszwecken verwendet werden kann. Wenn Sie versuchen, einen Schlüssel anzugeben, der bereits im System verwendet wird, wird das Feld rot.</p> <p>Es kann nützlich sein, eine Abkürzung zu verwenden, die für diejenigen erkennbar ist, die sie verwenden werden.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> <p>Sie können den Schlüsselcode für die Status Planung, Aktuell und Abgeschlossen nicht ändern. Dies ist wichtig, wenn Sie einen Bericht im Textmodus erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status ausblenden</td> 
      <td> <p>(Nur Projekt- und Aufgabenstatus)</p> <p>Aktivieren Sie diese Option, wenn der Status für Benutzer ausgeblendet werden soll. Wenn sie deaktiviert ist (Standardeinstellung), können alle Untergruppen unter der Gruppe den Status verwenden.</p> <p>Tipp: Sie können den Status eines Problems ausblenden, indem Sie alle vier Ausgabetypen deaktivieren (Fehlerbericht, Reihenfolge ändern, Problem, Anforderung).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für alle Gruppen sperren</td> 
      <td> 
       <p>Wenn Sie diese Option aktiviert lassen, können die Benutzer in Ihrer Gruppe und ihren Untergruppen den Status anzeigen und verwenden und Gruppenadministratoren können ihn nicht für niedrigere Untergruppen anpassen.</p> 
       <p>Wenn diese Option deaktiviert ist, können Gruppenadministratoren den Status für niedrigere Untergruppen anpassen.</p> 
       <p><b>NOTE</b>: Sie können sowohl gesperrte als auch entsperrte Status in einem Gruppengenehmigungsprozess verwenden. Wenn Sie einen Gruppengenehmigungsprozess mit einem entsperrten Gruppenstatus erstellen, können Benutzer den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem anhängen, das mit der Gruppe verknüpft ist.</p> 
       <p>Weitere Informationen zum Sperren von Status finden Sie unter <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Gesperrte und entsperrte Gruppenstatus</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Der Status ist jetzt für alle Projekte verfügbar, die mit Ihrer Gruppe oder Untergruppe verbunden sind. Wenn Sie sie gesperrt haben, ist sie für die Verwendung durch Untergruppen verfügbar.

   Sie können den Status als Standardstatus für die Gruppe konfigurieren. Weitere Informationen finden Sie unter [Benutzerdefinierten Status als Standardstatus für eine Gruppe verwenden](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Benutzerdefinierten Status für mehrere Gruppen erstellen

Wenn Sie Workfront-Administrator sind, können Sie einen benutzerdefinierten Status für mehrere Gruppen erstellen, indem Sie einen systemweiten Status erstellen und diesen Status dann für alle Gruppen ausblenden, die ihn nicht benötigen.

Wenn Sie Gruppenadministrator (oder Workfront-Administrator) sind, können Sie einen benutzerspezifischen Status für mehrere Untergruppen innerhalb einer von Ihnen verwalteten Gruppenhierarchie erstellen, indem Sie einen Status für eine übergeordnete Gruppe erstellen und diesen Status dann für alle niedrigeren Untergruppen ausblenden, die ihn nicht benötigen.

1. Wenn Sie Workfront-Administrator sind, erstellen Sie einen systemweiten entsperrten Status wie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Löschen Sie im Feld oben rechts **Systemstatus**, geben Sie den Namen einer Gruppe ein, in der Sie den Status ausblenden möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.
1. Bewegen Sie den Mauszeiger über den Status, den Sie in der Gruppe ausblenden möchten, und klicken Sie dann auf **Bearbeiten** angezeigt.

   ![](assets/hover-click-edit.jpg)

1. Aktivieren Sie die **Status ausblenden** angezeigt.

   ![](assets/hide-group-status.png)

1. Klicken Sie auf **Speichern**.

   Der Status ist abgeblendet und nicht mehr für alle Benutzer dieser Gruppe sichtbar.

1. Wiederholen Sie die Schritte 3 bis 5, um den benutzerdefinierten Status für alle anderen Gruppen auszublenden, die ihn nicht benötigen.
