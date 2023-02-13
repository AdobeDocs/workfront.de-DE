---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Hinzufügen einer Liste von Aufgabennachfolgern in einer Spalte'
description: Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte "Aufgabenerfolger"enthält die Nummer des Nachfolgers sowie den Namen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Ansicht: Hinzufügen einer Liste von Aufgabennachfolgern in einer Spalte

Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die **Aufgabenerfolger** enthält die Anzahl der Nachfolger sowie den Namen.

![task_view_with_a_list_of_succeors_png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Hinzufügen einer Liste von Aufgabennachfolgern in einer Spalte

So fügen Sie diese Spalte einer Aufgabenansicht hinzu:

1. Wechseln Sie zu einer vorhandenen Aufgabenansicht.
1. Erweitern Sie das Dropdown-Menü Ansicht und wählen Sie **Ansicht anpassen**.
1. Klicken **Spalte hinzufügen**.
1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über die **In dieser Spalte anzeigen** und klicken Sie auf **Klicken, um Text zu bearbeiten**.

1. Entfernen Sie den gesamten Text im Feld Textmodus und ersetzen Sie ihn durch den folgenden Code:

   <pre>displayName=Task Success<br>listdelimiter=<br><br>listmethod=nested(Succors).lists<br>textmode=true<br>type=iterate<br>valueExpression=CONCAT({Nachfolger}.{taskNumber},' - ',{success}.{name})<br>valueFormat=HTML</pre>

1. Klicken **Ansicht speichern**.
