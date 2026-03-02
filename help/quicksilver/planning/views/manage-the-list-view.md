---
title: Verwalten der Listenansicht in Adobe Workfront Planning
description: In Adobe Workfront Planning können Sie Objekte und deren Felder in einer Listenansicht anzeigen, wenn Sie auf der Seite „Verbundene Datensätze“ eines Datensatzes darauf zugreifen. Dieser Artikel beschreibt, wie Sie eine Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes erstellen oder bearbeiten können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: ce3ca4d55fd3fe0630da4961f27159fe5e31612a
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---


# Verwalten der Listenansicht in Adobe Workfront Planning

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Projekte und deren Felder in einer Listenansicht anzeigen, wenn Sie auf die Seite „Verbundene Datensätze“ eines Datensatzes zugreifen. <!--change 'projects' to other objects when they become available and the location of the list view-->

In diesem Artikel wird beschrieben, wie Sie eine Listenansicht erstellen oder bearbeiten können, die Projekte auf der Seite „Verbundene Datensätze“ eines Datensatzes anzeigt, und wie Sie die Projekte in der Ansicht bearbeiten können. <!--change 'projects' to other objects when they become available and the location of the list view-->

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

* Sie können nicht alle Objekttypen auf den Datensatztypseiten in einer Listenansicht anzeigen.

  Sie können die folgenden Objekte nur in einer Listenansicht anzeigen, wenn Sie sie auf der Seite „Verbundene Datensätze“ eines Datensatzes anzeigen:

   * Workfront-Projekte

  Informationen zum Erstellen einer verbundenen Datensatzseite finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Bevor Sie eine Listenansicht auf einer verbundenen Datensatzseite eines Datensatzes anzeigen können, müssen Sie Workfront-Projekte mit Planungs-Datensatztypen verbinden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).


## Verwalten einer Listenansicht {#manage-a-list-view}

Listenansichten ähneln erweiterten Listen. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Klicken Sie auf eine Arbeitsbereichskarte und dann auf eine Karte vom Typ Datensatz.
1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes, um die Vorschau- oder Detailseite des Datensatzes zu öffnen.
1. Fügen Sie eine **Seite „Verbundene Datensätze** für verbundene Projekte hinzu, wie im Artikel [Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) beschrieben.

   Auf der Seite „Verbundene Datensätze“ werden Projekte angezeigt, die mit dem Datensatz in der Listenansicht verbunden sind.

   <!--add new screen shot when they release Conditional formatting MVP -->

   ![Projekte auf der Seite mit verbundenen Datensätzen in der Listenansicht](assets/projects-on-connected-records-page-list-view.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um die Listenansicht zu ändern:

   1. Erweitern Sie das Dropdown-Menü Ansichten in der oberen rechten Ecke der Liste, um eine andere Ansicht auszuwählen, oder klicken Sie auf **Neue Ansicht** und erstellen Sie eine andere.

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
      1. <span class="preview">Wählen Sie in der **Wenn**-Zeile ein Feld aus, wählen Sie einen Feldwert aus und klicken Sie dann auf **Bedingung hinzufügen**. </span>

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
      1. (Optional) Klicken Sie auf das Symbol **Farbkreis** ![Farbkreis-Symbol](assets/color-circle.png) neben dem ausgewählten Feld, um es zu erweitern und eine andere Farbe auszuwählen.
      1. Aktivieren Sie die Einstellung **Auf Zeile anwenden**, um die Formatierung auf die gesamte Zeile des Felds anzuwenden, das die Bedingungen erfüllt.
      1. (Optional) Klicken Sie im Feld **Format** auf **Bedingung hinzufügen**, um eine weitere Regel für ein anderes Feld hinzuzufügen, und wiederholen Sie dann die obigen Schritte.
      1. (Optional) Klicken Sie auf **Alle löschen**, um alle Formatierungen zu entfernen.
      1. Klicken Sie außerhalb des Felds **Format**, um es zu schließen.

         Dadurch gelangen Sie zurück zur Listenansicht.
Die Formatierung wird sofort auf die Listenansicht angewendet.
Ein blauer Punkt neben dem Symbol **Zellen formatieren** gibt an, dass auf die Ansicht eine besondere Formatierung angewendet wurde.

      </div>

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

   Wählen Sie ein oder mehrere Elemente aus, beachten Sie die Aktionsleiste am unteren Rand der Liste und klicken Sie dann auf eine der folgenden Aktionen:

   * **Löschen**, um das Projekt zu löschen. Durch das Löschen eines Projekts wird es vom Datensatz getrennt und in den Papierkorb von Workfront verschoben. Workfront-Administratoren können gelöschte Projekte bis zu 30 Tage nach dem Löschen wiederherstellen.
   * **Trennen**, um das Projekt vom Datensatz zu trennen. Wenn Sie ein Projekt trennen, werden es und alle Werte seiner Suchfelder aus dem aktuellen Datensatz entfernt.

   ![Aktionsleiste in der Listenansicht der verbundenen Datensätze](assets/actions-bar-connected-records-page-list-view.png)

