---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Unvollständige projektübergreifende Vorgänger anzeigen'
description: Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Z1eiFj8bs-qj9Jxs3m7GnYDZE-bBPvGHE3VFEv3DOFM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 199
ht-degree: 26%

---

# Filter: Unvollständige projektübergreifende Vorgänger anzeigen

<!--Audited: 10/2024-->

Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern von projektübergreifenden Vorgängern

So wenden Sie diesen Filter an:

1. Zu einer Aufgabenliste oder einem Aufgabenbericht wechseln.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. (Bedingt) Klicken Sie auf **Textmodus** wenn Sie den Filter aus einer Liste aufgerufen haben, oder **Wechseln zum Textmodus** wenn Sie den Filter aus einem Bericht aufgerufen haben.
1. Fügen Sie im neuen Bereich den folgenden Code ein:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Bedingt) Klicken Sie auf **Filter speichern** wenn Sie den Filter über einen Bericht aufgerufen haben, oder **Anwenden** und dann **Als neu speichern** wenn Sie den Filter über eine Aufgabenliste aufgerufen haben.
