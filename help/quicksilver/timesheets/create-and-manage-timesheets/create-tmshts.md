---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch
description: Wenn Sie eine nicht wiederkehrende Arbeitszeittabelle benötigen, können Sie diese Arbeitszeittabelle manuell erstellen. Wenn das Enddatum der Arbeitszeittabelle erreicht ist und Sie mehr Arbeitszeittabellen benötigen, müssen Sie neue erstellen.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 1%

---

# Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch

<!--Audited: 6/2025-->

Wenn Sie eine nicht wiederkehrende Arbeitszeittabelle benötigen, können Sie diese Arbeitszeittabelle manuell erstellen. Wenn das Enddatum der Arbeitszeittabelle erreicht ist und Sie mehr Arbeitszeittabellen benötigen, müssen Sie neue erstellen.

Informationen zum Erstellen eines Arbeitszeittabellen-Profils, das ohne weiteres Eingreifen Ihrerseits wiederkehrende Arbeitszeittabellen für Ihre Benutzer generiert (empfohlen), finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Informationen zum manuellen Generieren von Arbeitszeittabellen für alle Benutzenden im System, die einem Arbeitszeittabellenprofil zugeordnet sind, finden Sie unter [Manuelles Generieren von Arbeitszeittabellen](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Einmalige Arbeitszeittabellen können nicht für Gruppen erstellt werden.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Beim Erstellen einer Einmalzeittabelle können Sie keine bestimmten allgemeinen Stundentypen auswählen, die in Ihre Arbeitszeittabelle aufgenommen werden sollen. Alle allgemeinen Stundentypen, die in Ihrem System aktiviert sind, werden in manuell erstellten Arbeitszeittabellen angezeigt.
>
>  Wenn Sie nur bestimmte allgemeine Stundentypen für die Anzeige in Ihren Arbeitszeittabellen auswählen möchten, verwenden Sie ein Arbeitszeittabellen-Profil. Weitere Informationen zu Arbeitszeittabellen-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Administrativer Zugriff auf Arbeitszeittabellen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch

{{step1-to-timesheets}}

Der **Alle**-Filter ist standardmäßig ausgewählt. Dadurch werden alle Arbeitszeittabellen angezeigt, auf die Sie Zugriff haben.

![Arbeitszeittabellen-Liste mit einer ausgewählten Arbeitszeittabelle](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Arbeitszeittabellen zu aktualisieren:

   * Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** in der rechten oberen Ecke der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen

     Oder

     Wählen Sie **Meine Arbeitszeittabellen** aus, um nur Ihre Arbeitszeittabellen anzuzeigen.

     Dadurch werden die Filter Meine Arbeitszeittabellen-Genehmigungen oder Meine Arbeitszeittabellen auf die Liste der Arbeitszeittabellen angewendet.

     ![Meine Arbeitszeittabellen-Filterschaltflächen auf der Seite mit der Arbeitszeittabellen-Liste](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png), um einen anderen Filter anzuwenden oder einen neuen zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Arbeitszeittabellen-Genehmigungen und Meine Arbeitszeittabellen werden nicht oben in der Arbeitszeittabellen-Liste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins die Filter Meine Arbeitszeittabellen und Meine Arbeitszeittabellen entweder aus den Listensteuerelementen im Setup-Bereich oder aus Ihrer Layoutvorlage entfernt haben. Weitere Informationen finden Sie in den folgenden Artikeln:
   > 
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optional) Klicken Sie auf das Symbol **Suchen** ![Suchsymbol](assets/search-icon.png), um einen Suchbegriff einzugeben und nach einer bestimmten Arbeitszeittabelle zu suchen. Sie können beispielsweise nach einem Arbeitszeittabellen-Zeitrahmen mit Besitzernamen suchen.

1. (Optional) Klicken Sie auf **Ansicht** ![Ansichtssymbol](assets/view-icon.png) oder **Gruppierung** ![Gruppierungssymbol](assets/grouping.png), um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klicken Sie **oben** der Liste der Arbeitszeittabellen auf „Neue Arbeitszeittabelle“.

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Arbeitszeittabelle erstellen für</strong> </td> 
      <td>Beginnen Sie mit der Eingabe des Namens des Benutzers, eines Aufgabengebiets oder eines Teams, für das Sie die Arbeitszeittabelle erstellen, und klicken Sie darauf, wenn sie in der Liste angezeigt werden.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Startdatum</strong> </td> 
      <td>Dies ist das Startdatum der Arbeitszeittabelle.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Enddatum</strong> </td> 
      <td> Dies ist das Enddatum der Arbeitszeittabelle.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Genehmigende Personen</strong> </td> 
      <td>Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verbundenen Benutzer genehmigen. Nur Benutzer mit Verwaltungsrechten für Arbeitszeittabellen können als genehmigende Personen festgelegt werden. Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.<br>Beginnen Sie mit der Eingabe der Namen der genehmigenden Personen für Arbeitszeittabellen und klicken Sie auf diese, wenn sie in der Liste angezeigt werden.<br>Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als "<strong>" </strong> und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Kann die Zeit bearbeiten</strong> </td>

   <td> <p>Wählen Sie diese Option aus, wenn Sie genehmigenden Personen erlauben möchten, Stunden auf der Arbeitszeittabelle zu bearbeiten.</p>

   Diese Option funktioniert zusammen mit der Einstellung **Bearbeitung von Arbeitszeittabellen auf Inhaber und Administratoren beschränken** im Bereich Setup > Arbeitszeittabellen und Stunden > Voreinstellungen. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren</a>.

   Die folgenden Szenarien sind vorhanden:

   <ul>
      <li>Wenn die <b>Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken</b> aktiviert ist:</li>
   <ul><li>Genehmigende Personen können Arbeitszeittabellen nur genehmigen und ablehnen, unabhängig davon, ob <b>Kann Zeit bearbeiten</b> aktiviert ist oder nicht. </li>
   <li>Die Manager der Arbeitszeittabellen-Besitzer können nur die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul>
   <li>Wenn die <b>Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken</b> deaktiviert ist:</li>
   <ul><li>Wenn die <b>Kann die Zeit bearbeiten</b> aktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li>
   <li>Wenn die <b>Kann die Zeit bearbeiten</b> deaktiviert ist, können genehmigende Personen die Arbeitszeittabelle nicht senden, erneut öffnen oder schließen und können die Zeit auch nicht bearbeiten. Genehmigende Personen können die Arbeitszeittabelle nur genehmigen oder ablehnen. </li>
   <li>Die Manager von Arbeitszeittabellen-Besitzern können die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter senden, zurückrufen, erneut öffnen und bearbeiten.</li></ul>
   </ul>

   <p><b>NOTIZ</b>

   Nachdem Sie eine Arbeitszeittabelle zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um eine übermittelte Arbeitszeittabelle in den bearbeitbaren Status zurückzuversetzen, rufen Sie die Arbeitszeittabelle zurück oder bitten Sie die genehmigende Person, die Arbeitszeittabelle abzulehnen. Weitere Informationen finden Sie unter <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Arbeitszeittabelle zur Genehmigung einreichen</a> und <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Arbeitszeittabelle genehmigen</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td>Sie können das Feld „Überstunden“ auf der Arbeitszeittabelle ausblenden. Standardmäßig ist diese Option deaktiviert.</td> 
      </tr> 
      </tbody> 
   </table>

1. Klicken Sie **Arbeitszeittabelle erstellen**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Wenn Aufgaben und Probleme in den Arbeitszeittabellen der Benutzer angezeigt werden

Eine Aufgabe oder ein Problem, die bzw. das einem/r Benutzenden zugewiesen wurde, wird automatisch in der Arbeitszeittabelle eines/r Benutzenden angezeigt, wenn die Aufgabe oder das Problem eines der folgenden Kriterien erfüllt:

* Der Benutzer hat Stunden für die Aufgabe oder das Problem protokolliert
* Die geplanten Termine der Aufgabe oder des Problems liegen innerhalb der Termine der Arbeitszeittabelle
* Die Aufgabe oder das Problem hat ein tatsächliches Startdatum (die Aufgabe oder der Problemstatus ist in Bearbeitung)
* Die Aufgabe oder das Problem wird an die Arbeitszeittabelle angeheftet
* Das geplante Abschlussdatum liegt innerhalb des Datumsbereichs der Arbeitszeittabelle und der Status ist In Bearbeitung

Wenn die **Voreinstellungen Arbeitszeittabellen mit vorab befüllen…** (in den Arbeitszeittabellen- und Stundeneinstellungen) deaktiviert sind, zeigt die Arbeitszeittabelle Probleme und Aufgaben mit dem Status In Bearbeitung an. Weitere Informationen zu Arbeitszeittabellen und Stundenvoreinstellungen finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
