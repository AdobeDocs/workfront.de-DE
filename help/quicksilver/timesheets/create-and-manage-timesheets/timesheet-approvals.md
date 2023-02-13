---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Timesheet genehmigen
description: Der Prozess der Genehmigung von Timesheets bietet Managern einen Einblick in die Arbeitszeiten ihrer direkten Berichte. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob für den betreffenden Zeitraum eine ausreichende Anzahl von Stunden aufgezeichnet wurde.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Timesheet genehmigen

Der Prozess der Genehmigung von Timesheets bietet Managern einen Einblick in die Arbeitszeiten ihrer direkten Berichte. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob für den betreffenden Zeitraum eine ausreichende Anzahl von Stunden aufgezeichnet wurde.

Adobe Workfront bietet die Möglichkeit, die Validierungen von Zeitblättern zu konfigurieren, um sie in diesem Bereich zu unterstützen.

Informationen zum Übermitteln eines Zeitplans finden Sie unter [Zeitblatt zur Genehmigung einreichen](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Zeitblatt-Genehmiger bestimmen

In der Regel werden Timesheets von funktionalen Managern oder Personal genehmigt. (Timesheets werden normalerweise nicht von Projektmanagern genehmigt.)

Bei der Erstellung des Datenblatt-Profils wird ein Timesheet-Genehmiger definiert. Sie müssen über eine Planungslizenz verfügen, um als Genehmiger benannt zu werden.

Weitere Informationen zur Benennung von Zeitblatt-Genehmigern finden Sie im Abschnitt . [Erstellen oder Bearbeiten eines Zeitleistenprofils](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) im Artikel [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Timesheet genehmigen

Sie können alle Timesheets genehmigen, die übermittelt wurden und in denen Sie als Genehmiger benannt wurden. Wenn ein Timesheet zur Genehmigung vorgelegt wird, wird das Timesheet im **Genehmigungen** -Bereich **Startseite**  Seite. Weitere Informationen finden Sie unter [Validierung der Arbeit](../../review-and-approve-work/manage-approvals/approving-work.md).

Wenn der Workfront-Administrator die Genehmigung für das Datenblatt für den Benutzer und die Zurückweisung des Datenblatts an Benutzer-Ereignishandler aktiviert hat, werden Sie benachrichtigt, nachdem das Datenblatt genehmigt oder abgelehnt wurde. Informationen zum Aktivieren von Ereignisbenachrichtigungen finden Sie unter [In Adobe Workfront verfügbare Ereignisbenachrichtigungen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

So validieren Sie ein Zeitblatt:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken **Timesheets**.
1. Wählen Sie die **Meine Datenblatt-Genehmigungen** oben rechts auf der Seite, um nur die von Ihnen genehmigten Timesheets anzuzeigen

   Oder

   Wählen Sie die **Meine Datenblatt-Genehmigungen** Filter oben in der Liste des Zeitplans.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Die Option &quot;Meine Timesheet-Genehmigungen&quot;wird nicht oben in der Liste der Zeitblätter oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator den Filter Meine Zeitblatt-Genehmigungen entweder aus dem Bereich &quot;Listen-Steuerelemente&quot;im Bereich &quot;Einstellungen&quot;oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optional) Klicken Sie auf die **suchen** icon ![](assets/search-icon.png) am Anfang der Timesheet-Liste und geben Sie einen Suchbegriff ein, um nach einem bestimmten Timesheet zu suchen. Sie können nach einem Zeitrahmen, nach dem Namen eines Eigentümers oder Genehmigers suchen.
1. Klicken Sie auf den Zeitrahmen des zu validierenden Zeitplans. Das Timesheet wird geöffnet.

   >[!TIP]
   Timesheets, die auf die Genehmigung warten, haben den Status [!UICONTROL Gesendet].


1. Klicken **Genehmigen**

   Oder

   Wenn Sie das Timesheet ablehnen möchten, klicken Sie auf **Ablehnen** in der linken unteren Ecke des Zeitblatts.

   Wenn die Genehmigung erteilt wurde, ändert sich der Status des Zeitblatts in **Geschlossen**.

   Wenn die Änderung abgelehnt wird, ändert sich der Status des Zeitblatts in **Zurückgewiesen**.
