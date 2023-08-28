---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Timesheet-Informationen bearbeiten
description: Als Benutzer mit Administratorzugriff auf Timesheets können Sie Informationen zu vorhandenen Timesheets in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die Genehmiger oder den Zeitrahmen des Zeitblatts bearbeiten.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# Timesheet-Informationen bearbeiten

Als Benutzer mit Administratorzugriff auf Timesheets können Sie Informationen zu vorhandenen Timesheets in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die Genehmiger oder den Zeitrahmen des Zeitblatts bearbeiten.

Sie können Informationen in einem einzigen Zeitblatt bearbeiten oder mehrere Zeitpläne in großen Mengen bearbeiten.

>[!IMPORTANT]
>
>Wenn Benutzer mit Timesheet-Profilen verknüpft sind und die Timesheets automatisch generiert werden, spiegeln die Änderungen an vorhandenen Timesheets nicht die Timesheets wider, die für zukünftige Datumsangaben erstellt werden. Bei allen automatisch erstellten Timesheets werden die Einstellungen in den Timesheet-Profilen festgelegt. Weitere Informationen finden Sie unter [Erstellen von Timesheet-Profilen](../create-and-manage-timesheets/create-timesheet-profiles.md)


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
   <td> <p>Sie müssen über Administratorzugriff auf Timesheets verfügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Timesheets bearbeiten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Timesheets**.

   Die **Alle** ist standardmäßig ausgewählt, wodurch alle Timesheets angezeigt werden, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Klicken Sie auf die **suchen** icon ![](assets/search-icon.png) und geben Sie einen Suchbegriff ein und suchen Sie nach einem bestimmten Zeitblatt. Sie können beispielsweise nach einem Zeitrahmen für ein Zeitblatt oder nach dem Namen des Eigentümers suchen.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Auswählen **Meine Datenblatt-Genehmigungen** oben rechts auf der Seite, um nur die von Ihnen genehmigten Timesheets anzuzeigen

     Oder

     Auswählen **Meine Timesheets** , um nur Ihre Timesheets anzuzeigen.

     Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) um einen anderen Filter anzuwenden oder einen neuen zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   >
   >   
   >   
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Optional) Klicken Sie auf die **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) Symbole, um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Wählen Sie einen oder mehrere Timesheets aus und klicken Sie dann auf das **Bearbeiten** icon ![](assets/edit-icon.png) oben in der Liste der Zeitpläne.
1. Zeigen Sie die folgenden Informationen an oder geben Sie sie an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Besitzerin bzw. Besitzer</strong> </td> 
      <td> <p>Dies ist der Name des Benutzers, für den das Timesheet erstellt wurde. Dieses Feld kann nicht bearbeitet werden. </p> <p>Das Feld wird nicht angezeigt, wenn Sie mehrere Timesheets auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Startdatum</strong> </td> 
      <td>Dies ist das Startdatum des Zeitplans.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enddatum</strong> </td> 
      <td> Dies ist das Enddatum des Zeitplans.</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td> Dies ist der Status des Zeitblatts.
      Die folgenden Optionen sind für den Status von Zeitblättern möglich: 
      <ul><li><b>Öffnen</b>: Das Timesheet ist geöffnet und die Stundeneinträge können bearbeitet werden.</li>
      <li><b>Gesendet</b>: Das Timesheet wird den vorgesehenen Genehmigern zur Genehmigung vorgelegt.</li>
      <li><b>Abgelehnt</b>: Das Timesheet wurde von den Genehmigern nicht genehmigt und steht nun dem Benutzer erneut zur Bearbeitung der Zeiteinträge zur Verfügung.</li>
      <li><b>Geschlossen</b>: Das Timesheet wird entweder vom Benutzer geschlossen oder vom Genehmiger genehmigt, sodass es nun geschlossen wird. Sie können einem geschlossenen Timesheet keine Zeit hinzufügen.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Genehmigende Personen</strong> </td> 
      <td> <p>Genehmiger sind Benutzer, die das Timesheet für die mit dem Timesheet verknüpften Benutzer validieren. Nur Benutzer mit administrativem Zugriff auf Timesheets können als Genehmiger festgelegt werden. </p> <p>Weitere Informationen zu den Verwaltungsrechten für Zeitblätter finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p>Geben Sie die Namen der Timesheet-Genehmiger ein und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.</p> <p>Sie können mehrere Genehmiger auf einem Zeitblatt haben. In diesem Fall wird das Timesheet nach Genehmigung durch einen der Genehmiger als <strong>Geschlossen</strong> und wird aus der Liste der Zeitdatenblatt-Genehmigungen aller verbleibenden Genehmiger entfernt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kann Zeit bearbeiten</strong> </td> 
      <td> <p>Wählen Sie diese Option aus, wenn Sie zulassen möchten, dass Genehmiger Stunden auf dem Timesheet bearbeiten können.</p> <p>Diese Option ist nicht verfügbar, wenn Sie mehrere Timesheets auswählen. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td> <p>Sie können das Feld Überstunden auf dem Timesheet ausblenden.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
