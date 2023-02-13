---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Übersicht über die Updates-Registerkarte
description: Der Tab Updates enthält bis zu 200 der letzten Updates, die in den letzten 90 Tagen vorgenommen wurden.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 799a2f3463ee98d57b13edfda8a0c93629439ea3
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 6%

---

# Übersicht über die Updates-Registerkarte

Der Tab Updates enthält bis zu 200 der letzten Updates, die in den letzten 90 Tagen vorgenommen wurden. Sie können auf Aktualisierungen der folgenden Objekte antworten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Projekte</li> 
     <li>Portfolios</li> 
     <li>Programme</li> 
     <li>Vorlagen</li> 
     <li>Vorlagenaufgaben</li> 
     <li>Aufgaben</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Probleme</li> 
     <li>Wiederholungen</li> 
     <li>Storys</li> 
     <li>Benutzer</li> 
     <li>Dokumente</li> 
     <li>Arbeitszeittabellen</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Aktualisierungen, die auch bei Objekten mit höherem Rang angezeigt werden

Wie in der folgenden Tabelle dargestellt, erscheinen Antworten auf Aktualisierungen bestimmter Objekte auch auf der Registerkarte Updates von Objekten mit höherem Rang.

Wenn Sie beispielsweise einer Aufgabe eine Aktualisierung hinzufügen, wird die Aktualisierung für die Aufgabe auf der Registerkarte Updates und für das Projekt, das die Aufgabe enthält, auf der Registerkarte Updates angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objekt, dem die ursprüngliche Aktualisierung hinzugefügt wurde</strong> </th> 
   <th> <p><strong>Objekt mit einer höheren Rangfolge, bei dem die ursprüngliche Aktualisierung ebenfalls angezeigt wird</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Anfrage</td> 
   <td>Projekt</td> 
  </tr> 
  <tr> 
   <td>Aufgabe</td> 
   <td>Projekt</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Programm, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Dokument </td> 
   <td>Objekt, an das das Dokument angehängt ist, Projekt </td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>Portfolio</td> 
  </tr> 
  <tr> 
   <td>Benutzer</td> 
   <td>Team</td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle</td> 
   <td>Benutzer, Team</td> 
  </tr> 
  <tr> 
   <td>Vorlagenaufgabe</td> 
   <td>Vorlage</td> 
  </tr> 
  <tr> 
   <td>Story</td> 
   <td>Iteration, Team</td> 
  </tr> 
  <tr> 
   <td>Wiederholung</td> 
   <td>Team</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Antworten, die zu Systemaktualisierungen hinzugefügt werden, werden nicht auf das übergeordnete Objekt aktualisiert. Nur direkte Antworten auf ein untergeordnetes Objekt und Antworten, die zu vorhandenen Updates hinzugefügt werden, werden zu übergeordneten Objekten aggregiert.

Informationen zur Objekthierarchie in Adobe Workfront finden Sie unter [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Einschränkungen der Registerkarte Aktualisierungen

### Einschränkungen für Benutzer und Teams

Sie können keine Aktualisierungen für Teams vornehmen. Auf der Registerkarte Updates für Teams werden die Aktualisierungen für die folgenden Objekte angezeigt:

* Benutzer
* Arbeitszeittabellen
* Storys
* Wiederholungen

Auf der Registerkarte Updates für Benutzer und Teams können Sie die Aktualisierungen anzeigen, die in den letzten 90 Tagen vorgenommen wurden.

Wenn Sie alle Aktualisierungen sehen möchten, die über die 90-Tage-Beschränkung hinaus für einen Benutzer oder ein Team vorgenommen wurden, können Sie einen Bericht für Anmerkungen erstellen. Der Bericht sollte keinen Zeitfilter enthalten, der alle für Benutzer oder Teams vorgenommenen Aktualisierungen anzeigt. Weitere Informationen finden Sie unter [Benutzerdefinierten Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Einschränkungen bei der Eingabe von Kommentaren im Namen eines anderen Benutzers

Adobe Workfront-Administratoren und Gruppenadministratoren können sich als andere Benutzer anmelden und Aktionen in Workfront ausführen, z. B. Kommentare eingeben. (Weitere Informationen finden Sie unter [Anmelden als anderer Benutzer](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md). Alle Kommentare, die im Namen eines anderen Nutzers gemacht werden, sind auf dem Kommentar angegeben.

Ein Gruppenadministrator kann im Namen einer anderen Person Kommentare abgeben, diesen Kommentar jedoch nicht löschen. Nur ein Adobe Workfront-Administrator kann einen Kommentar löschen, den er für einen anderen Benutzer abgegeben hat.

## Systemaktualisierungen zu Arbeitselementen mit dem Journaleintragsbericht anzeigen

Der Bericht Journaleintrag zeigt Systemaktualisierungen aus dem Bereich Updates von Projekten, Aufgaben und Problemen an.

Im Bericht sehen Sie Folgendes:

* Anzahl der Statusänderungen
* Beim Löschen einer Aufgabe oder eines Problems
* Änderung der Werte in wichtigen benutzerdefinierten Feldern im Verlauf eines Projekts
* Wichtige Daten im Laufe eines Projekts
* Wenn sich die Priorität im Laufe eines Projekts geändert hat
* Wenn sich der Eigentümer eines Projekts geändert hat

Weitere Informationen finden Sie unter [Bericht zum Bereich &quot;Updates&quot;](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
