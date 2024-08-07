---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Timesheet genehmigen
description: Der Prozess der Genehmigung von Timesheets bietet Managern einen Einblick in die Arbeitszeiten ihrer direkten Berichte. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob für den betreffenden Zeitraum eine ausreichende Anzahl von Stunden aufgezeichnet wurde.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Timesheet genehmigen

<!--Audited: 8/2024-->

Der Prozess der Genehmigung von Timesheets bietet Managern einen Einblick in die Arbeitszeiten ihrer direkten Berichte. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob für den betreffenden Zeitraum eine ausreichende Anzahl von Stunden aufgezeichnet wurde.

Adobe Workfront bietet die Möglichkeit, die Validierungen von Zeitblättern zu konfigurieren, um sie in diesem Bereich zu unterstützen.

Informationen zum Übermitteln eines Zeitblatts finden Sie unter [Zeitblatt zur Genehmigung einreichen](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Neu: Standard</p>
   <p>Aktuell: Plan </p> 
   <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf Timesheets und Stunden </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zeitblatt-Genehmiger bestimmen

In der Regel werden Timesheets von funktionalen Managern oder Personal genehmigt. Timesheets werden in der Regel nicht von Projektmanagern genehmigt. Projektmanager können die in Projekten protokollierte Zeit genehmigen, Teams oder Personalverantwortliche sollten jedoch Zeitpläne genehmigen.

Bei der Erstellung des Datenblatt-Profils wird ein Timesheet-Genehmiger definiert. Sie müssen über eine Planungslizenz verfügen, um als Genehmiger benannt zu werden.

Weitere Informationen zum Benennen von Timesheet-Genehmigern finden Sie im Abschnitt &quot;[Erstellen oder Bearbeiten eines Timesheet-Profils](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)&quot;im Artikel &quot;[Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)&quot;.

## Timesheet genehmigen

Sie können alle Timesheets genehmigen, die übermittelt wurden und in denen Sie als Genehmiger benannt wurden. Wenn ein Timesheet zur Genehmigung eingereicht wird, wird das Timesheet im Bereich **Genehmigungen** auf Ihrer Seite **Startseite** aufgelistet. Weitere Informationen finden Sie unter [Arbeiten genehmigen](../../review-and-approve-work/manage-approvals/approving-work.md).

Wenn der Workfront-Administrator die Genehmigung für das Datenblatt für den Benutzer und die Zurückweisung des Datenblatts an Benutzer-Ereignishandler aktiviert hat, werden Sie benachrichtigt, nachdem das Datenblatt genehmigt oder abgelehnt wurde. Weitere Informationen zum Aktivieren von Ereignisbenachrichtigungen finden Sie unter [Ereignislaufbenachrichtigungstypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

So validieren Sie ein Zeitblatt:

{{step1-to-timesheets}}

Der Bereich **Timesheets** wird geöffnet.

1. Wählen Sie oben rechts auf der Seite die Option &quot;**My Timesheet Approvals**&quot;, um nur die von Ihnen genehmigten Timesheets anzuzeigen.

   Oder

   Wählen Sie den Filter **Meine Timesheet-Genehmigungen** oben in der Timesheet-Liste aus.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Die Option &quot;Meine Timesheet-Genehmigungen&quot;wird nicht oben in der Liste der Zeitblätter oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator den Filter Meine Zeitblatt-Genehmigungen entweder aus dem Bereich &quot;Listen-Steuerelemente&quot;im Bereich &quot;Einstellungen&quot;oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   >
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Optional) Klicken Sie oben in der Timesheet-Liste auf das Symbol **Suchen** ![](assets/search-icon.png) und geben Sie einen Suchbegriff ein, um nach einem bestimmten Timesheet zu suchen. Sie können nach einem Zeitrahmen, nach dem Namen eines Eigentümers oder Genehmigers suchen.
1. Klicken Sie auf den Zeitrahmen des zu validierenden Zeitplans. Das Timesheet wird geöffnet.

   >[!TIP]
   >
   >Timesheets, die auf die Genehmigung warten, haben den Status &quot;[!UICONTROL Gesendet]&quot;.


1. Klicken Sie auf **Genehmigen** .

   Oder

   Wenn Sie das Timesheet ablehnen möchten, klicken Sie in der linken unteren Ecke des Zeitblatts auf **Ablehnen** .

   Falls genehmigt, ändert sich der Status des Zeitblatts in **Geschlossen**.

   Wenn die Änderung abgelehnt wird, ändert sich der Status des Zeitblatts in **Abgelehnt**.
