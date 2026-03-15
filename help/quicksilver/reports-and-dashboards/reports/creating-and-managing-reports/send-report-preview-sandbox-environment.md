---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Senden eines Berichts in der Sandbox-Umgebung in der Vorschau
description: Die Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in den Umgebungen Vorschau und Benutzerdefinierte Sandbox-Aktualisierung verfügbar sind. Diese Funktion ist in der Produktionsumgebung nicht verfügbar.
author: Courtney
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 9%

---

# Senden eines Berichts in der Sandbox-Umgebung in der Vorschau

<!-- Audited: 11/2024 -->

Die Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in der Vorschau und in benutzerdefinierten Sandbox-Aktualisierungsumgebungen verfügbar sind. Diese Funktion ist in der Produktionsumgebung nicht verfügbar.

Sie können Optionen für die Berichtsbereitstellung in jeder Adobe Workfront-Testumgebung einrichten.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Während die Testumgebungen so eng wie möglich an Ihre Produktionsumgebung angebunden sind, unterscheiden sich einige Funktionen von Ihrer Produktionsumgebung.

Sie können Berichte in den Testumgebungen planen, deren Bereitstellung sich jedoch von der Art der Bereitstellung in der Produktionsumgebung unterscheidet.

Informationen zum Planen von Berichten für die Bereitstellung in der Produktionsumgebung finden Sie unter [Übersicht über die Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Je nachdem, wo Sie die Berichte planen, unterscheidet sich die Bereitstellungsfunktionalität zwischen den Sandboxes &quot;Vorschau&quot; und &quot;Benutzerdefinierte Aktualisierung&quot;.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Abo</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p>
   <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
     <td> <p>Berechtigungen für einen Bericht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Berichte in der Vorschau-Umgebung planen

* [Berichte in der Vorschau-Umgebung planen](#schedule-reports-in-the-preview-environment)

### Berichte in der Vorschau-Umgebung planen

Ob ein zugestellter Bericht in der Vorschau-Umgebung erstellt wird oder nicht, hängt davon ab, ob **E-Mails von dieser Testumgebung empfangen** aktiviert ist oder nicht.

Weitere Informationen zum Aktivieren von E-Mails aus der Sandbox-Umgebung finden Sie unter [Senden von E-Mails aus der Vorschau-Sandbox-Umgebung aktivieren](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![E-Mails von Sandbox-Option empfangen](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Die Planung von Berichten für die Bereitstellung in der Preview-Umgebung ist identisch mit der Planung von Berichten in der Produktionsumgebung. Informationen zum Planen eines Berichts für die Bereitstellung finden Sie unter [Übersicht zur Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wenn Sie einen Bericht für die Bereitstellung in der Preview-Umgebung planen, gibt es die folgenden Szenarien:

* Wenn **E-Mails aus dieser Testumgebung empfangen** für den Benutzer deaktiviert ist, der den Bericht erhält, wird beim Planen der Übermittlung des Berichts keine Datei erstellt.
* Wenn **E-Mails aus dieser Testumgebung empfangen** für den Benutzer aktiviert ist, der den Bericht erhält, wird die Datei, die beim Planen des Berichts für die Übermittlung erstellt wird, auf der Registerkarte Dokumente des Benutzers hinzugefügt.

## Planen von Berichten in der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen

Ob ein bereitgestellter Bericht in der benutzerdefinierten Aktualisierungs-Sandbox erstellt wird oder nicht, hängt davon ab, ob die Einstellung E-Mails von dieser Testumgebung empfangen aktiviert ist oder nicht.

Informationen zur Aktivierung von E-Mails in der Vorschau-Umgebung finden Sie im Abschnitt [Anzeigen und Ändern Ihrer E-Mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view)Benachrichtigungseinstellungen im Artikel [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Option „E-Mails von Sandbox empfangen“](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Die Planung von Berichten für die Bereitstellung in der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen ist identisch mit der Planung von Berichten in der Produktionsumgebung. Informationen zum Planen eines Berichts für die Bereitstellung finden Sie unter [Übersicht zur Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wenn Sie einen Bericht für die Bereitstellung in der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen planen, gibt es die folgenden Szenarien:

* Wenn die Option &quot;E-Mails aus dieser Testumgebung empfangen&quot; für den Benutzer deaktiviert ist, der den Bericht erhält, wird beim Planen der Übermittlung des Berichts keine Datei erstellt.
* Wenn die Option &quot;E-Mails aus dieser Testumgebung empfangen&quot; für den Benutzer aktiviert ist, der den Bericht erhält, wird der Bericht als E-Mail-Anhang an die E-Mail-Adresse gesendet, die dem Benutzer zugeordnet ist.

## Benachrichtigung externer Benutzer

Externe Benutzer erhalten keine Berichte, die von den Workfront-Testumgebungen gesendet wurden, und sie erhalten keine E-Mail-Benachrichtigung.

Externe Benutzer erhalten E-Mail-Berichte nur, wenn sie von einer Produktionsumgebung bereitgestellt werden.
