---
title: Erinnerungsnachrichten einrichten
description: Erinnerungsbenachrichtigungen generieren E-Mails, die an Benutzer basierend auf angegebenen Kriterien gesendet werden. Erinnerungsbenachrichtigungen erinnern Benutzer an eine Aktion, die sie für eine Aufgabe, ein Problem, ein Projekt oder eine Arbeitszeittabelle ausführen müssen.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 2%

---

# Einrichten von Erinnerungsbenachrichtigungen

<!-- Audited: 1/2024 -->

Als Workfront-Admin können Sie Erinnerungsbenachrichtigungen für Benutzende erstellen und sie mit Objekten verknüpfen, auf die Ihre Benutzenden besondere Aufmerksamkeit richten sollen.

Erinnerungsbenachrichtigungen generieren E-Mails, die an Benutzer basierend auf angegebenen Kriterien gesendet werden. Erinnerungsbenachrichtigungen erinnern Benutzer an eine Aktion, die sie für eine Aufgabe, ein Problem, ein Projekt oder eine Arbeitszeittabelle ausführen müssen.

Nachdem Sie die Erinnerungsbenachrichtigungen erstellt haben, können Benutzer sie manuell mit Arbeitselementen wie Projekten, Aufgaben, Problemen und Arbeitszeittabellen verknüpfen. Weitere Informationen finden Sie unter [Erinnerungsnachricht an ein Objekt anhängen](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Planer oder höher mit administrativem Zugriff auf Erinnerungsnachrichten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-Mail-Erinnerung anpassen

Sie können den Betreff, den Textkörper und das HTML in der E-Mail mit der Erinnerungsbenachrichtigung anpassen.

Sie können auch die in der Erinnerungsnachricht enthaltene Standard-E-Mail verwenden. Die standardmäßige E-Mail verwendet den Namen der Erinnerungsbenachrichtigung als E-Mail-Betreff und den Objektnamen im E-Mail-Textkörper, einschließlich des Ereignisses, das die Benachrichtigung ausgelöst hat.

Wenn Sie die Erinnerungs-E-Mail anpassen möchten, müssen Sie eine E-Mail-Vorlage erstellen und sie an die Erinnerungsbenachrichtigung anhängen.

Informationen zum Erstellen einer E-Mail-Vorlage finden Sie unter [Konfigurieren von E-Mail-Vorlagen](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Erinnerungsnachricht erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **E** > **Benachrichtigungen** > **Erinnerungsbenachrichtigungen**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Klicken Sie **Neue Erinnerungsnachricht**.

1. Klicken Sie in der Dropdown-Liste auf den Objekttyp, den Sie mit der Erinnerungsbenachrichtigung verknüpfen möchten.

   Wenn Sie beispielsweise eine Erinnerungsnachricht an eine Arbeitszeittabelle anhängen möchten, klicken Sie auf **Arbeitszeittabelle**.

1. Geben **im angezeigten** „Neue Erinnerungsnachricht“ die folgenden Informationen an.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name der Erinnerungsbenachrichtigung</td> 
      <td>Geben Sie einen Namen für die Erinnerungsnachricht an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wartezeit</td> 
      <td> <p>Geben Sie die Anzahl der Stunden, Arbeitstage, Tage (Kalendertage), Wochen oder Monate vor oder nach dem Datum im Feld <strong>Timing</strong> an.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li> <p>Erinnerungsbenachrichtigungen beginnen 24 Stunden nach dem angegebenen Datum und sobald alle Kriterien erfüllt sind.</p> </li> 
         <li> <p>Erinnerungsbenachrichtigungen für Projekte, Aufgaben und Probleme Trigger jeden Abend um Mitternacht, US Mountain Time. Alle Objekte, die ab diesem Tag für eine Erinnerungsbenachrichtigung qualifiziert sind, erhalten kurz nach diesem Trigger eine Benachrichtigung an die angegebenen Benutzenden.</p> </li> 
         <li> <p>Erinnerungsbenachrichtigungen für Arbeitszeittabellen werden zum angegebenen Zeitpunkt gesendet, basierend auf Ihrer Zeitzone und dem Enddatum, Startdatum oder letzten Aktualisierungsdatum der Arbeitszeittabelle.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Trigger Wählen Sie das Ereignis aus, für das die Erinnerungsbenachrichtigung geplant werden soll.</p> <p>Wenn die Erinnerungsnachricht für Projekte, Aufgaben oder Probleme vorgesehen ist, beziehen sich die verfügbaren Optionen auf das Fertigstellungs- oder Startdatum. Die Erinnerungsnachricht berücksichtigt den Zeitstempel von Abschluss- und Startdatum von Projekten, Aufgaben und Problemen.</p>

   <p>Wenn die Erinnerungsnachricht für Arbeitszeittabellen vorgesehen ist, beziehen sich die verfügbaren Optionen auf das Enddatum, das Startdatum oder das Datum der letzten Aktualisierung. Die Erinnerungsbenachrichtigung für Arbeitszeittabellen berücksichtigt den Zeitstempel der Arbeitszeittabellen-Enddatum, -Start und -Datum der letzten Aktualisierung. Die Arbeitszeittabelle beginnt um Mitternacht am Tag des Startdatums (12:00 Uhr) und endet direkt vor Mitternacht am Enddatum (23:59 Uhr).</p>

   <p><b>NOTIZ</b></p>
      <p>Erinnerungsbenachrichtigungen zu Arbeitszeittabellen werden nur einmal alle 24 Stunden verteilt.</p> <p>Wenn Sie innerhalb eines Zeitraums von 24 Stunden mehrere Erinnerungsbenachrichtigungen eingerichtet haben, sendet Workfront eine Benachrichtigungs-E-Mail mit allen in dieser Benachrichtigung enthaltenen Erinnerungen.</p>
      <p>Wenn Sie beispielsweise drei Erinnerungsbenachrichtigungen so konfigurieren, dass sie 10 Stunden vor, 2 Stunden vor und 1 Stunde vor einem Fälligkeitsdatum an den Trigger gesendet werden, werden alle drei Erinnerungen in derselben Benachrichtigung zusammengefasst, wenn sie am selben Tag gesendet werden.</p> <p>Wenn Sie jedoch eine Erinnerungsnachricht 26 Stunden vor und eine weitere eine Stunde vor einem Fälligkeitsdatum einstellen, erhalten Benutzerinnen und Benutzer zwei separate Benachrichtigungen. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kriterien</td> 
      <td> <p>Wählen Sie die Kriterien aus, um die Erinnerungsnachricht als geplant festzulegen. Erinnerungsnachrichten sind nur geplant, wenn die Kriterienauswahl erfüllt ist.</p> <p>Die folgenden Kriterienoptionen sind je nach dem Objekttyp verfügbar, den Sie in Schritt 4 ausgewählt haben:</p> 
       <ul> 
        <li><strong>Unvollständig in aktuellen Projekten:</strong> <i> (Verfügbar für Aufgaben- und Problemerinnerungen)</i> Die Erinnerungsbenachrichtigung ist so geplant, dass sie nur gesendet wird, wenn der Objektstatus, mit dem die Erinnerungsbenachrichtigung verknüpft ist, nicht abgeschlossen ist und der Projektstatus „Aktuell“ ist.</li> 
        <li><strong>Alle in aktuellen Projekten:</strong> <i>(Verfügbar für Aufgaben- und Problemerinnerungen)</i> Die Erinnerungsbenachrichtigung ist so geplant, dass sie unabhängig vom Objektstatus gesendet wird, und nur dann, wenn der Projektstatus, mit dem die Erinnerungsbenachrichtigung verknüpft ist, „Aktuell“ ist.</li> 
        <li><strong>Unvollständige Projekte:</strong> <i>(Verfügbar für Projekterinnerungen)</i> Die Erinnerungsbenachrichtigung wird planmäßig gesendet, wenn der Projektstatus alles andere als vollständig ist.</li> 
        <li><strong>Alle Projekte:</strong> <i>(Verfügbar für Projekterinnerungen)</i> Die Erinnerungsbenachrichtigung ist unabhängig vom Projektstatus so geplant, dass sie gesendet wird.</li> 
        <li><strong>Offene Arbeitszeittabellen:</strong> <i>(Verfügbar für Arbeitszeittabellen-Erinnerungen)</i> Die Erinnerungsbenachrichtigung ist so geplant, dass sie gesendet wird, wenn der Arbeitszeittabellen-Status „Offen“ lautet.</li> 
        <li><strong>Übermittelte Arbeitszeittabellen:</strong> <i>(Verfügbar für Arbeitszeittabellen-Erinnerungen)</i> Die Erinnerungsbenachrichtigung ist so geplant, dass sie gesendet wird, wenn der Arbeitszeittabellen-Status übermittelt wird.</li> 
        <li><strong>Offene Arbeitszeittabelle oder weniger als 40 Stunden pro Woche:</strong> <i>(Verfügbar für Arbeitszeittabellen-Erinnerungen)</i> Die Erinnerungsbenachrichtigung wird planmäßig gesendet, wenn der Arbeitszeittabellen-Status „Offen“ ist oder wenn die Arbeitszeittabelle weniger als 40 Stunden protokolliert hat.</li> 
        <li><strong>E-Mail-Vorlage</strong> Wählen Sie aus der Dropdown-Liste eine E-Mail-Vorlage aus, die Ihrer Erinnerung angehängt werden soll.<br>Informationen zum Erstellen einer E-Mail-Vorlage finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref"> von E-Mail-Vorlagen</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empfängerinnen und Empfänger</td> 
      <td><p>Wählen Sie je nachdem, für welches Objekt die Erinnerungsnachricht bestimmt ist, unter den folgenden Benutzertypen die Benachrichtigung aus:</p>
      <ul>
      <li>Zugewiesen an</li>
      <li>Eingegeben von</li>
      <li>Projektteam (alle Benutzer im Projektteam erhalten die Erinnerung)</li>
      <li>Abhängige Aufgabe - Verantwortliche (Benutzer, denen abhängige Aufgaben zugewiesen sind, erhalten die Erinnerung)</li>
      <li>Projektbesitzer</li>
      <li>Zugewiesen an (Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind, erhalten die Erinnerung)</li>
      <li>Arbeitszeittabellen-Besitzer</li>
      <li>Person, die Arbeitszeittabellen genehmigt</li>
      <li>Vorgesetzter des Arbeitszeittabellen-Besitzers</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
1. Hängen Sie die Erinnerungsbenachrichtigung an ein Arbeitselement an, wie in [Erinnerungsbenachrichtigung an ein Objekt anfügen](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md) beschrieben.

## Erhalten einer Erinnerungsnachricht

Wenn die Bedingung für das Element erfüllt ist, an das die Erinnerungsbenachrichtigung angehängt ist, wird eine E-Mail-Benachrichtigung an den in der Erinnerungsbenachrichtigung definierten Benutzer ausgelöst.

Weitere Informationen zum Empfang von Erinnerungsbenachrichtigungen finden Sie [ Abschnitt „Erinnerungsbenachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) in [Adobe Workfront-](../../../workfront-basics/using-notifications/wf-notifications.md).

## Versand der Testerinnerungsnachricht

Erinnerungsnachrichten Trigger jeden Abend um Mitternacht, Mountain Time. Alle Objekte, die für den Trigger „Erinnerungsbenachrichtigung“ qualifiziert sind, erhalten kurz danach eine Benachrichtigung an die benannten Benutzenden.

Damit Erinnerungsnachrichten manuell an Trigger gesendet werden, muss zunächst die Bedingung für die Erinnerung erfüllt sein.\
Wenn beispielsweise eine Erinnerung eine Stunde nach dem geplanten Abschlussdatum eines Projekts auf &quot;Trigger&quot; gesetzt wird, muss diese Zeit zwischen dem Festlegen der Erinnerung und jetzt vergangen sein. Bei Projekten, bei denen die geplanten Abschlussdaten vor der Aktivierung der Erinnerung überschritten wurden, wird keine Benachrichtigung Trigger.

So führen Sie eine Erinnerungsnachricht manuell an den Trigger durch:

{{step-1-to-setup}}

1. Klicken Sie **System** > **Diagnostics** in der linken unteren Ecke von Workfront.

1. Klicken Sie **Erinnerungsnachrichten senden** und warten Sie auf die Bestätigung oben im Bildschirm, dass sie gesendet wurden.

   Die in der Erinnerungsnachricht angegebenen Benutzer erhalten eine E-Mail.

![](assets/reminder-test.png)