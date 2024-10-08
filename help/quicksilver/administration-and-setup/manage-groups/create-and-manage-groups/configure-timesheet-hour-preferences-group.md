---
user-type: administrator
product-area: system-administration;user-management
keywords: group,Preferences,task,groups,issue,unlock
navigation-topic: create-and-manage-groups
title: Konfigurieren von Timesheet- und Stunden-Voreinstellungen für eine Gruppe
description: Auf Systemebene kann ein Adobe Workfront-Administrator die Abschnitte "Allgemeine Voreinstellungen"und "Timesheet- und Stundenvoreinstellungen"entsperren und Zeitesheets vorab ausfüllen. Auf diese Weise können Gruppenadministratoren die Optionen in diesen Abschnitten unabhängig für ihre eigenen Gruppen konfigurieren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 1%

---

# Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe

Ein Adobe Workfront-Administrator kann die folgenden Abschnitte der Voreinstellungen für Zeitpläne und Stunden auf Systemebene entsperren, sodass Gruppenadministratoren sie unabhängig für ihre eigenen Gruppen konfigurieren können:

* Allgemeine Einstellungen
* Wo Benutzende die Zeit protokollieren können
* Vorab-Ausfüllen von Arbeitszeittabellen

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Die folgenden Abschnitte auf der Seite &quot;Timesheet- und Stundeneinstellungen&quot;können nur auf Systemebene konfiguriert werden und können nicht für Gruppen entsperrt werden:

* Gelöschte Projekte, Aufgaben und Probleme

Informationen dazu, wie ein Workfront-Administrator die Voreinstellung für ein Zeitblatt und eine Stunde entsperrt, finden Sie im Abschnitt [Zeitblatt- und Stundeneinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Zeitblatt und Stundeneinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) .

>[!TIP]
>
>Eine Konfiguration auf Gruppenebene ist auch für Projektvoreinstellungen sowie für Aufgaben- und Problemvoreinstellungen möglich. Weitere Informationen finden Sie unter [Konfigurieren von Projektanvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Konfigurieren von Aufgaben und Ausgabevoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voreinstellungen für Gruppenzeitpläne und -zeiten

Beachten Sie die folgenden Informationen zum Konfigurieren eines entsperrten Zeitblatts oder einer Stundenvoreinstellung für eine Gruppe:

* Wenn Sie Gruppenadministrator sind und für Ihre Gruppe ein Timesheet oder eine Stundenvorgabe konfigurieren, wirkt sich dies auf Personen aus, die die Gruppe als ihre Startseite verwenden.
* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommene Voreinstellung gehen verloren.
* Ein Timesheet übernimmt die für die Startseite des Timesheet-Eigentümers konfigurierten Voreinstellungen für das Zeitblatt und die Stunde.

  <!--
  Add example here?
  -->

* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt und sie für Ihre Gruppe konfiguriert hat, können Sie sie sperren, um sicherzustellen, dass alle in den Gruppen unter Ihrer Gruppe dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Vorgabe zum Sperren oder Entsperren eines Gruppen-Timesheets und einer Stunde](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Konfigurieren einer entsperrten Zeitleiste oder einer Stundenvoreinstellung für eine Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie &quot;Einrichtung&quot;> &quot;Zeitblatt und Stunden&quot;> &quot;Voreinstellungen&quot;aufrufen und dann im Feld oben auf der Seite nach dem Gruppennamen suchen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, deren Timesheet- oder Stundeneinstellungen Sie konfigurieren möchten.
1. Klicken Sie im linken Bereich auf **Timesheets und Stunden**.

1. Konfigurieren Sie auf der angezeigten Seite im Abschnitt **Allgemeine Voreinstellungen** eine der folgenden Optionen:

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Voreinstellung bewegen und eine QuickInfo angezeigt wird, um Ihnen mitzuteilen, dass sie gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen in der Organisation zu entsperren.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Protokollzeit für zukünftige Daten</td> 
      <td> <p>Ermöglicht Benutzern, die Zeit für zukünftige Daten im gesamten System zu protokollieren in:</p> 
       <ul> 
       <li>Alle Projekte, Aufgaben und Probleme, auf die sie Zugriff auf die Protokollzeit haben, unabhängig von der Gruppe des Projekts</li> 
       <li>Ihre Timesheets als "Allgemeine Zeit"</li>
       </ul> 
       <p>Dies ist nützlich, wenn Benutzer planen, außerhalb des Büros zu sein, und diese Zeit vorher protokollieren möchten.</p> 
       <p><b>HINWEIS</b>: Sie können Benutzer nicht daran hindern, die Zeit für Aufgaben oder Probleme zu protokollieren, die geschlossen oder abgebrochen werden. Sie können Benutzer nur daran hindern, die Zeit für komplette oder tote Projekte zu protokollieren. Es wird empfohlen, Filter in Listen mit Aufgaben und Problemen zu verwenden, um auszuschließen, dass abgeschlossene oder abgebrochene Aufgaben für Benutzer nicht sichtbar sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufwendungen aus einem Zeitblatt hinzufügen</td> 
      <td> <p>Ermöglicht Benutzern, sowohl Zeit als auch Ausgaben im Timesheet aufzuzeichnen.</p> 
      <p>Wenn diese Voreinstellung für eine Gruppe aktiviert ist und die Gruppe als Startseite für bestimmte Benutzer festgelegt ist, wird neben den Projekten und Aufgaben in den Timesheets dieser Benutzer ein Ausgabensymbol angezeigt. Benutzer können auf dieses Symbol klicken, um Ausgaben für das Projekt oder die Aufgabe hinzuzufügen oder zu bearbeiten.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manuelles Zuweisen von Vorgangsrollen zu Stundeneinträgen</td> 
      <td> <p>Benutzern die manuelle Auswahl von Aufgaben ermöglichen, die in ihrem Benutzerprofil zugewiesen oder dem Objekt zugewiesen sind.</p> <p><b>WICHTIG</b>:  
        <ul> 
         <li>Wenn Sie diese Einstellung deaktivieren, nachdem Sie Stundeneinträgen Auftragsrollen zugewiesen haben, müssen die Benutzer die Stunden anpassen, die auf der Registerkarte Stunden des Projekts, der Aufgabe oder des Problems unter verschiedenen Rollen protokolliert wurden.</li> 
         <li>Wenn dem Benutzer in seinem Profil keine Auftragsrolle zugewiesen ist und im Dialogfeld "Erweiterte Zuweisungen"eine Aufgabe als Aufgabeneigentümer zugewiesen ist, wird diese Auftragsrolle angezeigt, wenn der Benutzer die Zeit für die Aufgabe protokolliert.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren</td> 
      <td> <p>Beschränken Sie die Bearbeitung auf die Inhaber von Zeitblättern, unabhängig von der Gruppe des Projekts und den Workfront-Administratoren. Wenn diese Option deaktiviert ist, können Timesheets auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Timesheets und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Timesheet-Genehmiger, wenn auf dem Timesheet "Kann Stunden bearbeiten"aktiviert ist</p> </li> 
        <li> <p>Manager des Timesheet-Eigentümers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Beschränkung der Stundenbearbeitung auf Inhaber und Administratoren</td> 
      <td>Beschränken Sie die Bearbeitung auf Benutzer, die die Stunden eingeben, und Workfront-Administratoren. Diese Einstellung gilt für die Registerkarte Stunden in einem Projekt oder in einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren Sie im Abschnitt &quot;**Wo Benutzer die Zeit protokollieren können**&quot;eine der folgenden Optionen:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Direkte Protokollzeit für Projekte</td> 
      <td>Ermöglicht Benutzern die Protokollzeit für das Projekt (sowohl auf der Registerkarte Updates als auch im Timesheet). Wenn Sie die Aufnahmezeit Ihrer Benutzer auf Projektebene beschränken möchten, lassen Sie diese Option deaktiviert.</td>
     </tr>
     <tr>
      <td role="rowheader">Protokollzeit für abgeschlossene Projekte</td>
      <td>Ermöglicht Benutzern das Aufzeichnen der Zeit für ein Projekt, das als abgeschlossen gekennzeichnet wurde. Wenn diese Option deaktiviert ist, können Benutzer die Zeit für die Arbeit, die sie an Projekten abgeschlossen haben, nicht im Status Fertig stellen aufzeichnen.</td>
     </tr>
     <tr>
      <td role="rowheader">Protokollzeit für Projekte, die tot sind</td> 
      <td>Wenn diese Option aktiviert ist, können Benutzer Stunden für Projekte mit dem Status "Dead"protokollieren.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Diese Voreinstellung wird je nach Konfiguration der Voreinstellungen für die Home Group des Benutzers angewendet. Wenn diese Einstellungen in den Voreinstellungen für die Startseite des Benutzers aktiviert sind, können sie die Zeit direkt für Projekte protokollieren, einschließlich abgeschlossener oder veralteter Projekte, unabhängig davon, ob die Gruppeneinstellungen des Projekts dies zulassen oder nicht.

1. Konfigurieren Sie im Abschnitt **Vorfüllen von Timesheets** eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbeiten, die innerhalb von &lt;Anzahl der Wochen&gt; des Arbeitsbereichs des Zeitplans liegen</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich des Zeitblatts, das Datum der dem Benutzer zugewiesenen Aufgaben und Probleme enthält. Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern. Das bedeutet, dass das Timesheet mit Aufgaben und Problemen vorausgefüllt ist, die zwischen vier Wochen vor dem Datumsbereich des Zeitblatts und bis zu vier Wochen nach dem Datumsbereich des Zeitblatts liegen, wenn Sie für Ihren Bereich vier Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgeschlossene Aufgaben und Probleme</td> 
      <td>Wenn normalerweise mehrere Ressourcen einer einzelnen Aufgabe zugewiesen sind, empfehlen wir diese Einstellung. Das bedeutet, dass die anderen Ressourcen, die der Aufgabe zugewiesen sind, die Aufgabe bzw. das Problem in ihrem Timesheet finden können, um ihre Stunden aufzuzeichnen, wenn eine Ressource die Zeit für die Aufgabe aufzeichnet und sie als abgeschlossen kennzeichnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgaben und Probleme, bei denen im Datumsbereich des Zeitplans Daten geplant sind</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben und Probleme mit einem geplanten Startdatum oder einem geplanten Abschlussdatum, das in den Datumsbereich des Zeitblatts fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Aufgaben mit prognostizierten Daten im Datumsbereich des Zeitplans</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben mit einem geplanten Startdatum oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, selbst wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Zeitblatt-Datumsbereichs liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
