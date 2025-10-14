---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Einrichten automatischer Erinnerungen
description: Sie können automatische Erinnerungen einrichten, um Trigger-E-Mail-Benachrichtigungen zu senden, wenn alle Aufgaben oder Probleme fällig oder verspätet sind oder sich am geplanten Abschlussdatum befinden.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 3%

---

# Einrichten automatischer Erinnerungen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie automatische Erinnerungen einrichten, um E-Mail-Benachrichtigungen an Trigger zu senden, wenn alle Aufgaben oder Probleme fällig sind, sich verspäten oder fast zum geplanten Abschlussdatum liegen. Nach der Konfiguration dieser Einstellungen können Benutzer die automatischen Erinnerungen nicht mehr deaktivieren.

Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Eine automatische Erinnerung kann an eine oder mehrere der folgenden Adressen gesendet werden:

* Die einer Aufgabe oder einem Problem zugewiesenen Benutzer
* Der unmittelbare Manager des Benutzers
* Der Manager des direkten Managers

>[!NOTE]
>
>Sie können weder den Inhalt noch die Betreffzeile der E-Mail ändern, die von einer automatischen Erinnerung ausgelöst wird.

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Einrichten automatischer Erinnerungen

{{step-1-to-setup}}

1. Klicken Sie auf **E** > **Automatische Erinnerungen**.

1. Wählen Sie im Bereich **Verspätete Benachrichtigung senden an** eine der folgenden Optionen aus:

   <table>
    <tr>
        <td>Der „Zugewiesen an“-Benutzer</td>
        <td>Wählen Sie diese Option aus, wenn der/die Benutzende, der/die einer Aufgabe oder einem Problem zugewiesen wurde, eine verspätete Benachrichtigung über den Verzug seines/ihres Arbeitselements erhalten soll.</td>
        <td></td>
    </tr>
    <tr>
        <td>Den Manager des Benutzers</td>
        <td>Wählen Sie diese Option aus, wenn der Manager des Benutzers eine verspätete Benachrichtigung darüber erhalten soll, dass das Arbeitselement des direkt unterstellten Mitarbeiters verspätet ist.</td>
        <td></td>
    </tr>
    <tr>
        <td>Den Vorgesetzten des Managers</td>
        <td>Wählen Sie diese Option aus, wenn der Manager des direkten Managers eine verspätete Benachrichtigung über ein Arbeitselement erhalten soll, bei dem einer der direkt unterstellten Mitarbeiter zu spät kommt.</td>
        <td></td>
    </tr>
    <tr>
        <td>Der „Zugewiesen an“-Benutzer</td>
        <td>(Im Bereich <b>Erinnerungsnachricht senden an</b>) Wählen Sie diese Option aus, wenn der/die Benutzende, der/die einer Aufgabe oder einem Problem zugewiesen wurde, eine Benachrichtigung erhalten soll, dass sich das Arbeitsdatum der Aufgabe oder des Problems nähert.</td>
        <td></td>
    </tr>
   </table>

1. Wählen Sie die Zeit aus, zu der die automatische Erinnerung gesendet werden soll, indem Sie die Zeit vor oder nach dem Fälligkeitsdatum des Arbeitselements auswählen.

   Die Zeit wird ab dem geplanten Abschlussdatum der Aufgabe oder des Problems berechnet.

   Anzahl der Minuten, Stunden, Tage, Wochen oder Monate angeben, um Zeit zum geplanten Abschlussdatum der Aufgaben oder Probleme hinzuzufügen. Wählen Sie **Verstrichene Minuten**, **Verstrichene Stunden**, **Verstrichene Tage** oder **Verstrichene Wochen**, um die Zeit hinzuzufügen, die alle Wochenenden, Feiertage und arbeitsfreien Stunden umfasst, wie in Ihrem Zeitplan angegeben.

   Wenn beispielsweise eine Aufgabe am Freitag zugewiesen wurde und eine Dauer von 3 verstrichenen Tagen hat, wird das Abschlussdatum der Aufgabe auf Montag festgelegt (unter der Annahme, dass Samstag und Sonntag ein Wochenende ist). Wenn die Aufgabe eine Dauer von 3 Tagen hat (nicht abgelaufen), wird das Abschlussdatum der Aufgabe auf Mittwoch festgelegt.

   ![Zeitinkremente](assets/time-increments-for-automatic-reminder.png)

1. Klicken Sie auf **Speichern**.

## Automatische Erinnerungen empfangen

Wenn Sie in einer automatischen Erinnerungsbenachrichtigung die angegebene Entität sind, erhalten Sie eine E-Mail, wenn die angegebene Frist eingehalten wird. Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Aufgaben mit bestimmten Abhängigkeitstypen werden möglicherweise nach dem angegebenen Startdatum bereitgestellt, obwohl sie überfällig sind. Wenn eine Aufgabe beispielsweise einen Vorgänger mit einer FS-Abhängigkeit (Finish-Start) hat, wird sie nicht in die E-Mail aufgenommen, auch wenn sie das angegebene Startdatum überschritten hat, da Sie die Aufgabe erst starten können, wenn der Vorgänger abgeschlossen ist.

Weitere Informationen zum Empfang automatischer Erinnerungs-E-Mails finden Sie [&#x200B; Abschnitt „Automatische &#x200B;](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders)&quot; in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md).

## Automatische Erinnerungen senden

Automatische Erinnerungen werden gesendet, sobald die vom Workfront-Administrator festgelegte Zeit erreicht ist.

Wenn Sie Trigger beim manuellen Versand der automatischen Erinnerungs-E-Mails haben möchten, können Sie dies mithilfe von Diagnostics tun. Weitere Informationen zum Zugriff auf und zur Verwendung von Diagnoseprogrammen in Workfront finden Sie unter [Verwenden von Diagnoseprogrammen zum Trigger automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
