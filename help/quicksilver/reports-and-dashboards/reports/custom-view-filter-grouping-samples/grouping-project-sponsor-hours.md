---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Projektsponsor für Stunden'
description: Diese Stundengruppierung organisiert Stunden nach Sponsor des Projekts, in dem die Stunden protokolliert werden. Die standardmäßige Report Builder-Benutzeroberfläche für Ihre Gruppierungen bietet keine Zuordnung zum Feld Projektsponsor . Sie müssen die Textmodus-Oberfläche verwenden, um auf dieses Feld zuzugreifen.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: bc99e303047b989b972974b398420a9180e40874
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Gruppierung: Projektsponsor für Stunden

<!--Audited: 10/2024-->

Diese Stundengruppierung organisiert Stunden nach Sponsor des Projekts, in dem die Stunden protokolliert werden. Die standardmäßige Report Builder-Benutzeroberfläche für Ihre Gruppierungen bietet keine Zuordnung zum Feld Projektsponsor . Sie müssen die Textmodus-Oberfläche verwenden, um auf dieses Feld zuzugreifen.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Nach Projektsponsor gruppieren für Stunden

Um diese Gruppierung anzuwenden:

1. Zu einer Stundenliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im angezeigten Bereich und ersetzen Sie ihn durch den folgenden Code:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Klicken Sie **Fertig**.
1. Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.
