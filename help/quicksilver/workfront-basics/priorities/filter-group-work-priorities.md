---
navigation-topic: get-started-with-workfront
title: Filtern und Gruppieren Ihrer Arbeit mit Prioritäten
description: Sie können Filter verwenden, um Arbeit zu finden und nach Arbeit zu suchen, und dann eine Gruppierung anwenden, um sie zu organisieren.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 8eb9dcaf-bba3-466d-b06d-5383991bc4ea
source-git-commit: 7a6a34ee5b4986137a04d654cf58bfa5f2465715
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 6%

---

# Filtern und Gruppieren Ihrer Arbeit mit Prioritäten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>

Sie können Filter verwenden, um die gesuchte Arbeit zu finden, und dann eine Gruppierung anwenden, um sie zu organisieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
   <p>Aktuell: Anforderung oder höher</p>
   <p>Neu: Mitwirkender oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>Anzeigen- oder Bearbeitungszugriff für das Objekt, auf dem die Aktualisierung ausgeführt wird</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen des Zugriffs auf das Objekt</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern und Gruppieren Ihrer Arbeit mit Prioritäten in der Produktion

### Filtern von Arbeit

Sie können die Ihnen zugewiesenen Aufgaben und Probleme filtern.

{{step1-to-priorities}}

1. Klicken **oben** in der Arbeitsliste auf „Filter“.
1. Wählen Sie einen oder mehrere Filter aus, um Ihre Arbeitselemente einzugrenzen.
   ![](assets/filters.png)

+++Erweitern um detaillierte Informationen zu den verfügbaren Filtern
<table>
  <tbody>
   <tr>
   <th>Filter</th>
   <th>Beschreibung</th>
   </tr>
    <tr>
      <td>Es wird daran gearbeitet</td>
      <td>Zeigt Elemente an, an denen Sie derzeit arbeiten</td>
    </tr>
    <tr>
      <td>Startbereit</td>
      <td>Zeigt Elemente an mit 
      <ul>
      <li>Keine unvollständigen Vorgänger oder Aufgabenbeschränkungen</li>
      <p>und</p>
      <li>Das geplante Startdatum liegt in den letzten oder bis zu zwei Wochen in der Zukunft</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Nicht bereit</td>
      <td>Zeigt Elemente an, die
       <ul>
      <li>Unvollständige Vorgänger oder Aufgabenbeschränkungen verhindern, dass das Element bearbeitet wird</li>
      <p>oder</p>
      <li>Das geplante Startdatum liegt mehr als zwei Wochen in der Zukunft</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Angefordert</td>
      <td>Zeigt Probleme an, mit denen Sie noch nicht begonnen haben</td>
    </tr>
      <td>Fertig</td>
      <td>Zeigt Arbeiten an, die in den letzten zwei Wochen abgeschlossen wurden. Diese Filteroption umfasst keine Genehmigungen.</td>
    </tr>
    <tr>
    <td>Projekt</td>
    <td>Zeigt Projekte mit Aufgaben oder Problemen an, denen Sie zugewiesen wurden</td>
    </tr>
    <tr>
    <td>Fälligkeitsdatum</td>
    <td>Zeigt Arbeit nach geplantem Abschlussdatum an</td>
    </tr>
    <tr>
    <td>Status</td>
    <td>Zeigt Aufgaben oder Probleme mit dem Status Neu, In Bearbeitung und Abgeschlossen an</td>
    </tr>
    <tr>
    <td>Mein Fokus</td>
    <td>Zeigt Aufgaben oder Probleme in an, denen Fokusebenen zugewiesen sind. Fokusebenen werden von den einzelnen Benutzenden zugewiesen und verwaltet.</td>
    </tr>
  </tbody>
</table>

+++

1. (Optional) Klicken Sie auf **Zurück zur Standardeinstellung**, um Ihre Auswahl zurückzusetzen.

### Arbeiten gruppieren

{{step1-to-priorities}}

1. Klicken **oben** in der Arbeitsliste auf „Gruppen“.
1. Gruppe auswählen, um die Arbeitsliste zu organisieren
   ![](assets/groups.png)

+++Erweitern um detaillierte Informationen zu verfügbaren Gruppen anzuzeigen

| Gruppe | Beschreibung |
|-----------|-------------|
| Keine | Dadurch werden Gruppierungen aus der Arbeitsliste entfernt. |
| Mein Fokus | Dadurch werden Elemente basierend auf der zugewiesenen Fokusebene gruppiert. |
| Fällige Woche | Dadurch werden Elemente nach der Woche gruppiert, in der sie fällig sind. Fälligkeitsdaten werden durch das geplante Abschlussdatum bestimmt. |
| Status | Elemente werden nach folgenden Status gruppiert: Neu, In Bearbeitung, Abgeschlossen. <br>Hinweis: Benutzerdefinierte Status können derzeit nicht in Prioritäten verwendet werden. |
| Projekt | Dadurch werden Elemente nach Projekt gruppiert. |

+++

### Arbeit sortieren

Um Ihre Arbeit zu sortieren, öffnen Sie **Gruppe** und klicken Sie auf **Aufsteigend sortieren** oder **Absteigend sortieren**.

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>Die Sortieroption ist vorübergehend nicht verfügbar, wenn eine Gruppe angewendet wurde.



### Alle Abschnitte erweitern oder reduzieren

Um alle Abschnitte zu erweitern oder zu reduzieren, öffnen Sie **Gruppe** und klicken Sie auf **Alle erweitern** oder **Alle reduzieren**.

![](assets/expand-sort-groups.png)

<div class="preview">

## Filtern und Gruppieren Ihrer Arbeit mit Prioritäten in der Vorschau

### Arbeiten mit Standardfiltern filtern

Sie können die Ihnen zugewiesenen Aufgaben und Probleme filtern.

{{step1-to-priorities}}

1. Klicken **oben links** der Arbeitsliste auf „Filter“.
1. Klicken Sie **Standardfilter**.
1. Wählen Sie einen oder mehrere Filter aus, um Ihre Arbeitselemente einzugrenzen.
   ![](assets/filter-new.png)

+++Erweitern um detaillierte Informationen zu den verfügbaren Filtern
<table>
  <tbody>
   <tr>
   <th>Filter</th>
   <th>Beschreibung</th>
   </tr>
    <tr>
      <td>Es wird daran gearbeitet</td>
      <td>Zeigt Elemente an, an denen Sie derzeit arbeiten</td>
    </tr>
    <tr>
      <td>Startbereit</td>
      <td>Zeigt Elemente an mit 
      <ul>
      <li>Keine unvollständigen Vorgänger oder Aufgabenbeschränkungen</li>
      <p>und</p>
      <li>Das geplante Startdatum liegt in den letzten oder bis zu zwei Wochen in der Zukunft</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Nicht bereit</td>
      <td>Zeigt Elemente an, die
       <ul>
      <li>Unvollständige Vorgänger oder Aufgabenbeschränkungen verhindern, dass das Element bearbeitet wird</li>
      <p>oder</p>
      <li>Das geplante Startdatum liegt mehr als zwei Wochen in der Zukunft</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Angefordert</td>
      <td>Zeigt Probleme an, mit denen Sie noch nicht begonnen haben</td>
    </tr>
      <td>Fertig</td>
      <td>Zeigt Arbeiten an, die in den letzten zwei Wochen abgeschlossen wurden. Diese Filteroption umfasst keine Genehmigungen.</td>
    </tr>
    <tr>
    <td>Projekt</td>
    <td>Zeigt Projekte mit Aufgaben oder Problemen an, denen Sie zugewiesen wurden</td>
    </tr>
    <tr>
    <td>Fälligkeitsdatum</td>
    <td>Zeigt Arbeit nach geplantem Abschlussdatum an</td>
    </tr>
    <tr>
    <td>Status</td>
    <td>Zeigt Aufgaben oder Probleme mit dem Status Neu, In Bearbeitung und Abgeschlossen an</td>
    </tr>
    <tr>
    <td>Mein Fokus</td>
    <td>Zeigt Aufgaben oder Probleme in an, denen Fokusebenen zugewiesen sind. Fokusebenen werden von den einzelnen Benutzenden zugewiesen und verwaltet.</td>
    </tr>
  </tbody>
</table>

+++

1. (Optional) Klicken Sie auf **Zurück zur Standardeinstellung**, um Ihre Auswahl zurückzusetzen.

<!--### Filter your work with Smart filters

Use natural language to filter quickly filter work.

{{step1-to-priorities}}

1. Click **Filters** in the top left of the worklist.
1. Click **Smart filters**. 
1. Type how you want to filter your work. 

    You can type things like

    * Show me late tasks
    * Show my top priorities
    * Show work due today

-->

### Arbeiten gruppieren

{{step1-to-priorities}}

1. Klicken **oben links** der Arbeitsliste auf „Gruppen“.
1. Gruppe auswählen, um die Arbeitsliste zu organisieren
   ![](assets/groups-new.png)

+++Erweitern um detaillierte Informationen zu verfügbaren Gruppen anzuzeigen

| Gruppe | Beschreibung |
|-----------|-------------|
| Projekt | Dadurch werden Elemente nach Projekt gruppiert. |
| Mein Fokus | Dadurch werden Elemente basierend auf der zugewiesenen Fokusebene gruppiert. |
| Fällige Woche | Dadurch werden Elemente nach der Woche gruppiert, in der sie fällig sind. Fälligkeitsdaten werden durch das geplante Abschlussdatum bestimmt. |
| Status | Elemente werden nach folgenden Status gruppiert: Neu, In Bearbeitung, Abgeschlossen. <br>Hinweis: Benutzerdefinierte Status können derzeit nicht in Prioritäten verwendet werden. |

+++



### Arbeit sortieren

**In Gruppen sortieren**

Um Ihre Arbeit innerhalb einer Gruppe zu sortieren, öffnen Sie **Gruppe** und klicken Sie auf **Aufsteigend sortieren** oder **Absteigend sortieren**.

![](assets/sort-in-groups.png)

**Sortieren von Spalten**

Um einzelne Spalten zu sortieren, gehen Sie zur Spalte und klicken Sie auf den Abwärtspfeil.

![Pfeil nach unten in der Spalte](assets/sort-columns.png)



### Alle Gruppenabschnitte erweitern oder reduzieren

Um alle Gruppenabschnitte zu erweitern oder zu reduzieren, öffnen Sie **Gruppe** und klicken Sie auf **Alle erweitern** oder **Alle reduzieren**.

![](assets/expand-collapse-groups.png)

</div>