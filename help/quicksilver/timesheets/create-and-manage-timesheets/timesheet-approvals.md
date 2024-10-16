---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Ein Datenblatt genehmigen
description: Der Prozess der Genehmigung von Timesheets bietet Managern einen Einblick in die Arbeitszeiten ihrer direkten Berichte. Die Genehmiger können überprüfen, ob die aufgezeichnete Zeit in den richtigen Bereichen zugewiesen wurde und ob für den betreffenden Zeitraum eine ausreichende Anzahl von Stunden aufgezeichnet wurde.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '686'
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

Sie können alle Timesheets genehmigen, die übermittelt wurden und in denen Sie als Genehmiger benannt wurden. Wenn ein Timesheet zur Genehmigung eingereicht wird, wird das Timesheet im Widget **Meine Genehmigungen** in Ihrem Bereich **Home** aufgelistet. Weitere Informationen finden Sie unter [Arbeiten genehmigen](../../review-and-approve-work/manage-approvals/approving-work.md).

Wenn die folgenden Benachrichtigungseinstellungen vorhanden sind, erhält der Benutzer, der das Datenblatt zur Validierung einreicht, nach der Validierung des Datenblatts eine E-Mail:

* Der Workfront-Administrator hat die Genehmigung des Zeitblatts für Benutzer und die Zurückweisung des Zeitblatts an Benutzer -Ereignishandler aktiviert. Weitere Informationen zum Aktivieren von Ereignisbenachrichtigungen finden Sie unter [Ereignislaufbenachrichtigungstypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* Auf der Profilseite des Benutzers ist die Option Persönliche Benachrichtigung bestätigt. Weitere Informationen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Timesheet im Bereich &quot;Timesheets&quot;genehmigen

{{step1-to-timesheets}}

Der Bereich **Timesheets** wird geöffnet.

1. (Bedingt) Wenn das letzte Mal, dass Sie auf Timesheets zugreifen, geöffnet wird, klicken Sie in der oberen linken Ecke des Bildschirms auf **Zurück zu Timesheets** .

1. Wählen Sie oben rechts auf der Seite die Option &quot;**My Timesheet Approvals**&quot;, um nur die von Ihnen genehmigten Timesheets anzuzeigen.

   Oder

   Wählen Sie den Filter **Meine Timesheet-Genehmigungen** oben in der Timesheet-Liste aus.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Die Option &quot;Meine Timesheet-Genehmigungen&quot;wird nicht oben in der Liste der Zeitblätter oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator den Filter Meine Zeitblatt-Genehmigungen entweder aus dem Bereich &quot;Listen-Steuerelemente&quot;im Bereich &quot;Einstellungen&quot;oder aus Ihrer Layout-Vorlage entfernt hat.
   >
   >Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
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

### Genehmigen von Timesheets über den Startbereich

{{step1-to-home}}

Der Startbereich wird geöffnet.

1. Stellen Sie sicher, dass das Widget **Meine Genehmigungen** zu Ihrem Startbereich hinzugefügt wurde. Weitere Informationen finden Sie unter [Hinzufügen, Bearbeiten oder Entfernen von Widgets in der neuen Startseite](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).
1. Suchen Sie im Widget Meine Validierungen nach einer Timesheet-Validierung.
1. (Optional) Erweitern Sie das Dropdown-Menü rechts neben den Schaltflächen Genehmigen oder Ablehnen , um einen Kommentar zu Ihrer Entscheidung hinzuzufügen, und klicken Sie dann auf **Hinzufügen**.
1. Klicken Sie auf eine der folgenden Schaltflächen, um Ihre Validierungsentscheidung zu treffen:

   * Genehmigen
   * Ablehnen

   Die Genehmigung wird aus dem Widget **Meine Genehmigungen** entfernt.


