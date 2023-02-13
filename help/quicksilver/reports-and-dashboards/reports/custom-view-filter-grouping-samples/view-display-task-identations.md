---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Einzüge von Aufgaben in Aufgabenlisten anzeigen'
description: In dieser Aufgabenansicht können Sie der Spalte "Task Name"Code hinzufügen, um die Aufgaben, die gemäß der Arbeitsaufschlüsselungsstruktur des Projekts eingerückt sind, anzuzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Ansicht: Einzüge von Aufgaben in einer Aufgabenliste anzeigen

In dieser Aufgabenansicht können Sie der Spalte &quot;Task Name&quot;Code hinzufügen, um die Aufgaben, die gemäß der Arbeitsaufschlüsselungsstruktur des Projekts eingerückt sind, anzuzeigen.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Einzüge von Aufgaben in einer Spalte einer Aufgabenliste anzeigen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Task Name&quot;im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie in der neuen Spalte auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im

   ```
   valuefield=
   ```

   und ersetzen Sie sie durch den folgenden Code:

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klicken **Speichern**, dann **Ansicht speichern**.
