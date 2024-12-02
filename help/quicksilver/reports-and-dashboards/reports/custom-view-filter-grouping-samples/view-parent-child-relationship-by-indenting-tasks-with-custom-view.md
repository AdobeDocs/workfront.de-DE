---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Anzeigen der übergeordneten/untergeordneten Beziehung in einer Aufgabe durch Einzug der Aufgaben'
description: Sie können die Unterscheidung zwischen übergeordneten und untergeordneten Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Ansicht: Anzeigen der übergeordneten/untergeordneten Beziehung in einer Aufgabe durch Einrücken der Aufgaben

<!--Audited: 11/2024-->

Sie können die Unterscheidung zwischen übergeordneten und untergeordneten Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Anforderung zum Ändern einer Ansicht</li> 
   <li>Berichtänderung planen</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkender beim Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen der übergeordneten/untergeordneten Beziehung in einer Aufgabe durch Einrücken der Aufgaben

1. Wechseln Sie zum Projekt mit der Aufgabenliste, die Sie exportieren möchten.
1. Klicken Sie auf das Dropdownmenü **Ansicht** und wählen Sie **Neue Ansicht** aus.
1. Klicken Sie in der Spaltenüberschrift **Aufgabenname** auf .
1. Wählen Sie oben rechts **In den Textmodus wechseln** aus.
1. Klicken Sie auf **Textmodus bearbeiten** und entfernen Sie den gesamten vorhandenen Text.
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

1. Klicken Sie auf **Fertig** > **Ansicht speichern**.
