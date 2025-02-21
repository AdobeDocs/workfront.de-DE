---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Anzeigen der hierarchischen Beziehung in einer Aufgabe durch Einrücken der Aufgaben'
description: Sie können die Unterscheidung von hierarchischen Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Anzeigen : Die hierarchische Beziehung einer Aufgabe durch Einrücken der Aufgaben anzeigen

<!--Audited: 11/2024-->

Sie können die Unterscheidung von hierarchischen Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.

![Einzug des übergeordneten untergeordneten Elements](assets/parent-child-indented-custom-view-350x94.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Änderung einer Ansicht anfordern</li> 
   <li>Planen der Änderung eines Berichts</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkende zum Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
