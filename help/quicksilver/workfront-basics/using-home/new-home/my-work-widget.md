---
product-area: home
navigation-topic: use-the-home-area
title: Verwalten Ihrer Arbeit mit dem Widget "Meine Arbeit"
description: Das Widget Meine Arbeit zeigt alle zugewiesenen Aufgaben, Probleme und Anforderungen an einem Ort an. Hier können Sie Ihre Arbeit filtern und organisieren, die Zeit protokollieren, Aktualisierungen vornehmen und Arbeitselemente als abgeschlossen markieren.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 20791e9f2cc0716b9b0ddd8f98c31ae0bea7ff45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 5%

---


# Verwalten Ihrer Arbeit mit dem Widget &quot;Meine Arbeit&quot;

Das Widget Meine Arbeit zeigt alle zugewiesenen Aufgaben, Probleme und Anforderungen an einem Ort an. Hier können Sie Ihre Arbeit filtern und organisieren, die Zeit protokollieren, Aktualisierungen vornehmen und Arbeitselemente als abgeschlossen markieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> <p>Aktuell: Contribute</p>
   <p>Oder</p> 
   <p>Neu:[!UICONTROL Light] oder höher<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höher Zugriff auf Projekte, Aufgaben, Probleme und Dokumente</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Contribute-Berechtigungen oder höher für die Aufgaben und Probleme, an denen Sie arbeiten müssen</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeiten mit Filtern suchen

Sie können die Filter &quot;Meine Arbeit&quot;so anpassen, dass sie sich auf bestimmte Elemente in Ihrer Arbeitsliste konzentrieren:

![](assets/filter-my-work-widget.png)

### Filterdetails

<table>
  <tbody>
    <tr>
      <td>Arbeiten an</td>
      <td>Zeigt Elemente an, an denen Sie derzeit arbeiten</td>
    </tr>
    <tr>
      <td>Startbereit</td>
      <td>Zeigt Elemente mit 
      <ul>
      <li>Keine unvollständigen Vorgänger oder Aufgabeneinschränkungen</li>
      <p>und</p>
      <li>Das geplante Startdatum liegt in der Vergangenheit oder bis zu zwei Wochen in der Zukunft</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Nicht bereit</td>
      <td>Zeigt Elemente an,
       <ul>
      <li>Unvollständige Vorgänger oder Aufgabenbeschränkungen, die verhindern, dass das Element bearbeitet wird</li>
      <p>oder</p>
      <li>Das geplante Startdatum liegt in Zukunft bei mehr als zwei Wochen.</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Angefordert</td>
      <td>Zeigt Probleme an, mit denen Sie noch nicht begonnen haben</td>
    </tr>
    <tr>
      <td>Von mir delegiert</td>
      <td>Zeigt Elemente an, die Sie anderen Benutzern zugewiesen haben</td>
    </tr>
    <tr>
      <td>An mich delegiert</td>
      <td>Zeigt Elemente an, die Ihnen von Benutzern zugewiesen wurden</td>
    </tr>
    <tr>
      <td>Abgeschlossen</td>
      <td>Zeigt die Arbeit an, die in den letzten zwei Wochen abgeschlossen wurde. Diese Filteroption umfasst keine Genehmigungen.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>Wenn Sie spezifischere Filteroptionen suchen, können Sie die Widgets My Task oder My Issue verwenden. Weitere Informationen zu den Filtern &quot;Meine Aufgabe&quot;und &quot;Mein Problem&quot;finden Sie unter [Übersicht über die Filter für neue Widgets &quot;Startseite&quot;](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md).

## Organisieren der Arbeit

Sie können die Sortier- und Gruppenfunktionen des Widgets &quot;Meine Arbeit&quot;verwenden, um Ihre Arbeit so zu organisieren, dass es für Sie sinnvoll ist.

### Sortieren

Sie können die Arbeitsliste nach

* Fälligkeitsdatum
Bei bereits fällig gewordenen Elementen wird neben dem Datum ein Warnsymbol angezeigt. Workfront verwendet das geplante Abschlussdatum, um festzustellen, ob Aufgaben und Probleme überfällig sind.
* Name
* Prozent abgeschlossen
* Status

>[!TIP]
>
>Um eine Liste zu erstellen, die alle fälligen Elemente am oberen Rand des Widgets &quot;Meine Arbeit&quot;anzeigt, sortieren Sie nach Fälligkeitsdatum und wenden Sie keine Gruppierung an.


![](assets/sort-my-work-widget.png)

### Gruppe

Sie können die Arbeitsliste nach

* Projekt
* Status
* Fälligkeitsdatum
Das Fälligkeitsdatum wird durch das geplante Abschlussdatum bestimmt.

>[!NOTE]
>
>Wenn Sie eine Gruppierung anwenden, bestimmt Ihre Auswahl im Menü Sortieren die Reihenfolge innerhalb der Gruppierung.


![](assets/group-my-work-widget.png)

## Aktualisieren der Arbeitselementinformationen in der Zusammenfassung

Sie können das Bedienfeld Zusammenfassung öffnen, um Informationen in einer Aufgabe oder einem Problem schnell zu aktualisieren. In der Zusammenfassung können Sie

* Prozentualen Fertigstellungsgrad aktualisieren
* Aktualisierung hinzufügen
* Navigieren Sie zum Dokumentbereich, um ein Dokument hochzuladen.
* Anzeigen von Arbeitselementdetails und Aktualisieren benutzerdefinierter Felder
Workfront-Administratoren können anpassen, welche Felder in der Zusammenfassung in der Layoutvorlage angezeigt werden. Weitere Informationen finden Sie unter [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Status des Arbeitselements ändern
* Unteraufgaben anzeigen
* Zeit erfassen
* Angehängte Genehmigungsprozesse anzeigen

Um die Zusammenfassung zu öffnen, bewegen Sie den Mauszeiger über das Arbeitselement und klicken Sie dann auf das Symbol **Zusammenfassung** ![](assets/open-summary-new-home.png).

Weitere Informationen zur Verwendung des Bedienfelds &quot;Zusammenfassung&quot;finden Sie unter [Übersicht &quot;Zusammenfassung&quot;](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

## Verwenden von Schnellaktionen zum Aktualisieren von Arbeitselementen

Sie können das Schnellaktionsmenü verwenden, um

* Zeit erfassen
* Aktualisieren hinzufügen
* Benutzerdefiniertes Formular aktualisieren
* Datei hochladen

Um das Schnellaktionsmenü zu finden, halten Sie den Mauszeiger über das Arbeitselement. Die Liste der Schnellaktionen wird neben der Schaltfläche **Bearbeiten** oder **Fertig** angezeigt.

![](assets/quick-actions-new-home.png)


## Anzeigen von Genehmigungen und Teamanfragen

Genehmigungen und Teamanfragen werden nicht im Widget Meine Arbeit angezeigt. Wenn Sie regelmäßig mit Genehmigungen und Teamanfragen arbeiten, empfehlen wir, die folgenden Widgets zu Ihrer neuen Startseite hinzuzufügen:

* Warten auf Genehmigung
* Alle Genehmigungen
* Team-Anforderungen

Weitere Informationen zum Hinzufügen von Widgets zur neuen Startseite finden Sie unter [Hinzufügen, Bearbeiten oder Entfernen von Widgets in der neuen Startseite](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).




