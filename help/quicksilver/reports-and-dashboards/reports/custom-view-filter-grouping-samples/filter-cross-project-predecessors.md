---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Anzeige unvollständiger projektübergreifender Vorgänger'
description: Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Filter: Anzeige unvollständiger projektübergreifender Vorgänger

<!--Audited: 10/2024-->

Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.

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

## Filtern von projektübergreifenden Vorgängern

So wenden Sie diesen Filter an:

1. Zu einer Aufgabenliste oder einem Aufgabenbericht wechseln.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. (Bedingt) Klicken Sie auf **Textmodus** wenn Sie den Filter aus einer Liste aufgerufen haben, oder **Wechseln zum Textmodus** wenn Sie den Filter aus einem Bericht aufgerufen haben.
1. Fügen Sie im neuen Bereich den folgenden Code ein:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Bedingt) Klicken Sie auf **Filter speichern** wenn Sie den Filter über einen Bericht aufgerufen haben, oder **Anwenden** und dann **Als neu speichern** wenn Sie den Filter über eine Aufgabenliste aufgerufen haben.
