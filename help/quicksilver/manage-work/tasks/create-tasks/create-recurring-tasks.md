---
product-area: projects
navigation-topic: create-tasks
title: Wiederkehrende Aufgaben erstellen
description: Sie können wiederkehrende Aufgaben für Aufgaben erstellen, die Sie im Rahmen eines Projekts wiederholen müssen.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 297e72ebb70c335078d65e7ed6e28862285d2fb1
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# Wiederkehrende Aufgaben erstellen

<!--Audited: 01/2024-->

Sie können wiederkehrende Aufgaben für Aufgaben erstellen, die Sie im Rahmen eines Projekts wiederholen müssen.

Allgemeine Informationen zu wiederkehrenden Aufgaben, einschließlich der Auswirkungen der Bearbeitung einer vorhandenen wiederkehrenden Aufgabe, finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p> 
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen zum Projekt mit der Möglichkeit, Aufgaben oder höher hinzuzufügen.</p> 
   <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> 
   <p> Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Aufgabe freigeben </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Wiederkehrende Aufgabe erstellen

>[!NOTE]
>
>Eine wiederkehrende Aufgabe kann nicht durch Ändern einer vorhandenen Aufgabe erstellt werden. Sie müssen eine Aufgabe von Grund auf neu erstellen.

1. Wechseln Sie zu dem Projekt, in dem Sie eine wiederkehrende Aufgabe erstellen möchten, und klicken Sie dann auf das **Aufgaben** im linken Bereich.
1. Klicks **Neue Aufgabe**.

   Das Dialogfeld &quot;Neue Aufgabe&quot;wird angezeigt.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Klicks **Weitere Optionen** Geben Sie dann einen Namen für die Aufgabe in die **Aufgabenname** -Feld.
1. Fahren Sie mit der Aktualisierung der Aufgabe genauso fort wie beim Hinzufügen einer neuen Aufgabe. Weitere Informationen zum Hinzufügen einer neuen Aufgabe finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   Die Dauer und die für eine neue wiederkehrende Aufgabe angegebenen geplanten Stunden sind die Dauer und die geplanten Stunden eines jeden Vorkommens. Die Dauer der übergeordneten Aufgabe ist die Zeit zwischen dem geplanten Startdatum der frühesten Aufgabe und dem geplanten Abschlussdatum der letzten Aufgabe. Die &quot;Geplante Stunden&quot;der übergeordneten Aufgabe ist die Gesamtanzahl aller geplanten Stunden von allen Vorkommen.

1. Klicks **Übersicht** im linken Bereich.
1. Scrollen Sie nach unten zum **Wiederholungsplan** und wählen Sie dann die **Machen Sie dies zu einer wiederkehrenden Aufgabe** -Option.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. Im **Häufigkeit** in der Dropdown-Liste die Anzahl der Zeiteinheiten, in denen die Aufgabe ausgeführt werden soll, und den Typ der Zeiteinheiten. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Wiederholungstyp</th> 
      <th>Beschreibung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Tag</strong> </td> 
      <td> <p>Die Aufgabe wiederholt sich täglich, alle 2 Tage, alle 3 Tage usw., je nach ausgewählter Häufigkeit. Sie können Aufgaben so konfigurieren, dass sie bis zu jedem 6. Tag wiederholt werden. Die Standardeinstellung ist 1 Tag. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Arbeitstag</strong> </td> 
      <td> <p> Die Aufgabe wiederholt sich jeden Arbeitstag, alle 2 Arbeitstage, alle 3 Arbeitstage usw., je nach der von Ihnen ausgewählten Häufigkeit. Sie können Aufgaben so konfigurieren, dass sie bis zu jedem sechsten Arbeitstag wiederholt werden.</p> <p>Diese Option verwendet den vom Systemadministrator festgelegten Standardzeitplan, wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Woche</strong> </td> 
      <td> <p> Die Aufgabe wiederholt sich wöchentlich, alle 2 Wochen, alle 3 Wochen usw., je nach der von Ihnen ausgewählten Häufigkeit.</p> <p>Im <strong>Wiederholungen</strong> -Feld den Wochentag auswählen, an dem die einzelnen Aufgaben ausgeführt werden sollen. Sie können mehrere Tage auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Monat</strong> </td> 
      <td> <p>Die Aufgabe wiederholt sich jeden Monat, alle 2 Monate, alle 3 Monate usw., je nach ausgewähltem Kadaver. Sie können zwischen 1 und 12 Monaten auswählen. </p> <p>Im <strong>Wiederholungen</strong> aus den folgenden Optionen auswählen, wenn die Aufgabe ausgeführt werden soll:</p> 
       <ul> 
        <li> <p><strong>jeden Monat &lt;month date=""&gt;</strong> </p> <p>Sie können Tage zwischen 1 und 30 wählen oder Sie können <strong>last</strong>. Sie können beispielsweise "jeden Monat am 30."auswählen. </p> </li> 
        <li> <p><strong>jeden Monat am &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>Im ersten Dropdown-Menü können Sie eine Zahl zwischen 1 und 4 für die Anzahl der Wochen im Monat auswählen oder "Letzte"auswählen. </p> <p>Im zweiten Dropdown-Menü können Sie einen beliebigen Wochentag auswählen. </p> <p>Sie können beispielsweise "jeden Monat am 2. Dienstag"auswählen. </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn dem Zeitplan des Projekts eine Ausnahme vom Typ &quot;Planung&quot;zugeordnet ist, können wiederkehrende Aufgaben während der Ausnahme nicht gestartet werden. Wiederkehrende Aufgaben, die während der planmäßigen Ausnahme auftreten, werden für den ersten Geschäftstag geplant, der auf die Ausnahme folgt. Weitere Informationen zu geplanten Ausnahmen finden Sie im Artikel [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. Im **Starts** -Feld das Datum und die Uhrzeit für den Beginn der wiederkehrenden Aufgaben auswählen.
1. Im **Ends** -Feld das Datum und die Uhrzeit für den Abschluss der wiederkehrenden Aufgaben auswählen

   Oder

   Auswählen **after `<number>` Vorfälle** um anzugeben, wie oft die wiederkehrende Aufgabe ausgeführt werden soll. Workfront erstellt für die Aufgaben dieselbe Anzahl von Wiederholungen wie die in diesem Feld angegebene Anzahl.

1. Klicks **Aufgabe erstellen.**

   Die Aufgabenliste wird angezeigt. Die wiederkehrende Aufgabe wird als übergeordnetes Element erstellt, und alle Wiederholungen sind untergeordnete Elemente. Workfront hat die Namen der untergeordneten Aufgaben automatisch generiert, indem Sie den Namen verwendet haben, den Sie für die übergeordnete Aufgabe eingegeben haben, gefolgt von einer Zahl. Die wiederkehrenden Aufgaben werden am Ende der Aufgabenliste platziert.

   Weitere Informationen dazu, welche Felder von der übergeordneten wiederkehrenden Aufgabe automatisch ausgefüllt werden, finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Optional) Ändern Sie jede wiederkehrende Aufgabe wie jede andere Aufgabe im Projekt.

   Sie können beispielsweise Zuweisungen, Vorläufer und Zeiträume hinzufügen und andere Informationen über die Aufgabe, einschließlich benutzerdefinierter Felder, ändern.

   >[!IMPORTANT]
   >
   >Die Änderung der übergeordneten Wiederholung nach der individuellen Änderung der untergeordneten Elemente kann zu unterschiedlichen Informationen zwischen den untergeordneten Elementen oder zwischen den untergeordneten Elementen und dem übergeordneten Element führen. Weitere Informationen finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
