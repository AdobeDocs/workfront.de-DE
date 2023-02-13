---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Anzeigen der übergeordneten/untergeordneten Beziehung in einer Aufgabe durch Einrücken der Aufgaben'
description: Sie können die Unterscheidung zwischen übergeordneten und untergeordneten Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Ansicht: Anzeigen der übergeordneten/untergeordneten Beziehung in einer Aufgabe durch Einrücken der Aufgaben

Sie können die Unterscheidung zwischen übergeordneten und untergeordneten Beziehungen in einer exportierten Aufgabenliste beibehalten, indem Sie der Aufgabenliste eine benutzerdefinierte Ansicht hinzufügen und sicherstellen, dass diese Ansicht ausgewählt ist, bevor Sie die Liste exportieren.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Wechseln Sie zum Projekt mit der Aufgabenliste, die Sie exportieren möchten.
1. Klicken Sie auf **Ansicht** und wählen Sie **Neue Ansicht**.

1. Benennen Sie den Filter in der linken oberen Ecke des Bildschirms.
1. Klicken Sie in **Aufgabenname** Spaltenüberschrift.

1. Auswählen **In den Textmodus wechseln** in der oberen rechten Ecke.
1. Klicken Sie auf eine beliebige Stelle im Textfeld, um den Text zu bearbeiten, und entfernen Sie den gesamten vorhandenen Text.
1. Fügen Sie den folgenden Text ein:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Klicken Sie auf **Speichern**.
1. Klicken **Ansicht speichern**.
