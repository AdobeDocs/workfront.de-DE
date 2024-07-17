---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Liste der Aufgabennachfolger in einer Spalte hinzufügen"
description: Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte "Aufgabenerfolger"enthält die Nummer des Nachfolgers sowie den Namen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 2%

---

# Ansicht: Hinzufügen einer Liste von Aufgabennachfolgern in einer Spalte

Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte **Aufgabenerfolger** enthält die Nummer des Nachfolgers sowie den Namen.

![task_view_with_a_list_of_succeors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen einer Liste von Aufgabennachfolgern in einer Spalte

So fügen Sie diese Spalte einer Aufgabenansicht hinzu:

1. Wechseln Sie zu einer vorhandenen Aufgabenansicht.
1. Erweitern Sie das Dropdown-Menü Ansicht und wählen Sie **Ansicht anpassen** aus.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Bewegen Sie den Mauszeiger über den Bereich **In dieser Spalte anzeigen** und klicken Sie auf **Klicken Sie auf , um Text zu bearbeiten**.

1. Entfernen Sie den gesamten Text im Feld Textmodus und ersetzen Sie ihn durch den folgenden Code:
   <pre>displayName=Task Successors<br>listdelimiter=<br><br>listmethod=nested(Succors).lists<br>textmode=true<br>type=iterate<br>valueExpression=CONCAT({successor}).{taskNumber},' - ',{successor}.{name})<br>valueFormat=HTML</pre>

1. Klicken Sie auf **Ansicht speichern**.
