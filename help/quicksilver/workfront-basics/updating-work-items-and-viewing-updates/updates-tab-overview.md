---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Übersicht über den Aktualisierungsabschnitt
description: Im Abschnitt Updates werden bis zu 200 der letzten Aktualisierungen angezeigt, die in den letzten 90 Tagen vorgenommen wurden.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# Übersicht über den Aktualisierungsabschnitt

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

Im Abschnitt &quot;Updates&quot;eines Objekts werden Kommentare angezeigt, die Benutzer zum Objekt oder zu Systemaktualisierungen vornehmen, die Änderungen am Objekt verfolgen.

## Überblick über den Abschnitt &quot;Aktualisierungen&quot;

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

Der Abschnitt Updates eines Objekts zeigt bis zu 200 der letzten Aktualisierungen an, die in den letzten 90 Tagen vorgenommen wurden.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

Im Abschnitt Updates werden die folgenden Informationen angezeigt:

* Stellungnahmen von Verwendern und Antworten auf diese Stellungnahmen.
* Systemaktualisierungen, bei denen es sich um Informationsmeldungen handelt, die Workfront erstellt, um bestimmte Ereignisse auf einem Objekt aufzuzeichnen. Sie können beispielsweise Änderungen an Status, Namen oder benutzerdefinierten Feldern mit Systemaktualisierungen erfassen. Ihr Workfront- oder Gruppenadministrator kann Systemaktualisierungen für Ihre Objekte aktivieren. Weitere Informationen finden Sie unter [Systemaktualisierungen konfigurieren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Der Abschnitt Updates wird für die folgenden Objekte angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Dokumente</li> 
     <li>Ziele</li> 
     <li>Probleme</li> 
     <li>Wiederholungen</li> 
     <li>Projekte</li> 
     <li>Programme</li> 
     <li>Portfolios</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Storys</li> 
     <li>Aufgaben</li> 
     <li>Vorlagen</li> 
     <li>Vorlagenaufgaben</li> 
     <li>Arbeitszeittabellen</li> 
     <li>Benutzende</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Aktualisierungen, die auch bei Objekten mit höherem Rang angezeigt werden

Wie in der folgenden Tabelle dargestellt, erscheinen Antworten auf Aktualisierungen bestimmter Objekte auch im Abschnitt Updates von Objekten mit höherem Rang.

Wenn Sie beispielsweise einer Aufgabe eine Aktualisierung hinzufügen, wird die Aktualisierung im Abschnitt Updates für die Aufgabe und im Abschnitt Updates für das Projekt, das die Aufgabe enthält, angezeigt.

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
   <td>Problem</td> 
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

<tr> 
   <td>Ziele</td> 
   <td>Ergebnis, Aktivität</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Antworten, die zu Systemaktualisierungen hinzugefügt werden, werden nicht auf das übergeordnete Objekt aktualisiert. Nur direkte Antworten auf ein untergeordnetes Objekt und Antworten, die zu vorhandenen Updates hinzugefügt werden, werden zu übergeordneten Objekten aggregiert.
>
>Informationen zur Objekthierarchie in Adobe Workfront finden Sie unter [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Einschränkungen des Abschnitts Updates

### Einschränkungen für Benutzer und Teams

Sie können keine Aktualisierungen für Teams vornehmen. Im Abschnitt Updates für Teams werden die in den folgenden Objekten eingegebenen Aktualisierungen angezeigt:

* Benutzende
* Arbeitszeittabellen
* Storys
* Wiederholungen

Im Abschnitt Updates für Benutzer und Teams können Sie die Aktualisierungen anzeigen, die in den letzten 90 Tagen vorgenommen wurden.

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
