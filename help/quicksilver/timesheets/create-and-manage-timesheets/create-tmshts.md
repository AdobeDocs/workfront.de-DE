---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Erstellen eines Datenblatts für die einmalige Verwendung
description: Sie können ein einmalig zu verwendendes Timesheet manuell erstellen, wenn Sie ein nicht wiederkehrendes Timesheet wünschen. Wenn das Enddatum des Timesheets erreicht ist und Sie mehr Timesheets benötigen, müssen Sie neue erstellen.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# Erstellen eines Datenblatts für die einmalige Verwendung

Sie können ein einmalig zu verwendendes Timesheet manuell erstellen, wenn Sie ein nicht wiederkehrendes Timesheet wünschen. Wenn das Enddatum des Timesheets erreicht ist und Sie mehr Timesheets benötigen, müssen Sie neue erstellen.

Informationen zum Erstellen eines Timesheet-Profils, das wiederkehrende Timesheets für Ihre Benutzer generiert, ohne dass Sie weitere Eingriffe von Ihnen vornehmen (empfohlen), finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Timesheets für die einmalige Verwendung können nicht für Gruppen erstellt werden.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Bei der Erstellung eines Zeitblatts mit nur einer Verwendung können Sie keine bestimmten allgemeinen Stundentypen auswählen, die in Ihr Zeitblatt aufgenommen werden sollen. Alle allgemeinen Stundentypen, die in Ihrem System aktiviert sind, werden in manuell erstellten Timesheets angezeigt.
>
>  Wenn Sie nur bestimmte allgemeine Stundentypen auswählen möchten, die in Ihren Timesheets angezeigt werden sollen, verwenden Sie ein Timesheet-Profil. Weitere Informationen zu Timesheet-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>Sie müssen über Administratorzugriff auf Timesheets verfügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p><b> NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Datenblatts für die einmalige Verwendung

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Timesheets**. Die **Alle** -Filter ist standardmäßig ausgewählt. Dadurch werden alle Timesheets angezeigt, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Auswählen **Meine Datenblatt-Genehmigungen** oben rechts auf der Seite, um nur die von Ihnen genehmigten Timesheets anzuzeigen

      Oder

      Auswählen **Meine Timesheets** , um nur Ihre Timesheets anzuzeigen.

      Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) um einen anderen Filter anzuwenden oder einen neuen zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   > 
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (Optional) Klicken Sie auf die **Suche** icon ![](assets/search-icon.png) um einen Suchbegriff einzugeben und nach einem bestimmten Zeitblatt zu suchen. Sie können beispielsweise nach einem Zeitrahmen für das Zeitblatt des Eigentümernamens suchen.

1. (Optional) Klicken Sie auf die **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) Symbole, um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klicken **Neues Zeitblatt** oben in der Liste der Timesheets.

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Arbeitszeittabelle erstellen für</strong> </td> 
      <td>Geben Sie den Namen des Benutzers, die Rolle des Auftrags oder das Team ein, für das Sie das Timesheet erstellen, und klicken Sie auf diesen, wenn er in der Liste angezeigt wird.</td> 
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
      <td role="rowheader"><strong>Genehmigende Personen</strong> </td> 
      <td>Genehmiger sind Benutzer, die das Timesheet für die mit dem Timesheet verknüpften Benutzer validieren. Als Genehmiger können nur Benutzer mit Zeitblatt-Administratorrechten festgelegt werden. Weitere Informationen zu den Verwaltungsrechten für Zeitblätter finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.<br>Geben Sie die Namen der Timesheet-Genehmiger ein und klicken Sie auf diese, wenn sie in der Liste angezeigt werden.<br>Sie können mehrere Genehmiger auf einem Zeitblatt haben. In diesem Fall wird das Timesheet nach Genehmigung durch einen der Genehmiger als <strong>Geschlossen</strong> und wird aus der Liste der Zeitdatenblatt-Genehmigungen aller verbleibenden Genehmiger entfernt.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Kann Zeit bearbeiten</strong> </td>

   <td> <p>Wählen Sie diese Option aus, wenn Sie zulassen möchten, dass Genehmiger Stunden auf dem Timesheet bearbeiten können.</p>

   Diese Option funktioniert zusammen mit dem **Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren** im Bereich Einstellungen > Timesheet &amp; Stunden > Voreinstellungen . Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Zeitblatt- und Stundenvoreinstellungen konfigurieren</a>.

   Die folgenden Szenarien existieren:

   <ul>
      <li>Wenn die <b>Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren</b> -Option aktiviert ist:</li>
   <ul><li>Die Genehmiger können das Timesheet nur genehmigen und ablehnen, unabhängig davon, ob die <b>Kann die Zeit bearbeiten</b> aktiviert ist oder nicht. </li>
   <li>Die Manager der Timesheet-Eigentümer können nur die Timesheets ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul>
   <li>Wenn die <b>Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren</b> ist deaktiviert:</li>
   <ul><li>Wenn die <b>Kann die Zeit bearbeiten</b> aktiviert ist, können Genehmiger das Timesheet senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li>
   <li>Wenn die <b>Kann die Zeit bearbeiten</b> deaktiviert ist, können Genehmiger das Timesheet nicht senden, erneut öffnen oder schließen und können die Zeit nicht bearbeiten. Die Validierer können das Timesheet nur genehmigen oder ablehnen. </li>
   <li>Die Manager von Timesheet-Eigentümern können die Timesheets ihrer direkt unterstellten Mitarbeiter senden, abrufen, erneut öffnen und bearbeiten.</li></ul>
   </ul>

   <p><b>NOTIZ</b>

   Sobald Sie ein Zeitblatt zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um ein gesendetes Timesheet in einen bearbeitbaren Zustand zurückzuversetzen, rufen Sie das Timesheet auf oder lassen Sie den Genehmiger das Timesheet zurückweisen. Weitere Informationen finden Sie unter <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Zeitblatt zur Genehmigung einreichen</a> und <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Timesheet genehmigen</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td>Sie können das Feld Überstunden auf dem Timesheet ausblenden. Diese Option ist standardmäßig deaktiviert.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klicken **Erstellen eines Zeitplans**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Wann Aufgaben und Probleme in den Timesheets der Benutzer angezeigt werden

Eine einem Benutzer zugewiesene Aufgabe bzw. ein Problem wird automatisch auf dem Timesheet eines Benutzers angezeigt, wenn die Aufgabe oder das Problem eines der folgenden Kriterien erfüllt:

* Der Benutzer hat Stunden für die Aufgabe oder das Problem protokolliert
* Die geplanten Termine der Aufgabe oder Ausgabe entsprechen den Daten des Zeitplans
* Die Aufgabe bzw. das Problem hat das tatsächliche Startdatum (die Aufgabe bzw. der Problemstatus wird ausgeführt)
* Die Aufgabe bzw. das Problem wird auf das Zeitblatt übertragen
* Das geplante Abschlussdatum fällt in den Datumsbereich des Zeitblatts und der Status läuft

Wenn die Variable **Vorfüllen von Timesheets mit ...** Voreinstellungen (in den Voreinstellungen für Timesheets und Stunde ) deaktiviert sind, zeigt das Timesheet Probleme und Aufgaben mit dem Status In Bearbeitung an. Weitere Informationen zu den Voreinstellungen für Timesheets und Stunden finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
