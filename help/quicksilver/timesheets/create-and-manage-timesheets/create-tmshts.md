---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch
description: Wenn Sie eine nicht wiederkehrende Arbeitszeittabelle benötigen, können Sie diese Arbeitszeittabelle manuell erstellen. Wenn das Enddatum der Arbeitszeittabelle erreicht ist und Sie mehr Arbeitszeittabellen benötigen, müssen Sie neue erstellen.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 7%
---
# Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch

<!--Audited: 6/2025-->

Wenn Sie eine nicht wiederkehrende Arbeitszeittabelle benötigen, können Sie diese Arbeitszeittabelle manuell erstellen. Wenn das Enddatum der Arbeitszeittabelle erreicht ist und Sie mehr Arbeitszeittabellen benötigen, müssen Sie neue erstellen.

Informationen zum Erstellen eines Arbeitszeittabellen-Profils, das ohne weiteres Eingreifen Ihrerseits wiederkehrende Arbeitszeittabellen für Ihre Benutzer generiert (empfohlen), finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Informationen zum manuellen Generieren von Arbeitszeittabellen für alle Benutzenden im System, die einem Arbeitszeittabellenprofil zugeordnet sind, finden Sie unter [Manuelles Generieren von Arbeitszeittabellen](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* Einmalige Arbeitszeittabellen können nicht für Gruppen erstellt werden.
>* Beim Erstellen einer Einmalzeittabelle können Sie keine bestimmten allgemeinen Stundentypen auswählen, die in Ihre Arbeitszeittabelle aufgenommen werden sollen. Alle allgemeinen Stundentypen, die in Ihrem System aktiviert sind, werden in manuell erstellten Arbeitszeittabellen angezeigt.
>
>Wenn Sie nur bestimmte allgemeine Stundentypen für die Anzeige in Ihren Arbeitszeittabellen auswählen möchten, verwenden Sie ein Arbeitszeittabellen-Profil. Weitere Informationen zu Arbeitszeittabellen-Profilen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Administrativer Zugriff auf Arbeitszeittabellen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Erstellen einer Arbeitszeittabelle für den einmaligen Gebrauch

{{step1-to-timesheets}}

Alle Arbeitszeittabellen, auf die Sie Zugriff haben, werden standardmäßig angezeigt.

![Arbeitszeittabellen-Liste](assets/list-of-all-timesheets.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Arbeitszeittabellen zu aktualisieren:

   * Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** in der rechten oberen Ecke der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen.

     ODER

     Wählen Sie **Meine Arbeitszeittabellen** aus, um nur Ihre Arbeitszeittabellen anzuzeigen.

     Dadurch werden die Filter **Meine Arbeitszeittabellen-Genehmigungen** oder **Meine Arbeitszeittabelle** auf die Liste der Arbeitszeittabellen angewendet.

   * Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png), um einen Filter anzuwenden oder einen neuen Filter zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Arbeitszeittabellen-Genehmigungen und Meine Arbeitszeittabellen werden nicht oben in der Arbeitszeittabellen-Liste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins die Filter Meine Arbeitszeittabellen und Meine Arbeitszeittabellen entweder aus den Listensteuerelementen im Setup-Bereich oder aus Ihrer Layoutvorlage entfernt haben. Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Optional) Klicken Sie auf das Symbol **Suchen** ![Suchsymbol](assets/search-icon.png), um einen Suchbegriff einzugeben und nach einer bestimmten Arbeitszeittabelle zu suchen. Sie können beispielsweise nach einem Arbeitszeittabellen-Zeitrahmen mit Besitzernamen suchen.

1. (Optional) Klicken Sie auf **Ansicht** ![Ansichtssymbol](assets/view-icon.png) oder **Gruppierung** ![Gruppierungssymbol](assets/grouping.png), um eine Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Klicken Sie **oben** der Liste der Arbeitszeittabellen auf „Neue Arbeitszeittabelle“.

   Folgende Angaben sind erforderlich:

   | Feldname | Beschreibung |
   | --------- | ---------- |
   | Arbeitszeittabelle erstellen für | Beginnen Sie mit der Eingabe des Namens des Benutzers, eines Aufgabengebiets oder eines Teams, für das Sie die Arbeitszeittabelle erstellen, und klicken Sie darauf, wenn sie in der Liste angezeigt werden. |
   | Startdatum | Dies ist das Startdatum der Arbeitszeittabelle. |
   | Enddatum | Dies ist das Enddatum der Arbeitszeittabelle. |
   | Genehmigende Personen | <p>Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verbundenen Benutzer genehmigen. Nur Benutzer mit Verwaltungsrechten für Arbeitszeittabellen können als genehmigende Personen festgelegt werden. Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Geben Sie die Namen der genehmigenden Personen für Arbeitszeittabellen ein und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.</p> <p>Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als &quot;**&quot;** und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.</p> |
   | Kann Zeit bearbeiten | <p>Wählen Sie diese Option aus, wenn Sie genehmigenden Personen erlauben möchten, Stunden auf der Arbeitszeittabelle zu bearbeiten.</p><p>Diese Option funktioniert zusammen mit der Einstellung **Bearbeitung von Arbeitszeittabellen auf Inhaber und Administratoren beschränken** im Bereich Setup > Arbeitszeittabellen und Stunden > Voreinstellungen. Weitere Informationen finden Sie unter [Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).</p><p>Die folgenden Szenarien sind vorhanden:</p><p>Wenn die **Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken** aktiviert ist:</p><ul><li>Genehmigende Personen können Arbeitszeittabellen nur genehmigen und ablehnen, unabhängig davon, ob **Kann Zeit bearbeiten** aktiviert ist oder nicht.</li><li>Die Manager der Arbeitszeittabellen-Besitzer können nur die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul><p>Wenn die **Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken** deaktiviert ist:</p><ul><li>Wenn **Kann die Zeit bearbeiten** aktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li><li>Wenn **Kann die Zeit bearbeiten** deaktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle nicht senden, erneut öffnen oder schließen und auch die Zeit nicht bearbeiten. Genehmigende Personen können die Arbeitszeittabelle nur genehmigen oder ablehnen.</li><li>Die Manager von Arbeitszeittabellen-Besitzern können die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter senden, zurückrufen, erneut öffnen und bearbeiten.</li></ul><p>**HINWEIS**</br> Nachdem Sie eine Arbeitszeittabelle zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um eine übermittelte Arbeitszeittabelle in den bearbeitbaren Status zurückzuversetzen, rufen Sie die Arbeitszeittabelle zurück oder bitten Sie die genehmigende Person, die Arbeitszeittabelle abzulehnen. Weitere Informationen finden Sie unter [Arbeitszeittabelle zur Genehmigung einreichen](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) und [Arbeitszeittabelle genehmigen](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md). |
   | Überstunden | Sie können das Feld **Überstunden** auf der Arbeitszeittabelle ausblenden. Standardmäßig ist diese Option deaktiviert. |

1. Klicken Sie **Arbeitszeittabelle erstellen**.

## Wenn Aufgaben und Probleme in den Arbeitszeittabellen der Benutzer angezeigt werden

Eine Aufgabe oder ein Problem, die bzw. das einem/r Benutzenden zugewiesen wurde, wird automatisch in der Arbeitszeittabelle eines/r Benutzenden angezeigt, wenn die Aufgabe oder das Problem eines der folgenden Kriterien erfüllt:

* Der Benutzer hat Stunden für die Aufgabe oder das Problem protokolliert
* Die geplanten Termine der Aufgabe oder des Problems liegen innerhalb der Termine der Arbeitszeittabelle
* Die Aufgabe oder das Problem hat ein tatsächliches Startdatum (die Aufgabe oder der Problemstatus ist in Bearbeitung)
* Die Aufgabe oder das Problem wird an die Arbeitszeittabelle angeheftet
* Das geplante Abschlussdatum liegt innerhalb des Datumsbereichs der Arbeitszeittabelle und der Status ist In Bearbeitung

Wenn die **Voreinstellungen Arbeitszeittabellen mit vorab befüllen…** (in den Arbeitszeittabellen- und Stundeneinstellungen) deaktiviert sind, zeigt die Arbeitszeittabelle Probleme und Aufgaben mit dem Status In Bearbeitung an. Weitere Informationen zu Arbeitszeittabellen und Stundenvoreinstellungen finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
