---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: unvollständige, projektübergreifende Vorgänger anzeigen'
description: Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# Filter: unvollständige projektübergreifende Vorläufer anzeigen

Dieser Aufgabenfilter gibt unvollständige projektübergreifende Vorgänger zurück.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Filtern von projektübergreifenden Vorgängern

So wenden Sie diesen Filter an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Filter** Dropdown-Menü auswählen **Neuer Filter**.

1. Klicken **In den Textmodus wechseln**.
1. Im **Festlegen von Filterregeln für Ihren Bericht** -Bereich, fügen Sie den folgenden Code ein:
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. Klicken **Filter speichern**.
