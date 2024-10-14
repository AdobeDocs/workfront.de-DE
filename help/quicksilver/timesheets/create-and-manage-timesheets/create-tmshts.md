---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Einmaliges Erstellen eines Datenblatts
description: Sie können ein einmalig zu verwendendes Timesheet manuell erstellen, wenn Sie ein nicht wiederkehrendes Timesheet wünschen. Wenn das Enddatum des Timesheets erreicht ist und Sie mehr Timesheets benötigen, müssen Sie neue erstellen.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 0%

---

# Erstellen eines Datenblatts für die einmalige Verwendung

Sie können ein einmalig zu verwendendes Timesheet manuell erstellen, wenn Sie ein nicht wiederkehrendes Timesheet wünschen. Wenn das Enddatum des Timesheets erreicht ist und Sie mehr Timesheets benötigen, müssen Sie neue erstellen.

Weitere Informationen zum Erstellen eines Timesheet-Profils, das wiederkehrende Timesheets für Ihre Benutzer generiert, ohne dass Sie weitere Eingriffe von Ihnen erhalten (empfohlen), finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Timesheets für die einmalige Verwendung können nicht für Gruppen erstellt werden.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Bei der Erstellung eines Zeitblatts mit nur einer Verwendung können Sie keine bestimmten allgemeinen Stundentypen auswählen, die in Ihr Zeitblatt aufgenommen werden sollen. Alle allgemeinen Stundentypen, die in Ihrem System aktiviert sind, werden in manuell erstellten Timesheets angezeigt.
>
>  Wenn Sie nur bestimmte allgemeine Stundentypen auswählen möchten, die in Ihren Timesheets angezeigt werden sollen, verwenden Sie ein Timesheet-Profil. Weitere Informationen zu Timesheet-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über Administratorzugriff auf Timesheets verfügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Datenblatts für die einmalige Verwendung

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Timesheets**. Der Filter **Alle** ist standardmäßig ausgewählt. Dadurch werden alle Timesheets angezeigt, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Wählen Sie oben rechts auf der Seite die Option **My Timesheet Approvals** aus, um nur die von Ihnen genehmigten Zeitpläne anzuzeigen

     Oder

     Wählen Sie **Meine Timesheets** aus, um nur Ihre Timesheets anzuzeigen.

     Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) , um einen anderen Filter anzuwenden, oder erstellen Sie einen neuen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   > 
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optional) Klicken Sie auf das Symbol **Suchen** ![](assets/search-icon.png), um einen Suchbegriff einzugeben und nach einem bestimmten Zeitblatt zu suchen. Sie können beispielsweise nach einem Zeitrahmen für das Zeitblatt des Eigentümernamens suchen.

1. (Optional) Klicken Sie auf die Symbole **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) , um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klicken Sie oben in der Liste der Timesheets auf **Neues Timesheet** .

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Erstellen Sie ein Timesheet für </strong> </td> 
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
      <td role="rowheader"><strong>Genehmiger</strong> </td> 
      <td>Genehmiger sind Benutzer, die das Timesheet für die mit dem Timesheet verknüpften Benutzer validieren. Als Genehmiger können nur Benutzer mit Zeitblatt-Administratorrechten festgelegt werden. Weitere Informationen zu den Verwaltungsrechten für Zeitblätter finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.<br>Geben Sie die Namen der Timesheet-Genehmiger ein und klicken Sie auf diese, wenn sie in der Liste angezeigt werden.<br>Sie können mehrere Genehmiger auf einem Zeitblatt haben. In diesem Fall wird das Timesheet nach Genehmigung durch einen der Genehmiger als <strong>Geschlossen</strong> markiert und aus der Liste der Zeitblatt-Genehmigungen aller verbleibenden Genehmiger entfernt.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Kann die Zeit bearbeiten</strong> </td>

   <td> <p>Wählen Sie diese Option aus, wenn Sie zulassen möchten, dass Genehmiger Stunden auf dem Timesheet bearbeiten können.</p>

   Diese Option funktioniert zusammen mit der Einstellung **Eingrenzen Sie die Bearbeitung des Zeitblatts auf Inhaber und Administratoren** im Bereich Setup > Zeitblatt &amp; Stunden > Voreinstellungen . Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Konfigurieren der Voreinstellungen für das Zeitblatt und die Stunde</a>.

   Die folgenden Szenarien existieren:

   <ul>
      <li>Wenn die Option <b>Zeitleistenbearbeitung auf Inhaber und Administratoren beschränken</b> aktiviert ist:</li>
   <ul><li>Genehmiger können das Zeitblatt nur genehmigen und ablehnen, unabhängig davon, ob die <b>Kann die Bearbeitungszeit</b> aktiviert ist oder nicht. </li>
   <li>Die Manager der Timesheet-Eigentümer können nur die Timesheets ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul>
   <li>Wenn die Option <b>Zeitleistenbearbeitung auf Inhaber und Administratoren beschränken</b> deaktiviert ist:</li>
   <ul><li>Wenn die Option <b>Kann die Zeit bearbeiten</b> aktiviert ist, können Genehmiger das Timesheet senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li>
   <li>Wenn die Option <b>Kann die Zeit bearbeiten</b> deaktiviert ist, können Genehmiger das Timesheet nicht senden, erneut öffnen oder schließen und können die Zeit nicht bearbeiten. Die Validierer können das Timesheet nur genehmigen oder ablehnen. </li>
   <li>Die Manager von Timesheet-Eigentümern können die Timesheets ihrer direkt unterstellten Mitarbeiter senden, abrufen, erneut öffnen und bearbeiten.</li></ul>
   </ul>

   <p><b>NOTIZ</b>

   Sobald Sie ein Zeitblatt zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um ein gesendetes Timesheet in einen bearbeitbaren Zustand zurückzuversetzen, rufen Sie das Timesheet auf oder lassen Sie den Genehmiger das Timesheet zurückweisen. Weitere Informationen finden Sie unter <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Zeitblatt zur Genehmigung einreichen</a> und <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Zeitblatt genehmigen</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td>Sie können das Feld Überstunden auf dem Timesheet ausblenden. Diese Option ist standardmäßig deaktiviert.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klicken Sie auf **Zeitblatt erstellen**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Wann Aufgaben und Probleme in den Timesheets der Benutzer angezeigt werden

Eine einem Benutzer zugewiesene Aufgabe bzw. ein Problem wird automatisch auf dem Timesheet eines Benutzers angezeigt, wenn die Aufgabe oder das Problem eines der folgenden Kriterien erfüllt:

* Der Benutzer hat Stunden für die Aufgabe oder das Problem protokolliert
* Die geplanten Termine der Aufgabe oder Ausgabe entsprechen den Daten des Zeitplans
* Die Aufgabe bzw. das Problem hat das tatsächliche Startdatum (die Aufgabe bzw. der Problemstatus wird ausgeführt).
* Die Aufgabe bzw. das Problem wird auf das Zeitblatt übertragen.
* Das geplante Abschlussdatum fällt in den Datumsbereich des Zeitblatts und der Status läuft

Wenn die Voreinstellungen für das Vorfüllen von Zeitesheets mit ...**(in den Voreinstellungen für Timesheets und Stunde) deaktiviert sind, werden im Timesheet Probleme und Aufgaben mit dem Status &quot;In Bearbeitung&quot;angezeigt.** Weitere Informationen zu den Voreinstellungen für Timesheets und Stunden finden Sie unter [Konfigurieren von Voreinstellungen für Zeitblätter und Stunden](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
