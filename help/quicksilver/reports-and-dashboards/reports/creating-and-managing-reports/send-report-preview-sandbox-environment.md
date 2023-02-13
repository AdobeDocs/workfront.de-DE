---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Bericht in der Vorschau-Sandbox-Umgebung senden
description: Die Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in den Umgebungen "Vorschau"und "Benutzerdefinierte Sandbox-Aktualisierung"verfügbar sind. Diese Funktion ist nicht in der Produktionsumgebung verfügbar.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Bericht in der Vorschau-Sandbox-Umgebung senden

Die Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in den Umgebungen &quot;Vorschau&quot;und &quot;Benutzerdefinierte Sandbox-Aktualisierung&quot;verfügbar sind. Diese Funktion ist nicht in der Produktionsumgebung verfügbar.

Sie können in jeder Adobe Workfront-Testumgebung Berichtsbereitstellungsoptionen einrichten.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Während die Testumgebungen so nah wie möglich an Ihrer Produktionsumgebung funktionieren sollen, unterscheiden sich einige Funktionen von Ihrer Produktionsumgebung.

Sie können Berichte in den Testumgebungen planen, die Art ihrer Bereitstellung unterscheidet sich jedoch von der Bereitstellung in der Produktionsumgebung.

Informationen zum Planen von Berichten für die Bereitstellung in der Produktionsumgebung finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Je nachdem, wo Sie die Berichte planen, unterscheidet sich die Bereitstellungsfunktion zwischen den Sandboxes Vorschau und Benutzerdefinierte Aktualisierung .

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Planen von Berichten in der Vorschau-Umgebung

* [Planen von Berichten in der Vorschau-Umgebung](#schedule-reports-in-the-preview-environment)

### Planen von Berichten in der Vorschau-Umgebung

Ob ein bereitgestellter Bericht in der Vorschau-Umgebung erstellt wird oder nicht, hängt davon ab, ob **Empfangen von E-Mails aus dieser Testumgebung** aktiviert ist oder nicht.

Informationen zum Aktivieren von E-Mails aus der Sandbox-Umgebung finden Sie unter [Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Die Planung von Berichten zur Bereitstellung in der Vorschau-Umgebung entspricht der Planung von Berichten in der Produktionsumgebung. Weitere Informationen zum Planen eines Berichts für die Bereitstellung finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wenn Sie einen Bericht für die Bereitstellung in der Vorschau-Umgebung planen, gibt es die folgenden Szenarien:

* Wann **Empfangen von E-Mails aus dieser Testumgebung** für den Benutzer deaktiviert ist, der den Bericht erhält, wird bei der Versandplanung des Berichts keine Datei erzeugt.
* Wann **Empfangen von E-Mails aus dieser Testumgebung** für den Benutzer aktiviert ist, der den Bericht erhält, wird die Datei, die bei der Versandplanung des Berichts erstellt wird, im Tab Dokumente des Benutzers hinzugefügt.

## Berichte in der Umgebung der benutzerdefinierten Aktualisierungs-Sandbox planen

Ob ein bereitgestellter Bericht in der Sandbox für benutzerdefinierte Aktualisierung erstellt wird, hängt davon ab, ob die Einstellung E-Mails von dieser Testumgebung empfangen aktiviert ist oder nicht.

Informationen zum Aktivieren von E-Mails aus der Vorschau-Umgebung finden Sie im Abschnitt . [E-Mail-Benachrichtigungseinstellungen anzeigen und ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) im Artikel [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Die Terminierung von Berichten für die Bereitstellung in der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen ist mit der Planung von Berichten in der Produktionsumgebung identisch. Weitere Informationen zum Planen eines Berichts für die Bereitstellung finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wenn Sie einen Bericht für die Bereitstellung in der Sandbox-Umgebung für benutzerdefinierte Aktualisierung planen, gibt es die folgenden Szenarien:

* Wenn die Option E-Mails aus dieser Testumgebung empfangen für den Benutzer, der den Bericht erhält, deaktiviert ist, wird bei der Versandplanung des Berichts keine Datei erzeugt.
* Wenn die Option E-Mails von dieser Testumgebung empfangen für den Benutzer aktiviert ist, der den Bericht erhält, wird der Bericht per E-Mail als Anhang an die mit dem Benutzer verknüpfte E-Mail-Adresse gesendet.

## Benachrichtigung externer Benutzer

Externe Benutzer erhalten weder Berichte, die von den Workfront-Testumgebungen gesendet werden, noch eine E-Mail-Benachrichtigung.

Externe Benutzer erhalten nur Berichte per E-Mail, wenn sie aus einer Produktionsumgebung bereitgestellt werden.
