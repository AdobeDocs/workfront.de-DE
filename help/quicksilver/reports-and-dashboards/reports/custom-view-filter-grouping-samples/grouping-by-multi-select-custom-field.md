---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Gruppieren eines Berichts mit einem aus mehreren Auswahlen bestehenden benutzerdefinierten Feld
description: Sie können in einem Adobe Workfront-Bericht nur mithilfe des Textmodus nach dem Wert in einem benutzerdefinierten Mehrfachfeld gruppieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Gruppieren eines Berichts nach einem benutzerdefinierten Mehrfachfeld

<!--Audited: 10/2024-->

Sie können in einem Adobe Workfront-Bericht nur mithilfe des Textmodus nach dem Wert in einem benutzerdefinierten Mehrfachfeld gruppieren.

Beispiele für benutzerdefinierte Mehrfachauswahl-Felder:

* Kontrollkästchen
* Dropdown-Menüs mit Mehrfachauswahl

Informationen zur Verwendung des Textmodus finden Sie im Artikel [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md) .

## Überlegungen beim Gruppieren nach einem benutzerdefinierten Mehrfachfeld

* Ein Bericht, der eine Textmodellgruppierung verwendet, kann nicht grafisch dargestellt werden. Sie müssen ein zusätzliches berechnetes Feld erstellen, das auf das benutzerdefinierte Mehrfachauswahlfeld verweist, um den Bericht auch nach dem Wert des benutzerdefinierten Mehrfachfelds zu kartieren.

  Weitere Informationen finden Sie unter [Bericht durch ein benutzerdefiniertes Mehrfachauswahlfeld grafisch darstellen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Elemente mit einer der ausgewählten Optionen werden nur einmal gezählt.

  Wenn Sie beispielsweise über ein benutzerdefiniertes Kontrollkästchen mit Auswahl 1 und Auswahl 2 als Optionen verfügen und das Formular an Aufgaben anhängen, werden die Aufgaben, für die sowohl Auswahl 1 als auch Auswahl 2 ausgewählt sind, getrennt von den Aufgaben gruppiert, für die nur Auswahl 1 oder Auswahl 2 ausgewählt ist.


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
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppieren eines Berichts nach benutzerdefinierten Feldern mit Mehrfachauswahl

Um eine Gruppierung nach einem benutzerdefinierten Mehrfachfeld zu ermöglichen, müssen folgende Voraussetzungen erfüllt sein:

* Erstellen Sie das benutzerdefinierte Mehrfachauswahlfeld in einem benutzerdefinierten Formular.\
  Informationen zum Erstellen benutzerdefinierter Formulare und zum Hinzufügen benutzerdefinierter Felder finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Hängen Sie das benutzerdefinierte Formular an Objekte an.
* Füllen Sie das benutzerdefinierte Feld mit Mehrfachauswahl mit einem Wert für jedes Objekt.

So gruppieren Sie ein benutzerdefiniertes Feld mit Mehrfachauswahl in einem Bericht:

1. Erstellen Sie einen Bericht oder bearbeiten Sie einen vorhandenen Bericht, in dem Sie eine Gruppierung für ein benutzerdefiniertes Feld mit Mehrfachauswahl hinzufügen möchten.\
   Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.
1. Wählen Sie die Registerkarte **Gruppierungen** aus.
1. Klicken Sie auf **Wechseln zum Textmodus**.

1. Wählen Sie den Text im Feld **Gruppieren nach** aus und ersetzen Sie ihn durch den folgenden Code:

   <pre>
   group.0.displayName=Multi-select Custom Field Name
   group.0.valueExpression={DE:Multi-select Custom Field Name}
   group.0.valueFormat=HTML
   group.0.textmode=true
   </pre>

1. Ersetzen Sie &quot;Benutzerdefinierter Feldname mit Mehrfachauswahl&quot;durch den tatsächlichen Namen Ihres benutzerdefinierten Mehrfachauswahlfelds, wie er in Ihrer Workfront-Instanz angezeigt wird.
1. Klicken Sie auf **Speichern und schließen**.

   Die Objekte im Bericht werden nach den Werten des benutzerdefinierten Mehrfachauswahlfelds gruppiert.

   ![](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   Der Name der Gruppierungen des Berichts entspricht den Namen des benutzerdefinierten Mehrfachfelds, gefolgt von den im Feld ausgewählten Werten.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
