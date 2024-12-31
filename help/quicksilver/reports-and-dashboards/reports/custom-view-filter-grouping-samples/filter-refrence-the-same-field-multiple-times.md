---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Erstellen Sie mehrere Filterregeln, die auf dasselbe Feld verweisen (AND-Anweisungen)'
description: Wenn Sie in der Standardmodus-Benutzeroberfläche versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des UND-Qualifizierers), wird einer der Filter gelöscht, wenn Sie den Bericht speichern und Report Builder beenden.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Filter: Erstellen Sie mehrere Filterregeln, die auf dasselbe Feld verweisen (AND-Anweisungen)

<!--Audited: 10/2024-->

Wenn Sie in der Standardmodus-Benutzeroberfläche versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des UND-Qualifizierers), wird einer der Filter gelöscht, wenn Sie den Bericht speichern und Report Builder beenden.

**Beispiel** Es empfiehlt sich, nur Aufgaben anzuzeigen, die das Wort „grün“, aber nicht das Wort „rot“ im Namen enthalten. Adobe Workfront erlaubt es nicht, die folgenden Filterregeln über die Standardmodus-Benutzeroberfläche zu speichern, da sie auf dasselbe Feld (Aufgabenname) verweisen, aber unterschiedliche Modifikatoren verwenden und auf verschiedene Werte verweisen:

* Aufgabenname > Enthält > Grün
* Aufgabenname > enthält nicht > Rot

Sie können diesen Filter jedoch im Textmodus erstellen.

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen mehrerer Filterregeln, die auf dasselbe Feld verweisen

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.
1. Klicken Sie **Textmodus**.
1. Fügen Sie in dem angezeigten Feld den folgenden Code hinzu:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Um ähnliche Filter zu erstellen, erstellen Sie zuerst die erste Anweisung. Beispiel:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Kopieren Sie die Anweisung und fügen Sie sie beliebig oft ein. Sie können dann so viele Anweisungen hinzufügen, wie Sie benötigen, um auf dasselbe Feld zu verweisen (in unserem Fall „Name„), und die folgenden Änderungen an den zusätzlichen Anweisungen vornehmen:
   >
   >1. Den beiden kopierten Zeilen muss für jeden neuen Feldwert „AND:1:&quot;, „AND:2:&quot;, „AND:3:&quot; usw. vorangestellt werden.
   >1. Ersetzen Sie die Feldzeile durch den neuen Feldwert (nach dem Zeichen &quot;=„).
   >1. Ersetzen Sie die Modifikatorzeile (_mod) durch den neuen Modifikator.
   >   
   >Bei diesen Anweisungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken Sie **Übernehmen** und dann **Als neu speichern**.
