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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sxv8RUKwTr-SABLfOrmTa0J9ToM62-1tF5rFEnu41UI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f283a5f64062e5878373527de46b0d993b545ba7
workflow-type: tm+mt
source-wordcount: 836
ht-degree: 6%

---

# Einrichten automatischer Erinnerungen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie automatische Erinnerungen einrichten, um E-Mail-Benachrichtigungen an Trigger zu senden, wenn alle Aufgaben, Probleme oder anderen zugewiesenen Arbeitselemente fällig oder verspätet sind oder sich am geplanten Abschlussdatum befinden.

Nach der Konfiguration dieser Einstellungen können Benutzer die automatischen Erinnerungen nicht mehr deaktivieren. Automatische Erinnerungen werden unabhängig von den Benachrichtigungseinstellungen eines Benutzers im Bereich Meine Einstellungen gesendet.

Bei verspäteten Benachrichtigungen wird die E-Mail jede Nacht gesendet, bis die Aufgabe oder das Problem abgeschlossen ist. Das bedeutet, dass der/die Benutzende jeden Tag eine Benachrichtigung erhält, solange die Aufgabe oder das Problem nicht abgeschlossen ist.

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

## Details der automatischen Erinnerungsfunktion

### Unterschied zu anderen Erinnerungsarten

Automatische Erinnerungen sind die Erinnerungsfunktion auf Einrichtungsebene für Workfront-Aufgaben und -Probleme und sind von der Erinnerungsfunktion auf Objektebene getrennt. Informationen zum Unterschied zwischen automatischen Erinnerungen und Erinnerungsbenachrichtigungen finden Sie unter [Automatische Erinnerungen vs. Erinnerungsbenachrichtigungen](/help/quicksilver/administration-and-setup/tips-tricks-and-troubleshooting/auto-reminders-vs-reminder-notifications.md).

Korrekturabzugs- und Korrekturabzugsentscheidungen werden auch nicht durch automatische Erinnerungen verarbeitet und folgen einem separaten Erinnerungsvorgang. Weitere Informationen zu Proofing und Erinnerungen an Korrekturabzugsentscheidungen finden Sie in den Artikeln unter [Benachrichtigungen und Erinnerungen zu Korrekturabzügen](/help/quicksilver/workfront-proof/wp-emailsntfctns/wp-emails-and-notifications.md).

## Überlegungen zur Verwendung automatischer Erinnerungen

Beachten Sie bei der Verwendung automatischer Erinnerungen Folgendes:

* Überfällige E-Mails werden als eine Auswahl-E-Mail pro Empfänger und Tag und nicht als separate E-Mails pro Element gesendet.
* Das Aktivieren automatischer Erinnerungen kann dazu führen, dass Probleme oder Aufgaben, die bereits überfällig sind, in der nächsten überfälligen Auswahl-E-Mail angezeigt werden, unabhängig davon, wie lange das Element überfällig ist.
* Erinnerungen gelten nur für Projekte mit dem Status „Aktuell/Aktiv“.
* „Tage“ bei der automatischen Erinnerungseinrichtung beziehen sich auf planbare Geschäftstage, nicht auf verstrichene Tage oder Kalenderzeiten.



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
