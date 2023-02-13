---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: Projektsponsor für eine Aufgabenliste"
description: Mit dieser Aufgabengruppierung können Sie Aufgaben nach dem Projektsponsor gruppieren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Gruppierung: Projektsponsor für eine Aufgabenliste

Mit dieser Aufgabengruppierung können Sie Aufgaben nach dem Projektsponsor gruppieren.

![](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## Gruppe nach Projektsponsor für eine Aufgabenliste

So wenden Sie diese Gruppierung an:

1. Gehen Sie zur Aufgabenliste.
1. Im **Gruppierung** Dropdown-Menü auswählen **Neue Gruppierung**.

1. Klicken **In den Textmodus wechseln**.
1. Entfernen Sie den Text, der im Textbearbeitungsfenster angezeigt wird.
1. Kopieren Sie den folgenden Code und fügen Sie ihn in das Textbearbeitungsfenster ein:

   ```
   group.0.name=Project Sponsor<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=string
   ```

1. Klicken **Gruppierung speichern**.
