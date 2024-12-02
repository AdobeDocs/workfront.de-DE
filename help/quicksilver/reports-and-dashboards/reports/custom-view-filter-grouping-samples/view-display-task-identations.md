---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Anzeigen von Aufgabeinsätzen in einer Aufgabenliste'
description: In dieser Aufgabenansicht können Sie der Spalte "Task Name"Code hinzufügen, um die Aufgaben, die gemäß der Arbeitsaufschlüsselungsstruktur des Projekts eingerückt sind, anzuzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Anzeigen: Einzüge von Aufgaben in einer Aufgabenliste anzeigen

<!--Audited: 11/2024-->

In dieser Aufgabenansicht können Sie der Spalte &quot;Task Name&quot;Code hinzufügen, um die Aufgaben, die gemäß der Arbeitsaufschlüsselungsstruktur des Projekts eingerückt sind, anzuzeigen.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Einzüge von Aufgaben in einer Spalte einer Aufgabenliste anzeigen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdownmenü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und beginnen Sie mit der Eingabe &quot;Aufgabenname&quot;im Feld **In dieser Spalte anzeigen** und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie in der neuen Spalte auf **In Textmodus wechseln** > **Textmodus bearbeiten** .
1. Entfernen Sie den Text, den Sie in der Zeile `valuefield=` finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
