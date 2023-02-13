---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Löschen von Timesheets in Adobe Workfront
description: Die Änderungen, die Sie an einem Timesheet-Profil vornehmen, sind für die derzeit vorhandenen Timesheets nicht sofort wirksam, wie unter Erstellen, Bearbeiten und Zuweisen von Zeitzeichenprofilen beschrieben. Um die Änderungen in vorhandenen Timesheets sichtbar zu machen, müssen Sie die generierten Timesheets löschen und neue erstellen. Dies gilt nur für Timesheets, die durch das Verknüpfen von Timesheet-Profilen mit Benutzern generiert wurden.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Löschen von Timesheets in Adobe Workfront

Die Änderungen, die Sie an einem Timesheet-Profil vornehmen, sind für die derzeit vorhandenen Timesheets nicht sofort wirksam, wie hier beschrieben: [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Um die Änderungen in vorhandenen Timesheets sichtbar zu machen, müssen Sie die generierten Timesheets löschen und neue erstellen. Dies gilt nur für Timesheets, die durch das Verknüpfen von Timesheet-Profilen mit Benutzern generiert wurden.

>[!NOTE]
>
>Manuell erstellte Timesheets können nicht durch die Neuerstellung von Timesheets neu erstellt werden, es sei denn, die Benutzer wurden seit der manuellen Erstellung des Timesheets mit einem Timesheet-Profil verknüpft. Das Löschen eines manuell erstellten Zeitblatts kann zu Datenverlust führen. Informationen zum Erstellen einzelner Timesheets finden Sie unter [Erstellen eines Datenblatts für die einmalige Verwendung](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Adobe Workfront-Administratoren oder -Gruppenadministratoren können für alle Benutzer des Systems Timesheets generieren. Weitere Informationen zum manuellen Generieren von Timesheets finden Sie unter:

* [Manuelles Generieren von Timesheets](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Erstellen und Verwalten von Timesheet-Profilen einer Gruppe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Ein gelöschtes Timesheet kann nicht wiederhergestellt werden.
>* Es wird empfohlen, vergangene Timesheets nicht zu löschen, da sie nicht automatisch auf der Grundlage von Timesheet-Profilen erstellt werden. Sie können die aktuellen und zukünftigen Timesheets löschen und manuell generieren, wenn Sie möchten, dass die Änderungen an Ihren Timesheet-Profilen sofort in den neuen Timesheets sichtbar sind.
>* Wenn Sie Timesheets löschen, werden die Stunden, die mit Aufgaben, Problemen und Projekten protokolliert wurden, nicht gelöscht. Nur die allgemeinen Stunden werden mit dem Timesheet gelöscht. Geben Sie in einem separaten Texteditor an, welche allgemeinen Stunden mit dem Zeitblatt verknüpft sind. Nachdem das Timesheet gelöscht wurde, können Sie es im neuen Timesheet einloggen.
>


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen über Administratorzugriff auf Timesheets verfügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Löschen von Timesheets in einer Liste

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Timesheets**. Die **Alle** -Filter ist standardmäßig ausgewählt und es werden alle Timesheets angezeigt, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Auswählen **Meine Datenblatt-Genehmigungen** oben rechts auf der Seite, um nur die von Ihnen genehmigten Timesheets anzuzeigen

      Oder

      Auswählen **Meine Timesheets** , um nur Ihre Timesheets anzuzeigen.

      Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) um einen anderen Filter anzuwenden oder einen neuen zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optional) Klicken Sie auf die **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) Symbole, um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Wählen Sie einen oder mehrere zu löschende Timesheets aus und klicken Sie auf die Schaltfläche **Löschen**  ![](assets/delete.png) -Symbol oben in der Liste der Timesheets.

1. Klicken **Löschen**.

   Die ausgewählten Timesheets werden gelöscht und können nicht wiederhergestellt werden.

   Um neue Timesheets zu erstellen, stellen Sie sicher, dass Benutzer mit einem Timesheet-Profil verknüpft sind, und bitten Sie den Workfront-Administrator oder einen Gruppenadministrator, neue Timesheets zu erstellen.

   Weitere Informationen finden Sie unter folgenden Themen:

   * [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Manuelles Generieren von Timesheets](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Erstellen und Verwalten von Timesheet-Profilen einer Gruppe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Zeitblatt aus der Timesheet-Seite löschen

1. Klicken Sie auf [!UICONTROL **Hauptmenü**] icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken Sie auf das zu löschende Timesheet, um es zu öffnen.
1. Klicken Sie auf [!UICONTROL **Mehr**] icon ![](assets/more-icon.png) rechts neben dem Namen des Zeitplans klicken Sie auf **Löschen**.

   ![Timesheet aus der Timesheet-Seite löschen](assets/delete-timesheet-from-timesheet-page.png)
1. Klicken [!UICONTROL **Löschen**] zur Bestätigung.

   Das Zeitblatt wird gelöscht und kann nicht wiederhergestellt werden.
