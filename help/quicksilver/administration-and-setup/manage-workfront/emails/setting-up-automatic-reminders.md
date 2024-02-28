---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Einrichten automatischer Erinnerungen
description: Einrichten automatischer Erinnerungen
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 4%

---

# Einrichten automatischer Erinnerungen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie automatische Erinnerungen an Trigger-E-Mail-Benachrichtigungen einrichten, wenn alle Aufgaben oder Probleme fällig, spät oder in der Nähe des geplanten Fertigstellungsdatums sind. Nach der Konfiguration dieser Einstellungen können Benutzer automatische Erinnerungen nicht deaktivieren.

Bei verspäteten Benachrichtigungen wird die E-Mail nächtlich gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Eine automatische Erinnerung kann an eine oder mehrere der folgenden Aktionen gesendet werden:

* Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind
* Der sofortige Manager des Benutzers
* Der Manager des unmittelbaren Geschäftsführers

>[!NOTE]
>
>Sie können den Inhalt oder die Betreffzeile der E-Mail, die durch eine automatische Erinnerung ausgelöst wird, nicht ändern.

## Zugriffsanforderungen

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Einrichten automatischer Erinnerungen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **Email** >**Automatische Erinnerungen**.

1. Im **Verspätete Benachrichtigung an senden** eine der folgenden Optionen auswählen:

   <table>
    <tr>
        <td>Der Benutzer "Zugeordnet nach"</td>
        <td>Wählen Sie diese Option aus, wenn der Benutzer, der einer Aufgabe oder einem Problem zugewiesen ist, eine verspätete Benachrichtigung über das Arbeitselement erhalten soll.</td>
        <td></td>
    </tr>
    <tr>
        <td>Den Manager des Benutzers</td>
        <td>Wählen Sie diese Option aus, wenn der Manager des Benutzers eine verspätete Benachrichtigung erhalten soll, dass das Arbeitselement seines direkt unterstellten Mitarbeiters verspätet ist.</td>
        <td></td>
    </tr>
    <tr>
        <td>Den Vorgesetzten des Managers</td>
        <td>Wählen Sie diese Option aus, wenn Sie möchten, dass der Manager des unmittelbaren Managers eine verspätete Benachrichtigung über ein Arbeitselement eines Benutzers im direkten Bericht erhält.</td>
        <td></td>
    </tr>
    <tr>
        <td>Der Benutzer "Zugeordnet nach"</td>
        <td>(Im <b>Terminerinnerung senden an</b> Bereich.) Wählen Sie diese Option aus, wenn der Benutzer, der einer Aufgabe oder einem Problem zugewiesen ist, eine Benachrichtigung über sein Arbeitselement erhalten soll, die sich dem Fälligkeitsdatum nähert.</td>
        <td></td>
    </tr>
</table>

1. Wählen Sie den Zeitpunkt für den automatischen Versand der Erinnerung aus, indem Sie die Zeit vor oder nach dem Fälligkeitsdatum des Arbeitselements auswählen.

   Die Zeit wird ausgehend vom geplanten Abschlussdatum der Aufgabe oder des Problems berechnet.

   Geben Sie die Anzahl der Minuten, Stunden, Tage, Wochen oder Monate an, um dem geplanten Abschlussdatum der Aufgaben oder Probleme Zeit hinzuzufügen. Auswählen **Vergangene Minuten**, **Verstrichene Stunden**, **Vergangene Tage** oder **Verstrichene Wochen** um Zeit hinzuzufügen, die wie in Ihrem Zeitplan angegeben Wochenenden, Feiertage und Arbeitsstunden umfasst.

   Wenn beispielsweise eine Aufgabe am Freitag zugewiesen wird und eine Dauer von 3 verstrichenen Tagen hat, wird das Datum für die Aufgabenfertigstellung auf Montag gesetzt (vorausgesetzt Samstag und Sonntag sind Wochenende). Wenn die Aufgabe eine Dauer von 3 Tagen hat (nicht verstrichen), wird das Datum für den Abschluss der Aufgabe auf Mittwoch festgelegt.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Klicken Sie auf **Speichern**.

## Automatische Erinnerungen empfangen

Wenn Sie in einer Benachrichtigung zur automatischen Erinnerung als bestimmte Entität ausgewählt wurden, erhalten Sie eine E-Mail, sobald der angegebene Termin erreicht ist. Bei verspäteten Benachrichtigungen wird die E-Mail nächtlich gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Aufgaben mit bestimmten Abhängigkeitstypen können nach dem angegebenen Startdatum bereitgestellt werden, auch wenn sie überfällig sind. Wenn eine Aufgabe beispielsweise über einen Vorgänger mit der Abhängigkeit &quot;Finish-Start&quot;(fs) verfügt, wird sie auch dann nicht in die E-Mail aufgenommen, wenn sie das angegebene Startdatum überschritten hat, da Sie die Aufgabe erst starten können, wenn der Vorgänger abgeschlossen ist.

Weitere Informationen zum Empfang automatischer Reminders-E-Mails finden Sie im [Automatische Erinnerungen](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) Abschnitt in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md).

## Automatische Erinnerungen senden

Automatische Erinnerungen werden gesendet, sobald die vom Workfront-Administrator ausgewählte Zeit abgelaufen ist.

Wenn Sie Trigger beim manuellen Versand der automatischen Erinnerungsnachrichten haben möchten, können Sie dies mithilfe von Diagnostics tun. Weitere Informationen zum Zugriff auf und zur Verwendung von Diagnose in Workfront finden Sie unter [Verwenden der Diagnose für den Trigger automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
