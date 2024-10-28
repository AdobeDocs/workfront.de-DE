---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filter: Mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen ("AND"-Anweisungen)"'
description: Wenn Sie in der Benutzeroberfläche des Standardmodus versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des AND-Qualifizierers), wird einer der Filter beim Speichern des Berichts und Beenden des ReportBuilder gelöscht.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Filter: Erstellen Sie mehrere Filterregeln, die auf dasselbe Feld verweisen (&quot;AND&quot;-Anweisungen)

<!--Audited: 10/2024-->

Wenn Sie in der Benutzeroberfläche des Standardmodus versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des AND-Qualifizierers), wird einer der Filter beim Speichern des Berichts und Beenden des ReportBuilder gelöscht.

**Beispiel:** Möglicherweise möchten Sie nur Aufgaben anzeigen, die das Wort &quot;grün&quot;enthalten, jedoch nicht das Wort &quot;rot&quot;im Namen enthalten. Adobe Workfront ermöglicht es Ihnen nicht, die folgenden Filterregeln mithilfe der Benutzeroberfläche des Standardmodus zu speichern, da sie dasselbe Feld (Aufgabenname) referenziert, aber unterschiedliche Modifikatoren verwendet und sich auf unterschiedliche Werte bezieht:

* Aufgabenname > Enthält > Grün
* Aufgabenname > enthält nicht > Rot

Sie können diesen Filter jedoch im Textmodus erstellen.

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

## Mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Filter** die Option **Neuer Filter** aus.
1. Klicken Sie auf **Textmodus**.
1. Fügen Sie im angezeigten Feld den folgenden Code hinzu:

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
   >Kopieren Sie die Anweisung und fügen Sie sie beliebig oft ein. Anschließend können Sie so viele Anweisungen hinzufügen, wie Sie benötigen, um auf dasselbe Feld zu verweisen (in unserem Fall &quot;name&quot;), und die folgenden Änderungen an den zusätzlichen Anweisungen vornehmen:
   >
   >1. Stellen Sie den beiden kopierten Zeilen &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot; usw. für jeden neuen Feld möglichen Wert voran.
   >1. Ersetzen Sie die Feldzeile durch den neuen Feldwert (nach dem Zeichen &quot;=&quot;).
   >1. Ersetzen Sie die Modifikatorzeile (_Mod) durch den neuen Modifikator.
   >   
   >Bei diesen Anweisungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken Sie auf **Anwenden** und dann auf **Als neu speichern**.
