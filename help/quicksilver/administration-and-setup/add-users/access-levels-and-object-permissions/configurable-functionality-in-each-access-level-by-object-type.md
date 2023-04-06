---
title: Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp
description: In diesem Artikel wird erläutert, was Sie als Adobe Workfront-Administrator für jeden Objekttyp in den einzelnen veralteten Zugriffsebenen zulassen können. Außerdem wird erläutert, was die Standardkonfiguration für die einzelnen Arten von Legacy-Zugriffsrechten ist.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '3456'
ht-degree: 10%

---

# Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp

In diesem Artikel wird erläutert, was Sie als Adobe Workfront-Administrator für jeden Objekttyp in den einzelnen veralteten Zugriffsebenen zulassen können. Außerdem wird erläutert, was die Standardkonfiguration für die einzelnen Arten von Legacy-Zugriffsrechten ist.

Informationen zu allen für einen Objekttyp verfügbaren Funktionen in den einzelnen Zugriffsebenen finden Sie unter [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projekte

Sie können für jede Legacy-Zugriffsebene die folgenden Optionen für Projekte konfigurieren:

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
   <td>Planer (Lizenztyp planen)</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Projekte.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Kopieren</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Anzeigen</p> </li> 
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
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht eingeschränkten Bearbeitungszugriff auf Projekte. Informationen dazu, wie der Zugriff auf die Bearbeitung auf eine Worker-Zugriffsebene im Vergleich zu einer Planer-Zugriffsebene (die den uneingeschränkten Zugriff auf Projekte ermöglicht, finden Sie im Abschnitt . <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projekte</a> im Artikel <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Für jeden Objekttyp verfügbare Funktionen</a>.</p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Projekte freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche "Bearbeiten"klicken, deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl) <p>Der Zugriff auf die Ansicht ist eingeschränkt, da Sie sie nicht anpassen können, um die Projektfreigabe zu aktivieren oder zu deaktivieren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Projekte ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aufgaben

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Aufgaben konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Zur Feinabstimmung können Sie die Möglichkeit konfigurieren, Aufgaben freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Aufgaben.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
     <li><p> <b>Anzeigen</b></p> <p>Zur Feinabstimmung können Sie die Möglichkeit konfigurieren, Aufgaben freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Aufgaben.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl)<p>Der Zugriff auf die Ansicht ist eingeschränkt, da Sie sie nicht anpassen können, um die Projektfreigabe zu aktivieren oder zu deaktivieren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Zugriff auf Aufgaben ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Probleme

Sie können für jede Legacy-Zugriffsebene die folgenden Optionen für Probleme konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Anzeigen</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Probleme.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Probleme.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Probleme.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, Probleme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Probleme.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Probleme ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfolios

Sie können für jede Legacy-Zugriffsebene die folgenden Optionen für Portfolios konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Zur Feinabstimmung können Sie die Möglichkeit konfigurieren, Portfolios freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Portfolios.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> <p>Der Zugriff auf Portfolios ist nicht möglich.</p> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Portfolios ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programme

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Programme konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Zur Feinabstimmung können Sie die Möglichkeit konfigurieren, Programme freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Programme.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> <p>Der Zugriff auf Programme ist nicht möglich.</p> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Programme ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Berichte, Dashboards und Kalender

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Berichte, Dashboards und Kalender konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Anzeigen</b></p><p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> ), dann deaktivieren oder aktivieren Sie die folgenden Aktionen. Beide sind standardmäßig aktiviert:</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Berichte, Dashboards und Kalender.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Integrierte Berichte anzeigen</b>, <b>Berichte öffentlich freigeben</b>und <b>Systemweit freigeben</b>.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Berichte öffentlich freigeben (extern)</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> (Standardauswahl)<p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie die folgenden Aktionen. Beide sind standardmäßig aktiviert:</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b> (Standardauswahl)<p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie die folgenden Aktionen. Standardmäßig ist nur die Option Freigeben aktiviert.</p> 
      <ul> 
       <li> <p>Integrierte Berichte anzeigen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Ansicht</b> (Standardauswahl): Ermöglicht schreibgeschützten Zugriff auf Berichte, Dashboards und Kalender, die für sie freigegeben wurden.</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, integrierte Berichte anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> Schaltfläche, dann deaktivieren oder aktivieren <b>Integrierte Ansicht</b>(standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Berichte, Dashboards und Kalender ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filter, Ansichten und Gruppierungen

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Filter, Ansichten und Gruppierungen konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b></p><p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
     <li> <p><b>Anzeigen</b></p><p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
       <li> <p>Systemweit freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b>:</p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Filter, Ansichten und Gruppierungen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Filter, Ansichten und Gruppierungen.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
   <td> <p>Der Zugriff auf Filter, Ansichten und Gruppierungen ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dokumente

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Dokumente konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Dokumente.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Dokumente öffentlich freigeben</b> und <b>Systemweit freigeben</b>.</p> 
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
     <li> <p><b>Anzeigen</b></p><p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Dokumente.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Dokumente öffentlich freigeben</b> und <b>Systemweit freigeben</b>.</p> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Dokumente.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie die folgenden Aktionen. Alle sind standardmäßig aktiviert, mit Ausnahme der letzten beiden, <b>Dokumente öffentlich freigeben</b> und <b>Systemweit freigeben</b>.</p> 
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
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Anzeigen</b></p><p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Dokumente freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Dokumente.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li> <p>Freigeben</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Dokumente ist in dieser Zugriffsebene nicht konfigurierbar. Externe Benutzer können Workfront jedoch verwenden, um Dokumente anzuzeigen, zu überprüfen und herunterzuladen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzende

Sie können für jede Legacy-Zugriffsebene die folgenden Optionen für Benutzer konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <p><b>Anzeigen</b></p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktdaten der Benutzer anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie die <b>Kontaktangaben anzeigen</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff für Benutzer.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie die folgenden Aktionen. Nur die ersten beiden Optionen, <b>Erstellen</b> und <b>Löschen</b>, sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Erstellen</p> </li> 
       <li> <p>Löschen</p> </li> 
       <li>Benutzeradmin. (Alle Benutzer)</li> 
       <li> <p>Benutzeradmin. (Gruppenbenutzer)</p> </li> 
      </ul> <p>Informationen zu den beiden Benutzeradministratoroptionen finden Sie im Abschnitt . <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Benutzerzugriff konfigurieren, um Benutzer mithilfe einer benutzerdefinierten Zugriffsebene zu bearbeiten</a> im Artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Arbeitskraft </td> 
   <td> 
    <ul> 
     <li><p> <b>Ansicht</b> (nur Option verfügbar)</p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktdaten der Benutzer anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie die <b>Kontaktangaben anzeigen</b> (standardmäßig aktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li><p> <b>Ansicht</b> (nur Option verfügbar)</p> <p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktdaten der Benutzer anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und aktivieren oder deaktivieren Sie die <b>Kontaktangaben anzeigen</b> (standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b> (nur Option verfügbar)</p><p>Um dies zu verfeinern, können Sie die Möglichkeit konfigurieren, die Kontaktdaten der Benutzer anzuzeigen. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und aktivieren oder deaktivieren Sie die <b>Kontaktangaben anzeigen</b> (standardmäßig deaktiviert).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Benutzer ist nicht verfügbar. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Teams

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Teams konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li><b>Anzeigen</b> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Beide sind standardmäßig deaktiviert.</p> 
      <ul> 
       <li>Alle Teams anzeigen</li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Teams.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Alle sind standardmäßig aktiviert, mit Ausnahme von <b>Teams bearbeiten, die ich verwende</b>.</p> 
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
      <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li>Alle Teams anzeigen</li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Teams.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Nur die erste Option, <b>Teams bearbeiten, die ich verwende</b>ist standardmäßig deaktiviert.</p> 
      <ul> 
       <li> <p>Teams bearbeiten, zu denen ich gehöre</p> </li> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li> <p>Meinen Gruppen zugeordnete Teams anzeigen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b> (nur Option verfügbar)</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p>Alle Teams anzeigen</p> </li> 
       <li>Meinen Gruppen zugeordnete Teams anzeigen</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <p><b>Ansicht</b> (nur Option verfügbar)</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
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

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Vorlagen konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li><p> <b>Anzeigen</b></p> <p>Um dies anzupassen, können Sie die Möglichkeit konfigurieren, Vorlagen freizugeben. Klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf der Schaltfläche Anzeigen deaktivieren oder aktivieren Sie die <b>Freigeben</b> (standardmäßig aktiviert).</p> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Vorlagen.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Alle sind standardmäßig aktiviert.</p> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
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

In jeder Legacy-Zugriffsebene können Sie die folgenden Optionen für Finanzdaten konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <p><b>Anzeigen</b>:</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Beide sind standardmäßig aktiviert.</p> 
      <ul> 
       <li>Funktionsbezogene Fakturierung und Kostensätze anzeigen</li> 
       <li> <p>Benutzerfakturierung und Kostensätze anzeigen</p> </li> 
      </ul> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf Finanzdaten.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Ansicht</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen*. Nur die letzten beiden Optionen, <b>Anzeigen der Rollenabrechnung und der Kosten</b> und <b>Anzeigen der Benutzerabrechnung und der Kosten</b>, sind standardmäßig aktiviert.</p> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (Standardauswahl)</p> </li> 
     <li><b>Anzeigen</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
   <td> 
    <ul> 
     <li> <p><b>Kein Zugriff</b> (nur Option verfügbar)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externer Benutzer</td> 
   <td> <p>Der Zugriff auf Finanzdaten ist nicht möglich. Externe Benutzer können Workfront nur verwenden, um Dokumente zu überprüfen und herunterzuladen und Kalender anzuzeigen, die für sie freigegeben sind.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Weitere Informationen zu diesen Optionen finden Sie unter [Übersicht über Rechnungsstellung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Ressourcenverwaltung

Sie können für jede Legacy-Zugriffsebene die folgenden Optionen für die Ressourcenverwaltung konfigurieren:

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
   <td>Planer </td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Anzeigen</b> </li> 
     <li> <p><b>Bearbeiten</b> (Standardauswahl): Ermöglicht uneingeschränkten Bearbeitungszugriff auf die Ressourcenverwaltung.</p> <p>Um dies anzupassen, klicken Sie auf das Zahnradsymbol <img src="assets/gear-icon-in-access-levels.png"> auf <b>Bearbeiten</b> und deaktivieren oder aktivieren Sie eine der folgenden Optionen. Nur die erste Option, <b>Bearbeiten von Prioritäten und Budgetzeiten im Planer</b>ist standardmäßig aktiviert.</p> 
      <ul> 
       <li> <p> Prioritäten und Budgetstunden im Planer bearbeiten</p> </li> 
       <li> <p>Ressourcenpools verwalten</p> <p><b>NOTE</b>: Um Ressourcenpools zu verwalten, benötigt ein Benutzer zusätzlichen Zugriff auf Finanzdaten und Berechtigungen für Projektfinanzierungen. Wenn Sie Ressourcen-Management-Zugriff für einen Planer-Benutzer gewähren, der keinen Zugriff auf Finanzdaten hat, kann der Benutzer die stündlichen Zuweisungen weiterhin im Ressourcenplaner sehen, aber nicht zur Kostenansicht wechseln oder den Geschäftsfall anzeigen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a> und <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Freigeben von Finanzberechtigungen für ein Objekt</a>.</p> </li> 
       <li> <p>Geplante Stunden im Workload Balancer aktualisieren</p> <p><b>NOTE</b>: Um die geplanten Stunden im Arbeitslastausgleich zu aktualisieren, benötigt ein Benutzer die Berechtigung, zum Objekt beizutragen, wobei unter Erweiterte Einstellungen die Option Zuweisungen vornehmen aktiviert ist. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über die Freigabe von Berechtigungen für Objekte</a>.</p> </li> 
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
   <td>Prüfer</td> 
   <td> 
    <ul> 
     <li> <b>Kein Zugriff</b> </li> 
     <li> <b>Ansicht</b> (Standardauswahl)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Antragsteller</td> 
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

## Bereich &quot;Szenario-Planer&quot;

Die Standardeinstellung für alle bisherigen Zugriffsebenen ist &quot;Kein Zugriff&quot;. Ein Workfront-Administrator kann diese Option ändern, um Zugriff für alle Planer-, Worker- und Reviewer-Zugriffsebenen anzuzeigen oder zu bearbeiten.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Benutzer können einen Plan anzeigen, den ein anderer Benutzer nur erstellt hat, wenn ein Link zum Plan für sie freigegeben ist.

## Workfront Goals Area

Alle sechs standardmäßigen Zugriffsstufen (und alle vier Lizenztypen) können Workfront-Ziele bearbeiten und anzeigen.

Die Standardoption ist &quot;Bearbeiten&quot;.
