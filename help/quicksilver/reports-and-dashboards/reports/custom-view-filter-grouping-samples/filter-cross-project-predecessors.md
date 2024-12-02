---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: unvollständige projektübergreifende Vorgänger anzeigen'
description: Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Filter: unvollständige projektübergreifende Vorgänger anzeigen

<!--Audited: 10/2024-->

Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.

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

## Filtern von projektübergreifenden Vorgängern

So wenden Sie diesen Filter an:

1. Gehen Sie zu einer Aufgabenliste oder einem Aufgabenbericht.
1. Wählen Sie aus dem Dropdownmenü **Filter** die Option **Neuer Filter** aus.

1. (Bedingt) Klicken Sie auf **Textmodus** , wenn Sie von einer Liste aus auf den Filter zugegriffen haben, oder auf **Wechseln in Textmodus** , wenn Sie über einen Bericht auf den Filter zugegriffen haben.
1. Fügen Sie in den neuen Bereich den folgenden Code ein:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Bedingt) Klicken Sie auf **Filter speichern** , wenn Sie aus einem Bericht auf den Filter zugegriffen haben, oder auf **Anwenden** und dann auf **Als neu speichern** , wenn Sie über eine Aufgabenliste auf den Filter zugegriffen haben.
