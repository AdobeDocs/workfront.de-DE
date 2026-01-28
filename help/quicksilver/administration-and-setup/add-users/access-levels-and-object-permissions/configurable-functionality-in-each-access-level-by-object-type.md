---
title: Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp (veraltet)
description: In diesem Artikel wird erläutert, was Sie als Adobe Workfront-Administrator für jeden Objekttyp in jeder Zugriffsebene zulassen können. Außerdem wird erläutert, was die Standardkonfiguration für jeden Zugriffsebenen-Typ ist.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '3510'
ht-degree: 10%

---

# Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp (veraltet)

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die alten Zugriffsebenen. Informationen zu den aktuellen Zugriffsebenen finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Beim Konfigurieren einer Zugriffsebene für Ihre Organisation können Sie festlegen, welche spezifischen Aktionen der Zugriffsebene zur Verfügung stehen.

In diesem Artikel werden die Optionen erläutert, die ein Adobe Workfront-Administrator für jeden Objekttyp in jeder Zugriffsebene auswählen kann. Außerdem wird erläutert, was die Standardkonfiguration für jeden Zugriffsebenen-Typ ist.

Wenn beispielsweise ein Workfront-Administrator für Projekte mit einer bestimmten Zugriffsebene „Anzeigen“ auswählt, können Benutzende mit dieser Zugriffsebene nur Projekte anzeigen, aber nicht bearbeiten.

Informationen zu allen für einen Objekttyp in jeder Zugriffsebene verfügbaren Funktionen finden Sie unter [Funktionalität für jeden Objekttyp verfügbar](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projekte

In jeder Zugriffsebene können Sie die folgenden Optionen für Projekte konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planer (Planlizenztyp)</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Projekte.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Kopieren</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Ansicht</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den eingeschränkten Bearbeitungszugriff auf Projekte. Informationen dazu, wie der Bearbeitungszugriff in einer Worker-Zugriffsebene im Vergleich zu einer Planer-Zugriffsebene (die den vollständigen Bearbeitungszugriff auf Projekte ermöglicht) eingeschränkt ist, finden Sie im Abschnitt <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projekte</a> im Artikel <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Für jeden Objekttyp verfügbare Funktionen</a>.</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> der Schaltfläche Bearbeiten und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl) <p>Der Ansichtszugriff ist eingeschränkt, da Sie ihn nicht optimieren können, um die Projektfreigabe zu aktivieren oder zu deaktivieren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Projekte ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aufgaben

In jeder Zugriffsebene können Sie die folgenden Optionen für Aufgaben konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Aufgaben freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Aufgaben.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Aufgaben freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Aufgaben.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl)<p>Der Ansichtszugriff ist eingeschränkt, da Sie ihn nicht optimieren können, um die Projektfreigabe zu aktivieren oder zu deaktivieren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Aufgaben ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Probleme

In jeder Zugriffsebene können Sie die folgenden Optionen für Probleme konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Probleme.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Probleme.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Probleme.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Probleme.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Probleme ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfolios

In jeder Zugriffsebene können Sie die folgenden Optionen für Portfolios konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Portfolios freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht die vollständige Bearbeitung von Portfolios.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> <p>Zugriff auf Portfolios ist nicht verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Portfolios ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programme

In jeder Zugriffsebene können Sie die folgenden Optionen für Programme konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Programme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Programme.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> <p>Zugriff auf Programme ist nicht verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Programme ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Berichte, Dashboards und Kalender

In jeder Zugriffsebene können Sie die folgenden Optionen für Berichte, Dashboards und Kalender konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b></p><p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Aktionen. Beide sind standardmäßig aktiviert:</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Berichte, Dashboards und Kalender.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Integrierte Berichte anzeigen</b>, <b>Berichte öffentlich freigeben</b> und <b>systemweit freigeben</b>.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Öffentliche Freigabe von Berichten (extern)</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl)<p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Aktionen. Beide sind standardmäßig aktiviert:</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b> (Standardauswahl)<p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Aktionen. Standardmäßig ist nur die Option Freigeben aktiviert.</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Anzeigen</b> (Standardauswahl): Ermöglicht den schreibgeschützten Zugriff auf Berichte, Dashboards und Kalender, die für sie freigegeben wurden.</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, integrierte Berichte anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der <b>Ansicht</b>-Schaltfläche und deaktivieren oder aktivieren Sie <b>Integrierte Ansicht</b> (standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Berichte, Dashboards und Kalender ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filter, Ansichten und Gruppierungen

In jeder Zugriffsebene können Sie die folgenden Optionen für Filter, Ansichten und Gruppierungen konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b>:</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Filter, Ansichten und Gruppierungen ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dokumente

In jeder Zugriffsebene können Sie die folgenden Optionen für Dokumente konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Dokumente.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Dokumente öffentlich freigeben</b> und <b>systemweit freigeben</b>.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Dokumente öffentlich freigeben (extern)</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Dokumente.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Dokumente öffentlich freigeben</b> und <b>systemweit freigeben</b>.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Dokumente öffentlich freigeben (extern)</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Dokumente.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Aktionen. Alle sind standardmäßig aktiviert, mit Ausnahme der letzten beiden, <b>Dokumente öffentlich freigeben</b> und <b>systemweit freigeben</b>.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Dokumente öffentlich freigeben (extern)</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Dokumente.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Dokumente kann auf dieser Zugriffsebene nicht konfiguriert werden. Externe Benutzer können Workfront jedoch verwenden, um Dokumente anzuzeigen, zu überprüfen und herunterzuladen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzende

In jeder Zugriffsebene können Sie die folgenden Optionen für Benutzerinnen und Benutzer konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktinformationen von Benutzern anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> der Schaltfläche <b>Anzeigen</b> und deaktivieren oder aktivieren Sie dann die Option <b>Kontaktinformationen anzeigen</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht Benutzern die vollständige Bearbeitung.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Aktionen. Nur die ersten beiden Optionen <b>Erstellen</b> und <b>Löschen</b> sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li>Benutzeradmin. (Alle Benutzer)</li> 
       <li> <p>Benutzeradmin. (Gruppenbenutzer)</p> </li> 
      </ul> <p>Informationen zu den beiden Optionen für Benutzeradministratoren finden Sie im Abschnitt <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Konfigurieren des Benutzerzugriffs zum Bearbeiten von Benutzern mit einer benutzerdefinierten Zugriffsebene</a> im Artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li><p> <b>Anzeigen</b> (nur Option verfügbar)</p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktinformationen von Benutzern anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> der Schaltfläche <b>Anzeigen</b> und deaktivieren oder aktivieren Sie dann die Option <b>Kontaktinformationen anzeigen</b> (standardmäßig aktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li><p> <b>Anzeigen</b> (nur Option verfügbar)</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktinformationen von Benutzern anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> der Schaltfläche <b>Anzeigen</b> und aktivieren oder deaktivieren Sie dann die Option <b>Kontaktinformationen anzeigen</b> (standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b> (nur Option verfügbar)</p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktinformationen von Benutzern anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> der Schaltfläche <b>Anzeigen</b> und aktivieren oder deaktivieren Sie dann die Option <b>Kontaktinformationen anzeigen</b> (standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Benutzerzugriff ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Teams

In jeder Zugriffsebene können Sie die folgenden Optionen für Teams konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li><b>Anzeigen</b> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Beide sind standardmäßig deaktiviert.</p> 
      <ul> 
       <li>Alle Teams anzeigen</li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht Teams vollen Bearbeitungszugriff.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Alle sind standardmäßig aktiviert, mit Ausnahme der <b>Teams bearbeiten, in denen ich mitarbeite</b>.</p> 
      <ul> 
       <li>Erstellen</li> 
       <li>Löschen</li> 
       <li> <p>Teams bearbeiten, zu denen ich gehöre</p> </li> 
       <li> <p>Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadmins)</p> </li> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Anzeigen</b>
      <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li>Alle Teams anzeigen</li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht Teams vollen Bearbeitungszugriff.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Nur die erste Option <b>Teams bearbeiten, an denen </b> mitwirke) ist standardmäßig deaktiviert.</p> 
      <ul> 
       <li> <p>Teams bearbeiten, zu denen ich gehöre</p> </li> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b> (nur Option verfügbar)</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li>Meinen Gruppen zugeordnete Teams anzeigen</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b> (nur Option verfügbar)</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li>Meinen Gruppen zugeordnete Teams anzeigen</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Teams ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Vorlagen

In jeder Zugriffsebene können Sie die folgenden Optionen für Vorlagen konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Vorlagen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Ansicht und deaktivieren oder aktivieren Sie dann die Option <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Vorlagen.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Vorlagen ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Finanzdaten

In jeder Zugriffsebene können Sie die folgenden Optionen für Finanzdaten konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b>:</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li>Funktionsbezogene Fakturierung und Kostensätze anzeigen</li> 
       <li> <p>Benutzerfakturierung und Kostensätze anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf Finanzdaten.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Ansicht</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen*. Standardmäßig sind nur die letzten beiden Optionen <b>Funktionsabrechnung und Kostensätze anzeigen</b> und <b>Benutzerabrechnung und Kostensätze anzeigen</b> aktiviert.</p> 
      <ul> 
       <li>Funktionsbezogene Fakturierung und Kostensätze bearbeiten</li> 
       <li> <p>Benutzerfakturierung und Kostensätze bearbeiten</p> </li> 
       <li>Funktionsbezogene Fakturierung und Kostensätze anzeigen</li> 
       <li> <p>Benutzerfakturierung und Kostensätze anzeigen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (Standardauswahl)</p> </li> 
     <li> <b>Anzeigen</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (Standardauswahl)</p> </li> 
     <li><b>Anzeigen</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugang zu Finanzdaten ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Informationen zu diesen Optionen finden Sie unter [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Ressourcenverwaltung

In jeder Zugriffsebene können Sie die folgenden Optionen für die Ressourcenverwaltung konfigurieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zugriffsebene</th> 
   <th>Optionen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planerin oder Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Anzeigen</b> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht den vollständigen Bearbeitungszugriff auf das Ressourcen-Management.</p> <p>Klicken Sie zur Feinabstimmung auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie dann eine der folgenden Optionen. Nur die erste Option <b>Prioritäten und Budgetstunden im Planer bearbeiten</b> ist standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p> Prioritäten und Budgetstunden im Planer bearbeiten</p> </li> 
       <li> <p>Ressourcenpools verwalten</p> <p><b>HINWEIS</b>: Zum Verwalten von Ressourcenpools benötigt ein Benutzer zusätzlichen Zugriff auf Finanzdaten und Berechtigungen für die Projektfinanzierung. Wenn Sie einem Planer-Benutzer Zugriff auf die Ressourcenverwaltung gewähren, der keinen Zugriff auf Finanzdaten hat, kann der Benutzer die stündlichen Zuordnungen weiterhin im Ressourcenplaner sehen, aber nicht zur Kostenansicht wechseln oder den Business Case anzeigen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a> und <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Finanzberechtigungen für ein Objekt freigeben</a>.</p> </li> 
       <li> <p>Geplante Stunden im Workload Balancer aktualisieren</p> <p><b>HINWEIS</b>: Um geplante Stunden im Workload-Balancer zu aktualisieren, benötigt ein Benutzer die Berechtigung, zum -Objekt beizutragen, wobei „Zuweisungen vornehmen“ unter „Erweiterte Einstellungen“ aktiviert ist. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über Freigabeberechtigungen für Objekte</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li><b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfende Person</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Anfragenden</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> (nur Option verfügbar) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bereich für Szenarienplaner

Die Standardeinstellung für alle Zugriffsebenen ist Kein Zugriff. Ein Workfront-Administrator kann dies ändern, um Zugriff für Planer-, Worker- und Reviewer-Zugriffsebenen anzuzeigen oder zu bearbeiten.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Benutzende können einen Plan, den ein anderer Benutzer erstellt hat, nur anzeigen, wenn eine Verknüpfung zum Plan für sie freigegeben wurde.

## Workfront-Zielbereich

Alle sechs Standardzugriffsebenen (und alle vier Lizenztypen) können Workfront-Ziele bearbeiten und anzeigen.

Bearbeiten ist die Standardoption.
