---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Persönliche Aufgaben'
description: Dieser Aufgabenfilter gibt Ad-hoc-Arbeitsanfragen zurück, die an einen Benutzer gesendet werden, oder Aufgabenelemente, die von Benutzern in ihrem Home-Bereich hinzugefügt werden. Persönliche Aufgaben sind nicht mit einem Projekt verbunden, können aber bei Bedarf in ein Projekt verschoben werden.
author: Nolan
feature: Reports and Dashboards
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Filter: persönliche Aufgaben

<!--Audited: 10/2024-->

Dieser Aufgabenfilter gibt Ad-hoc-Arbeitsanfragen zurück, die an einen Benutzer gesendet werden, oder Aufgabenelemente, die von Benutzern in ihrem Home-Bereich hinzugefügt werden.

Ad-hoc-Arbeitsanfragen und zu erledigende Elemente werden in Adobe Workfront als persönliche Aufgaben gespeichert.

Persönliche Aufgaben sind nicht mit einem Projekt verbunden, können aber bei Bedarf in ein Projekt verschoben werden.

![](assets/personal-tasks-report.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Persönliche Aufgaben filtern

So erstellen Sie diesen Filter:

1. Gehen Sie zu einer Aufgabenliste oder einem Aufgabenbericht.
1. Klicken Sie im Dropdownmenü **Filter** auf **Neuer Filter**.
1. (Bedingt) Klicken Sie auf **Filterregel hinzufügen** , wenn Sie auf den Filter aus einem Bericht zugreifen, oder wählen Sie im ersten Feld Ihre Filterkriterien aus, wenn Sie auf den Filter aus einer Liste zugreifen.
1. (Bedingt) Wählen Sie die folgenden Filterkriterien aus:

   * Aus einem Listenfilter: **Aufgabe** > **persönlich** **ist wahr**
   * Aus einem Berichtsfilter: **Aufgabe** > **Persönlich** > **Entspricht** > **Wahr**.
1. Speichern Sie den Filter.

   In der Liste werden nur persönliche Aufgaben angezeigt, die sich nicht auf Projekte beziehen.
