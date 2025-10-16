---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabelle zur Genehmigung einreichen
description: Durch das Einreichen Ihrer Arbeitszeittabelle zur Genehmigung erhält Ihr Vorgesetzter Einblick in Ihre Arbeitszeit. Genehmigende Personen können überprüfen, ob alle aufgezeichneten Zeiten in den richtigen Bereichen zugewiesen wurden und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Arbeitszeittabelle zur Genehmigung einreichen

<!--Audited: 8/2024-->

Durch das Einreichen Ihrer Arbeitszeittabelle zur Genehmigung erhält Ihr Vorgesetzter Einblick in Ihre Arbeitszeit. Genehmigende Personen können überprüfen, ob alle aufgezeichneten Zeiten in den richtigen Bereichen zugewiesen wurden und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Licht oder höher </p>
   <p>Überprüfen oder höher </p>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme anzeigen oder erhöhen </p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Hochladen von Berechtigungen für die Arbeitszeittabelle</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabelle zur Genehmigung einreichen

* [Arbeitszeittabelle zur Genehmigung einreichen](#submit-a-timesheet-for-approval)
* [Anzeigen des Status einer übermittelten Arbeitszeittabelle](#view-the-status-of-a-submitted-timesheet)

### Arbeitszeittabelle zur Genehmigung einreichen

Nachdem eine genehmigende Person für Arbeitszeittabellen festgelegt wurde (wie im Abschnitt [Bestimmen von ](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver)) im Artikel [Genehmigen einer Arbeitszeittabelle](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md) beschrieben), ändert sich die Schaltfläche **Schließen** am unteren Rand der Arbeitszeittabelle in eine Schaltfläche **Zur Genehmigung einreichen**.

So senden Sie eine Arbeitszeittabelle zur Genehmigung:

1. Wechseln Sie zu einer Arbeitszeittabelle, die für eine genehmigende Person konfiguriert wurde.
1. Zeit erfassen, wie in [Zeit erfassen](../../timesheets/create-and-manage-timesheets/log-time.md) beschrieben
1. Klicken Sie **Zur Genehmigung einreichen**, um den Genehmigungsprozess für Arbeitszeittabellen zu starten.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Die Schaltfläche **Zur Genehmigung einreichen** wird durch die Schaltflächen **Genehmigen**, **Ablehnen** und **Rückruf** ersetzt. Der Status der Arbeitszeittabelle ändert sich in **Gesendet**.

   Wenn Ihre Arbeitszeittabelle zur Genehmigung eingereicht wird, sieht die genehmigende Person die Arbeitszeittabelle, die im Widget **Meine Genehmigungen** im Bereich **Startseite** aufgeführt ist. Folgendes kann passieren:

   * Wenn er/sie die Genehmigung erteilt **ändert sich die Schaltfläche** Rückruf **in „Erneut öffnen** und der Arbeitszeittabellen-Status ändert sich in &quot;**Öffnen**.
   * Wenn er/sie ihn ablehnt, ersetzt **Schaltfläche „Zur Genehmigung**&quot; die Schaltfläche **Rückruf** und der Arbeitszeittabellen-Status wird auf **Abgelehnt** aktualisiert.

1. (Optional) Klicken Sie **Rückruf**, wenn Sie die Arbeitszeittabelle erneut öffnen und Ihre Zeit aktualisieren müssen. Weitere Informationen finden Sie [ Abschnitt „Arbeitszeittabelle ](#recall-a-timesheet)&quot; in diesem Artikel.

### Anzeigen des Status einer übermittelten Arbeitszeittabelle {#view-the-status-of-a-submitted-timesheet}

Sie können den Status einer Arbeitszeittabelle anzeigen, nachdem Sie sie übermittelt haben.

Wenn der Workfront-Administrator die Arbeitszeittabellen-Genehmigung für den Benutzer und die Arbeitszeittabellen-Ablehnung für Benutzer-Ereignishandler aktiviert hat, werden Sie benachrichtigt, nachdem die Arbeitszeittabelle genehmigt oder abgelehnt wurde. Informationen zur Aktivierung von Ereignisbenachrichtigungen finden Sie [Ereignistypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Ohne diese Benachrichtigungen können Sie sich im Arbeitszeittabellen-Bereich von Workfront über den Status Ihrer gesendeten Arbeitszeittabellen informieren.

So zeigen Sie den Status einer Arbeitszeittabelle an:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken Sie **Arbeitszeittabellen**. Der **Alle**-Filter ist standardmäßig ausgewählt.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Arbeitszeittabellen zu aktualisieren:

   * Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** in der rechten oberen Ecke der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen

     Oder

     Wählen Sie **Meine Arbeitszeittabellen** aus, um nur Ihre Arbeitszeittabellen anzuzeigen.

     Dadurch werden die Filter Meine Arbeitszeittabellen-Genehmigungen oder Meine Arbeitszeittabellen auf die Liste der Arbeitszeittabellen angewendet.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) , um einen anderen Filter anzuwenden, oder erstellen Sie einen neuen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Arbeitszeittabellen-Genehmigungen und Meine Arbeitszeittabellen werden nicht oben in der Arbeitszeittabellen-Liste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins die Filter Meine Arbeitszeittabellen und Meine Arbeitszeittabellen entweder aus den Listensteuerelementen im Setup-Bereich oder aus Ihrer Layoutvorlage entfernt haben. Weitere Informationen finden Sie in den folgenden Artikeln:
   >
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Bedingt) Wenn Sie **Meine Arbeitszeittabellen** ausgewählt haben, stellen Sie sicher, dass die Ansicht **Standard** angewendet wird, und beachten Sie die Spalte **Status**.

   Arbeitszeittabellen können die folgenden Status aufweisen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öffnen</td> 
      <td> <p>Ihre Arbeitszeittabelle ist derzeit geöffnet und Sie können die Zeit protokollieren. </p> <p>Eine zurückgerufene Arbeitszeittabelle wird mit dem Status Offen angezeigt. Weitere Informationen finden Sie <a href="#recall-a-timesheet" class="MCXref xref"> Abschnitt „Arbeitszeittabelle </a>" in diesem Artikel. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gesendet</td> 
      <td>Sie haben Ihre Arbeitszeittabelle zur Genehmigung eingereicht, sie wurde jedoch noch nicht genehmigt. Sie können eine gesendete Arbeitszeittabelle abrufen, um sie weiter zu bearbeiten. Weitere Informationen finden Sie <a href="#recall-a-timesheet" class="MCXref xref"> Abschnitt „Arbeitszeittabelle </a>" in diesem Artikel. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geschlossen</td> 
      <td> <p>Die folgenden Szenarien sind vorhanden:</p> 
       <ul> 
        <li> <p>Wenn die Arbeitszeittabelle keine genehmigende Person enthält, haben Sie Ihre Zeit gespeichert und geschlossen.</p> </li> 
        <li> <p>Wenn die Arbeitszeittabelle eine genehmigende Person enthält, haben Sie diese zur Genehmigung eingereicht und sie wurde genehmigt.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgelehnt</td> 
      <td>Sie haben die Arbeitszeittabelle zur Genehmigung eingereicht und die genehmigende Person hat sie abgelehnt.</td> 
     </tr> 
    </tbody> 
   </table>

## Arbeitszeittabelle zurückrufen {#recall-a-timesheet}

Sie können eine Arbeitszeittabelle zurückrufen, die bereits zur Genehmigung eingereicht wurde. Nur Arbeitszeittabellen, die noch nicht genehmigt wurden, können zurückgerufen werden.

So rufen Sie eine Arbeitszeittabelle ab:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie **Arbeitszeittabellen**.
1. Klicken Sie **Meine Arbeitszeittabellen** in der oberen rechten Ecke des Bildschirms oder wählen Sie **Meine Arbeitszeittabellen** aus dem Dropdown-Menü **Filtern** ![](assets/filter-nwepng.png).
1. Klicken Sie auf den Zeitrahmen für eine Arbeitszeittabelle mit dem Status **Gesendet**.
1. Klicken Sie auf **Rückruf**.

   Die Arbeitszeittabelle kann erneut bearbeitet werden, und ihr Status ändert sich in **Offen**.
