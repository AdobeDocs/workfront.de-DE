---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabelle genehmigen
description: Der Prozess der Genehmigung von Arbeitszeittabellen bietet Managern Einblick in die Arbeitszeit ihrer direkt unterstellten Mitarbeiter. Die genehmigenden Personen können überprüfen, ob alle aufgezeichneten Zeiten in den richtigen Bereichen aufgezeichnet wurden und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 1%

---

# Arbeitszeittabelle genehmigen

<!--Audited: 8/2024-->

Der Prozess der Genehmigung von Arbeitszeittabellen bietet Managern Einblick in die Arbeitszeit ihrer direkt unterstellten Mitarbeiter. Die genehmigenden Personen können überprüfen, ob alle aufgezeichneten Zeiten in den richtigen Bereichen aufgezeichnet wurden und ob eine ausreichende Anzahl von Stunden für den Zeitraum aufgezeichnet wurde.

Adobe Workfront bietet die Möglichkeit, Arbeitszeittabellen-Genehmigungen zu konfigurieren, die in diesem Bereich unterstützt werden.

Informationen zum Senden einer Arbeitszeittabelle finden Sie unter [Senden einer Arbeitszeittabelle zur Genehmigung](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

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
   <td><p>Administrativer Zugriff auf Arbeitszeittabellen und Stunden</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabellen-Genehmiger bestimmen

Normalerweise werden Arbeitszeittabellen von funktionalen Managern oder Personalmitarbeitern genehmigt. Arbeitszeittabellen werden normalerweise nicht von Projektmanagern genehmigt. Projektmanager können die für Projekte aufgezeichnete Zeit genehmigen, Team- oder Personalmanager müssen jedoch Arbeitszeittabellen genehmigen.

Bei der Erstellung des Arbeitszeittabellen-Profils wird eine Person definiert, die Arbeitszeittabellen genehmigt. Sie müssen über eine Planlizenz verfügen, um als genehmigende Person benannt zu werden.

Weitere Informationen zum Bestimmen von Arbeitszeittabellen-Genehmigern finden Sie im Abschnitt [Erstellen oder Bearbeiten eines Arbeitszeittabellen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) im Artikel [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Arbeitszeittabelle genehmigen

Sie können alle eingereichten Arbeitszeittabellen genehmigen, wenn Sie als genehmigende Person benannt wurden. Wenn eine Arbeitszeittabelle zur Genehmigung eingereicht wird, wird sie im Widget **Meine Genehmigungen** im Bereich **Startseite** aufgelistet. Weitere Informationen finden Sie unter [Arbeiten genehmigen](../../review-and-approve-work/manage-approvals/approving-work.md).

Wenn die folgenden Benachrichtigungseinstellungen eingerichtet sind, erhält der Benutzer, der die Arbeitszeittabelle zur Genehmigung einreicht, eine E-Mail, nachdem eine Arbeitszeittabelle genehmigt wurde:

* Der Workfront-Administrator hat die Arbeitszeittabellen-Genehmigung für den Benutzer und die Arbeitszeittabellen-Ablehnung für Benutzer-Ereignishandler aktiviert. Informationen zur Aktivierung von Ereignisbenachrichtigungen finden Sie [Ereignistypen](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* Die persönliche Benachrichtigung „Meine Arbeitszeittabelle ist genehmigt“ wird auf der Profilseite des Benutzers aktiviert. Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Genehmigen einer Arbeitszeittabelle im Bereich Arbeitszeittabellen

{{step1-to-timesheets}}

Der Bereich **Arbeitszeittabellen** wird geöffnet.

1. (Bedingt) Wenn Sie das letzte Mal, als Sie auf zugegriffen haben, geöffnet haben **klicken Sie in** linken oberen Ecke des Bildschirms auf „Zurück zu Arbeitszeittabellen“.

1. Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** oben rechts auf der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen

   Oder

   Wählen Sie den Filter **Meine Arbeitszeittabellen** oben in der Arbeitszeittabellen-Liste aus.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Die Option Meine Arbeitszeittabellen-Genehmigungen wird nicht oben in der Arbeitszeittabellen-Liste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins den Filter Meine Arbeitszeittabellen-Genehmigungen entweder aus den Listensteuerelementen im Bereich Setup oder aus Ihrer Layoutvorlage entfernt haben.
   >
   >Weitere Informationen finden Sie [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Optional) Klicken Sie auf das **Suchen**-Symbol oben ![](assets/search-icon.png) in der Arbeitszeittabellenliste und geben Sie einen Suchbegriff ein, um eine bestimmte Arbeitszeittabelle zu finden. Sie können nach einem Zeitrahmen oder dem Namen eines Verantwortlichen oder einer genehmigenden Person suchen.
1. Klicken Sie auf den Zeitrahmen für die Arbeitszeittabelle, die Sie genehmigen möchten. Die Arbeitszeittabelle wird geöffnet.

   >[!TIP]
   >
   >Arbeitszeittabellen, die auf Genehmigung warten, haben den Status [!UICONTROL Eingereicht].


1. Klicken Sie auf **Genehmigen**

   Oder

   Wenn Sie die Arbeitszeittabelle ablehnen möchten, klicken **unten links** der Arbeitszeittabelle auf „Ablehnen“.

   Wenn genehmigt, ändert sich der Status der Arbeitszeittabelle in **Geschlossen**.

   Wenn er abgelehnt wird, ändert sich der Arbeitszeittabellen-Status in **Abgelehnt**.

### Genehmigen von Arbeitszeittabellen im Bereich „Startseite“

{{step1-to-home}}

Der Bereich Home wird geöffnet.

1. Stellen Sie sicher, dass das Widget **Meine Genehmigungen** zu Ihrem Bereich Startseite hinzugefügt wurde. Weitere Informationen finden Sie unter [Hinzufügen, Bearbeiten oder Entfernen von Widgets in der neuen Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
1. Suchen Sie eine Arbeitszeittabellen-Genehmigung in Ihrem Widget Meine Genehmigungen .
1. (Optional) Erweitern Sie das Dropdown-Menü rechts neben den Schaltflächen Genehmigen oder Ablehnen , um einen Kommentar zu Ihrer Entscheidung hinzuzufügen, und klicken Sie dann auf **Hinzufügen**.
1. Klicken Sie auf eine der folgenden Schaltflächen, um Ihre Genehmigungsentscheidung zu treffen:

   * Genehmigen
   * Ablehnen

   Die Genehmigung wird aus dem Widget **Meine Genehmigungen** entfernt.


