---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Einrichten automatischer Erinnerungen
description: Sie können automatische Erinnerungen einrichten, um Trigger-E-Mail-Benachrichtigungen zu senden, wenn alle Aufgaben oder Probleme fällig oder verspätet sind oder sich am geplanten Abschlussdatum befinden.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 8%

---

# Einrichten automatischer Erinnerungen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie automatische Erinnerungen einrichten, die E-Mail-Benachrichtigungen auslösen, wenn alle Aufgaben oder Probleme fällig sind, verspätet oder kurz vor dem geplanten Abschlussdatum liegen. Nachdem Sie diese Einstellungen konfiguriert haben, können Benutzer automatische Erinnerungen nicht mehr deaktivieren.

Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Eine automatische Erinnerung kann an eine oder mehrere der folgenden Adressen gesendet werden:

* Die einer Aufgabe oder einem Problem zugewiesenen Benutzer
* Der unmittelbare Manager des Benutzers
* Der Manager des direkten Managers

>[!NOTE]
>
>Sie können weder den Inhalt noch die Betreffzeile der E-Mail ändern, die von einer automatischen Erinnerung ausgelöst wird.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Einrichten automatischer Erinnerungen

{{step-1-to-setup}}

1. Klicken Sie auf **E** > **Automatische Erinnerungen**.

1. Wählen Sie im Bereich **Verspätete Benachrichtigung senden an** eine der folgenden Optionen aus:

   <table>
    <tr>
        <td>Der „Zugewiesen an“-Benutzer</td>
        <td>Wählen Sie diese Option, wenn der Benutzer, der einer Aufgabe oder einem Problem zugewiesen ist, eine verspätete Benachrichtigung über seine Arbeitsaufgabe erhalten soll, die verspätet ist.</td>
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

   Anzahl der Minuten, Stunden, Tage, Wochen oder Monate angeben, um Zeit zum geplanten Abschlussdatum der Aufgaben oder Probleme hinzuzufügen. Wählen Sie **Verstrichene Minuten**, **Verstrichene Stunden**, **Verstrichene Tage** oder **Verstrichene Wochen** aus, um Zeit hinzuzufügen, die alle Wochenenden, Feiertage und arbeitsfreien Stunden enthält, wie in Ihrem Zeitplan angegeben.

   Wenn ein Vorgang beispielsweise am Freitag zugewiesen ist und eine Dauer von 3 verstrichenen Tagen hat, wird das Abschlussdatum des Vorgangs auf Montag festgelegt (vorausgesetzt, Samstag und Sonntag sind ein Wochenende). Wenn der Vorgang eine Dauer von 3 Tagen hat (nicht verstrichen), wird das Abschlussdatum des Vorgangs auf Mittwoch festgelegt.

   ![Zeitinkremente](assets/time-increments-for-automatic-reminder.png)

1. Klicken Sie auf **Speichern**.

## Automatische Erinnerungen empfangen

Wenn Sie in einer automatischen Erinnerungsbenachrichtigung die angegebene Entität sind, erhalten Sie eine E-Mail, wenn die angegebene Frist eingehalten wird. Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist.

Aufgaben mit bestimmten Abhängigkeitstypen werden möglicherweise nach dem angegebenen Startdatum bereitgestellt, obwohl sie überfällig sind. Wenn eine Aufgabe beispielsweise einen Vorgänger mit einer FS-Abhängigkeit (Finish-Start) hat, wird sie nicht in die E-Mail aufgenommen, auch wenn sie das angegebene Startdatum überschritten hat, da Sie die Aufgabe erst starten können, wenn der Vorgänger abgeschlossen ist.

Weitere Informationen zum Empfang automatischer Erinnerungs-E-Mails finden Sie [ Abschnitt „Automatische ](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders)&quot; in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md).

## Automatische Erinnerungen senden

Automatische Erinnerungen werden gesendet, sobald die vom Workfront-Administrator festgelegte Zeit erreicht ist.

Wenn Sie das manuelle Senden der automatischen Erinnerungs-E-Mails auslösen möchten, können Sie dies mithilfe der Diagnose tun. Weitere Informationen zum Zugreifen auf und Verwenden von Diagnostics in Workfront finden Sie unter [Verwenden von Diagnostics zum Auslösen automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
