---
navigation-topic: use-lists
title: Erste Schritte mit Listen in  [!DNL Adobe Workfront]
description: Sie können Listen von Objekten in  [!DNL Adobe Workfront]  anzeigen, um Informationen zu ihnen abzurufen, z. B. ihr Start- und Fälligkeitsdatum, die ihnen zugewiesenen Benutzer und andere Objekte, die ihnen zugeordnet sind.
feature: Get Started with Workfront
author: Courtney
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2301'
ht-degree: 4%

---

# Erste Schritte mit Listen in [!DNL Adobe Workfront]

<!--Audited: 12/2025-->

Sie können Listen von Objekten in [!DNL Adobe Workfront] anzeigen, um Informationen zu ihnen abzurufen, z. B. ihr Start- und Fälligkeitsdatum, ihnen zugewiesene Benutzer und andere Objekte, die ihnen zugeordnet sind.

Im Folgenden sind einige Eigenschaften von Listen in [!DNL Workfront] aufgeführt:

* Führt die automatische Aktualisierung alle fünf Minuten auf, um Informationen zu aktualisieren, die andere Benutzer im System anderswo aktualisieren.
* Einige Bereiche in [!DNL Workfront] sind mit standardmäßigen Objektlisten vorkonfiguriert.

  Sie können die meisten dieser vorkonfigurierten Listen anpassen.

* Ein [!DNL Workfront] kann benutzerdefinierte Listen erstellen, die auf verschiedene Bereiche von [!DNL Workfront] angewendet werden können.

  Weitere Informationen zum Erstellen von Listen auf Systemebene finden Sie im Artikel [Erstellen, Bearbeiten und Freigeben von Standardfiltern, -ansichten und -gruppierungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

* Im Folgenden sind die Listentypen in Workfront aufgeführt:

   * Standardlisten
   * Verbesserte Listen

  Weitere Informationen finden Sie im Abschnitt [Der Unterschied zwischen der Standardliste und der erweiterten Liste](#the-difference-between-the-standard-and-the-enhanced-lists) in diesem Artikel.

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
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigung für einen Filter, eine Ansicht oder eine Gruppierung mit Zugriff auf die Freigabe anzeigen oder höher </p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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

Im Folgenden sind einige Typen von Objektlisten aufgeführt, die Sie in [!DNL Workfront] finden können, sowie einige Bereiche, in denen sie standardmäßig angezeigt werden, wenn Sie über Rechte zum Anzeigen eines Objekts verfügen.

>[!NOTE]
>
>Diese Liste ist nicht umfassend. Jede dieser Objektlisten kann auch in einem Bericht oder in einem Dashboard angezeigt werden. Beispielsweise zeigt ein Projektbericht oder ein Dashboard, der bzw. das einen Projektbericht enthält, auch eine Liste von Projekten an.



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] list</strong></th> 
   <th><strong>Position der Objektliste</strong></th> 
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
     <li> <p>[!UICONTROL-Portfolio] &gt;[!UICONTROL auf ein Portfolio klicken] &gt;[!UICONTROL-Programme]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Projekte</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL auf ein Portfolio klicken] &gt;[!UICONTROL Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL klicken Sie auf ein Portfolio] &gt;[!UICONTROL Programme] &gt;[!UICONTROL klicken Sie auf ein Programm] &gt;[!UICONTROL Projekte]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Aufgaben</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Projekte] &gt;[!UICONTROL klicken auf ein Projekt] &gt; [!UICONTROL-Aufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL auf ein Projekt klicken] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt;[!UICONTROL Unteraufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL auf ein Projekt klicken] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt; [!UICONTROL Vorgänger*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Problemliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Klicken] Sie auf ein Projekt &gt;[!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL auf ein Projekt klicken] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt; [!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL auf ein Projekt klicken] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt;[!UICONTROL auf eine Aufgabe klicken] &gt; [!UICONTROL Probleme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste von Berichten</td> 
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
     <li> <p>[!UICONTROL Benutzende]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Dokumente</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL auf ein Portfolio klicken] &gt; [!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL auf ein Portfolio klicken] &gt;[!UICONTROL Programme] &gt;[!UICONTROL auf ein Programm klicken] &gt;[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL-Projekte] &gt;[!UICONTROL klicken auf ein Projekt] &gt;[!UICONTROL-Dokumente]</p> </li> 
     <li> <p>[!UICONTROL-Projekte] &gt;[!UICONTROL klicken auf ein Projekt] &gt;[!UICONTROL-Aufgaben] &gt;[!UICONTROL klicken auf eine Aufgabe] &gt; [!UICONTROL-Dokumente]</p> </li> 
     <li> <p>[!UICONTROL-Projekte] &gt; [!UICONTROL klicken] auf ein Projekt &gt; [!UICONTROL-Probleme] &gt;[!UICONTROL klicken auf ein Problem] &gt; [!UICONTROL-Dokumente]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Arbeitszeittabellen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Arbeitszeittabellen] &gt; [!UICONTROL-Arbeitszeittabellen]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Abrechnungssätze</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL auf ein Projekt klicken] &gt;[!UICONTROL Abrechnungssätze*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Rechnungsnachweise</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL auf ein Projekt klicken] &gt; [!UICONTROL Rechnungsnachweise]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Risiken</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Projekte] &gt;[!UICONTROL klicken auf ein Projekt] &gt;[!UICONTROL-Risiken]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Ausgaben</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL klicken] Sie auf ein Projekt &gt;[!UICONTROL Ausgaben]</p> </li> 
     <li> <p>[!UICONTROL-Projekte] &gt; [!UICONTROL klicken auf ein Projekt] &gt;[!UICONTROL-Aufgaben] &gt;[!UICONTROL klicken auf eine Aufgabe] &gt;[!UICONTROL-Ausgaben]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Stundeneinträge</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL] Klicken Sie auf ein Projekt</p> </li> 
     <li> <p>[!UICONTROL-Projekte] &gt;[!UICONTROL klicken auf ein Projekt] &gt;[!UICONTROL-Aufgaben] &gt;[!UICONTROL klicken auf eine Aufgabe] &gt;[!UICONTROL-Stunden]</p> </li> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL click] a project &gt;[!UICONTROL Issues] &gt;[!UICONTROL click] a issue &gt;[!UICONTROL Hours]</p> </li>
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
     <li> <p>[!UICONTROL-Setup] &gt;[!UICONTROL-Gruppen]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL klicken Sie auf die übergeordnete Gruppe] &gt;[!UICONTROL-Untergruppen] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Team-Liste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Unternehmen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Firmen]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Zeitpläne</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Setup] &gt;[!UICONTROL-Zeitpläne]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste der Layoutvorlagen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL-Setup] &gt;[!UICONTROL-Layoutvorlagen]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

*Sie können die Liste im angegebenen Bereich nicht anpassen. Ein [!DNL Workfront]-Administrator kann eine benutzerdefinierte Liste auf Systemebene erstellen. Sie können auch einen Bericht für dieses Objekt erstellen, wenn Sie auf der Zugriffsebene Zugriff zum Bearbeiten von Berichten haben.

## Elemente auflisten

Eine Liste enthält bestimmte Elemente, die ihr Format und die angezeigten Informationen definieren. Sie können verschiedene Systemlistenelemente finden, die standardmäßig verfügbar sind. Sie können auch benutzerdefinierte Elemente erstellen, die Ihren Anforderungen entsprechen.

>[!NOTE]
>
>Wenn Sie einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung aus einer Liste auswählen, bleibt diese Auswahl erhalten, selbst wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen.

Im Folgenden sind die Elemente einer Liste aufgeführt:

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
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>Filter verhindern, dass unnötige Informationen basierend auf den von Ihnen angegebenen Kriterien aus einer Liste entfernt werden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Übersicht über Filter</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Ansicht]</strong></td> 
   <td> <p>Ansichten definieren, welche Felder (Spalten) auf dem Bildschirm angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Übersicht über Ansichten in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Gruppierung]</strong></td> 
   <td> <p>Durch Gruppierungen werden die Objekte in der Liste anhand der von Ihnen angegebenen Kriterien in Bereiche getrennt.</p> <p>Beispielsweise können die Probleme in einer Liste in Abschnitten nach Status oder Priorität angezeigt werden.</p> <p>In einer Standardgruppierung können bis zu drei Ebenen von Gruppierungen vorhanden sein. Wenn Sie im Textmodus eine Gruppierung konfigurieren, können Sie eine vierte Ebene hinzufügen.</p> <p>Weitere Informationen zu Gruppierungen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Gruppierungen - Übersicht in [!DNL Adobe Workfront]</a>.</p> <p>Weitere Informationen zum Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Textmodus - Übersicht</a>.</p> </td> 
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

Sie können die folgenden Aktionen in einer Liste ausführen:

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
   <td> <p>Aktualisieren Sie Aufgaben und Probleme auf Projektebene mithilfe des Bedienfelds [!UICONTROL Zusammenfassung].</p> <p><b>TIPP:</b></p> <p>Die Zusammenfassung ist nicht für alle Objekte verfügbar und nicht in den Aufgaben- oder Problemberichten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Übersicht </a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Listenanzeige anpassen</strong> </td> 
   <td> <p>Sie können das Erscheinungsbild einer Liste, die Spaltenanordnung, die Sortierreihenfolge von Elementen oder die Anzahl der angezeigten Elemente anpassen.</p> <p><b>HINWEIS:</b></p> <p>Änderungen an der Anzahl der Elemente, die auf einer Seite angezeigt werden sollen, werden zurückgesetzt, wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen. Änderungen können auch nach 8 Stunden rückgängig gemacht werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Ändern der Anzeige einer Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Schnellfilter</strong> </td> 
   <td> <p>Mit einem Schnellfilter können Sie nur Elemente finden, die Ihnen wichtig sind, sodass Sie diese schnell überprüfen, aktualisieren oder für andere freigeben können.</p> <p><b>WICHTIG:</b></p> <p> Sie können nach Elementen suchen, die ein Suchwort enthalten, indem Sie den Schnellfilter verwenden, unabhängig davon, ob dieses Element auf Ihrem Bildschirm angezeigt wird oder nachdem Sie zum Ende der Seite gescrollt haben. Wenn Sie die Suchfunktionen Ihres Browsers verwenden, können Sie nur Elemente finden, die bereits auf dem Bildschirm sichtbar sind. Wenn Ihre Liste mehrere Seiten enthält, werden mit Schnellfiltern nur die Elemente auf der aktuellen Seite gesucht.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Anwenden des Schnellfilters auf eine Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Exportieren</strong> </td> 
   <td> <p>Eine Liste von Objekten aus [!DNL Workfront] exportieren. Wenn eine Liste mehr als 2000 Elemente enthält, ist das Exportieren der Liste die einzige Möglichkeit, alle Elemente auf einer Seite zu überprüfen.</p> <p>Weitere Informationen zum Exportieren einer Liste finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Exportieren einer Liste</a>. Weitere Informationen zu Exportformaten und -beschränkungen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportieren von Daten</a>.</p> </td> 
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
   <td> <p>Fügen Sie eine Aufgabe unter der ausgewählten Aufgabe ein.</p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Bearbeiten]</td> 
   <td>Bearbeiten Sie das ausgewählte Element.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>Kopieren Sie das ausgewählte Element.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Löschen]</td> 
   <td>Löschen Sie das ausgewählte Element.</td> 
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
   <td>[!UICONTROL-Export]</td> 
   <td>Exportieren Sie die Liste in PDF-, Excel- oder tabulatorgetrennte Dateien.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Zeigt die Liste in der agilen Ansicht an.<br>Diese Option ist nur für Aufgaben verfügbar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt-Diagramm]</td> 
   <td> <p>Zeigt die Liste in der [!UICONTROL Gantt Chart]-Ansicht an.</p> <p>Dies ist nur für Projekte und Aufgaben verfügbar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Filter]</td> 
   <td> <p>Zeigt eine Liste von Filtern und zusätzliche Optionen zum Verwalten von Filtern an, einschließlich der Erstellung von Filtern. </p> <p>Auf einem kleinen Bildschirm wird der Filtername durch das Filtersymbol ersetzt. Wenn Sie einen anderen Filter als "[!UICONTROL All]" anwenden, wird auf dem Filtersymbol ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL View]</td> 
   <td> <p>Zeigt eine Liste mit Ansichten und zusätzliche Optionen zum Verwalten von Ansichten an, einschließlich der Erstellung einer Ansicht. </p> <p>Auf einem kleinen Bildschirm wird der Anzeigename durch das Symbol [!UICONTROL-Ansicht] ersetzt. Ein blauer Punkt wird auf dem Symbol [!UICONTROL View] angezeigt, wenn Sie eine andere Ansicht als "[!UICONTROL Standard]" anwenden.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Grouping]</td> 
   <td> <p>Zeigt eine Liste von Gruppierungen an sowie zusätzliche Optionen zum Verwalten von Gruppierungen, einschließlich der Erstellung einer Gruppierung. </p> <p>Auf einem kleinen Bildschirm wird der Gruppierungsname durch das Symbol [!UICONTROL grouping] ersetzt. Auf dem Symbol [!UICONTROL Grouping] wird ein blauer Punkt angezeigt, wenn Sie eine andere Gruppierung als "[!UICONTROL Nothing]" anwenden.</p> </td> 
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
   <td>[!UICONTROL-Kommentar] /[!UICONTROL-Update]</td> 
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
   <td> <p>Nur ein [!DNL Workfront]-Administrator und Benutzer mit einer [!UICONTROL Plan]-Lizenz können sie erstellen.</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>Ein Standardsatz ist verfügbar unter [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Anpassbar im Standardmodus</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Anpassbar im Textmodus</p> </td> 
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
   <td> <p>Sie können die Übermittlung per E-Mail planen.</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können einer Layoutvorlage</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie benutzerdefinierten Abschnitten hinzufügen </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie zu einem Dashboard hinzufügen</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können Eingabeaufforderungen verwenden, um ihre Anzeige anzupassen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie in einem Diagramm anzeigen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können darin enthaltene Objekte inline bearbeiten</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

*Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen haben, um sie erstellen zu können. Weitere Informationen finden Sie unter [Zugriff auf Filter, Ansichten und Gruppierungen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

**Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen sowie auf Berichte, Dashboards und Kalender haben, um diese erstellen zu können. Weitere Informationen finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

***Sie können Listen für Berichte, die in einem Dashboard platziert werden, nur anpassen, wenn der Ersteller des Berichts die Listenelemente so konfiguriert hat, dass sie im Dashboard sichtbar sind.

>[!NOTE]
>
>Sie können keine Liste zu einem Dashboard hinzufügen, ohne zuvor einen Bericht zu erstellen und ihn zum Dashboard hinzuzufügen.

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Informationen zum Erstellen benutzerdefinierter Abschnitte finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Der Unterschied zwischen der Standard- und der erweiterten Liste

In [!DNL Workfront] gibt es zwei Arten von Listen:

* Standardlisten

  ![Standardprojektliste](assets/standard-list-screen-shot-gray-groupings.png)

* Erweiterte Listen

  ![Erweiterte Listen](assets/enhanced-status-list.png)

Die Funktionen der einzelnen erweiterten Listen unterscheiden sich je nachdem, auf welche Seite Sie zugreifen.

Weitere Informationen zu erweiterten Listen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).



Die folgende Tabelle zeigt einige der Unterschiede zwischen den standardmäßigen und erweiterten Listen in [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Standardlisten</b></td> 
   <td><b>Erweiterte Listen</b></td> 
  </tr> 
  <tr>
  <td> <p>Standardmäßig <strong> (alle</strong> oder bis <strong>2000</strong> Elemente angezeigt</p> </td> 
   <td> Anzeigen aller Elemente in der Liste nach manuellem Scrollen </td> 
  </tr>

<tr> 
   <td>Die Interaktion mit den Elementen in der Liste ist bei allen Objekttypen gleich und erfolgt über die Symbole oben in der Liste.  </td> 
   <td>Die Interaktion mit den Elementen in der Liste kann je nach Objekttyp unterschiedlich sein. Verwenden Sie dazu die Symbole oben in der Liste sowie die blaue Symbolleiste, die nach der Auswahl von Listenelementen aktiviert wird. </td> 
  </tr>

</td> 
  </tr> 
  <tr> 
   <td><p>Sie können Änderungen der Zellfarbe auf Elemente in einer Liste anwenden</p></td>
   <td><p>Die Zellenfarbänderungen können nicht auf Elemente in einer Liste angewendet werden. </p></td>
   </td> 
   <td></td> 
  </tr> 
 </tbody> 
</table>

<!--
consider adding things like adding fields on the fly in an enhanced list when we will be able to do this-->

<!--old table: 
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Legacy lists</b></td> 
   <td><b>Updated lists</b></td> 
  </tr> 
  <td> <p>Display <strong>100</strong> items by default</p> </td> 
   <td> <p>Display <strong>All</strong> or up to <strong>2000</strong> items by default</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use CTRL+F to find items in a list</p> </td> 
   <td> <p>Use quick filters to quickly find information in a large list</p> <p>For information about using quick filters in lists, see <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Apply the quick filter to a list</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>You can't inline edit custom fields with rich text formatting.</td> 
   <td> <p>Text in custom fields with formatting can be configured to allow bold, italics, underline, bullets, numbering, hyperlinks, and block quotes.</p> <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Conditional formatting can change the text color of links in a list</td> 
   <td>Cannot apply text color changes to links in a list</td> 
  </tr> 
 </tbody> 
</table>
-->
