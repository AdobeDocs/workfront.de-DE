---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Aufgaben nach Portfolio, Programm und Projekt"
description: Verwenden Sie diese Aufgabengruppierung, um Aufgaben nach Portfolio, Programm und dann nach dem Projekt zu gruppieren, mit dem sie verknüpft sind.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Gruppierung: Aufgaben nach Portfolio, Programm und Projekt

Verwenden Sie diese Aufgabengruppierung, um Aufgaben nach Portfolio, Programm und dann nach dem Projekt zu gruppieren, mit dem sie verknüpft sind.

![](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Gruppenaufgaben nach Portfolio, Programm und Projekt

So wenden Sie diese Gruppierung an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text im **Gruppieren Ihres Berichts** Bereich.
1. Ersetzen Sie den Text durch den folgenden Code:

   <pre>group.0.linkedname=project<br>group.0.namekey=portfolio<br>group.0.notime=false<br>group.0.valueField=project:portfolio:name<br>group.0.valueFormat=string<br>group.1.linkedname=project<br>group.1.namekey=program<br>group.1.notime=false<br>group.1.valueField=project:program:name<br>group.1.valueFormat=string<br>group.2.name=Project<br>group.2.valueField=project:name<br>group.2.valueFormat=HTML<br>textmode=true<br></pre>

1. Klicken **Gruppierung speichern**.
