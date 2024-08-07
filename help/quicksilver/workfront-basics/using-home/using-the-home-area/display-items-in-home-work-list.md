---
product-area: projects
navigation-topic: use-the-home-area
title: Anzeigen von Elementen in der [!UICONTROL Arbeitsliste] im Startbereich
description: Die [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] zeigt alle Arbeitselemente an, die Ihnen zugewiesen sind. Sie können steuern, welche Elemente in Ihrer [!UICONTROL Arbeitsliste] angezeigt werden, indem Sie Filter verwenden und Ihre Arbeitselemente gruppieren und sortieren.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1837'
ht-degree: 0%

---

# Elemente in der [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] anzeigen

<!-- Audited: 1/2024 -->


Die [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] zeigt alle Arbeitselemente an, die Ihnen zugewiesen sind. Sie können steuern, welche Elemente in Ihrer [!UICONTROL Arbeitsliste] angezeigt werden, indem Sie Filter verwenden und Ihre Arbeitselemente gruppieren und sortieren.

>[!NOTE]
>
>* Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird das Problem aus dem Startbereich des dem Problem zugewiesenen Benutzers entfernt.
>
>* Beim Konvertieren einer Aufgabe in ein Projekt wird die Aufgabe gelöscht und aus dem Startbereich des der Aufgabe zugewiesenen Benutzers entfernt.


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
   <td> <p>Neu:</p><ul><li>[!UICONTROL Mitarbeiter] nur für Genehmigungen</li> <li>[!UICONTROL Standard] oder höher für alle anderen Objekte</li> <p>Oder</p> 
  </ul><p>Aktuell:</p><ul><li>[!UICONTROL Review] nur für Genehmigungen</li> <li>[!UICONTROL Arbeit] oder höher für alle anderen Objekte</li> </td> 
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

## Filtern der [!UICONTROL Arbeitsliste]

Sie können Elemente in der [!UICONTROL Arbeitsliste] filtern, um nur bestimmte Elementtypen anzuzeigen. Sie können beispielsweise die [!UICONTROL Arbeitsliste] filtern, um nur Probleme oder Anforderungen anzuzeigen.

>[!NOTE]
>
>Die Filteroptionen werden im Browser gespeichert. Wenn Sie denselben Browser auf demselben Computer verwenden (und die Site-Daten nicht löschen), ändern sich die ausgewählten Filter nicht. Wenn Sie Browser oder Computer wechseln, kehren die Filter zur Standardoption zurück, bei der alle Filter deaktiviert sind.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Startseite]**.
1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Filter]** ![](assets/filter-nwepng.png) . Wenn Filter ausgewählt sind, wird die Anzahl der ausgewählten Filter anstelle des Symbols angezeigt.
1. Wählen Sie aus den folgenden Filteroptionen aus, um den Typ der anzuzeigenden Elemente anzugeben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Zeigt alle Elemente an und wählt sie aus. Dazu gehören Aufgaben, Probleme, Genehmigungen, persönliche Aufgaben sowie abgeschlossene Aufgaben und Probleme. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aufgaben: Arbeiten am]</strong></td> 
      <td> <p>Zeigt nur Aufgaben an, an denen Sie aktiv arbeiten. Hierbei handelt es sich um Aufgaben, die Ihnen zugewiesen sind und für die Sie auf die Schaltfläche [!UICONTROL Bearbeiten] geklickt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aufgaben: Bereit zum Start]</strong></td> 
      <td> 
       <div> 
        <p>Zeigt nur Aufgaben an, die für den Start bereit sind. Beide der folgenden Anweisungen müssen wahr sein:</p> 
        <ul> 
         <li> <p>Die Aufgaben und ihre Eltern haben keine Vorgänger oder Aufgabeneinschränkungen, die sie daran hindern, daran gearbeitet zu werden.</p> </li> 
         <li> <p>Das geplante [!UICONTROL Startdatum] der Aufgaben liegt in der Vergangenheit oder bis zu zwei Wochen in der Zukunft.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aufgaben: Nicht bereit]</strong></td> 
      <td> 
       <div> 
        <p>Zeigt nur Aufgaben an, die noch nicht startbereit sind. Jede der folgenden Anweisungen muss "true"lauten:</p> 
        <ul> 
         <li> <p>Die Aufgaben und ihre Eltern haben möglicherweise Vorgänger oder Aufgabeneinschränkungen, die deren Bearbeitung verhindern.</p> </li> 
         <li> <p>Die Aufgaben verfügen über ein [!UICONTROL Geplantes Startdatum], das in Zukunft mehr als zwei Wochen beträgt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Probleme: Arbeiten am]</strong></td> 
      <td> <p>Zeigt nur Probleme an, an denen Sie aktiv arbeiten. Hierbei handelt es sich um Probleme, die Ihnen zugewiesen sind und für die Sie auf die Schaltfläche [!UICONTROL Bearbeiten] geklickt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Probleme: angefordert]</strong></td> 
      <td>Zeigt nur Probleme an, denen Sie zugewiesen sind, für die Sie jedoch nicht auf die Schaltfläche [!UICONTROL Bearbeiten] geklickt haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Persönlich</strong></td> 
      <td>Zeigt nur persönliche Aufgaben an. Dies sind Aufgaben, die Sie als [!UICONTROL Aufgaben]-Aufgabe erstellen, wie im Abschnitt <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Erstellen einer persönlichen Aufgabe</a> im Artikel <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Arbeitselemente aus dem [!UICONTROL Home]-Bereich erstellen</a> beschrieben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Validierungen]</strong></td> 
      <td> 
       <div> 
        <p>Zeigt nur die Ihnen zugewiesenen oder zugewiesenen Genehmigungen und die von Ihnen eingereichten Genehmigungen an. Zu den Genehmigungen gehören Genehmigungen für Arbeitselemente (Projekte, Aufgaben und Probleme) sowie Genehmigungen für Dokumente, Testsendungen, Zugriffsanfragen und Timesheets. Weitere Informationen zu Genehmigungen finden Sie in den folgenden Artikeln:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Genehmigungen anzeigen</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Arbeitsgenehmigungen</a> </p> </li> 
        </ul> 
        <p>Hinweis: Die von Ihnen eingereichten Validierungen, bei denen Sie auch einer der Genehmiger sind, werden zweimal gezählt.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegiert: Delegiert von mir]</strong></td> 
      <td> 
       <div> 
        <p>Zeigt nur Arbeitselemente an, die Sie einem anderen Benutzer zugewiesen haben.</p> 
        <p>Weitere Informationen zum Delegieren von Aufgaben finden Sie unter <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delegieren von Aufgaben und Problemen an einen anderen Benutzer</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegiert: mir zugewiesen]</strong></td> 
      <td> 
       <div> 
        <p>Zeigt nur Arbeitselemente an, die Ihnen vorübergehend von einem anderen Benutzer zugewiesen wurden.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Abgeschlossen]</strong></td> 
      <td> <p>Zeigt nur abgeschlossene Aufgaben, Probleme und persönliche Aufgaben an. Die abgeschlossene Arbeit wird für die letzten zwei Wochen angezeigt und in der Arbeitsliste nach der Woche gruppiert, in der sie abgeschlossen wurden. Genehmigungen sind nicht enthalten.</p> <p>Abgeschlossene Arbeiten werden in der [!UICONTROL Arbeitsliste] ausgeblendet, sofern Sie diesen Filter nicht auswählen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* Filteroptionen basieren auf Objekten (Aufgaben, Probleme, Genehmigungen, Persönliche Aufgaben).
   >* Aufgaben und Probleme werden weiter nach ihrem Status gefiltert, entsprechend unserer Bereitschaft, daran zu arbeiten ([!UICONTROL Arbeiten an], [!UICONTROL Bereit zum Start], [!UICONTROL Nicht bereit] für Aufgaben und [!UICONTROL Arbeiten an] und [!UICONTROL Angefordert] für Probleme). Sie können auswählen, ob Aufgaben oder Probleme in einem bestimmten Status angezeigt werden sollen, oder auf Aufgaben oder Probleme klicken, um alle Status auszuwählen und anzuzeigen.
   >* Es gibt einen separaten Filter für abgeschlossene Elemente, der sowohl Aufgaben als auch Probleme enthält. Dies umfasst keine Genehmigungen. Der Filter [!UICONTROL Abgeschlossen] enthält persönliche Aufgaben.
   >* Sie können festlegen, dass immer nur ein Status angezeigt werden soll. Beispielsweise können Sie nur [!UICONTROL Arbeiten an] Aufgaben und nur [!UICONTROL Angeforderte] Probleme anzeigen. Sie können auch mehrere Status gleichzeitig auswählen.
   >* Sie können keine Filter auf Elemente anwenden, die einem Ihrer Teams zugewiesen sind, und Teamzuweisungen sind nicht in den Elementen enthalten, die Ihnen direkt zugewiesen sind.


1. (Optional) Organisieren Sie die [!UICONTROL Arbeitsliste] weiter, wie im Abschnitt [Gruppe beschrieben, und sortieren Sie nach Datum, Projekt und Priorität](#group-and-sort-by-date-project-and-priority) in diesem Artikel.

## Gruppieren und sortieren nach [!UICONTROL Datum], [!UICONTROL Projekt] und [!UICONTROL Priorität]

Sie können die [!UICONTROL Arbeitsliste] nach dem [!UICONTROL geplanten Abschlussdatum], dem [!UICONTROL Veröffentlichungsdatum], dem [!UICONTROL Projekt] oder dem [!UICONTROL My Priority] gruppieren und sortieren. Die gewählte Option bestimmt, wie Elemente in der [!UICONTROL Arbeitsliste] gruppiert werden.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Startseite]**.
1. Klicken Sie auf das Dropdownmenü **[!UICONTROL Gruppieren nach]** ![Gruppieren nach ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Geplanter Abschluss]</strong></td> 
      <td> <p> Elemente werden in den folgenden Gruppen in der [!UICONTROL Arbeitsliste] angezeigt, je nach ihrem geplanten [!UICONTROL Abschlussdatum] (die Anzahl der in jeder Gruppierung enthaltenen Elemente wird in Klammern neben dem Überschriftentitel angezeigt):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Kein geplanter Abschlussdatum]</p> </li> 
        <li> <p>[!UICONTROL Diese Woche]</p> <p>Diese Gruppierung wird standardmäßig erweitert.</p> </li> 
        <li> <p>[!UICONTROL Nächste Woche]</p> </li> 
        <li> <p>[!UICONTROL Geplant], gefolgt von verschiedenen geplanten [!UICONTROL Abschlussdaten] (mehrere Gruppierungen)</p> </li> 
        <li> <p>[!UICONTROL Abgeschlossen]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Geplanter Start]</strong></td> 
      <td> <p>Elemente werden in den folgenden Gruppierungen in der [!UICONTROL Arbeitsliste] angezeigt, je nach ihrem geplanten [!UICONTROL Startdatum] (die Anzahl der in jeder Gruppierung enthaltenen Elemente wird in Klammern neben dem Überschriftentitel angezeigt):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Diese Woche] </p> <p>Diese Gruppierung wird standardmäßig erweitert.</p> </li> 
        <li> <p>[!UICONTROL Nächste Woche]</p> </li> 
        <li> <p>[!UICONTROL Geplant], gefolgt von verschiedenen [!UICONTROL geplanten Startdaten] (mehreren Gruppierungen)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Veröffentlichungsdatum]</strong></td> 
      <td> <p>Elemente werden in den folgenden Gruppierungen in der [!UICONTROL Arbeitsliste] angezeigt (die Anzahl der Elemente innerhalb jeder Gruppierung wird in Klammern neben dem Überschriftentitel angezeigt):</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Nächste Woche gebunden]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Projekt]</strong></td> 
      <td>Elemente werden nach Projekt gruppiert und Projekte werden alphabetisch in der [!UICONTROL Arbeitsliste] angezeigt. (Die Anzahl der Elemente in den einzelnen Gruppierungen wird in Klammern neben dem Überschriftentitel angezeigt.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>Elemente werden in der von Ihnen gewählten Reihenfolge angezeigt. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorisieren von Arbeiten im [!UICONTROL Home]-Bereich</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>Die Standardsortierung ist aufsteigend. Wenn Sie die Sortierung in absteigend ändern, werden die ausgewählten Sortieroptionen im Browser gespeichert. Wenn Sie denselben Browser auf demselben Computer verwenden (und die Site-Daten nicht löschen), ändert sich die Sortierung nicht. Wenn Sie jedoch Browser oder Computer wechseln, wird die Sortierung zur Standardsortierung geändert.

## Anzeigen verspäteter Elemente

[!DNL Adobe Workfront] verwendet die folgenden Daten, um zu ermitteln, ob Arbeitsersuchen zu spät sind:

* **Aufgaben**: [!UICONTROL Geplantes Abschlussdatum]
* **Issues**: [!UICONTROL Geplantes Abschlussdatum]
* **Dokumente**: [!UICONTROL Gesendetes Datum]
* **Timesheets**: [!UICONTROL Gesendetes Datum]
* **Genehmigungen**: [!UICONTROL Gesendetes Datum]
* **Genehmigungen für Testversand**: [!UICONTROL Frist für den Testversand]

## Durchsuchen der [!UICONTROL Arbeitsliste]

Wenn Sie die [!UICONTROL Arbeitsliste] durchsuchen, werden alle Ihnen zugewiesenen Elemente bei der Suche zurückgegeben (auch Elemente, die derzeit nicht auf dem Bildschirm geladen sind). Wenn die Option [!UICONTROL Abschluss anzeigen] ausgewählt ist, werden auch alle Elemente zurückgegeben, die Sie in den letzten zwei Wochen als vollständig markiert haben.

Darüber hinaus werden nur die Namen der Arbeitselemente durchsucht (Informationen innerhalb des Arbeitselements werden nicht durchsucht, ebenso nicht die Namen der Projekte, in denen sich das Arbeitselement befindet).

So durchsuchen Sie die [!UICONTROL Arbeitsliste]:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Startseite]**.
1. (Optional) Filtern und gruppieren Sie die [!UICONTROL Arbeitsliste], wie unter [Filtern der [!UICONTROL Arbeitsliste]](#filter-the-work-list) und der [Gruppe und sortieren Sie nach Datum, Projekt und Priorität](#group-and-sort-by-date-project-and-priority).

1. (Optional) Wenn Sie nach einem Arbeitselement suchen, das bereits abgeschlossen ist, müssen Sie die [!UICONTROL Arbeitsliste] so konfigurieren, dass vor der Suche abgeschlossene Elemente angezeigt werden.

1. Klicken Sie auf das Suchsymbol ![Suche](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Beginnen Sie mit der Eingabe des Namens des gesuchten Elements.\
   Die [!UICONTROL Arbeitsliste] wird automatisch gefiltert, um Elemente mit einem übereinstimmenden Namen einzuschließen.

## Größe der Arbeitsliste ändern

Sie können die Größe der [!UICONTROL Arbeitsliste] so ändern, dass sie zwischen etwa einem Viertel des Startbereichs und etwa der Hälfte des Bereichs [!UICONTROL Home] verbraucht.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Startseite]**.
1. Bewegen Sie den Mauszeiger über den rechten Rand der [!UICONTROL Arbeitsliste] und ziehen Sie dann nach links oder rechts, bis die Arbeitsliste die gewünschte Größe aufweist.

## Reduzieren und Erweitern von Gruppierungen

Elemente in der [!UICONTROL Arbeitsliste] werden innerhalb von Gruppierungen angezeigt. Sie können Gruppierungen reduzieren und erweitern, um zu steuern, wie viele Informationen zu einem bestimmten Zeitpunkt auf der Seite angezeigt werden.

Sie können Gruppierungen in der [!UICONTROL Arbeitsliste] reduzieren und erweitern, um besser steuern zu können, welche Informationen sichtbar sind.\
Standardmäßig wird die Gruppierung [!UICONTROL Diese Woche] erweitert und alle anderen Gruppierungen werden reduziert. Alle Änderungen, die Sie vornehmen, werden beim nächsten Zugriff auf den Startbereich gespeichert.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Startseite]**.
1. Klicken Sie auf den Pfeil **[!UICONTROL Erweitern]** oder **[!UICONTROL Reduzieren]** neben allen Gruppen, die Sie erweitern oder reduzieren möchten.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Oder\
   Um alle Gruppierungen gleichzeitig zu erweitern oder zu reduzieren, klicken Sie auf den Pfeil **[!UICONTROL Erweitern]** oder **[!UICONTROL Reduzieren]** neben einer beliebigen Gruppierung, während Sie die Taste [!UICONTROL Umschalt] gedrückt halten.
