---
title: Übersicht über Projektbeschränkungen
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: In Adobe Workfront gibt es Beschränkungen für die Anzahl der Objekte, die mit einem Projekt verknüpft werden können. Es gibt Projektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront zu verbessern.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Übersicht über Projektbeschränkungen

In Adobe Workfront gibt es Beschränkungen für die Anzahl der Objekte, die mit einem Projekt verknüpft werden können. Es gibt Projektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront zu verbessern.

Die folgenden mit Projekten verknüpften Objekte weisen die folgenden Beschränkungen auf:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Aufgaben</p></td> 
   <td>  <p>Pro Projekt sind maximal 5.000 Aufgaben zulässig. Wenn sich die Anzahl der Aufgaben diesem Maximum nähert, wird eine Warnmeldung angezeigt. Wenn das Maximum erreicht ist, wird eine Fehlermeldung angezeigt und zusätzliche Aufgaben können nicht zum Projekt hinzugefügt werden.</p> <p>Um dieses Maximum zu vermeiden, verschieben Sie Aufgaben, die geschlossen sind, in ein anderes Projekt, das für geschlossene Aufgaben vorgesehen ist. Die Berichte über diese Projekte müssen möglicherweise angepasst werden.</p>

<b>WICHTIG</b>

Bei Projekten, bei denen Aufgaben stark von Abhängigkeiten abhängig sind, kann es bei der Berechnung der Zeitleiste oder bei der Arbeit im Projekt zu Leistungseinbußen kommen.

Aus diesem Grund empfehlen wir, dass die Anzahl der Aufgaben in Projekten mit komplexen Abhängigkeiten viel niedriger als die maximal zulässige Anzahl von 5.000 Aufgaben sein sollte.

Beispiele für Aufgabenabhängigkeiten, die die Neuberechnung der Zeitleiste des Projekts beeinflussen oder verhindern können:

<ul><li>Anzahl untergeordneter Elemente</li>
   <li>Mehrere Einzugsebenen für Aufgaben</li>
   <li>Anzahl der Vorgänger</li>
   <li>Mehrere Zuweisungen</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Probleme</p></td> 
   <td>  <p>Die maximale Anzahl von Problemen pro Projekt beträgt 10.000. Eine Warnmeldung wird angezeigt, wenn sich die Anzahl der Probleme diesem Maximum nähert. Wenn das Maximum erreicht ist, wird eine Fehlermeldung angezeigt und zusätzliche Probleme können nicht zum Projekt hinzugefügt werden.</p> <p>Um zu vermeiden, dass dieses Maximum erreicht wird, verschieben Sie Probleme, die geschlossen sind, in ein anderes Projekt, das für geschlossene Probleme vorgesehen ist. Die Berichte über diese Projekte müssen möglicherweise angepasst werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Dauer</p></td> 
   <td> <p>Die maximale Dauer eines Projekts muss 15 Jahre betragen, damit Workfront seinen Zeitplan automatisch berechnet. Wenn sich die Projektdauer dem Maximum nähert, wird eine Warnmeldung angezeigt. Wenn das Maximum erreicht ist, wird eine Warnmeldung angezeigt und die automatischen Zeitleistenberechnungen werden nicht mehr angezeigt.</p> <p>Die automatischen Zeitleistenberechnungen werden wieder aufgenommen, sobald die Projektdauer durch eine Anpassung der Termine der Aufgaben im Projekt auf unter 15 Jahre reduziert wird.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Zeitleistenberechnungen</p></td> 
   <td>Workfront führt keine automatischen Zeitleistenberechnungen für Projekte durch, die in den letzten sechs Monaten nicht aktualisiert wurden. Die Zeitleistenberechnungen werden erst fortgesetzt, wenn eine Aktualisierung vorgenommen wurde.<p>Für Projekte, die in den letzten drei Monaten nicht aktualisiert wurden, führt Workfront wöchentlich anstatt nachts Zeitleistenberechnungen durch.</p><p>Informationen zur Berechnung der Projektzeitleiste finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Projektzeitleisten neu berechnen</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
