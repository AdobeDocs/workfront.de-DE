---
navigation-topic: use-lists
title: Erste Schritte mit Listen in [!DNL Adobe Workfront]
description: Sie können Listen von -Objekten in anzeigen [!DNL Adobe Workfront]  um Informationen über sie zu erhalten, z. B. ihr Start- und Fälligkeitsdatum, ihnen zugewiesene Benutzer und andere Objekte, die mit ihnen verknüpft sind.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: f0b3b8aa64fa0b03a196bbcc2bdd037eeeb0f89e
workflow-type: tm+mt
source-wordcount: '2275'
ht-degree: 1%

---

# Erste Schritte mit Listen in [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Sie können Listen von Objekten in [!DNL Adobe Workfront] anzeigen, um Informationen zu ihnen zu erhalten, z. B. ihr Start- und Fälligkeitsdatum, ihnen zugewiesene Benutzer und andere Objekte, die mit ihnen verknüpft sind.

Im Folgenden finden Sie einige Merkmale von Listen in [!DNL Workfront]:

* Listen werden automatisch alle fünf Minuten aktualisiert, um Informationen zu aktualisieren, die andere Benutzende im System an anderer Stelle aktualisieren.
* Einige Bereiche in [!DNL Workfront] sind mit standardmäßigen Objektlisten vorkonfiguriert.

  Sie können die meisten dieser vorkonfigurierten Listen anpassen.

* Ein [!DNL Workfront] kann benutzerdefinierte Listen erstellen, die auf verschiedene Bereiche von [!DNL Workfront] angewendet werden können.

  Weitere Informationen zum Erstellen von Listen auf Systemebene finden Sie im Artikel [Erstellen, Bearbeiten und Freigeben von Standardfiltern, -ansichten und -gruppierungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für einen Filter, eine Ansicht oder eine Gruppierung mit Zugriff auf die Freigabe </p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL View] or higher access to filters, views, groupings</p> <P>For items in the [!UICONTROL Setup] area, you need administrative access for the item or the [!UICONTROL System Administrator] access level.</P> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level.<br>For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] or higher permissions with access to share</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.
-->

## Objektlisten

Im Folgenden finden Sie einige Objektlisten, die Sie in [!DNL Workfront] finden können, sowie einige der Bereiche, in denen sie standardmäßig angezeigt werden, wenn Sie über die Berechtigung zum Anzeigen eines Objekts verfügen.

>[!NOTE]
>
>* Diese Liste ist nicht vollständig. Jede dieser Objektlisten kann auch in einem Bericht oder Dashboard angezeigt werden. Beispielsweise zeigt ein Projektbericht oder ein Dashboard, der bzw. das einen Projektbericht enthält, auch eine Liste der Projekte an.
>* In dieser Liste bedeutet „Auswählen“, dass Sie auf den Namen des Elements klicken müssen, nicht auf das Kontrollkästchen links neben dem Namen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Speicherort der Objektliste</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Liste der Portfolios</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Programme</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Projektliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL -Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme] &gt;[!UICONTROL Programm auswählen] &gt;[!UICONTROL Projekte]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt; [!UICONTROL Aufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Teilaufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Vorgänger*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Problemliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt;[!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Unteraufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Probleme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Berichte</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Berichte]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Dashboards</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Iterationen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterationen]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Benutzerliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Benutzer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Dokumente</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL -Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme] &gt;[!UICONTROL Programm auswählen] &gt;[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL -Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL -Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL select] ein Projekt &gt; [!UICONTROL Probleme] &gt;[!UICONTROL Problem auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Arbeitszeittabellen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Arbeitszeittabelle] s &gt; [!UICONTROL Alle Arbeitszeittabellen]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Abrechnungssätze</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Abrechnungssätze*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Rechnungsnachweise</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt; [!UICONTROL Rechnungsnachweise]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Risiken</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Risiken]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ausgabenliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL -Projekte] &gt; Projekt auswählen &gt;[!UICONTROL -Ausgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Ausgaben]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Stundeneinträge</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; Projekt auswählen</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Stunden]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL select] ein Projekt &gt;[!UICONTROL Probleme] &gt;[!UICONTROL select] ein Problem &gt;[!UICONTROL Stunden]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der benutzerdefinierten Formulare</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Setup] &gt;[!UICONTROL Custom Forms] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Liste der Gruppen oder Untergruppen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL select the parent group] &gt;[!UICONTROL subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Teamliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Gesellschaften</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Firmen]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Zeitpläne</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Zeitpläne]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Layout-Vorlagen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Layout-Vorlagen]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Die Liste kann nicht im angegebenen Bereich angepasst werden. Ein [!DNL Workfront] kann eine benutzerdefinierte Liste auf Systemebene erstellen oder einen Bericht für dieses Objekt erstellen, wenn Sie auf Zugriffsebene Zugriff zum Bearbeiten von Berichten haben.

## Listenelemente

Eine Liste enthält bestimmte Elemente, die ihr Format und die angezeigten Informationen definieren. Es gibt mehrere Systemlistenelemente, die standardmäßig verfügbar sind. Sie können auch benutzerdefinierte Elemente erstellen, um Ihre Anforderungen zu erfüllen.

>[!NOTE]
>
>Wenn Sie einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung aus einer Liste auswählen, wird diese Auswahl auch dann beibehalten, wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen.

Eine Liste umfasst die folgenden Elemente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Element</strong></th> 
   <th><strong>Erklärung</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL filter]</strong></td> 
   <td> <p>Filter verhindern basierend auf den von Ihnen angegebenen Kriterien unnötige Informationen aus einer Liste. </p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filter - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL -Ansicht]</strong></td> 
   <td> <p>In Ansichten wird festgelegt, welche Felder (Spalten) auf dem Bildschirm angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Ansichten - Übersicht in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL -Gruppierung]</strong></td> 
   <td> <p>Gruppierungen trennen die Objekte auf der Liste in Bereiche basierend auf den von Ihnen angegebenen Kriterien.</p> <p>Beispielsweise können die Probleme in einer Liste in Abschnitten nach Status oder Priorität angezeigt werden.</p> <p>In einer Standardgruppierung können bis zu drei Ebenen von Gruppierungen vorhanden sein. Wenn Sie im Textmodus eine Gruppierung konfigurieren, können Sie eine vierte Ebene hinzufügen.</p> <p>Weitere Informationen zu Gruppierungen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Gruppierungen - Übersicht in [!DNL Adobe Workfront]</a>.</p> <p>Weitere Informationen zum Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Textmodus - Übersicht</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Diese Elemente werden standardmäßig oben in jeder Liste angezeigt. Sie bleiben haften und bewegen sich nicht, wenn Sie durch die Liste scrollen. Bewegen Sie den Mauszeiger über das Symbol für jedes Element, um es zu identifizieren.

![Listenelemente](assets/nwe-list-elements.png)

Sie können Listenelemente in den folgenden Bereichen anpassen und für andere Benutzer freigeben:

* Jede standardmäßige Systemliste, die im Abschnitt [Erste Schritte mit Listen in [!DNL Adobe Workfront]](#default-workfront-lists) in diesem Artikel gefunden wird
* Alle Berichte, die für Sie freigegeben wurden

Die Bauelemente für Listen sind die gleichen wie die Bauelemente für Berichte.

Weitere Informationen zum Erstellen und Anpassen der Erstellungselemente von Listen und Berichten finden Sie [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Aktionen auflisten

Sie können die folgenden Aktionen in einer Liste abschließen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong></th> 
   <th><strong>Information</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Inline-Bearbeitung</strong> </td> 
   <td> <p>Objekte und deren Informationen direkt in der Liste bearbeiten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Inline-Bearbeitung von Elementen in einer Liste in [!DNL Adobe Workfront]</a>.</p> 
   <p><b>HINWEIS:</b></p>
   <p>In einer Gruppierung ist keine Inline-Bearbeitung möglich.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Aktualisierung mit der [!UICONTROL Summary]</strong> </td> 
   <td> <p>Aktualisieren Sie Aufgaben und Probleme auf Projektebene mithilfe des Bedienfelds [!UICONTROL Zusammenfassung].</p> <p><b>TIPP:</b></p> <p>Die Zusammenfassung ist nicht für alle Objekte verfügbar und auch nicht in Aufgaben- oder Problemberichten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Listenanzeige anpassen</strong> </td> 
   <td> <p>Passen Sie das Erscheinungsbild einer Liste, die Spaltenanordnung, die Sortierreihenfolge der Elemente oder die Anzahl der angezeigten Elemente an.</p> <p><b>HINWEIS:</b></p> <p>Änderungen an der Anzahl der Elemente, die auf einer Seite angezeigt werden sollen, werden rückgängig gemacht, wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen. Änderungen können auch nach einem Zeitraum von 8 Stunden rückgängig gemacht werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Ändern der Anzeige einer Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Schnellfilter</strong> </td> 
   <td> <p>Wenden Sie einen Schnellfilter an, um nur Elemente zu finden, die für Sie wichtig sind, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.</p> <p><b>WICHTIG:</b></p> <p> Sie können Elemente, die ein Suchwort enthalten, mithilfe des Schnellfilters finden, unabhängig davon, ob dieses Element auf Ihrem Bildschirm sichtbar ist oder angezeigt wird, nachdem Sie zum unteren Seitenrand gescrollt haben. Wenn Sie die Suchfunktionen Ihres Browsers verwenden, können Sie nur Elemente finden, die bereits auf dem Bildschirm sichtbar sind. Wenn Ihre Liste mehrere Seiten umfasst, finden Schnellfilter nur die Elemente auf der aktuellen Seite.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Anwenden des Schnellfilters auf eine Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportieren</strong> </td> 
   <td> <p>Exportiert eine Objektliste aus [!DNL Workfront]. Wenn eine Liste mehr als 2.000 Elemente enthält, ist der Export der Liste die einzige Möglichkeit, alle Elemente auf einer Seite zu überprüfen.</p> <p>Weitere Informationen zum Exportieren einer Liste finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Liste exportieren</a>. Weitere Informationen zu Exportformaten und -beschränkungen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportieren von Daten</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Listen-Symbolleiste

In der folgenden Tabelle werden viele der in der Symbolleiste verfügbaren Symbole aufgelistet und angegeben, was passiert, wenn Sie darauf klicken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Symbol</strong></td> 
   <td><strong>Beschreibung</strong></td> 
   <td><strong>Bei Klick</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Element oder Benutzer hinzufügen]</td> 
   <td>Öffnen Sie weitere Optionen, einschließlich eines neuen Elements oder Benutzers.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgabe oben einfügen]</td> 
   <td> <p>Aufgabe oberhalb der ausgewählten Aufgabe einfügen.</p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgabe unten einfügen]</td> 
   <td> <p>Fügt eine Aufgabe unterhalb der ausgewählten Aufgabe ein.</p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Bearbeiten]</td> 
   <td>Das ausgewählte Element bearbeiten.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Kopiert das ausgewählte Element.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Löschen]</td> 
   <td>Löscht das ausgewählte Element.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Hinzufügen zu]</td> 
   <td> <p>Öffnen Sie das Dialogfeld, um das ausgewählte Problem zu einer Iteration hinzuzufügen.</p> <p>Dies ist nur für Probleme verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Freigabe]</td> 
   <td>Freigeben des ausgewählten Elements.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgaben einrücken und ausrücken] </td> 
   <td> <p>Ausgewählte Aufgabe ein- oder ausrücken. </p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Mehr]</td> 
   <td>Zusätzliche Optionen für das ausgewählte Element öffnen.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Schnellfilter] </p> </td> 
   <td> <p>Öffnen Sie das Schnellfilter-Suchfeld, um Elemente in der angezeigten Liste zu finden.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL -Export]</td> 
   <td>Exportieren Sie die Liste in Dateien mit PDF, Excel oder Tabulatoren.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Zeigt die Liste in der Agile-Ansicht an.<br>Dies ist nur für Aufgaben verfügbar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt-Diagramm]</td> 
   <td> <p>Liste in der Ansicht [!UICONTROL Gantt-Diagramm] anzeigen.</p> <p>Dies ist nur für Projekte und Aufgaben verfügbar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Filter]</td> 
   <td> <p>Zeigt eine Liste von Filtern und zusätzliche Optionen zum Verwalten von Filtern an, einschließlich der Erstellung von Filtern. </p> <p>Auf einem kleinen Bildschirm wird der Filtername durch das Filtersymbol ersetzt. Wenn Sie einen anderen Filter als "[!UICONTROL All]" anwenden, wird auf dem Filtersymbol ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL Ansicht] Dropdown-Menü</td> 
   <td> <p>Anzeigen einer Liste von Ansichten und zusätzlichen Optionen zum Verwalten von Ansichten, einschließlich der Erstellung einer Ansicht. </p> <p>Auf einem kleinen Bildschirm wird der Name der Ansicht durch das Symbol [!UICONTROL view] ersetzt. Wenn Sie eine andere Ansicht als "[!UICONTROL Standard]" anwenden, wird auf dem Symbol [!UICONTROL Ansicht] ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Gruppierung]</td> 
   <td> <p>Zeigt eine Liste von Gruppierungen und zusätzliche Optionen zum Verwalten von Gruppierungen an, einschließlich der Erstellung einer Gruppierung. </p> <p>Auf einem kleinen Bildschirm wird der Gruppierungsname durch das Symbol [!UICONTROL grouping] ersetzt. Wenn Sie eine andere Gruppierung als "[!UICONTROL Nothing]" anwenden, wird auf dem Symbol [!UICONTROL Gruppierung] ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Planmodus]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie die Änderungen, die Sie in einer Aufgabenliste vornehmen, automatisch oder manuell speichern möchten. </p> <p>Informationen zum Bearbeiten von Aufgaben in einer Liste finden Sie unter <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Bearbeiten von Aufgaben in einer Liste</a>. </p> <p>Dies ist nur für Aufgaben verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Zusammenfassung]</td> 
   <td> <p>Zeigt das Feld [!UICONTROL Zusammenfassung] für das ausgewählte Element an oder blendet es aus.</p> <p>Dies ist nur für Aufgaben und Probleme verfügbar.</p> <p>Informationen zum Bedienfeld [!UICONTROL Summary] finden Sie unter <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL entfernen]</td> 
   <td>Entfernen Sie etwas aus der Liste. Als Gruppenadministrator bzw. -administratorin, der Gruppen- oder Untergruppenmitgliedschaften verwaltet, entfernen Sie beispielsweise ein Gruppenmitglied, wie unter <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Anzeigen und Verwalten der Gruppenmitgliedschaften</a> beschrieben.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL -Kommentar] /[!UICONTROL -Update]</td> 
   <td> <p>Geben Sie einen Kommentar oder eine Aktualisierung ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Der Unterschied zwischen Listen und Berichten

Sowohl Listen als auch Berichte sind Raster, die Informationen zu einem Objekttyp enthalten.

In der folgenden Tabelle sind die Ähnlichkeiten und Unterschiede zwischen Listen und Berichten aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funktionalität</strong> </th> 
   <th><strong>Liste</strong> </th> 
   <th><strong>Bericht</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Jeder kann sie erstellen</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nur ein [!DNL Workfront] und Benutzer mit einer [!UICONTROL Plan]-Lizenz können sie erstellen</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Ein Standardsatz ist verfügbar unter [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Im Standardmodus anpassbar</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Im Textmodus anpassbar</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie für andere Benutzer freigeben</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie systemweit freigeben</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie außerhalb des Systems freigeben</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können in Formate exportieren, die durch PDF, [!DNL Excel] und Tabulatoren getrennt sind</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können den Versand in einer E-Mail planen</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können zu einer Layout-Vorlage hinzufügen</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie zu benutzerdefinierten Abschnitten hinzufügen </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie zu einem Dashboard hinzufügen</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können Eingabeaufforderungen verwenden, um anzupassen, was sie anzeigen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie in einem Diagramm anzeigen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können Objekte darin inline bearbeiten</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen haben, um sie erstellen zu können. Weitere Informationen finden Sie unter [Zugriff auf Filter, Ansichten und Gruppierungen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen sowie auf Berichte, Dashboards und Kalender haben, um sie erstellen zu können. Weitere Informationen finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Sie können Listen für Berichte, die in einem Dashboard platziert werden, nur anpassen, wenn der Ersteller des Berichts die Listenelemente so konfiguriert hat, dass sie im Dashboard sichtbar sind.

>[!NOTE]
>
>Sie können keine Liste zu einem Dashboard hinzufügen, ohne zuvor einen Bericht zu erstellen und ihn zum Dashboard hinzuzufügen.

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Informationen zum Erstellen benutzerdefinierter Abschnitte finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Der Unterschied zwischen den aktualisierten und den alten Listen

In [!DNL Workfront] gibt es zwei Arten von Listen:

* Legacy-Listen

  ![Blaue Gruppierungen](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Aktualisierte Listen

  ![Graue Gruppierungen](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Die folgende Tabelle zeigt einige der Unterschiede zwischen den alten und den aktualisierten Listen in [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Legacy-Listen</b></td> 
   <td><b>Aktualisierte Listen</b></td> 
  </tr> 
  <td> <p>Standardmäßig <strong>100</strong> Elemente anzeigen</p> </td> 
   <td> <p>Standardmäßig <strong> (alle</strong> oder bis <strong>2000</strong> Elemente angezeigt</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwenden Sie Strg+F, um Elemente in einer Liste zu finden</p> </td> 
   <td> <p>Verwenden Sie Schnellfilter, um Informationen in einer großen Liste schnell zu finden</p> <p>Informationen zur Verwendung von Schnellfiltern in Listen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Anwenden des Schnellfilters auf eine Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Felder können nicht inline mit Rich-Text-Formatierung bearbeitet werden.</td> 
   <td> <p>Text in benutzerdefinierten Feldern mit Formatierung kann so konfiguriert werden, dass fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierungen, Hyperlinks und Blockanführungszeichen zulässig sind.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Bedingte Formatierung kann die Textfarbe von Links in einer Liste ändern</td> 
   <td>Änderungen der Textfarbe können nicht auf Links in einer Liste angewendet werden</td> 
  </tr> 
 </tbody> 
</table>
