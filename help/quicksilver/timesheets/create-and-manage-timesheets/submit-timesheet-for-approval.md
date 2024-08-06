---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Zeitblatt zur Genehmigung einreichen
description: Durch die Übermittlung Ihres Zeitblatts zur Genehmigung erhalten Sie von Ihrem Manager einen Einblick in Ihre Arbeitszeit. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Zeitblatt zur Genehmigung einreichen

<!--Audited: 8/2024-->

Durch die Übermittlung Ihres Zeitblatts zur Genehmigung erhalten Sie von Ihrem Manager einen Einblick in Ihre Arbeitszeit. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Licht oder höher </p>
   <p>Aktuell: Überprüfen oder höher </p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme anzeigen oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Timesheet</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zeitblatt zur Genehmigung einreichen

* [Zeitblatt zur Genehmigung einreichen](#submit-a-timesheet-for-approval)
* [Status eines gesendeten Zeitblatts anzeigen](#view-the-status-of-a-submitted-timesheet)

### Zeitblatt zur Genehmigung einreichen

Nachdem ein Timesheet-Genehmiger festgelegt wurde (wie im Abschnitt [Zeitblatt-Genehmiger benennen](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) im Artikel [Zeitblatt genehmigen](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md) beschrieben), ändert sich die Schaltfläche **Schließen** am unteren Rand des Zeitblatts in die Schaltfläche **Zur Genehmigung übermitteln** .

So senden Sie ein Datenblatt zur Genehmigung:

1. Gehen Sie zu einem Timesheet, das für einen Genehmiger konfiguriert wurde.
1. Protokollzeit, wie in [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md) beschrieben.
1. Klicken Sie auf **Zur Genehmigung übermitteln** , um den Prozess zur Genehmigung des Zeitblatts zu starten.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Die Schaltfläche &quot;**Zur Genehmigung übermitteln**&quot; wird durch die Schaltflächen &quot;**Genehmigen**&quot;, &quot;**Ablehnen**&quot;und &quot;**Aufrufen**&quot; ersetzt. Der Status des Zeitblatts ändert sich in **Gesendet**.

   Wenn Ihr Timesheet zur Genehmigung eingereicht wird, wird dem Genehmiger das im Bereich **Genehmigungen** auf der Seite **Startseite** aufgelistete Timesheet angezeigt. Folgendes kann vorkommen:

   * Wenn sie es genehmigen, ändert sich die Schaltfläche **Recall** in **Re-open** und der Zeitdatenblattstatus wird in **Open** aktualisiert.
   * Wenn sie sie ablehnen, ersetzt die Schaltfläche &quot;**Zur Genehmigung übermitteln**&quot;die Schaltfläche &quot;**Rückruf**&quot;, und der Status des Zeitblatts wird auf &quot;**Abgelehnt**&quot;aktualisiert.

1. (Optional) Klicken Sie auf **Erinnern** , wenn Sie das Timesheet erneut öffnen und Ihre Zeit aktualisieren möchten. Weitere Informationen finden Sie im Abschnitt [Zeitblatt erinnern](#recall-a-timesheet) in diesem Artikel.

### Status eines gesendeten Zeitblatts anzeigen {#view-the-status-of-a-submitted-timesheet}

Sie können den Status eines Timesheets nach dem Senden anzeigen.

Wenn der Workfront-Administrator die Genehmigung für das Datenblatt für den Benutzer und die Zurückweisung des Datenblatts an Benutzer-Ereignishandler aktiviert hat, werden Sie benachrichtigt, nachdem das Datenblatt genehmigt oder abgelehnt wurde. Weitere Informationen zum Aktivieren von Ereignisbenachrichtigungen finden Sie unter [Ereignislaufbenachrichtigungstypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Ohne diese Benachrichtigungen können Sie über den Status Ihrer gesendeten Timesheets im Timesheet-Bereich von Workfront informiert werden.

So zeigen Sie den Status eines Zeitblatts an:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).
1. Klicken Sie auf **Timesheets**. Der Filter **Alle** ist standardmäßig ausgewählt.

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
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Bedingt) Wenn Sie **Meine Timesheets** ausgewählt haben, stellen Sie sicher, dass die Ansicht **Standard** angewendet wird, und beachten Sie die Spalte **Status** .

   Timesheets können die folgenden Status aufweisen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öffnen</td> 
      <td> <p>Ihr Timesheet ist derzeit geöffnet und Sie können die Zeit protokollieren. </p> <p>Ein zurückgerufenes Timesheet wird mit dem Status "Open"angezeigt. Weitere Informationen finden Sie im Abschnitt <a href="#recall-a-timesheet" class="MCXref xref">Zeitblatt erinnern</a> in diesem Artikel. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gesendet</td> 
      <td>Sie haben Ihr Datenblatt zur Genehmigung eingereicht, aber es wurde noch nicht genehmigt. Sie können sich an ein gesendetes Zeitblatt erinnern, um es weiter zu bearbeiten. Weitere Informationen finden Sie im Abschnitt <a href="#recall-a-timesheet" class="MCXref xref">Zeitblatt erinnern</a> in diesem Artikel. </td> 
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

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Timesheets**.
1. Klicken Sie oben rechts im Bildschirm auf **Meine Timesheets** oder wählen Sie aus dem Dropdownmenü **Filter** ![](assets/filter-nwepng.png) die Option **Meine Timesheets** aus.
1. Klicken Sie auf den Zeitrahmen für ein Zeitblatt mit dem Status &quot;**Gesendet**&quot;.
1. Klicken Sie auf **Recall**.

   Das Timesheet wird wieder bearbeitbar und erhält den Status **Öffnen**.
