---
navigation-topic: use-lists
title: Erste Schritte mit Listen in [!DNL Adobe Workfront]
description: Sie können Listen von Objekten in [!DNL Adobe Workfront] anzeigen, um Informationen zu ihnen zu erhalten, wie z. B. ihr Start- und Fälligkeitsdatum, die ihnen zugewiesenen Benutzer und andere ihnen zugeordnete Objekte.
feature: Get Started with Workfront
author: Nolan
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '2284'
ht-degree: 0%

---

# Erste Schritte mit Listen in [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Sie können Listen von Objekten in [!DNL Adobe Workfront] anzeigen, um Informationen zu ihnen zu erhalten, wie z. B. ihr Start- und Fälligkeitsdatum, die ihnen zugewiesenen Benutzer und andere ihnen zugeordnete Objekte.

Im Folgenden finden Sie einige Merkmale von Listen in [!DNL Workfront]:

* Listen werden automatisch alle fünf Minuten aktualisiert, um Informationen zu aktualisieren, die andere Benutzer im System an anderer Stelle aktualisieren.
* Einige Bereiche in [!DNL Workfront] sind mit Standardlisten von Objekten vorkonfiguriert.

  Sie können die meisten dieser vorkonfigurierten Listen anpassen.

* Ein [!DNL Workfront] -Administrator kann benutzerdefinierte Listen erstellen, die auf verschiedene Bereiche von [!DNL Workfront] angewendet werden.

  Weitere Informationen zum Erstellen von Listen auf Systemebene finden Sie im Artikel [Erstellen, Bearbeiten und Freigeben von Standardfiltern, Ansichten und Gruppierungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

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
   <ul><li><p>Mitwirkende oder höher </p></li>
   </ul>

<p>Aktuell:</p>
   <ul><li><p>Anforderung oder höher</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Hinzufügen höherer Berechtigungen für Filter, Ansichten oder Gruppen mit Zugriff auf die Freigabe </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Im Folgenden finden Sie einige Typen von Objektlisten, die Sie in [!DNL Workfront] finden können, sowie einige der Bereiche, in denen sie standardmäßig angezeigt werden, wenn Sie über die Berechtigung zum Anzeigen eines Objekts verfügen.

>[!NOTE]
>
>* Diese Liste ist nicht vollständig. Jede dieser Objektlisten kann auch in einem Bericht oder Dashboard angezeigt werden. Beispielsweise wird in einem Projekt- oder Dashboard, das einen Projektbericht enthält, auch eine Liste der Projekte angezeigt.
>* In dieser Liste bedeutet &quot;Auswählen&quot;, dass Sie auf den Namen des Elements klicken müssen, nicht auf das Kontrollkästchen links neben dem Namen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] Liste</strong></th> 
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
   <td>Programmliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Projekte</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Projekte]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme] &gt;[!UICONTROL Programm auswählen] &gt;[!UICONTROL Projekte]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt; [!UICONTROL Aufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Unteraufgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Vorgänger*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Probleme</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt;[!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Probleme]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Unteraufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Probleme]</p> </li> 
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
   <td>Liste der Benutzer</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Benutzer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Dokumentenliste</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt;[!UICONTROL Portfolio auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Portfolios] &gt; [!UICONTROL Portfolio auswählen] &gt;[!UICONTROL Programme] &gt;[!UICONTROL Programm auswählen] &gt;[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt; [!UICONTROL Probleme] &gt;[!UICONTROL Problem auswählen] &gt; [!UICONTROL Dokumente]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Timesheets</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Timesheet] s &gt; [!UICONTROL All Timesheets]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Abrechnungssätze</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL ein Projekt auswählen] &gt;[!UICONTROL Abrechnungsraten*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Rechnungsdatensätze</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL Projekt auswählen] &gt; [!UICONTROL Rechnungseinträge]</p> </li> 
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
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekte auswählen] ein Projekt &gt;[!UICONTROL Ausgaben]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt; [!UICONTROL ein Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Ausgaben]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Liste der Stundeneinträge</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Aufgaben] &gt;[!UICONTROL Aufgabe auswählen] &gt;[!UICONTROL Stunden]</p> </li> 
     <li> <p>[!UICONTROL Projekte] &gt;[!UICONTROL Projekt auswählen] &gt;[!UICONTROL Probleme] &gt;[!UICONTROL Auswählen] eines Problems &gt;[!UICONTROL Stunden]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td>Liste benutzerdefinierter Formulare</td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Setup] &gt; [!UICONTROL Benutzerdefinierter Forms] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>Liste von Gruppen oder Untergruppen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Groups] &gt;[!UICONTROL Select the parent group] &gt;[!UICONTROL Subgroups] </li> 
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
   <td>Liste der Unternehmen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Unternehmen]</p> </li> 
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
   <td>Liste der Layoutvorlagen</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt; [!UICONTROL Layout-Vorlagen]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

Die Liste kann nicht für den angegebenen Bereich angepasst werden. Ein [!DNL Workfront] -Administrator kann eine benutzerdefinierte Liste auf Systemebene erstellen oder Sie können einen Bericht für dieses Objekt erstellen, wenn Ihre Zugriffsebene Ihnen den Zugriff auf Berichte ermöglicht.

## Listenelemente

Eine Liste enthält bestimmte Elemente, die ihr Format und die angezeigten Informationen definieren. Sie finden mehrere Systemlistenelemente, die standardmäßig verfügbar sind. Sie können auch benutzerdefinierte Elemente erstellen, die Ihren Anforderungen entsprechen.

>[!NOTE]
>
>Wenn Sie einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung aus einer Liste auswählen, wird diese Auswahl beibehalten, auch wenn Sie sich bei [!DNL Workfront] abmelden oder Ihren Browser schließen.

Im Folgenden finden Sie die Elemente einer Liste:

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
   <td> <p>Filter halten unnötige Informationen basierend auf den von Ihnen angegebenen Kriterien aus einer Liste heraus. </p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filterübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Ansicht]</strong></td> 
   <td> <p>Ansichten definieren, welche Felder (Spalten) auf dem Bildschirm angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Übersicht über Ansichten in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Gruppierung]</strong></td> 
   <td> <p>Bei Gruppierungen werden die Objekte in der Liste je nach den von Ihnen angegebenen Kriterien in Bereiche unterteilt.</p> <p>Beispielsweise können die Probleme in einer Liste nach Status oder Priorität in Abschnitten angezeigt werden.</p> <p>Sie können bis zu drei Gruppierungsebenen in einer Standardgruppierung haben und eine vierte Ebene hinzufügen, wenn Sie eine Gruppierung im Textmodus konfigurieren.</p> <p>Weitere Informationen zu Gruppierungen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Gruppierungsübersicht in [!DNL Adobe Workfront]</a>.</p> <p>Weitere Informationen zum Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Textmodus - Übersicht</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Diese Elemente werden standardmäßig oben in jeder Liste angezeigt. Sie sind klebrig und bewegen sich nicht, wenn Sie durch die Liste scrollen. Bewegen Sie den Mauszeiger über das Symbol für jedes Element, um es zu identifizieren.

![](assets/nwe-list-elements.png)

Sie können Listenelemente in den folgenden Bereichen anpassen und für andere Benutzer freigeben:

* Jede Systemstandardliste, die im Abschnitt &quot;[Erste Schritte mit Listen in [!DNL Adobe Workfront]](#default-workfront-lists)&quot;in diesem Artikel gefunden wird
* Alle Berichte, die für Sie freigegeben wurden

Die Elemente zum Erstellen von Listen entsprechen denen für Berichte.

Weitere Informationen zum Erstellen und Anpassen der Elemente zum Erstellen von Listen und Berichten finden Sie unter [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Aktionen auflisten

Sie können die folgenden Aktionen in einer Liste ausführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong></th> 
   <th><strong>Informationen</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Inline-Bearbeitung</strong> </td> 
   <td> <p>Bearbeiten Sie Objekte und deren Informationen direkt in der Liste.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">Inline-Elemente in einer Liste in [!DNL Adobe Workfront]</a> bearbeiten.</p> 
   <p><b>NOTE:</b></p>
   <p>Eine Inline-Bearbeitung ist in einer Gruppierung nicht möglich.</p>

</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>Aktualisieren mit der [!UICONTROL Zusammenfassung]</strong> </td> 
   <td> <p>Aktualisieren Sie Aufgaben und Probleme auf Projektebene mithilfe des Bereichs [!UICONTROL Zusammenfassung] .</p> <p><b>TIPP:</b></p> <p>Die Zusammenfassung ist nicht für alle Objekte verfügbar und steht nicht in Aufgaben- oder Problemberichten zur Verfügung.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Übersicht der Zusammenfassung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Listenanzeige anpassen</strong> </td> 
   <td> <p>Passen Sie das Erscheinungsbild einer Liste, Spaltenanordnung, Sortierreihenfolge von Elementen oder Anzahl der angezeigten Elemente an.</p> <p><b>NOTE:</b></p> <p>Änderungen, die Sie an der Anzahl der Elemente vornehmen, die auf einer Seite angezeigt werden sollen, werden rückgängig gemacht, wenn Sie sich bei [!DNL Workfront] abmelden oder Ihren Browser schließen. Änderungen können auch nach einem Zeitraum von 8 Stunden rückgängig gemacht werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">Anzeige einer Liste ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Schnellfilter</strong> </td> 
   <td> <p>Wenden Sie einen Schnellfilter an, um nur Elemente zu finden, die für Sie wichtig sind, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.</p> <p><b>WICHTIG:</b></p> <p> Mithilfe des Schnellfilters können Sie Elemente finden, die ein Suchwort enthalten, unabhängig davon, ob dieses Element auf dem Bildschirm sichtbar ist oder angezeigt wird, nachdem Sie zum unteren Seitenrand gescrollt haben. Wenn Sie die Suchfunktionen Ihres Browsers verwenden, können Sie nur Elemente finden, die bereits auf dem Bildschirm sichtbar sind. Wenn Ihre Liste mehrere Seiten enthält, finden Schnellfilter nur die Elemente auf der aktuellen Seite.</p> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Anwenden des Schnellfilters auf eine Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Export</strong> </td> 
   <td> <p>Exportieren Sie eine Liste von Objekten aus [!DNL Workfront]. Wenn eine Liste mehr als 2000 Elemente enthält, ist der Export der Liste die einzige Möglichkeit, alle Elemente auf einer Seite zu überprüfen.</p> <p>Weitere Informationen zum Exportieren einer Liste finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">Liste exportieren</a>. Weitere Informationen zu Exportformaten und -beschränkungen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Daten exportieren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Listen-Symbolleiste

In der folgenden Tabelle sind viele der in der Symbolleiste verfügbaren Symbole aufgeführt und es wird angezeigt, was passiert, wenn Sie darauf klicken:

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
   <td>Öffnen Sie weitere Optionen, einschließlich Hinzufügen eines neuen Elements oder Benutzers.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgabe einfügen oben]</td> 
   <td> <p>Fügen Sie eine Aufgabe über der ausgewählten Aufgabe ein.</p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgabe unten einfügen]</td> 
   <td> <p>Fügen Sie eine Aufgabe unterhalb der ausgewählten Aufgabe ein.</p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
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
   <td> <p>Öffnen Sie das Dialogfeld, um das ausgewählte Problem einer Iteration hinzuzufügen.</p> <p>Dies ist nur für Probleme verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>Geben Sie das ausgewählte Element frei.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Aufgaben für Einzüge und Ausfälle] </td> 
   <td> <p>Einzug oder Auszug der ausgewählten Aufgabe. </p> <p>Dies ist nur für Aufgaben verfügbar. </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL Mehr]</td> 
   <td>Öffnen Sie zusätzliche Optionen für das ausgewählte Element.</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Schnellfilter] </p> </td> 
   <td> <p>Öffnen Sie das Suchfeld für Schnellfilter, um Elemente in der angezeigten Liste zu suchen.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>Exportieren Sie die Liste in PDF-, Excel- oder tabulatorgetrennte Dateien.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>Zeigen Sie die Liste in der Agile-Ansicht an.<br>Dies ist nur für Aufgaben verfügbar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Zeigen Sie die Liste in der Ansicht [!UICONTROL Gantt Chart] an.</p> <p>Dies ist nur für Projekte und Aufgaben verfügbar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Filter]</td> 
   <td> <p>Zeigen Sie eine Liste mit Filtern und zusätzlichen Optionen zum Verwalten von Filtern an, einschließlich der Erstellung eines Filters. </p> <p>Auf einem kleinen Bildschirm wird der Filtername durch das Filtersymbol ersetzt. Wenn Sie einen anderen Filter als "[!UICONTROL All]"anwenden, wird auf dem Filtersymbol ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Ansicht]</td> 
   <td> <p>Zeigen Sie eine Liste mit Ansichten und zusätzlichen Optionen zum Verwalten von Ansichten an, einschließlich der Erstellung einer Ansicht. </p> <p>Auf einem kleinen Bildschirm wird der Name der Ansicht durch das Symbol [!UICONTROL Ansicht] ersetzt. Wenn Sie eine andere Ansicht als "[!UICONTROL Standard]"anwenden, wird auf dem Symbol [!UICONTROL Ansicht] ein blauer Punkt angezeigt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>Dropdown-Menü [!UICONTROL Gruppierung]</td> 
   <td> <p>Zeigen Sie eine Liste mit Gruppierungen und zusätzlichen Optionen zum Verwalten von Gruppierungen an, einschließlich der Erstellung einer Gruppierung. </p> <p>Auf einem kleinen Bildschirm wird der Gruppierungsname durch das Symbol [!UICONTROL Gruppierung] ersetzt. Auf dem [!UICONTROL Gruppierungssymbol] wird ein blauer Punkt angezeigt, wenn Sie eine andere Gruppierung als "[!UICONTROL Nichts]"anwenden.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Planmodus]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie die Änderungen, die Sie in einer Aufgabenliste vornehmen, automatisch oder manuell speichern möchten. </p> <p>Informationen zum Bearbeiten von Aufgaben in einer Liste finden Sie unter <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Aufgaben in einer Liste bearbeiten</a>. </p> <p>Dies ist nur für Aufgaben verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Zusammenfassung]</td> 
   <td> <p>Anzeigen oder Ausblenden des Felds [!UICONTROL Zusammenfassung] für das ausgewählte Element</p> <p>Dies ist nur für Aufgaben und Probleme verfügbar.</p> <p>Weitere Informationen zum Bedienfeld [!UICONTROL Zusammenfassung] finden Sie unter <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">Zusammenfassung - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Entfernen]</td> 
   <td>Entfernen Sie etwas aus der Liste. Entfernen Sie beispielsweise als Gruppenadministrator, der Gruppen- oder Untergruppenmitgliedschaften verwaltet, ein Gruppenmitglied, wie unter <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">Mitgliedschaft einer Gruppe anzeigen und verwalten</a> beschrieben.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Kommentar] /[!UICONTROL Update]</td> 
   <td> <p>Geben Sie einen Kommentar oder eine Aktualisierung ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Unterschied zwischen Listen und Berichten

Sowohl Listen als auch Berichte sind Raster, die Informationen über einen Objekttyp enthalten.

In der folgenden Tabelle sind die Ähnlichkeiten und Unterschiede zwischen Listen und Berichten aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Funktionalität</strong> </th> 
   <th><strong>list</strong> </th> 
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
   <td> <p>Nur ein [!DNL Workfront] -Administrator und Benutzer mit einer [!UICONTROL Plan]-Lizenz können diese erstellen</p> </td> 
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
   <td> <p>Sie können in die Formate .pdf, [!DNL Excel] und "Tabulator - getrennt"exportieren</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können den Versand für eine E-Mail planen</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Sie können einer Layoutvorlage hinzufügen</p> </td> 
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
   <td> <p>Sie können Aufforderungen verwenden, um die Anzeige anzupassen</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Sie können sie in einer Grafik anzeigen</p> </td> 
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

Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen haben, um sie erstellen zu können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen sowie auf Berichte, Dashboards und Kalender haben, um sie erstellen zu können. Weitere Informationen finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Listen können nur dann für Berichte angepasst werden, wenn der Ersteller des Berichts die Listenelemente so konfiguriert hat, dass sie im Dashboard sichtbar sind.

>[!NOTE]
>
>Es ist nicht möglich, einem Dashboard eine Liste hinzuzufügen, ohne zuvor einen Bericht zu erstellen und ihn zuerst zum Dashboard hinzuzufügen.

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Informationen zum Erstellen benutzerdefinierter Abschnitte finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## Der Unterschied zwischen der aktualisierten und der alten Liste

Es gibt zwei Arten von Listen in [!DNL Workfront]:

* Alte Listen

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* Aktualisierte Listen

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

Die folgende Tabelle zeigt einige Unterschiede zwischen den alten und aktualisierten Listen in [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Alte Listen</b></td> 
   <td><b>Aktualisierte Listen</b></td> 
  </tr> 
  <td> <p>Standardmäßig <strong>100</strong> Elemente anzeigen</p> </td> 
   <td> <p>Standardmäßig <strong>Alle</strong> oder bis <strong>2000</strong> Elemente anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Mit Strg+F Elemente in einer Liste suchen</p> </td> 
   <td> <p>Verwenden Sie Schnellfilter, um schnell Informationen in einer großen Liste zu finden.</p> <p>Informationen zur Verwendung von Schnellfiltern in Listen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">Anwenden des Schnellfilters auf eine Liste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Felder mit Rich-Text-Formatierung können nicht inline bearbeitet werden.</td> 
   <td> <p>Text in benutzerdefinierten Feldern mit Formatierung kann so konfiguriert werden, dass fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen zulässig sind.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Benutzerdefiniertes Formular erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Durch die bedingte Formatierung kann die Textfarbe von Links in einer Liste geändert werden</td> 
   <td>Textfarbänderungen an Links in Listen können nicht angewendet werden</td> 
  </tr> 
 </tbody> 
</table>
