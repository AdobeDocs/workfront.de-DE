---
user-type: administrator
product-area: system-administration;user-management
keywords: Gruppe,Voreinstellungen,Aufgabe,Gruppen,Problem,Entsperren
navigation-topic: create-and-manage-groups
title: Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen für eine Gruppe
description: Auf Systemebene kann ein Adobe Workfront-Administrator die Abschnitte „Arbeitszeittabelle“ und „Stundeneinstellungen“, „Allgemeine Voreinstellungen“ und „Arbeitszeittabellen vorab ausfüllen“ entsperren. Dadurch können Gruppenadministratoren die Optionen in diesen Abschnitten unabhängig für ihre eigenen Gruppen konfigurieren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 1%

---

# Arbeitszeittabellen- und Stundeneinstellungen für eine Gruppe konfigurieren

Ein Adobe Workfront-Administrator kann die folgenden Abschnitte der Arbeitszeittabellen- und Stundenvoreinstellungen auf Systemebene entsperren, sodass Gruppenadministratoren sie unabhängig für ihre eigenen Gruppen konfigurieren können:

* Allgemeine Einstellungen
* Wo Benutzende die Zeit protokollieren können
* Vorab-Ausfüllen von Arbeitszeittabellen

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Die folgenden Abschnitte auf der Seite Arbeitszeittabelle und Stundeneinstellungen können nur auf Systemebene konfiguriert werden und können nicht für Gruppen entsperrt werden:

* Gelöschte Projekte, Aufgaben und Probleme

Informationen dazu, wie Workfront-Admins eine Arbeitszeittabelle und Stundeneinstellungen entsperren, finden Sie im Abschnitt [Arbeitszeittabelle und Stundeneinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Arbeitszeittabelle und Stundeneinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Die Konfiguration auf Gruppenebene ist auch für Projektvoreinstellungen sowie für Aufgaben- und Problemvoreinstellungen möglich. Weitere Informationen finden Sie unter [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Aufgaben- und Problemeinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabelle und Stundeneinstellungen gruppieren

Beachten Sie die folgenden Informationen zum Konfigurieren einer entsperrten Arbeitszeittabelle oder Ihrer Stundenvoreinstellung für eine Gruppe:

* Wenn Sie Gruppenadministrator sind und eine Arbeitszeittabelle oder Stundeneinstellung für Ihre Gruppe konfigurieren, wirkt sich dies auf Personen aus, die die Gruppe als Hauptgruppe verwenden.
* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommenen Voreinstellungen gehen verloren.
* Eine Arbeitszeittabelle übernimmt die Arbeitszeittabelle und die Stundeneinstellungen, die für die Hauptgruppe des Arbeitszeittabellen-Besitzers konfiguriert sind.

  <!--
  Add example here?
  -->

* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat und Sie sie für Ihre Gruppe konfigurieren, können Sie sie dann sperren, um sicherzustellen, dass alle Gruppen unter Ihrer Gruppe dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Sperren oder Entsperren einer Gruppenarbeitszeittabelle und Stundenvoreinstellung](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Konfigurieren einer entsperrten Arbeitszeittabelle oder Stundeneinstellung für eine Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einstellungen > Arbeitszeittabelle und Stunden > Voreinstellungen wechseln und dann im Feld oben auf der Seite nach dem Namen der Gruppe suchen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, deren Arbeitszeittabelle oder Stundeneinstellungen Sie konfigurieren möchten.
1. Klicken Sie im linken Bedienfeld auf **Arbeitszeittabellen und Stunden**.

1. Konfigurieren Sie auf der angezeigten Seite im Abschnitt **Allgemeine**&quot; eine der folgenden Optionen:

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Voreinstellung bewegen und eine QuickInfo angezeigt wird, die Ihnen mitteilt, dass sie gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen im Unternehmen zu entsperren.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zeit für zukünftige Termine protokollieren</td> 
      <td> <p>Ermöglicht es Benutzenden, die Zeit für zukünftige Datumsangaben im gesamten System in folgenden Bereichen zu erfassen:</p> 
       <ul> 
       <li>Alle Projekte, Aufgaben und Probleme, bei denen sie Zugriff auf die Protokollierung der Zeit haben, unabhängig von der Gruppe des Projekts</li> 
       <li>Ihre Arbeitszeittabellen als allgemeine Zeit</li>
       </ul> 
       <p>Dies ist nützlich, wenn Benutzer planen, nicht im Büro zu sein und diese Zeit im Voraus protokollieren möchten.</p> 
       <p><b>HINWEIS</b>: Sie können Benutzer nicht daran hindern, Zeit für Aufgaben oder Probleme zu protokollieren, die geschlossen oder abgebrochen wurden. Sie können nur verhindern, dass Benutzer die Zeit bei abgeschlossenen oder inaktiven Projekten protokollieren. Es wird empfohlen, in Listen von Aufgaben und Problemen Filter zu verwenden, um abgeschlossene oder abgebrochene Aufgaben von der Sichtbarkeit für Benutzer auszuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kosten aus einer Arbeitszeittabelle hinzufügen</td> 
      <td> <p>Ermöglicht Benutzern, sowohl Zeit als auch Ausgaben in der Arbeitszeittabelle aufzuzeichnen.</p> 
      <p>Wenn diese Einstellung für eine Gruppe aktiviert ist und die Gruppe für bestimmte Benutzer als Hauptgruppe festgelegt ist, wird neben Projekten und Aufgaben in den Arbeitszeittabellen dieser Benutzer ein Ausgabensymbol angezeigt. Die Benutzer können auf dieses Symbol klicken, um Ausgaben für das Projekt oder die Aufgabe hinzuzufügen oder zu bearbeiten.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabengebiete manuell Stundeneinträgen zuweisen</td> 
      <td> <p>Benutzerinnen und Benutzern erlauben, manuell ein beliebiges Aufgabengebiet auszuwählen, das in ihrem Benutzerprofil oder dem Objekt zugewiesen ist.</p> <p><b>WICHTIG</b>:  
        <ul> 
         <li>Wenn Sie diese Einstellung deaktivieren, nachdem Sie Stundeneinträgen Aufgabengebiete zugewiesen haben, müssen Benutzerinnen und Benutzer die Stunden anpassen, die in verschiedenen Rollen auf der Registerkarte Stunden des Projekts, der Aufgabe oder des Problems protokolliert sind.</li> 
         <li>Wenn dem/der Benutzenden in seinem/ihrem Profil kein Aufgabengebiet zugewiesen ist und im Dialogfeld Erweiterte Zuweisungen als Aufgabenbesitzer/in eine Aufgabe zugewiesen ist, wird dieses Aufgabengebiet angezeigt, wenn sich der/die Benutzende die Zeit für die Aufgabe anmeldet.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken</td> 
      <td> <p>Bearbeitung auf Arbeitszeittabellen-Besitzer beschränken, unabhängig von der Gruppe des Projekts und Workfront-Administratoren. Wenn diese Option deaktiviert ist, können Arbeitszeittabellen auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Arbeitszeittabellen und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Arbeitszeittabellen-Genehmiger, wenn „Kann Stunden bearbeiten“ in der Arbeitszeittabelle aktiviert ist</p> </li> 
        <li> <p>Der Manager des Arbeitszeittabellen-Besitzers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Stundenbearbeitung auf Eigentümer und Administratoren beschränken</td> 
      <td>Bearbeitung auf die Benutzenden beschränken, die die Stunden eingeben, und Workfront-Administratoren einschränken. Diese Einstellung gilt für die Registerkarte Stunden in einem Projekt oder einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren **im Abschnitt „Wo Benutzer die Zeit** können“ eine der folgenden Optionen:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Zeit direkt in Projekten protokollieren</td> 
      <td>Ermöglicht es den Benutzenden, die Zeit für das Projekt zu protokollieren (sowohl auf der Registerkarte „Aktualisierungen“ als auch auf der Arbeitszeittabelle). Wenn Sie möchten, dass Ihre Benutzerinnen und Benutzer die Zeit der Aufzeichnung nicht auf Projektebene erfassen, lassen Sie diese Option deaktiviert.</td>
     </tr>
     <tr>
      <td role="rowheader">Zeit für abgeschlossene Projekte protokollieren</td>
      <td>Ermöglicht Benutzern das Aufzeichnen der Zeit für ein Projekt, das als abgeschlossen markiert wurde. Wenn diese Option deaktiviert ist, können Benutzende die Zeit nicht für Arbeiten erfassen, die sie an Projekten im Status Abgeschlossen abgeschlossen haben.</td>
     </tr>
     <tr>
      <td role="rowheader">Zeit für eingestellte Projekte protokollieren</td> 
      <td>Wenn diese Option aktiviert ist, können Benutzer Stunden in Projekten mit dem Status „Inaktiv“ protokollieren.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Diese Voreinstellung wird basierend auf der Konfiguration der Hauptgruppen-Voreinstellungen des Benutzers angewendet. Wenn diese Einstellungen in den Hauptgruppeneinstellungen der Benutzenden aktiviert sind, können diese die Zeit direkt in Projekten protokollieren, einschließlich abgeschlossener oder inaktiver Projekte, unabhängig davon, ob die Gruppeneinstellungen des Projekts dies zulassen oder nicht.

1. Konfigurieren **im Abschnitt** vorab ausfüllen eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbeiten, die innerhalb &lt;Anzahl der Wochen&gt; des Arbeitsbereichs der Arbeitszeittabelle liegen</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich der Arbeitszeittabelle, die dem Benutzer zugewiesene Daten von Aufgaben und Problemen enthält. Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern. Das bedeutet, dass die Arbeitszeittabelle vorab mit Aufgaben und Problemen ausgefüllt wird, deren Termine zwischen vier Wochen vor dem Datumsbereich der Arbeitszeittabelle und bis zu vier Wochen nach dem Datumsbereich der Arbeitszeittabelle liegen, wenn Sie für Ihren Bereich 4 Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgeschlossene Aufgaben und Probleme</td> 
      <td>Wenn einer einzelnen Aufgabe normalerweise mehrere Ressourcen zugewiesen sind, empfehlen wir diese Einstellung. Wenn also eine Ressource die Zeit für einen Vorgang aufzeichnet und ihn als abgeschlossen markiert, können die anderen Ressourcen, die dem Vorgang zugewiesen sind, den Vorgang oder das Problem weiterhin in ihrer Arbeitszeittabelle finden, um ihre Stunden aufzuzeichnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgaben und Probleme mit geplanten Terminen im Datumsbereich der Arbeitszeittabelle</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält die Arbeitszeittabelle Aufgaben und Probleme, die entweder ein geplantes Startdatum oder ein Abschlussdatum haben, das in den Datumsbereich der Arbeitszeittabelle fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Aufgaben mit voraussichtlichen Terminen im Datumsbereich der Arbeitszeittabelle</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält die Arbeitszeittabelle Aufgaben mit einem voraussichtlichen Start- oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, auch wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Datumsbereichs der Arbeitszeittabelle liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
