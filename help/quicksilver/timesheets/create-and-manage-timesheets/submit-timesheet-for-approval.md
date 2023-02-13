---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Zeitblatt zur Genehmigung einreichen
description: Durch die Übermittlung Ihres Zeitblatts zur Genehmigung erhalten Sie von Ihrem Manager einen Einblick in Ihre Arbeitszeit. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Zeitblatt zur Genehmigung einreichen

Durch die Übermittlung Ihres Zeitblatts zur Genehmigung erhalten Sie von Ihrem Manager einen Einblick in Ihre Arbeitszeit. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff oder höher auf Aufgaben und Probleme anzeigen</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für Aufgaben und Probleme</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zeitblatt zur Genehmigung einreichen

* [Zeitblatt zur Genehmigung einreichen](#submit-a-timesheet-for-approval)
* [Status eines gesendeten Zeitblatts anzeigen](#view-the-status-of-a-submitted-timesheet)

### Zeitblatt zur Genehmigung einreichen

Nachdem ein Timesheet-Genehmiger festgelegt wurde (wie im Abschnitt beschrieben) [Zeitblatt-Genehmiger bestimmen](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) im Artikel [Timesheet genehmigen](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), die **Schließen** -Schaltfläche am unteren Rand des Zeitplans ändert sich in eine **Zur Genehmigung einreichen** Schaltfläche.

So senden Sie ein Datenblatt zur Genehmigung:

1. Gehen Sie zu einem Timesheet, das für einen Genehmiger konfiguriert wurde.
1. Protokollzeit, wie unter [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Klicken **Zur Genehmigung einreichen** , um den Prozess der Billigung des Zeitplans zu starten.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Die **Zur Genehmigung einreichen** -Schaltfläche ersetzt durch **Genehmigen**, **Ablehnen** und **Rückruf** Schaltflächen. Der Status des Zeitblatts ändert sich in **Gesendet**.

   Wenn Ihr Timesheet zur Genehmigung eingereicht wird, sieht der Genehmiger das im **Genehmigungen** Bereich auf **Startseite** Seite. Folgendes kann vorkommen:

   * Wenn sie sie genehmigen, wird die **Rückruf** Schaltflächenänderungen in **Erneutes Öffnen** und der Zeitdatenblatt-Status aktualisiert sich in **Öffnen**.
   * Wenn sie ihn ablehnen, wird die **Zur Genehmigung einreichen** -Schaltfläche ersetzt die **Rückruf** Schaltfläche und Status des Zeitplans aktualisiert sich in **Zurückgewiesen**.

1. (Optional) Klicken Sie auf **Rückruf** wenn Sie das Timesheet erneut öffnen und Ihre Zeit aktualisieren müssen. Weitere Informationen finden Sie unter [Zeitblatt zurückrufen](#recall-a-timesheet) in diesem Artikel.

### Status eines gesendeten Zeitblatts anzeigen {#view-the-status-of-a-submitted-timesheet}

Sie können den Status eines Timesheets nach dem Senden anzeigen.

Wenn der Workfront-Administrator die Genehmigung für das Datenblatt für den Benutzer und die Zurückweisung des Datenblatts an Benutzer-Ereignishandler aktiviert hat, werden Sie benachrichtigt, nachdem das Datenblatt genehmigt oder abgelehnt wurde. Informationen zum Aktivieren von Ereignisbenachrichtigungen finden Sie unter [In Adobe Workfront verfügbare Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Ohne diese Benachrichtigungen können Sie über den Status Ihrer gesendeten Timesheets im Timesheet-Bereich von Workfront informiert werden.

So zeigen Sie den Status eines Zeitblatts an:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken **Timesheets**. Die **Alle** -Filter ist standardmäßig ausgewählt.

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
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Bedingt) Wenn Sie ausgewählt haben **Meine Timesheets** stellen sicher, dass **Standard** -Ansicht angewendet wird und beachten Sie, dass **Status** Spalte.

   Timesheets können die folgenden Status aufweisen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öffnen</td> 
      <td> <p>Ihr Timesheet ist derzeit geöffnet und Sie können die Zeit protokollieren. </p> <p>Ein zurückgerufenes Timesheet wird mit dem Status "Open"angezeigt. Weitere Informationen finden Sie unter <a href="#recall-a-timesheet" class="MCXref xref">Zeitblatt zurückrufen</a> in diesem Artikel. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gesendet</td> 
      <td>Sie haben Ihr Datenblatt zur Genehmigung eingereicht, aber es wurde noch nicht genehmigt. Sie können sich an ein gesendetes Zeitblatt erinnern, um es weiter zu bearbeiten. Weitere Informationen finden Sie unter <a href="#recall-a-timesheet" class="MCXref xref">Zeitblatt zurückrufen</a> in diesem Artikel. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geschlossen</td> 
      <td> <p>Die folgenden Szenarien existieren:</p> 
       <ul> 
        <li> <p>Wenn das Timesheet keinen Genehmiger hat, haben Sie Ihre Zeit gespart und geschlossen.</p> </li> 
        <li> <p>Wenn das Timesheet über einen Genehmiger verfügt, haben Sie es zur Genehmigung eingereicht und es wurde genehmigt.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgelehnt</td> 
      <td>Sie haben das Timesheet zur Genehmigung eingereicht und der Genehmiger hat es abgelehnt.</td> 
     </tr> 
    </tbody> 
   </table>

## Zeitblatt zurückrufen {#recall-a-timesheet}

Sie können sich an ein bereits zur Validierung eingestelltes Timesheet erinnern. Es können nur Timesheets zurückgerufen werden, die noch nicht genehmigt wurden.

So rufen Sie ein Zeitblatt auf:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Timesheets**.
1. Klicken **Meine Timesheets** in der oberen rechten Ecke des Bildschirms klicken oder **Meine Timesheets** von **Filter** ![](assets/filter-nwepng.png) Dropdown-Menü.
1. Klicken Sie auf den Zeitrahmen für ein Zeitblatt mit dem Status **Gesendet**.
1. Klicken **Rückruf**.

   Das Timesheet wird erneut bearbeitbar und erhält den Status **Öffnen**.
