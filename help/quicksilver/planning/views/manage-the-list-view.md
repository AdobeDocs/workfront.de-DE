---
title: Verwalten der Listenansicht in Adobe Workfront Planning
description: In Adobe Workfront Planning können Sie Objekte und deren Felder in einer Listenansicht anzeigen, wenn Sie auf der Seite „Verbundene Datensätze“ eines Datensatzes darauf zugreifen. Dieser Artikel beschreibt, wie Sie eine Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes erstellen oder bearbeiten können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---


# Verwalten der Listenansicht in Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Objekte und deren Felder in einer Listenansicht anzeigen, wenn Sie auf der Seite „Verbundene Datensätze“ eines Datensatzes darauf zugreifen.

In diesem Artikel wird beschrieben, wie Sie eine Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes erstellen oder bearbeiten und die Objekte in der Ansicht bearbeiten können.

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

* Datensätze können nicht in den Datensatztypseiten in einer Listenansicht angezeigt werden. Sie können die folgenden Objekte nur in einer Listenansicht anzeigen, wenn Sie sie auf der Seite „Verbundene Datensätze“ eines Datensatzes anzeigen:

   * Workfront-Projekte

  Informationen zum Erstellen einer verbundenen Datensatzseite finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Bevor Sie eine Listenansicht auf einer verbundenen Datensatzseite eines Datensatzes anzeigen können, müssen Sie Workfront-Projekte mit Planungs-Datensatztypen verbinden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Listenansichten ähneln erweiterten Listen. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Verwalten einer Listenansicht {#manage-a-list-view}

Weitere Informationen zum Verwalten von Listenansichten in Workfront finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Klicken Sie auf eine Arbeitsbereichskarte und dann auf eine Karte vom Typ Datensatz.
1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes, um die Vorschau- oder Detailseite des Datensatzes zu öffnen.
1. Fügen Sie eine **Seite „Verbundene Datensätze** für verbundene Projekte hinzu, wie im Artikel [Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) beschrieben.

   Auf der Seite „Verbundene Datensätze“ werden Projekte angezeigt, die mit dem Datensatz in der Listenansicht verbunden sind.

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
      >Sie müssen über Verwaltungsberechtigungen für eine Ansicht verfügen, um sie bearbeiten, freigeben oder löschen zu können.
      >
      >Sie können keine Systemansichten ändern.
      >
   1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-icon.png), um der Ansicht einen Filter hinzuzufügen. Die Ergebnisse werden sofort in der Liste gefiltert. Filter können nicht gespeichert und benannt werden. Filter werden gespeichert, wenn Sie in Zukunft auf die Seite zugreifen, und sie sind Teil freigegebener Ansichten.
   1. Klicken Sie auf das **Spalten**-Symbol ![Spalten-Symbol](assets/columns-icon.png), um auszuwählen, welche Spalten in der Ansicht angezeigt oder ausgeblendet werden sollen.
   1. Bewegen Sie den Mauszeiger über den Namen einer Spalte, klicken Sie dann links neben dem Spaltennamen auf den Abwärtspfeil und dann auf eine der folgenden Aktionen:
      * **Umbenennen**, um eine **benutzerdefinierte Beschriftung** für die Spalte hinzuzufügen. Der Name des Originalfelds in Workfront ändert sich nicht.
      * **Sortieren**, um die Liste nach dem ausgewählten Feld zu sortieren. Ein Sortiersymbol, das die Sortierrichtung angibt, wird der Spaltenüberschrift hinzugefügt.
   1. Klicken Sie oben rechts in der Liste auf das Symbol **+** , um Spalten zur Liste hinzuzufügen oder daraus zu entfernen, und klicken Sie dann auf **Speichern**.

      Der **Spalten-Manager** wird geöffnet.

      Sie können der Listenansicht nur vorhandene Felder hinzufügen.
Sie können das primäre Feld in der Listenansicht, die in der ersten Spalte angezeigt wird, nicht entfernen.
1. (Optional) Fügen Sie ein Keyword in das Suchfeld in der oberen rechten Ecke der Liste ein, um nach einem Element zu suchen.

   Elemente, die mit Ihrem Suchbegriff übereinstimmen, werden in der Liste hervorgehoben.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um der Liste weitere Elemente hinzuzufügen und sie automatisch mit dem ausgewählten Datensatz zu verbinden:

   * Klicken Sie **Datensätze verbinden** in der oberen rechten Ecke der Liste, um vorhandene Elemente hinzuzufügen.
   * Klicken Sie **Neue Zeile** unten in der Liste, um neue Elemente hinzuzufügen.
1. Klicken Sie auf den Namen eines verbundenen Elements in der Liste, um es in einer anderen Browser-Registerkarte zu öffnen.
1. Doppelklicken Sie in eine Zelle der Liste, um die Informationen eines Felds zu bearbeiten, und drücken Sie dann die Eingabetaste, um die Änderungen zu speichern.

   Einige Felder sind schreibgeschützt. Beispielsweise ist der Bereich Prozent abgeschlossen eines Projekts ein Feld, das vom System berechnet wird, und Sie können ihn nicht manuell bearbeiten.

1. Bewegen Sie den Mauszeiger über den Namen eines Elements in der Liste und klicken Sie auf das Menü **Mehr** [Mehr](assets/more-menu.png) und klicken Sie auf **Anzeigen**, um das Projekt in einer anderen Registerkarte zu öffnen

   ODER

   Wählen Sie ein oder mehrere Elemente aus, beachten Sie die Aktionsleiste am unteren Rand der Liste und klicken Sie dann auf eine der folgenden Aktionen:

   * **Löschen**, um das Projekt zu löschen. Durch das Löschen eines Projekts wird es vom Datensatz getrennt und in den Papierkorb von Workfront verschoben. Workfront-Administratoren können gelöschte Projekte bis zu 30 Tage nach dem Löschen wiederherstellen.
   * **Trennen**, um das Projekt vom Datensatz zu trennen. Wenn Sie ein Projekt trennen, werden es und alle Werte seiner Suchfelder aus dem aktuellen Datensatz entfernt.

   ![Aktionsleiste in der Listenansicht der verbundenen Datensätze](assets/actions-bar-connected-records-page-list-view.png)

