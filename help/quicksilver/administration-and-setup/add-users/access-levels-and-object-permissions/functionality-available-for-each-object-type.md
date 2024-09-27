---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,chart,levels,permissions
navigation-topic: access-levels
title: Für jeden Objekttyp verfügbare Funktionen für verschiedene Zugriffsebenen
description: In den folgenden Tabellen sind die für jeden Objekttyp in den verschiedenen Zugriffsebenen verfügbaren Funktionen aufgeführt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 56f59e901e4c20159cd8b40cea0cbbe24271099b
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 10%

---

# Für jeden Objekttyp verfügbare Funktionen für verschiedene Zugriffsebenen

{{highlighted-preview}}

In den folgenden Tabellen sind die für jeden Objekttyp in den verschiedenen Zugriffsebenen verfügbaren Funktionen aufgeführt.

Sie zeigt außerdem an, welche Aktionen Workfront-Administratoren über eine Zugriffsebene deaktivieren oder aktivieren können.

>[!NOTE]
>
>In diesem Artikel werden die Funktionen beschrieben, die für den Zugriff auf die Ebenen im aktuellen Workfront-Planmodell verfügbar sind. Informationen zu den im neuen Planmodell verfügbaren Funktionen finden Sie unter [Für jeden Objekttyp verfügbare Funktionen für neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projekte

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf Projekte erhalten.

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; |   |   |   |   |
| Kopieren | ✓&#42; |   |   |   |   |
| Löschen | ✓&#42; |   |   |   |   |
| Freigeben | ✓&#42; | ✓&#42; |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Benutzerdefiniertes Formular hinzufügen | ✓ |   |   |   |   |
| Benutzerdefinierte Felder aktualisieren | ✓ | ✓ |   |   |   |
| Hinzufügen eines Validierungsprozesses | ✓ |   |   |   |   |
| Projekt genehmigen | ✓ | ✓ | ✓ |   |   |
| Dokument hinzufügen | ✓ | ✓ | ✓ |   |   |
| Problem hinzufügen | ✓ | ✓ |   |   |   |
|  Aufgaben hinzufügen | ✓ | ✓ |   |   |   |
| Aktualisierungen/Kommentare geben | ✓ | ✓ | ✓ |   |   |
| Status ändern | ✓ |   |   |   |   |
| Stunden protokollieren | ✓ | ✓ |   |   |   |
| Zuweisungen bearbeiten | ✓ | ✓ |   |   |   |
| Grundlinie verwalten | ✓ |   |   |   |   |
| Risiken verwalten | ✓ |   |   |   |   |
| Finanzen verwalten | ✓ |   |   |   |   |
| Aufwendungen hinzufügen/bearbeiten | ✓ | ✓ |   |   |   |
| Vorlagen anfügen | ✓ |   |   |   |   |
| Als Vorlage speichern | ✓ |   |   |   |   |
| Geschäftsfall hinzufügen/bearbeiten | ✓ |   |   |   |   |
| Bearbeiten von Projektdetails | ✓ |   |   |   |   |
| Bearbeitungsbesetzung | ✓ |   |   |   |   |
| In MS Project exportieren | ✓ | ✓ | ✓ |   |   |
| Finanz-/Zeitleistenskalierung neu berechnen | ✓ |   |   |   |   |
| Festlegen von Warteschlangeneigenschaften | ✓ |   |   |   |   |



&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Aufgaben

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; | ✓&#42; |   |   |   |
| Löschen | ✓&#42; | ✓&#42; |   |   |   |
| Freigeben | ✓&#42; | ✓&#42; |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Vorgänger hinzufügen | ✓ | ✓ |   |   |   |
|  Probleme hinzufügen | ✓ | ✓ |   |   |   |
| Aufgabe bearbeiten (ohne Status) | ✓ | ✓ |   |   |   |
| Aufgabenstatus ändern | ✓ | ✓ |   |   |   |
| Dokumente hinzufügen | ✓ | ✓ | ✓ |   |   |
| Aufgabe kopieren | ✓ | ✓ |   |   |   |
| Verschieben einer Aufgabe | ✓ | ✓ |   |   |   |
| Stunden protokollieren | ✓ | ✓ |   |   |   |
| Zuweisung akzeptieren | ✓ | ✓ |   |   |   |
| Zuweisung vornehmen | ✓ | ✓ | Nur Inline-Bearbeitung | Nur Inline-Bearbeitung |   |
| Benutzerdefiniertes Formular anhängen | ✓ | ✓ |   |   |   |
| Benutzerdefinierte Felder bearbeiten | ✓ | ✓ |   |   |   |
| Validierungsprozess erstellen | ✓ | ✓ |   |   |   |
| Aufgabe validieren | ✓ | ✓ | ✓ |   |   |
| Bearbeiten von Finanzen | ✓ |   |   |   |   |
| Aufwendungen hinzufügen/bearbeiten | ✓ | ✓ |   |   |   |
| Finanzen anzeigen | ✓ | ✓ | ✓ |   |   |
| Aktualisierungen/Kommentare | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Probleme

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Bearbeiten | ✓ | ✓ | ✓ | ✓ |   |
| Löschen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Freigeben | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Benutzerdefinierte Formulare anhängen | ✓ | ✓ | ✓ | ✓ |   |
| Benutzerdefinierte Felder bearbeiten | ✓ | ✓ | ✓ | ✓ |   |
| Genehmigen von Problemen | ✓ | ✓ | ✓ | ✓ |   |
| Hinzufügen eines Validierungsprozesses | ✓ | ✓ | ✓ | ✓ |   |
| Dokumente hinzufügen | ✓ | ✓ | ✓ | ✓ |   |
| Probleme kopieren | ✓ | ✓ | ✓ | ✓ |   |
| Probleme verschieben | ✓ | ✓ | ✓ | ✓ |   |
| Stunden protokollieren | ✓ | ✓ |   |   |   |
| Konvertieren eines Problems in ein Projekt | ✓ | ✓ |   |   |   |
| Konvertieren eines Problems in eine Aufgabe | ✓ |   |   |   |   |
| Accept-Zuweisungen | ✓ | ✓ |   |   |   |
| Zuweisungen vornehmen | ✓ | ✓ |   |   |   |
| Hinzufügen von Aktualisierungen und Kommentaren | ✓ | ✓ | ✓ | ✓ |   |



&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfolios

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf Portfolios haben.

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; |   |   |   |   |
| Löschen | ✓&#42; |   |   |   |   |
| Freigeben | ✓&#42; |   |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Details bearbeiten | ✓ |   |   |   |   |
| Benutzerdefinierte Formulare anhängen | ✓ |   |   |   |   |
| Benutzerdefinierte Felder bearbeiten | ✓ |   |   |   |   |
| Hinzufügen und Entfernen von Projekten | ✓ |   |   |   |   |
| Projekte genehmigen | ✓ |   |   |   |   |
| Portfolio-Optimierung | ✓ |   |   |   |   |
| Dokumente hinzufügen | ✓ | ✓ | ✓ |   |   |
| Hinzufügen von Aktualisierungen und Kommentaren | ✓ | ✓ | ✓ |   |   |



&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programme

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf Programme haben.

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; |   |   |   |   |
| Löschen | ✓&#42; |   |   |   |   |
| Freigeben | ✓&#42; |   |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Details bearbeiten | ✓ |   |   |   |   |
| Benutzerdefinierte Formulare anhängen | ✓ |   |   |   |   |
| Benutzerdefinierte Felder bearbeiten | ✓ |   |   |   |   |
| Hinzufügen und Entfernen von Projekten | ✓ |   |   |   |   |
| Projekte genehmigen | ✓ |   |   |   |   |
| Portfolio-Optimierung | ✓ |   |   |   |   |
| Dokumente hinzufügen | ✓ | ✓ | ✓ |   |   |
| Hinzufügen von Aktualisierungen und Kommentaren | ✓ | ✓ | ✓ |   |   |



&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Berichte, Dashboards und Kalender

Benutzer mit einer Planungslizenz haben vollen Zugriff auf Berichte. Alle anderen Zugriffsebenen haben Ansichtszugriff auf Berichte.

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfrage | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; |   |   |   |   |
| Löschen | ✓&#42; |   |   |   |   |
| Anzeigen integrierter Berichte | ✓&#42; |   |   |   |   |
| Freigeben | ✓&#42; | ✓ | ✓ |   |   |
| Öffentliche Freigabe von Kalendern und Berichten | ✓&#42; |   |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Bearbeiten | ✓ |   |   |   |   |
| Kopieren | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Anforderer können nur Berichte anzeigen, die für sie freigegeben wurden

## Filter, Ansichten und Gruppierungen

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Aktion</p> </th> 
   <th> <p>Planer</p> </th> 
   <th> <p>Arbeitskraft</p> </th> 
   <th> <p>Prüfende Person</p> </th> 
   <th> <p>Anfragender</p> </th> 
   <th>Externer Benutzer<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Erstellen</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Löschen</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Freigeben</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Systemweit freigeben</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dokumente

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Löschen (Dokumente und Ordner) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Freigeben | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Öffentliche Freigabe (extern) | ✓&#42; |   |   |   |   |
| Systemweit freigeben | ✓&#42; | ✓&#42; |   |   |   |
| Anzeigen | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Details bearbeiten | ✓ | ✓ | ✓ | ✓ |   |
| Download | ✓ | ✓ | ✓ | ✓ | ✓ |
| Checkout | ✓ | ✓ | ✓ | ✓ |   |
| Hinzufügen von Genehmigern | ✓ | ✓ | ✓ | ✓ |   |
| Dokumente genehmigen | ✓ | ✓ | ✓ | ✓ | ✓ |
| Benutzerdefinierte Formulare anhängen | ✓ | ✓ | ✓ | ✓ |   |
| Benutzerdefinierte Felder bearbeiten | ✓ | ✓ | ✓ | ✓ |   |
| Verschieben nach (Objekt) | ✓ | ✓ | ✓ | ✓ |   |
| Senden an (Integration) | ✓ | ✓ | ✓ | ✓ |   |
| Hinzufügen von Aktualisierungen und Kommentaren | ✓ | ✓ | ✓ | ✓ |   |
| Neue Version hochladen | ✓ | ✓ | ✓ | ✓ |   |
| Version löschen | ✓ | ✓ | ✓ | ✓ |   |
| Vorschau | ✓ | ✓ | ✓ | ✓ | ✓ |
| Korrekturabzug | ✓ | ✓ | ✓ | ✓ |   |
| Testversand erzeugen | ✓ | ✓ |   |   |   |
| Testversand durchführen | ✓ | ✓ | ✓ | ✓ |   |
| Hinzufügen/Entfernen&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Umbenennen&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Link (mit Integration) | ✓ | ✓ | ✓ | ✓ |   |
| Verknüpfung aufheben (mit Integration) | ✓ | ✓ | ✓ | ✓ |   |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Nur für Dokumentordner verfügbar, nicht für Dokumente

## Benutzende

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Aktion</p> </th> 
   <th> <p>Planer</p> </th> 
   <th>Arbeitskraft</th> 
   <th> <p>Prüfende Person</p> </th> 
   <th> <p>Anfragender</p> </th> 
   <th> <p>Externer Benutzer**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Erstellen</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Löschen</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten, Löschen, Deaktivieren, Anmelden als oder Zurücksetzen des Kennworts für jeden Benutzer</td> 
   <td>✓*<p><b>HINWEIS</b>: Sie können sich nicht als ein Benutzer anmelden, der ein Systemadministrator ist.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten, Löschen, Deaktivieren, Anmelden als oder Zurücksetzen des Kennworts für alle Benutzer in einer Gruppe, die sie verwalten</td> 
   <td>✓*<p><b>HINWEIS</b>: Sie können sich nicht als ein Benutzer anmelden, der ein Systemadministrator ist.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzer anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Kontaktdaten anzeigen</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Externe Benutzer können nur nach anderen Benutzern suchen

## Teams

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Aktion</p> </th> 
   <th> <p>Planer</p> </th> 
   <th>Arbeitskraft</th> 
   <th> <p>Prüfende Person</p> </th> 
   <th> <p>Anfragender</p> </th> 
   <th> <p>Externer Benutzer*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Erstellen</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Löschen</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten von Teams, die sie verwenden</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten von Teams in von ihnen verwalteten Gruppen</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Alle Teams anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Teams anzeigen, die mit ihren Gruppen verknüpft sind</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Vorlagen

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Erstellen | ✓&#42; |   |   |   |   |
| Löschen | ✓&#42; |   |   |   |   |
| Freigeben | ✓&#42; |   |   |   |   |
| Systemweit freigeben | ✓&#42; |   |   |   |   |
| Anzeigen | ✓&#42; |   |   |   |   |
| Kopieren | ✓ |   |   |   |   |
| Bearbeiten von Vorlagendetails | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Finanzdaten

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf Finanzdaten haben.

Die Lizenztypen Anforderung und Externer Benutzer sind hier nicht enthalten, da sie keinen Zugriff auf diese Objekte und Bereiche haben.

| Aktion | Planer | Arbeitskraft | Prüfende Person |
|---|---|---|---|
| Bearbeiten der Rollenabrechnung und der Kostensätze | ✓&#42; |   |   |
| Bearbeiten der Benutzerabrechnung und der Kostensätze | ✓&#42; |   |   |
| Anzeigen der Rollenabrechnung und der Kostensätze | ✓&#42; |   |   |
| Anzeigen von Benutzerabrechnungs- und Kostensätzen | ✓&#42; |   |   |
| Abrechnungsdatensätze verwalten | ✓ |   |   |
| Ausgaben verwalten | ✓ | ✓ |   |
| Finanzdaten anzeigen | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">Ratenkarten verwalten</span> | ✓ |   |   |
| Anzeigen von Informationen nach Kosten in den Tools für die Ressourcenplanung | ✓ |   |   |
| Budgetressourcen in den Tools für die Ressourcenplanung&#42;&#42; | ✓ |   |   |
| Anzeigen der Ressourcenzuordnung in den Tools für die Ressourcenplanung&#42; | ✓ | ✓ | ✓ |
| Risiken für Projekte erstellen | ✓ |   |   |
| Risiken in Projekten anzeigen | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Erfordert zusätzlichen Zugriff auf die Ressourcenverwaltung.

## Ressourcenverwaltung

Nur Benutzer mit einer Planungslizenz können vollen Zugriff auf [Objekt oder Bereich auswählen] haben. Andere Lizenztypen können eingeschränkten oder keinen Zugriff auf Resource Management in Workfront haben.

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Prioritäten und Budgetstunden im Planer bearbeiten | ✓&#42; |   |   |   |   |
| Erstellen, Bearbeiten, Löschen von Ressourcen-Pools&#42;&#42; | ✓&#42; |   |   |   |   |
| Geplante Stunden im Arbeitslastausgleich aktualisieren&#42;&#42;&#42; | ✓* |   |   |   |   |
| Anzeigen von Projektprioritäten im Ressourcenplaner | ✓&#42; |   |   |   |   |
| Anzeigen der Ressourcenzuordnung in den Tools für die Ressourcenplanung | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Anzeigen von Ressourcen-Pools | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Budgetressourcen in den Tools für die Ressourcenplanung&#42;&#42; | ✓ |   |   |   |   |
| Anhängen von Ressourcen an Projekte, Vorlagen und Benutzer | ✓ |   |   |   |   |

{style="table-layout:auto"}

&#42; Mithilfe einer Zugriffsebene können Workfront-Administratoren diese Funktion deaktivieren oder aktivieren. Weitere Informationen finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Erfordert zusätzlichen Zugriff auf Finanzdaten und Berechtigungen für Projektfinanzierungen. Wenn Sie Ressourcen-Management-Zugriff für einen Benutzer gewähren, der keinen Zugriff auf Finanzdaten hat, kann der Benutzer die stündlichen Zuweisungen weiterhin im Ressourcenplaner sehen, aber nicht zur Kostenansicht wechseln oder den Geschäftsfall anzeigen. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) und [Finanzberechtigungen für ein Objekt freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Erfordert Berechtigungen für Contribute für das Objekt, wobei &quot;Zuweisungen vornehmen&quot;unter &quot;Erweiterte Einstellungen&quot;aktiviert ist. Weitere Informationen finden Sie im Abschnitt [Vererbte Berechtigungen und die Hierarchie der Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) im Artikel [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Bereich &quot;Szenario-Planer&quot;

| Aktion | Planer | Arbeitskraft | Prüfende Person | Anfragender | Externer Benutzer |
|---|---|---|---|---|---|
| Vorhandene Pläne und Initiativen erstellen/bearbeiten | ✓ | ✓ | ✓ |   |   |
| Hinzufügen oder Bearbeiten von Informationen zu Aufgabenrollen in Plänen und Initiativen&#42; | ✓ | ✓ | ✓ |   |   |
| Hinzufügen oder Bearbeiten von Kosteninformationen zu Plänen und Initiativen&#42; | ✓ | ✓ | ✓ |   |   |
| Löschen von Plänen und Initiativen | ✓ | ✓ | ✓ |   |   |
| Szenarien im Hauptmenü anzeigen ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |   |
| Anzeigen von Plänen und Initiativen, die der Benutzer erstellt hat&#42; | ✓ | ✓ | ✓ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>Benutzer können einen Plan anzeigen, den ein anderer Benutzer nur erstellt hat, wenn ein Link zum Plan für sie freigegeben ist.

&#42; Damit Benutzer Finanzdaten in einem Plan oder einer Initiative anzeigen können, benötigen sie Zugriff auf Finanzdaten. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront Goals Area

| Aktionen | Anzeigen | Bearbeiten |
|---|---|---|
| Erstellen |   | ✓ |
| Alle Ziele bearbeiten/löschen |   | ✓ |
| Ziele anzeigen im Hauptmenü | ✓ | ✓ |
| Anzeigen des Zielbereichs über einen freigegebenen Link | ✓ | ✓ |
| Alle Ziele im System anzeigen | ✓ | ✓ |
| Alle Ziele aktivieren/deaktivieren/schließen |   | ✓ |
| Aktivitäten erstellen/bearbeiten/löschen |   | ✓ |
| Ergebnisse erstellen/bearbeiten/löschen |   | ✓ |
| Hinzufügen eines ausgerichteten Ziels |   | ✓ |
| Fortschritt eines Ergebnisses oder einer Aktivität aktualisieren |   | ✓ |
| Ziel, Ergebnis oder Aktivität besitzen | ✓ | ✓ |
| Kommentar zu einem Ziel | ✓ | ✓ |
| Ziele kopieren |   | ✓ |
| Ansicht des Bereichs &quot;Zielliste&quot;im linken Bereich | ✓ | ✓ |
| Anzeigen des Bereichs Diagramme im linken Bereich | ✓ | ✓ |
| Anzeigen der Zielausrichtung im linken Bereich | ✓ | ✓ |

