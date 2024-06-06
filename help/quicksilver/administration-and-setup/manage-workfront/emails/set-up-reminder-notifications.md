---
title: Einrichten von Erinnerungsbenachrichtigungen
description: Erinnerungsbenachrichtigungen generieren E-Mails, die an Benutzer basierend auf bestimmten Kriterien gesendet werden. Erinnerungsbenachrichtigungen erinnern Benutzer an eine Aktion, die für eine Aufgabe, ein Problem, ein Projekt oder ein Timesheet erforderlich ist.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '1215'
ht-degree: 2%

---

# Einrichten von Erinnerungsbenachrichtigungen

<!-- Audited: 1/2024 -->

Als Workfront-Administrator können Sie Erinnerungsbenachrichtigungen für Benutzer erstellen und sie mit Objekten verknüpfen, denen Ihre Benutzer besondere Aufmerksamkeit widmen sollen.

Erinnerungsbenachrichtigungen generieren E-Mails, die an Benutzer basierend auf bestimmten Kriterien gesendet werden. Erinnerungsbenachrichtigungen erinnern Benutzer an eine Aktion, die für eine Aufgabe, ein Problem, ein Projekt oder ein Timesheet erforderlich ist.

Nachdem Sie die Erinnerungsbenachrichtigungen erstellt haben, können Benutzer sie manuell mit Arbeitselementen wie Projekten, Aufgaben, Problemen und Timesheets verknüpfen. Weitere Informationen finden Sie unter [Erinnerungsbenachrichtigung an ein Objekt anhängen](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Planung oder höher mit Administratorzugriff auf Erinnerungsbenachrichtigungen</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## E-Mail zur Erinnerung anpassen

Sie können Betreff, Text und HTML in der E-Mail mit den Erinnerungsbenachrichtigungen anpassen.

Sie können auch die in der Erinnerungsbenachrichtigung enthaltene Standard-E-Mail verwenden. Die Standard-E-Mail verwendet den Namen der Erinnerungsbenachrichtigung als E-Mail-Betreff und den Objektnamen im E-Mail-Textkörper, einschließlich des Ereignisses, das die Benachrichtigung ausgelöst hat.

Wenn Sie die E-Mail-Erinnerung anpassen möchten, müssen Sie eine E-Mail-Vorlage erstellen und sie an die Erinnerungsbenachrichtigung anhängen.

Informationen zum Erstellen einer E-Mail-Vorlage finden Sie unter [E-Mail-Vorlagen konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Erstellen einer Erinnerungsbenachrichtigung

{{step-1-to-setup}}

1. Klicks **Email** > **Benachrichtigungen** > **Erinnerungsbenachrichtigungen**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Klicks **Neue Erinnerungsbenachrichtigung**.

1. Klicken Sie in der Dropdown-Liste auf den Objekttyp, den Sie mit der Erinnerungsbenachrichtigung verbinden möchten.

   Wenn Sie beispielsweise eine Erinnerungsbenachrichtigung an ein Zeitblatt anhängen möchten, klicken Sie auf **Datenblatt**.

1. Im **Neue Erinnerungsbenachrichtigung** die folgenden Informationen angeben.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name der Erinnerungsbenachrichtigung</td> 
      <td>Geben Sie einen Namen für die Erinnerungsbenachrichtigung an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wartezeit</td> 
      <td> <p>Geben Sie die Anzahl der Stunden, Arbeitstage, Tage (Kalendertage), Wochen oder Monate vor oder nach dem Datum in der <strong>Zeit</strong> -Feld.</p> <p><b>NOTE</b>:  
        <ul> 
         <li> <p>Erinnerungsbenachrichtigungen beginnen 24 Stunden nach dem angegebenen Datum und sobald alle Kriterien erfüllt sind.</p> </li> 
         <li> <p>Erinnerungsbenachrichtigungen für Projekte, Aufgaben und Ausgaben jeden Abend um Mitternacht, US Mountain Time, Trigger. Alle Objekte, die ab diesem Trigger für eine Erinnerungsbenachrichtigung qualifiziert sind, erhalten eine Benachrichtigung an die vorgesehenen Benutzer kurz danach.</p> </li> 
         <li> <p>Erinnerungsbenachrichtigungen für Timesheets werden zum angegebenen Zeitpunkt gesendet, basierend auf Ihrer Zeitzone und dem Enddatum, Startdatum oder letzten Aktualisierungsdatum des Timesheets.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Wählen Sie das Ereignis aus, das die geplante Erinnerungsbenachrichtigung Trigger.</p> <p>Wenn die Erinnerungsbenachrichtigung für Projekte, Aufgaben oder Probleme bestimmt ist, beziehen sich die verfügbaren Optionen auf das Abschlussdatum oder das Startdatum. Die Erinnerungsbenachrichtigung berücksichtigt den Zeitstempel des Abschlusses und Beginndatums von Projekten, Aufgaben und Problemen.</p>

   <p>Wenn die Erinnerungsbenachrichtigung für Timesheets bestimmt ist, beziehen sich die verfügbaren Optionen auf das Enddatum, das Startdatum oder das Datum der letzten Aktualisierung. Bei der Erinnerungsbenachrichtigung für Timesheets wird der Zeitstempel des Enddatums, des Starts und des letzten Aktualisierungsdatums berücksichtigt. Das Datenblatt beginnt um Mitternacht am Tag des Startdatums (12:00 Uhr) und endet direkt vor Mitternacht am Enddatum (23:59 Uhr).</p>

   <p><b>NOTIZ</b></p>
      <p>Erinnerungsbenachrichtigungen werden nur einmal alle 24 Stunden verteilt.</p> <p>Wenn Sie innerhalb von 24 Stunden mehrere Erinnerungsbenachrichtigungen einrichten, sendet Workfront eine Benachrichtigungs-E-Mail mit allen in dieser Benachrichtigung enthaltenen Erinnerungen.</p>
      <p>Wenn Sie beispielsweise drei Erinnerungsbenachrichtigungen für Trigger 10 Stunden vor, 2 Stunden vor und 1 Stunde vor dem Fälligkeitsdatum konfigurieren, werden die drei Erinnerungen alle in derselben Benachrichtigung zusammengefasst, wenn sie am selben Tag stattfinden.</p> <p>Wenn Sie jedoch eine Erinnerungsbenachrichtigung für 26 Stunden vor und eine weitere für 1 Stunde vor dem Fälligkeitsdatum festlegen, erhalten Benutzer zwei separate Benachrichtigungen. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kriterien</td> 
      <td> <p>Wählen Sie die Kriterien aus, um die Erinnerungsbenachrichtigung für die Planung zu qualifizieren. Erinnerungsbenachrichtigungen werden nur geplant, wenn die Kriterienauswahl erfüllt ist.</p> <p>Je nach dem in Schritt 4 ausgewählten Objekttyp stehen die folgenden Kriterienoptionen zur Verfügung:</p> 
       <ul> 
        <li><strong>In aktuellen Projekten unvollständig:</strong> <i>(Verfügbar für Aufgaben- und Problemerinnerungen)</i> Die Erinnerungsbenachrichtigung wird nur dann gesendet, wenn der Objektstatus, mit dem die Erinnerungsbenachrichtigung verknüpft ist, nicht abgeschlossen ist und der Projektstatus "Aktuell" lautet.</li> 
        <li><strong>Alle in aktuellen Projekten:</strong> <i>(Verfügbar für Aufgaben- und Problemerinnerungen)</i> Die Erinnerungsbenachrichtigung soll unabhängig vom Objektstatus und nur dann gesendet werden, wenn der Projektstatus, mit dem die Erinnerungsbenachrichtigung verknüpft ist, aktuell ist.</li> 
        <li><strong>Unvollständige Projekte:</strong> <i>(Verfügbar für Erinnerungen an Projekte)</i> Die Erinnerungsbenachrichtigung soll gesendet werden, wenn der Projektstatus etwas Anderes als "Abgeschlossen"ist.</li> 
        <li><strong>Alle Projekte:</strong> <i>(Verfügbar für Erinnerungen an Projekte)</i> Die Erinnerungsbenachrichtigung soll unabhängig vom Projektstatus gesendet werden.</li> 
        <li><strong>Öffnen Sie Timesheets:</strong> <i>(Verfügbar für Zeitblatt-Erinnerungen)</i> Die Erinnerungsbenachrichtigung wird geplant, wenn der Status des Zeitblatts "Open"lautet.</li> 
        <li><strong>Gesendete Timesheets:</strong> <i>(Verfügbar für Zeitblatt-Erinnerungen)</i> Die Erinnerungsbenachrichtigung wird geplant, wenn der Status des Zeitblatts übermittelt wird.</li> 
        <li><strong>Öffnen Sie das Datenblatt oder unter 40 Stunden pro Woche:</strong> <i>(Verfügbar für Zeitblatt-Erinnerungen)</i> Die Erinnerungsbenachrichtigung wird terminiert, wenn der Status des Timesheets "Open"lautet oder wenn das Timesheet weniger als 40 Stunden protokolliert wurde.</li> 
        <li><strong>E-Mail-Vorlage:</strong> Wählen Sie aus der Dropdown-Liste eine E-Mail-Vorlage aus, die an Ihre Erinnerung angehängt werden soll.<br>Informationen zum Erstellen einer E-Mail-Vorlage finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">E-Mail-Vorlagen konfigurieren</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empfängerinnen und Empfänger</td> 
      <td><p>Je nachdem, für welches Objekt die Erinnerungsbenachrichtigung bestimmt ist, wählen Sie aus den folgenden Typen von Benutzern aus, die die Benachrichtigung erhalten sollen:</p>
      <ul>
      <li>Zugewiesen an</li>
      <li>Eingegeben von</li>
      <li>Projektteam (alle Benutzer im Projektteam erhalten die Erinnerung)</li>
      <li>Abhängige Aufgabenzuweisungen (Benutzer, die abhängigen Aufgaben zugewiesen sind, erhalten die Erinnerung)</li>
      <li>Projektbesitzer</li>
      <li>Zugeordneter Benutzer (Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind, erhalten die Erinnerung)</li>
      <li>Arbeitszeittabellen-Besitzer</li>
      <li>Person, die Arbeitszeittabellen genehmigt</li>
      <li>Vorgesetzter des Arbeitszeittabellen-Besitzers</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
1. Hängen Sie die Erinnerungsbenachrichtigung an ein Arbeitselement an, wie unter [Erinnerungsbenachrichtigung an ein Objekt anhängen](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Benachrichtigung zur Erinnerung empfangen

Wenn die Bedingung für das Element erfüllt ist, an das die Erinnerungsbenachrichtigung angehängt ist, wird eine E-Mail-Benachrichtigung an den in der Erinnerungsbenachrichtigung definierten Benutzer ausgelöst.

Weitere Informationen zum Empfang von Erinnerungsbenachrichtigungen finden Sie im Abschnitt [Erinnerungsbenachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) Abschnitt in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md).

## Benachrichtigungsversand von Test-Erinnerungen

Erinnerungsbenachrichtigungen Trigger jede Nacht um Mitternacht, Mountain Time. Alle Objekte, die für eine Erinnerungsbenachrichtigung qualifiziert sind, senden kurz darauf eine Benachrichtigung an die vorgesehenen Trigger.

Damit Erinnerungsbenachrichtigungen manuell an den Trigger gesendet werden, muss zunächst die Bedingung für die Erinnerung erfüllt sein.\
Wenn eine Erinnerung beispielsweise eine Stunde nach dem geplanten Abschlussdatum eines Projekts auf den Trigger gesetzt wird, muss diese Zeit zwischen dem Zeitpunkt der Erinnerung und dem Zeitpunkt verstrichen sein. Bei Projekten, bei denen die geplanten Fertigstellungsdaten vor der Aktivierung der Erinnerung vergangen waren, wird keine Benachrichtigung Trigger.

So führen Sie eine Erinnerungsbenachrichtigung manuell zum Trigger durch:

{{step-1-to-setup}}

1. Klicks **System** > **Diagnose** in der linken unteren Ecke von Workfront.

1. Klicks **Erinnerungsbenachrichtigungen senden** und warten Sie auf die Bestätigung oben auf dem Bildschirm, dass sie gesendet wurden.

   Die in der Erinnerungsbenachrichtigung angegebenen Benutzer erhalten eine E-Mail.

![](assets/reminder-test.png)