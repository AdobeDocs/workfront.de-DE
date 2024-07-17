---
title: Übersicht über die Projektbeschränkungen
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront hat Beschränkungen dafür, wie viele Objekte mit einem Projekt verknüpft werden können. Es gibt Projektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront zu verbessern.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Übersicht über die Projektbeschränkungen

Adobe Workfront hat Beschränkungen dafür, wie viele Objekte mit einem Projekt verknüpft werden können. Es gibt Projektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront zu verbessern.

Die folgenden Objekte, die mit Projekten verknüpft sind, haben die folgenden Einschränkungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Aufgaben</p></td> 
   <td>  <p>Die maximale Anzahl von Aufgaben pro Projekt beträgt 5.000. Eine Warnmeldung wird angezeigt, wenn die Anzahl der Aufgaben diesem Höchstwert entspricht. Wenn das Maximum erreicht ist, wird eine Fehlermeldung angezeigt und dem Projekt können keine zusätzlichen Aufgaben hinzugefügt werden.</p> <p>Um dieses Maximum zu vermeiden, verschieben Sie Aufgaben, die für geschlossene Aufgaben geschlossen sind, in ein anderes Projekt. Die Berichte über diese Projekte müssen möglicherweise angepasst werden.</p>

<b>WICHTIG</b>

Bei Projekten mit vielen Abhängigkeiten von Aufgaben kann die Leistung bei der Berechnung der Timeline oder bei der Arbeit im Projekt beeinträchtigt sein.

Aus diesem Grund empfehlen wir, dass die Anzahl der Aufgaben in Projekten mit komplexen Abhängigkeiten deutlich niedriger sein sollte als die maximal zulässige Anzahl von 5.000 Aufgaben.

Beispiele für Aufgabenabhängigkeiten, die die Neuberechnung der Zeitleiste des Projekts beeinflussen oder verhindern können:

<ul><li>Anzahl der untergeordneten Elemente</li>
   <li>Einzug mehrerer Ebenen von Aufgaben</li>
   <li>Anzahl der Vorgänger</li>
   <li>Mehrere Zuweisungen</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Probleme</p></td> 
   <td>  <p>Die maximale Anzahl von Problemen pro Projekt beträgt 10.000. Eine Warnmeldung wird angezeigt, wenn die Anzahl der Probleme diesem Höchstwert entspricht. Wenn das Maximum erreicht ist, wird eine Fehlermeldung angezeigt und dem Projekt können keine zusätzlichen Probleme hinzugefügt werden.</p> <p>Um dieses Maximum zu vermeiden, verschieben Sie Probleme, die für ein anderes Projekt geschlossen sind, das für geschlossene Probleme vorgesehen ist. Die Berichte über diese Projekte müssen möglicherweise angepasst werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Dauer</p></td> 
   <td> <p>Die maximale Dauer eines Projekts muss 15 Jahre betragen, damit Workfront seinen Zeitrahmen automatisch berechnet. Es wird eine Warnmeldung angezeigt, wenn sich die Projektdauer der maximalen Dauer nähert. Wenn das Maximum erreicht ist, wird eine Warnmeldung angezeigt und die automatischen Timeline-Berechnungen treten nicht mehr auf.</p> <p>Die automatischen Timeline-Berechnungen werden fortgesetzt, sobald die Dauer eines Projekts unter 15 Jahre verringert wird, indem die Daten der Aufgaben im Projekt angepasst werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Timeline-Berechnungen</p></td> 
   <td>Workfront führt keine automatischen Timeline-Berechnungen für Projekte durch, die seit 6 Monaten nicht aktualisiert wurden, und wird erst fortgesetzt, wenn eine Aktualisierung vorgenommen wurde.<p>Für Projekte, die seit 3 Monaten nicht aktualisiert wurden, führt Workfront wöchentliche statt nächtliche Zeitleistenberechnungen durch.</p><p>Informationen zum Berechnen der Projekt-Timeline finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Projektzeitpläne neu berechnen</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->