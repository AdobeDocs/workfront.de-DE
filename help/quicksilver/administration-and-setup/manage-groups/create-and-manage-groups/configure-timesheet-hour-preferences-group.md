---
user-type: administrator
product-area: system-administration;user-management
keywords: group,Preferences,task,groups,issue,unlock
navigation-topic: create-and-manage-groups
title: Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe
description: Auf Systemebene kann ein Adobe Workfront-Administrator die Abschnitte "Allgemeine Voreinstellungen"und "Timesheet- und Stundenvoreinstellungen"entsperren und Zeitesheets vorab ausfüllen. Auf diese Weise können Gruppenadministratoren die Optionen in diesen Abschnitten unabhängig für ihre eigenen Gruppen konfigurieren.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 4%

---

# Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe

Ein Adobe Workfront-Administrator kann die folgenden Abschnitte der Voreinstellungen für Zeitpläne und Stunden auf Systemebene entsperren, sodass Gruppenadministratoren sie unabhängig für ihre eigenen Gruppen konfigurieren können:

* Allgemeine Einstellungen
* Arbeitszeittabellen vorab füllen mit

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Die folgenden Abschnitte auf der Seite &quot;Timesheet- und Stundeneinstellungen&quot;können nur auf Systemebene konfiguriert werden und können nicht für Gruppen entsperrt werden:

* Protokollierungszeit
* Einstellungen für die Löschung von Projekten, Aufgaben oder Problemen

Informationen dazu, wie ein Workfront-Administrator die Voreinstellung für ein Zeitblatt und eine Stunde freischaltet, finden Sie im Abschnitt [Zeitblatt- und Stundenvoreinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Eine Konfiguration auf Gruppenebene ist auch für Projektvoreinstellungen sowie für Aufgaben- und Problemvoreinstellungen möglich. Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Voreinstellungen für Gruppenzeiträume

Beachten Sie die folgenden Informationen zum Konfigurieren eines entsperrten Zeitblatts oder einer Stundenvoreinstellung für eine Gruppe:

* Wenn Sie Gruppenadministrator sind und für Ihre Gruppe ein Timesheet oder eine Stundenvorgabe konfigurieren, wirkt sich dies auf Personen aus, die die Gruppe als ihre Startseite verwenden.
* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommene Voreinstellung gehen verloren.
* Ein Timesheet übernimmt die für die Startseite des Timesheet-Eigentümers konfigurierten Voreinstellungen für das Zeitblatt und die Stunde.

   <!--
  Add example here?
  -->

* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt und sie für Ihre Gruppe konfiguriert hat, können Sie sie sperren, um sicherzustellen, dass alle in den Gruppen unter Ihrer Gruppe dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Voreinstellung für Zeitblatt und Stunde einer Gruppe sperren oder entsperren](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Konfigurieren einer entsperrten Zeitleiste oder einer Stundenvoreinstellung für eine Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie &quot;Einrichtung&quot;> &quot;Zeitblatt und Stunden&quot;> &quot;Voreinstellungen&quot;aufrufen und dann im Feld oben auf der Seite nach dem Gruppennamen suchen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, deren Timesheet- oder Stundeneinstellungen Sie konfigurieren möchten.
1. Klicken Sie im linken Bereich auf **Timesheets und Stunden**.

1. Auf der angezeigten Seite wird im **Allgemeine Voreinstellungen** konfigurieren Sie eine der folgenden Optionen:

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Voreinstellung bewegen und eine QuickInfo angezeigt wird, um Ihnen mitzuteilen, dass sie gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen in der Organisation zu entsperren.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zeit für zukünftige Termine protokollieren</td> 
      <td> <p>Ermöglicht Benutzern, die Zeit für zukünftige Daten im gesamten System zu protokollieren in:</p> 
       <ul> 
       <li>Alle Projekte, Aufgaben und Probleme, auf die sie Zugriff auf die Protokollzeit haben, unabhängig von der Gruppe des Projekts</li> 
       <li>Ihre Timesheets als "Allgemeine Zeit"</li>
       </ul> 
       <p>Dies ist nützlich, wenn Benutzer planen, außerhalb des Büros zu sein, und diese Zeit vorher protokollieren möchten.</p> 
       <p><b>NOTE</b>: Sie können Benutzer nicht daran hindern, die Zeit für Aufgaben oder Probleme zu protokollieren, die geschlossen oder abgebrochen werden. Sie können Benutzer nur daran hindern, die Zeit für komplette oder tote Projekte zu protokollieren. Es wird empfohlen, Filter in Listen mit Aufgaben und Problemen zu verwenden, um auszuschließen, dass abgeschlossene oder abgebrochene Aufgaben für Benutzer nicht sichtbar sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kosten aus einer Arbeitszeittabelle hinzufügen</td> 
      <td> <p>Ermöglicht Benutzern die Aufzeichnung von Zeit und Ausgaben im Zeitblatt.</p> 
      <p>Wenn diese Voreinstellung für eine Gruppe aktiviert ist und die Gruppe als Startseite für bestimmte Benutzer festgelegt ist, wird neben den Projekten und Aufgaben in den Timesheets dieser Benutzer ein Ausgabensymbol angezeigt. Benutzer können auf dieses Symbol klicken, um Ausgaben für das Projekt oder die Aufgabe hinzuzufügen oder zu bearbeiten.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabenbiete Stundeneinträgen manuell zuweisen</td> 
      <td> <p>Benutzern die manuelle Auswahl von Aufgaben ermöglichen, die in ihrem Benutzerprofil zugewiesen oder dem Objekt zugewiesen sind.</p> <p><b>WICHTIG</b>:  
        <ul> 
         <li>Wenn Sie diese Einstellung deaktivieren, nachdem Sie Stundeneinträgen Auftragsrollen zugewiesen haben, müssen die Benutzer die Stunden anpassen, die auf der Registerkarte Stunden des Projekts, der Aufgabe oder des Problems unter verschiedenen Rollen protokolliert wurden.</li> 
         <li>Wenn dem Benutzer in seinem Profil keine Auftragsrolle zugewiesen ist und im Dialogfeld "Erweiterte Zuweisungen"eine Aufgabe als Aufgabeneigentümer zugewiesen ist, wird diese Auftragsrolle angezeigt, wenn der Benutzer die Zeit für die Aufgabe protokolliert.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Bearbeitung von Stundenzetteln auf Eigentümer und Administratoren beschränken</td> 
      <td> <p>Beschränken Sie die Bearbeitung auf die Inhaber von Zeitblättern, unabhängig von der Gruppe des Projekts und den Workfront-Administratoren. Wenn diese Option deaktiviert ist, können Timesheets auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Timesheets und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Timesheet-Genehmiger, wenn auf dem Timesheet "Kann Stunden bearbeiten"aktiviert ist</p> </li> 
        <li> <p>Manager des Timesheet-Eigentümers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Beschränkung der Stundenbearbeitung auf Inhaber und Administratoren</td> 
      <td>Beschränken Sie die Bearbeitung auf den Benutzer, der die Stunden eingibt, und auf Workfront-Administratoren. Diese Einstellung gilt für die Registerkarte Stunden in einem Projekt oder in einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Im **Vorausfüllen von Timesheets mit** konfigurieren Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbeiten, die sich in &lt;number of="" weeks=""&gt; des Arbeitsbereichs des Zeitplans</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich des Zeitblatts, das Datum der dem Benutzer zugewiesenen Aufgaben und Probleme enthält. Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern. Das bedeutet, dass das Timesheet mit Aufgaben und Problemen vorausgefüllt ist, die zwischen vier Wochen vor dem Datumsbereich des Zeitblatts und bis zu vier Wochen nach dem Datumsbereich des Zeitblatts liegen, wenn Sie für Ihren Bereich vier Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgeschlossene Aufgaben und Probleme</td> 
      <td>Wenn normalerweise mehrere Ressourcen einer einzelnen Aufgabe zugewiesen sind, empfehlen wir diese Einstellung. Das bedeutet, dass die anderen Ressourcen, die der Aufgabe zugewiesen sind, die Aufgabe bzw. das Problem in ihrem Timesheet finden können, um ihre Stunden aufzuzeichnen, wenn eine Ressource die Zeit für die Aufgabe aufzeichnet und sie als abgeschlossen kennzeichnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgaben &amp; Problemen, die über geplante Termine innerhalb des Datumsbereichs der Arbeitszeittabelle verfügen</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben und Probleme mit einem geplanten Startdatum oder einem geplanten Abschlussdatum, das in den Datumsbereich des Zeitblatts fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Aufgaben mit prognostizierten Daten im Datumsbereich des Zeitplans</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben mit einem geplanten Startdatum oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, selbst wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Zeitblatt-Datumsbereichs liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
