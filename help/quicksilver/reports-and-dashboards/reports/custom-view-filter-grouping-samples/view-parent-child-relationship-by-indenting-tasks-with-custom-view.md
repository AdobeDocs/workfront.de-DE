---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Anzeigen der hierarchischen Beziehung in einer Aufgabe durch Einrücken der Aufgaben'
description: Sie können die Unterscheidung von hierarchischen Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QSBA40vOIbB8cm0YydDuJN9NS2X6SoXNF-dCBUHFniM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 21%

---

# Ansicht: Die Beziehung zwischen über- und untergeordneten Elementen in einer Aufgabe durch Einrücken der Aufgaben anzeigen

<!--Audited: 11/2024-->

Sie können die Unterscheidung von hierarchischen Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.

![Einzug des übergeordneten untergeordneten Elements](assets/parent-child-indented-custom-view-350x94.png)

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
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Anzeigen der hierarchischen Beziehung einer Aufgabe durch Einrücken der Aufgaben

1. Wechseln Sie zu dem Projekt mit der Aufgabenliste, die Sie exportieren möchten.
1. Klicken Sie auf **Dropdown** Menü „Ansicht“ und wählen Sie **Neue Ansicht**.
1. Klicken Sie in die Spaltenüberschrift **Aufgabenname**.
1. Wählen **oben** auf „Zum Textmodus wechseln“ aus.
1. Klicken Sie **Textmodus bearbeiten** und entfernen Sie den gesamten vorhandenen Text.
1. Fügen Sie den folgenden Text ein:


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.
