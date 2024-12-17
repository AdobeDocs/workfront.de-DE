---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Persönliche Aufgaben'
description: Dieser Aufgabenfilter gibt Ad-hoc-Arbeitsanfragen zurück, die an einen Benutzer gesendet wurden, oder Aufgabenelemente, die von Benutzern im Bereich Startseite hinzugefügt wurden. Persönliche Aufgaben sind nicht mit einem Projekt verbunden, können jedoch bei Bedarf in ein Projekt verschoben werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Filter: persönliche Aufgaben

<!--Audited: 10/2024-->

Dieser Aufgabenfilter gibt Ad-hoc-Arbeitsanfragen zurück, die an einen Benutzer gesendet wurden, oder Aufgabenelemente, die von Benutzern in ihrem Aufgaben-Widget im Bereich Startseite hinzugefügt wurden.

Ad-hoc-Arbeitsanfragen und -Aufgabenelemente werden in Adobe Workfront als persönliche Aufgaben gespeichert.

Persönliche Aufgaben sind nicht mit einem Projekt verbunden, können jedoch bei Bedarf in ein Projekt verschoben werden. Weitere Informationen finden Sie unter [Persönliche Aufgaben erstellen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

![](assets/personal-tasks-report.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Persönliche Aufgaben filtern

So erstellen Sie diesen Filter:

1. Zu einer Aufgabenliste oder einem Aufgabenbericht wechseln.
1. Klicken Sie **Dropdown-** „Filter“ auf **Neuer Filter**.
1. (Bedingt) Klicken Sie auf **Filterregel hinzufügen**, wenn Sie auf den Filter in einem Bericht zugreifen, oder beginnen Sie mit der Auswahl Ihrer Filterkriterien im ersten Feld, wenn Sie auf den Filter in einer Liste zugreifen.
1. (Bedingt) Wählen Sie die folgenden Filterkriterien aus:

   * Aus einem Listenfilter: **Aufgabe** > **Persönlich** **Ist wahr**
   * Über einen Berichtsfilter: **Aufgabe** > **Persönlich** > **Gleich (Groß-/Kleinschreibung beachten)** > **True**.
1. Speichern Sie den Filter.

   In der Liste werden nur persönliche Aufgaben angezeigt, die sich in keinem Projekt befinden.
