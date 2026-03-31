---
title: Verwalten der Listenansicht in Adobe Workfront Planning
description: In Adobe Workfront Planning können Sie Objekte und deren Felder in einer Listenansicht anzeigen, wenn Sie auf der Seite „Verbundene Datensätze“ eines Datensatzes darauf zugreifen. Dieser Artikel beschreibt, wie Sie eine Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes erstellen oder bearbeiten können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: ddf10844646a79c43accaffa1789caf24290cc8a
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---


# Verwalten der Listenansicht in Adobe Workfront Planning

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können Objekte in der Listenansicht in den folgenden Bereichen von Workfront Planning anzeigen:

* Eine Seite mit verbundenen Datensätzen für Projekte im Detailbereich eines Datensatzes

  ![Projekte auf der Seite mit verbundenen Datensätzen in der Listenansicht](assets/projects-on-connected-records-page-list-view.png)

* Eine Liste von Anfrageformularen auf der Ebene des Datensatztyps

  ![Anforderungsformulare in der Listenansicht](assets/request-forms-in-list-view.png)

In diesem Artikel wird beschrieben, wie Sie in einer Listenansicht, in der Objekte in Workfront Planning angezeigt werden, navigieren, erstellen oder bearbeiten können. <!--change 'projects' to other objects when they become available and the location of the list view-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p>
<p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p> Standard zum Erstellen und Löschen von Ansichten</p>
   <p>Mitwirkender oder höher zum Aktualisieren von Ansichtselementen</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Anzeigeberechtigungen für eine Ansicht, um die Anzeigeeinstellungen vorübergehend zu ändern oder zu duplizieren</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Überlegungen zu Listenansichten

* Beachten Sie Folgendes für die Listenansicht der verbundenen Datensätze:

   * Sie können Projekte nur in der Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes anzeigen. Die Listenansicht ist für kein anderes Objekt oder keinen anderen Datensatztyp auf einer verbundenen Datensatzseite verfügbar.

  Informationen zum Erstellen einer verbundenen Datensatzseite finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
   * Bevor Sie eine Listenansicht auf einer verbundenen Datensatzseite eines Datensatzes anzeigen können, müssen Sie Workfront-Projekte mit Planungs-Datensatztypen verbinden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   * Sie können mehrere Listenansichten für Projekte auf der Seite „Verbundene Datensätze“ eines Datensatzes erstellen.

* Beachten Sie Folgendes für die Listenansicht der Anfrageformulare:

   * Sie können keine zusätzlichen Listenansichten für Planungsanfrageformulare erstellen oder bearbeiten. Workfront erstellt für Anfrageformulare eine Listenansicht. <!--this will change-->

     Weitere Informationen zu Anfrageformularen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Je nachdem, wo sie angezeigt wird, enthält nicht jede Listenansicht alle in diesem Artikel beschriebenen Elemente.


## Verwalten einer Listenansicht {#manage-a-list-view}

Listenansichten ähneln erweiterten Listen. Die meisten Elemente aus erweiterten Ansichten sind auch in Listenansichten in Workfront Planning vorhanden.

Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Navigieren Sie zu einer Listenansicht in einem der folgenden Bereiche:

   * Seite „Verbundene Datensätze“ im Detailbereich eines Datensatzes
   * Die Seite mit den Anforderungsformularen eines Datensatzes

1. (Bedingt) Führen Sie einen der folgenden Schritte aus, wenn verfügbar, um die Listenansicht zu ändern:

   1. Erweitern Sie das Dropdown-Menü Ansichten in der linken oberen Ecke der Liste, um eine andere Ansicht auszuwählen, oder klicken Sie auf **Neue Ansicht** und erstellen Sie eine andere.

      Ansichten werden im gesamten System gemeinsam genutzt. Wenn Sie eine Projektansicht für einen Datensatztyp erstellen, können Sie sie für andere Datensatztypen anzeigen, die verbundene Projekte anzeigen.

   1. Bewegen Sie den Mauszeiger über den Namen einer vorhandenen Ansicht und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf eine der folgenden Aktionen:
      * **Umbenennen**, um der Ansicht einen neuen Namen zu geben
      * **Freigeben**, um die Ansicht für andere freizugeben
      * **Löschen** zum Löschen der Ansicht.

      >[!NOTE]
      >
      >* Sie müssen über Verwaltungsberechtigungen für eine Ansicht verfügen, um sie bearbeiten, freigeben oder löschen zu können.
      >
      >* Sie können keine Systemansichten ändern.
      >
      >* <span class="preview">Sie können eine Ansicht, die für Sie freigegeben wurde und für die Sie nur über die Berechtigung zum Anzeigen verfügen, zurücksetzen, nachdem Sie sie geändert haben, um ihre ursprünglichen Voreinstellungen wiederherzustellen, oder Sie können sie mit Ihren Änderungen kopieren und die Kopie freigeben. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

      <!--
        And hide everything else below for these elements, after moving it to the Use enhanced lists article: 
        1. <span class="preview">To update one of the following view elements, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md):</span>
            <div class="preview">
            * Filter
            * Columns
            * Format cells
            * Row height
            </div>
        -->

   1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-icon.png), um der Ansicht einen Filter hinzuzufügen. Die Ergebnisse werden sofort in der Liste gefiltert. Filter können nicht gespeichert und benannt werden. Filter werden gespeichert, wenn Sie in Zukunft auf die Seite zugreifen, und sie sind Teil freigegebener Ansichten.
   1. Klicken Sie auf das **Spalten**-Symbol ![Spalten-Symbol](assets/columns-icon.png), um auszuwählen, welche Spalten in der Ansicht angezeigt oder ausgeblendet werden sollen.
   1. Bewegen Sie den Mauszeiger über den Namen einer Spalte, klicken Sie dann links neben dem Spaltennamen auf den Abwärtspfeil und dann auf eine der folgenden Aktionen:
      * **Umbenennen**, um eine **benutzerdefinierte Beschriftung** für die Spalte hinzuzufügen. Der Name des Originalfelds in Workfront ändert sich nicht.
      * **Sortieren**, um die Liste nach dem ausgewählten Feld zu sortieren. Ein Sortiersymbol, das die Sortierrichtung angibt, wird der Spaltenüberschrift hinzugefügt.
   1. Klicken Sie oben rechts in der Liste auf das Symbol **+** , um Spalten zur Liste hinzuzufügen oder daraus zu entfernen, und klicken Sie dann auf **Speichern**.

      Der **Spalten-Manager** wird geöffnet.

      Sie können der Listenansicht nur vorhandene Felder hinzufügen.
Sie können das primäre Feld in der Listenansicht, die in der ersten Spalte angezeigt wird, nicht entfernen.

   1. <span class="preview">Klicken Sie auf das Symbol **Zellen formatieren** (Symbol ![Zellen formatieren](assets/format-cells-icon.png). Das Feld **Format** wird geöffnet.</span> <!--change the name of the box when they update it-->
      <span class="preview">Gehen Sie wie folgt vor: </span>

      1. Klicken Sie **Bedingung hinzufügen**.
      1. <span class="preview">Wählen Sie in der **Wenn**-Zeile ein Feld aus, wählen Sie einen Feldwert aus und fügen Sie einen Modifikator hinzu. Die Modifikatoren ändern sich je nach ausgewähltem Feldtyp. </span>

         >[!TIP]
         >
         ><span class="preview">Nur in der Listenansicht sichtbare Felder sind für die bedingte Formatierung verfügbar.</span>

      1. <span class="preview">(Optional) Anstatt einen Feldwert hinzuzufügen, klicken Sie auf das Symbol **Mit einem anderen Feld vergleichen** (![&#x200B; mit einem anderen Feld &#x200B;](assets/compare-to-another-field-icon.png)) und wählen Sie ein Feld aus, dessen Wert Sie mit dem Wert des ausgewählten Felds vergleichen möchten. Sie können beispielsweise nach Projekten filtern, deren Projektbesitzer mit dem Projektsponsor übereinstimmt. </span>

         >[!TIP]
         >
         ><span class="preview">Nur in der Listenansicht sichtbare Felder sind für die bedingte Formatierung verfügbar.</span>

      1. <span class="preview">(Optional) Klicken Sie **Bedingung hinzufügen** in der **Wenn**-Zeile, um derselben Regel weitere Bedingungen hinzuzufügen.</span>

         >[!TIP]
         >
         ><span class="preview">Sie können einer Bedingungsregel bis zu 10 Bedingungen hinzufügen und Sie können bis zu 20 Regeln für ein Feld hinzufügen.</span>

      <div class="preview">

      1. Klicken Sie auf den **OR**-Connector zwischen Bedingungen, um zu **AND** zu wechseln und anzugeben, dass mehrere Bedingungen gleichzeitig erfüllt sein müssen. **Oder** ist der Standard-Connector.
      1. Wählen Sie in **Zeile** Format“ ein Feld aus, um anzugeben, welche Spalte formatiert werden soll. <!--edit this area, if it changes names??-->
      1. (Optional) Klicken Sie auf das **Farbkreis**-Symbol ![Farbkreis-Symbol](assets/color-circle.png) neben dem ausgewählten Feld, um es zu erweitern und eine andere <!--for a cell or the text of the cell that matches your criteria--> auszuwählen. <!--is this where the bold, italic is? I had no UI for this when I wrote it-->
      1. Aktivieren Sie die Einstellung **Auf Zeile anwenden**, um die Formatierung auf die gesamte Zeile des Felds anzuwenden, das die Bedingungen erfüllt.
      1. (Optional) Klicken Sie im Feld **Format** auf **Bedingung hinzufügen**, um eine weitere Regel für ein anderes Feld hinzuzufügen, und wiederholen Sie dann die obigen Schritte.
      1. (Optional) Klicken Sie auf **Alle löschen**, um alle Formatierungen zu entfernen.
      1. Klicken Sie außerhalb des Felds **Format**, um es zu schließen.

         Dadurch gelangen Sie zurück zur Listenansicht.
Die Formatierung wird sofort auf die Listenansicht angewendet.
Ein blauer Punkt neben dem Symbol **Zellen formatieren** gibt an, dass auf die Ansicht eine besondere Formatierung angewendet wurde.

      </div>

   <!--leave these here-->

1. (Optional) Fügen Sie ein Keyword in das Suchfeld in der oberen rechten Ecke der Liste ein, um nach einem Element zu suchen.

   Elemente, die mit Ihrem Suchbegriff übereinstimmen, werden in der Liste hervorgehoben.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um der Liste weitere Elemente hinzuzufügen und sie automatisch mit dem ausgewählten Datensatz zu verbinden:

   * Klicken Sie **Datensätze verbinden** in der oberen rechten Ecke der Liste, um vorhandene Elemente hinzuzufügen.
   * Klicken Sie **Neue Zeile** unten in der Liste, um neue Elemente hinzuzufügen.
1. Klicken Sie auf den Namen eines verbundenen Elements in der Liste, um es in einer anderen Browser-Registerkarte zu öffnen.
1. Doppelklicken Sie in eine Zelle der Liste, um die Informationen eines Felds zu bearbeiten, und drücken Sie dann die Eingabetaste, um die Änderungen zu speichern.

   Einige Felder sind schreibgeschützt. Beispielsweise ist der Bereich Prozent abgeschlossen eines Projekts ein Feld, das vom System berechnet wird, und Sie können ihn nicht manuell bearbeiten.

1. Bewegen Sie den Mauszeiger über den Namen eines Elements in der Liste und klicken Sie auf das Menü **Mehr** [Mehr](assets/more-menu.png) und klicken Sie auf **Anzeigen**, um das Projekt in einer anderen Registerkarte zu öffnen

   Oder

   Wählen Sie ein oder mehrere Elemente aus, beachten Sie die Aktionsleiste am unteren Rand der Liste und klicken Sie auf eine der folgenden Aktionen, sofern verfügbar:

   * **Löschen**, um das Element zu löschen. Durch das Löschen eines Projekts wird es vom Datensatz getrennt und in den Papierkorb von Workfront verschoben. Workfront-Administratoren können gelöschte Projekte bis zu 30 Tage nach dem Löschen wiederherstellen. Beim Löschen eines Formulars werden die Anfragen oder Datensätze, die beim Senden des Formulars erstellt wurden, nicht gelöscht.
   * **Trennen**, um das Projekt vom Datensatz zu trennen. Wenn Sie ein Projekt trennen, werden es und alle Werte seiner Suchfelder aus dem aktuellen Datensatz entfernt.

   ![Aktionsleiste in der Listenansicht der verbundenen Datensätze](assets/actions-bar-connected-records-page-list-view.png)

