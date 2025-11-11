---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Erstellen eines Diagramms für einen Bericht mit einem benutzerdefinierten Mehrfachauswahlfeld
description: Sie können einen Bericht erst nach der Erstellung eines zusätzlichen berechneten Felds, das die im benutzerdefinierten Mehrfachauswahl-Feld ausgewählten Optionen erfasst, durch ein benutzerdefiniertes Mehrfachauswahl-Feld grafisch darstellen.
author: Jenny
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# Erstellen eines Diagramms für einen Bericht mit einem benutzerdefinierten Mehrfachauswahlfeld

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Anstatt ein Diagramm mit einem benutzerdefinierten Feld mit mehreren Auswahlmöglichkeiten zu erstellen, empfehlen wir, für jede Option eines benutzerdefinierten Felds mit mehreren Auswahlmöglichkeiten separate Felder zu erstellen.

Beispiele für benutzerdefinierte Felder mit Mehrfachauswahl:

* Kontrollkästchen
* Mehrfachauswahl-Dropdownmenüs

Informationen zur Verwendung des Textmodus finden Sie im Artikel [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Wenn es jedoch nicht möglich ist, separate Felder für jede Option eines Felds mit Mehrfachauswahl zu verwenden, können Sie einen Bericht anhand eines benutzerdefinierten Felds mit Mehrfachauswahl grafisch darstellen, indem Sie berechnete benutzerdefinierte Felder verwenden, um die Auswahl aus dem Mehrfachauswahl-Feld zuerst zu gruppieren. Danach können Sie den Bericht anhand der berechneten Felder grafisch darstellen.

>[!NOTE]
>
>Elemente, für die eine der ausgewählten Optionen ausgewählt ist, werden nur einmal gezählt.
>
>Wenn Sie beispielsweise ein benutzerdefiniertes Kontrollkästchen mit Auswahl 1 und Auswahl 2 als Optionen haben und das Formular an Aufgaben anhängen, werden die Aufgaben, für die sowohl Auswahl 1 als auch Auswahl 2 ausgewählt sind, in einem separaten Diagrammelement angezeigt als die Aufgaben, für die nur Auswahl 1 oder Auswahl 2 ausgewählt ist.
>
>Aufgaben, für die Auswahl 1 ausgewählt ist, werden nicht im selben Diagrammelement angezeigt wie die Aufgaben, für die Auswahl 1 und Auswahl 2 ausgewählt sind.

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie ein berechnetes benutzerdefiniertes Feld erstellen, das die aus dem benutzerdefinierten Mehrfachauswahl-Feld ausgewählten Werte anzeigt. Weitere Informationen finden Sie [&#x200B; Abschnitt „Erstellen eines berechneten benutzerdefinierten Felds, das auf ein benutzerdefiniertes Mehrfachauswahl-Feld verweist](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) in diesem Artikel.

## Erstellen eines Diagramms für einen Bericht mit mehreren benutzerdefinierten Feldern

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Sie können kein Diagramm in einem Bericht erstellen, indem Sie auf ein benutzerdefiniertes Feld mit mehreren Auswahlen verweisen. Stattdessen können Sie ein berechnetes Feld erstellen, das die Werte des benutzerdefinierten Mehrfachauswahl-Felds für ein bestimmtes Objekt aufzeichnet und nach dem berechneten Feld gruppiert. 

* [Erstellen Sie ein berechnetes benutzerdefiniertes Feld, das auf ein benutzerdefiniertes Feld mit Mehrfachauswahl verweist](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Erstellen eines Diagramms, das auf ein berechnetes benutzerdefiniertes Feld verweist](#build-a-chart-that-references-a-calculated-custom-field)

### Erstellen eines berechneten benutzerdefinierten Felds, das auf ein benutzerdefiniertes Mehrfachauswahl-Feld verweist {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Um ein berechnetes Feld zu erstellen, das auf ein benutzerdefiniertes Mehrfachauswahlfeld verweist, müssen die folgenden Voraussetzungen erfüllt sein:

* Ein benutzerdefiniertes Feld mit Mehrfachauswahl in einem benutzerdefinierten Formular.\
  Informationen zum Erstellen benutzerdefinierter Formulare und Hinzufügen benutzerdefinierter Felder zu ihnen finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Ein benutzerdefiniertes Formular mit dem benutzerdefinierten Mehrfachauswahl-Feld, das an -Objekte angehängt ist.
* Werte für das benutzerdefinierte Feld mit Mehrfachauswahl für jedes Objekt.

So erstellen Sie das berechnete benutzerdefinierte Feld, das auf das benutzerdefinierte Mehrfachauswahlfeld verweist:

1. Erstellen Sie ein benutzerdefiniertes Formular oder bearbeiten Sie ein vorhandenes.

   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Wählen Sie das Objekt oder die Objekte aus, die Sie mit dem benutzerdefinierten Formular verwenden möchten.
1. Klicken Sie auf **Feld hinzufügen** und dann auf **Berechnet**, um das benutzerdefinierte Feld mit Mehrfachauswahl zum Formular hinzuzufügen.

1. Benennen **im Feld** das neue berechnete Feld, um anzugeben, dass es auf das benutzerdefinierte Feld mit Mehrfachauswahl verweist.

   Beispiel: „Berechnetes Mehrfachauswahlfeld.“

1. Geben Sie **Feld** den folgenden Code ein:

   `{DE:Multi-select Custom Field}`

   Dadurch werden die im benutzerdefinierten Mehrfachauswahl-Feld ausgewählten Auswahlmöglichkeiten zum berechneten benutzerdefinierten Feld hinzugefügt. Beispiel: Wenn das Formular an Aufgaben angehängt ist und Auswahl 1 aus dem benutzerdefinierten Mehrfachauswahl-Feld ausgewählt ist, zeigt das berechnete benutzerdefinierte Feld den Wert „Auswahl 1“ an. Wenn Auswahl 1 und Auswahl 2 für eine andere Aufgabe ausgewählt sind, zeigt das berechnete benutzerdefinierte Feld den Wert „Auswahl 1, Auswahl 2“ an.

1. Ersetzen Sie „Benutzerdefiniertes Mehrfachauswahlfeld“ durch den tatsächlichen Namen des benutzerdefinierten Mehrfachauswahlfelds, wie er in Workfront angezeigt wird.

   ![Berechnetes benutzerdefiniertes Mehrfachauswahl-Feld](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Optional) Wenn das benutzerdefinierte Feld mit mehreren Auswahlmöglichkeiten bereits in diesem Formular vorhanden und dieses Formular bereits mit Objekten verbunden ist, aktivieren Sie die Option **Auf vorhandene Berechnungen anwenden**.

   Dadurch wird sichergestellt, dass das neue berechnete Feld automatisch mit dem Wert aus dem benutzerdefinierten Mehrfachauswahl-Feld ausgefüllt wird, da er zu den Formularen hinzugefügt wird, die bereits an die Objekte angehängt sind.

1. Klicken Sie auf **Übernehmen**.
1. Klicken Sie **Speichern und schließen**.

   Das berechnete benutzerdefinierte Feld wird zum benutzerdefinierten Formular hinzugefügt. Wenn das Formular derzeit mit Objekten verbunden ist, wird das Feld mit Informationen aus dem benutzerdefinierten Mehrfachauswahl-Feld gefüllt.

### Erstellen eines Diagramms, das auf ein berechnetes benutzerdefiniertes Feld verweist {#build-a-chart-that-references-a-calculated-custom-field}

1. (Optional) Um sicherzustellen, dass alle berechneten Felder, nach denen Sie ein Diagramm erstellen möchten, mit Werten gefüllt werden, wählen Sie auf der Registerkarte Details des Berichts alle Objekte aus, die das benutzerdefinierte Formular mit dem benutzerdefinierten Mehrfachauswahlfeld und dem berechneten benutzerdefinierten Feld enthalten, und klicken Sie dann auf **Bearbeiten**.
1. (Optional und bedingt) Wählen Sie das Feld **Benutzerdefinierte Ausdrücke neu berechnen** und klicken Sie dann auf **Änderungen speichern**.\
   ![Benutzerdefinierte Ausdrücke neu &#x200B;](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Diese Option wurde aus der Massenbearbeitung von Projekten entfernt.  Sie können Ausdrücke für Projekte weiterhin stapelweise neu berechnen, indem Sie oben in einer Projektliste auf das **Mehr**-Symbol ![Mehr](assets/more-icon-45x33.png) und dann auf **Ausdrücke neu berechnen** klicken.

1. Wechseln Sie zum Bericht, in dem Sie das Diagramm für das berechnete Feld hinzufügen möchten, das auf das benutzerdefinierte Feld mit Mehrfachauswahl verweist.
1. Klicken Sie **Berichtsaktionen** und dann **Bearbeiten**.

1. Wählen Sie die Registerkarte <strong>Gruppierungen</strong> und klicken Sie dann auf <strong>Gruppierung hinzufügen</strong>.
1. Fügen Sie das <strong>berechnete Mehrfachauswahlfeld</strong> hinzu, das Sie als Gruppierung erstellt haben.
1. Wählen Sie die <strong>Diagramm</strong> aus und fügen Sie Ihrem Bericht ein Diagramm hinzu.

   Wählen Sie beispielsweise ein **Spalten**-Diagramm.
   <br>Informationen zum Hinzufügen eines Diagramms zu einem Bericht finden Sie im Abschnitt <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Hinzufügen eines Diagramms zu einem Bericht</a> im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerspezifischen Berichts</a>.
1. Wählen Sie im Feld **Untere Achse (X** das Feld <strong>Berechnetes Mehrfachauswahlfeld</strong> aus, das im Diagramm angezeigt werden soll.
1. Klicken Sie auf <strong>Speichern + schließen</strong>.

   Der Bericht zeigt die Ergebnisse gruppiert nach dem berechneten Mehrfachauswahlfeld in einem Diagramm an.

   ![Mehrfachauswahlfeld im Diagramm](assets/chart-multi-select-field-column-chart-example.png)
