---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Erstellen Sie mehrere Filterregeln, die auf dasselbe Feld verweisen (AND-Anweisungen)'
description: Wenn Sie in der Standardmodus-Benutzeroberfläche versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des UND-Qualifizierers), wird einer der Filter gelöscht, wenn Sie den Bericht speichern und Report Builder beenden.
author: Courtney
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GkRwwb61-KuX14NsIAJVh0aG4CxipyKHymqI7eNAUEU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 383
ht-degree: 14%

---

# Filter: Mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen (UND-Anweisungen)

<!--Audited: 10/2024-->

Wenn Sie in der Standardmodus-Benutzeroberfläche versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des UND-Qualifizierers), wird einer der Filter gelöscht, wenn Sie den Bericht speichern und Report Builder beenden.

**Beispiel** Es empfiehlt sich, nur Aufgaben anzuzeigen, die das Wort „grün“, aber nicht das Wort „rot“ im Namen enthalten. Adobe Workfront erlaubt es nicht, die folgenden Filterregeln über die Standardmodus-Benutzeroberfläche zu speichern, da sie auf dasselbe Feld (Aufgabenname) verweisen, aber unterschiedliche Modifikatoren verwenden und auf verschiedene Werte verweisen:

* Aufgabenname > Enthält > Grün
* Aufgabenname > enthält nicht > Rot

Sie können diesen Filter jedoch im Textmodus erstellen.

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
