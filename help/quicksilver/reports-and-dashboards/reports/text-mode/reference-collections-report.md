---
product-area: reporting
navigation-topic: text-mode-reporting
title: Referenzieren von Sammlungen in einem Bericht
description: Referenzieren von Sammlungen in einem Bericht
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 6bd9dc626befc4dfa4054760e7ec7d677f6da6e5
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# Referenzieren von Sammlungen in einem Bericht

<!-- Audited: 1/2025 -->

Durch das Erstellen eines Berichts in Adobe Workfront können Sie eine Reihe von Objekten, die entsprechenden Felder oder verknüpfte Objekte in einer Liste, einem Raster oder einem Diagrammformat anzeigen.

Weitere Informationen zum Erstellen eines Berichts in Workfront finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> <p>Verwalten von Berechtigungen für Ansichten, Filter oder Gruppierungen </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Grundlegendes zu Sammlungen

Eine Auflistung ist eine Liste von Objekten, die mit einem anderen Objekt verknüpft sind.

Es bestehen die folgenden beiden Beziehungen zwischen Objekten in Workfront:

* **Eins-zu-eins-**: Ein Objekt kann jeweils nur mit einem anderen Objekt verknüpft werden.\
  Beispielsweise kann ein Projekt jeweils nur mit einem Portfolio verknüpft werden.

* **Eins-zu-Viele-Beziehung**: Ein Objekt kann gleichzeitig mit mehreren anderen Objekten verknüpft werden.\
  Beispielsweise kann ein Projekt mehrere Aufgaben haben. In diesem Fall bildet die Liste der Aufgaben eine Sammlung für das Projekt.

>[!IMPORTANT]
>
>Sie können mit dem standardmäßigen Report Builder einen Bericht erstellen, der die Eins-zu-eins-Beziehung zwischen Objekten anzeigt. Sie können jedoch nur einen Bericht erstellen, der die Eins-zu-Viele-Beziehung zwischen Objekten anzeigt, indem Sie die Textmodus-Schnittstelle in Report Builder verwenden.

Weitere Informationen zum Erstellen eines Berichts im standardmäßigen Report Builder finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Weitere Informationen zum Erstellen eines Berichts mithilfe der Textmodusschnittstelle finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über häufige Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Übersicht über die Textmodussyntax](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Suchen nach Sammlungsobjekten und ihren Feldern im API-Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Nicht alle Sammlungen können gemeldet werden.

Um zu verstehen, welche Objekte mit einer Sammlung anderer Objekte verknüpft werden können, müssen Sie den API-Explorer verwenden.\
Weitere Informationen zur API Explorer-Tabelle finden Sie unter [API Explorer](../../../wf-api/general/api-explorer.md).

So erfahren Sie, über welche Sammlungen berichtet werden kann:

1. Navigieren Sie zum [API-Explorer](../../../wf-api/general/api-explorer.md).
1. Suchen Sie das Objekt Ihres Berichts.
1. Wählen Sie die **Sammlungen** aus.

   >[!NOTE]
   >
   >Nur die auf dieser Registerkarte aufgelisteten Objekte können für das ausgewählte Objekt als Sammlung in einem Bericht dargestellt werden.

1. Erweitern Sie das -Objekt Ihrer Sammlung, indem Sie darauf klicken.
1. Klicken Sie auf den angezeigten Link, um zum Objekt Ihrer Sammlung zu gelangen.\
   Dadurch wird die **Felder** für das Objekt Ihrer Sammlung geöffnet.

   >[!NOTE]
   >
   >Nur die auf dieser Registerkarte aufgeführten Felder können im Sammlungsbericht referenziert werden oder die Felder, die mit auf dieser Registerkarte aufgeführten Objekten verknüpft sind.

## Referenzieren von Sammlungen in Berichten

In den folgenden Berichtelementen können Sie auf Objekte aus einer Sammlung verweisen:

* Ansichten
* Filter
* Prompts

In den folgenden Berichtelementen können Sie nicht auf Objekte aus einer Sammlung verweisen:

* Gruppierungen
* Diagramm

Sie können beispielsweise auf die Aufgaben- oder Problemkollektionen in einem Projektbericht verweisen, um Aufgaben- oder Probleminformationen auf Projektebene anzuzeigen.

* [Referenzieren einer Sammlung in der Ansicht eines Berichts](#reference-a-collection-in-the-view-of-a-report)
* [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report)
* [Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Referenzieren einer Sammlung in der Ansicht eines Berichts {#reference-a-collection-in-the-view-of-a-report}

In der Ansicht eines Berichts können Sie auf eine Auflistung von Objekten verweisen, um Attribute von Objekten anzuzeigen, die mit dem Objekt des Berichts verknüpft sind.

Sie können beispielsweise Aufgaben- oder Probleminformationen in einem Projektbericht anzeigen, indem Sie eine Sammlungsspalte für Aufgaben oder Probleme in der Ansicht des Berichts erstellen.

Sie können Informationen zu den Aufgaben oder Problemen, wie Namen, Daten, primäre Beauftragte, Prozent abgeschlossen usw., in der Sammlungsansicht anzeigen.

Die Ansicht zeigt Aufgaben- oder Probleminformationen in einem Listenformat an, wobei jede Zeile der Liste Informationen zu einer Aufgabe oder einem Problem darstellt. Die Liste der Aufgaben oder Probleme und deren Felder wird in derselben Zeile wie das Projekt angezeigt, zu dem die Aufgaben oder Probleme gehören.

![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png){width=400}

* [Hinzufügen einer Sammlungsspalte in einer Berichtsansicht](#add-a-collection-column-in-a-report-view)
* [Verstehen der Zeilen einer Sammlungsansicht im Textmodus](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Einschränkungen einer Sammlungsansicht](#limitations-of-a-collection-view)

### Hinzufügen einer Sammlungsspalte in einer Berichtsansicht {#add-a-collection-column-in-a-report-view}

So fügen Sie eine Sammlungsspalte in einer Berichtsansicht hinzu:

1. Klicken Sie auf das **Hauptmenü** (![-](assets/main-menu-icon.png)) und dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie weg von Ihrem Bericht und ermitteln Sie mithilfe des [API-Explorers](../../../wf-api/general/api-explorer.md), welche Sammlungen für das Objekt verfügbar sind, das Sie für Ihren Bericht ausgewählt haben.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen nach Sammlungsobjekten und ihren Feldern im API-Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des -Objekts für die Auflistung.

1. Navigieren Sie mithilfe [API-Explorers](../../../wf-api/general/api-explorer.md) zur Liste der Felder für das Objekt, das Sie in der Sammlung anzeigen möchten.

   Weitere Informationen zum Suchen der Felder des -Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen nach Sammlungsobjekten und ihren Feldern im API-Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des Felds, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und klicken Sie auf der Registerkarte **Spalten (Ansicht** auf **Spalte hinzufügen**.
1. Klicken Sie **In Textmodus wechseln**.
1. Klicken Sie **Textmodus bearbeiten**.
1. Wählen Sie den gesamten Text im **Textmodus**-Dialogfeld aus, entfernen Sie ihn und fügen Sie dann den folgenden Code ein, wenn Sie auf ein Feld des Sammlungsobjekts verweisen:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Ersetzen **Spaltenname** durch den Namen Ihrer Spalte in der `displayname`.
1. Ersetzen Sie **Sammlungsobjektname** durch den Namen Ihres Sammlungsobjekts in der `listmethod`, wie er im [API-Explorer) ](../../../wf-api/general/api-explorer.md).

1. Ersetzen Sie **Feld des Sammlungsobjekts** durch den Namen des Felds Ihres Sammlungsobjekts in der `valuefield`, wie er im [API-Explorer) ](../../../wf-api/general/api-explorer.md).

   Sie können **valueField** durch **valueExpression** ersetzen, wenn Sie einen benutzerdefinierten Ausdruck in Ihrer Ansicht erstellen möchten.

   Weitere Informationen zu berechneten benutzerdefinierten Ausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Wenn Sie beispielsweise eine Liste der Aufgaben in einem Projektbericht anzeigen möchten. Diese Sammlung verwendet eine `valuefield` zum Referenzieren der Namen der Aufgaben.

   Führen Sie einen der folgenden Schritte aus:

   * Verwenden Sie den folgenden Code, um Ihre Spalte zu erstellen:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Verwenden Sie den folgenden Code, um eine Liste der Probleme im Bericht anzuzeigen:

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     Beachten Sie, dass Sie in einer Auflistung **Probleme** für die **listMethod**-Zeile anstelle von **opTasks** verwenden müssen, dem Datenbanknamen für Probleme. Informationen dazu, wann &quot;**&quot; und** &quot;**&quot; beim** von Problemen verwendet werden sollten, finden [ unter „Verwenden von „OpTask“ und „Problem“ beim Referenzieren von Problemen](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Wenn Sie eine Liste der Aufgaben in einem Projektbericht zusammen mit dem primären Bearbeiter anzeigen möchten, verwenden Sie eine **valueExpression**-Zeile, um auf die Namen der Aufgaben neben den Namen des primären Beauftragten zu verweisen, anstatt auf **valueField**.

     Verwenden Sie den folgenden Code, um Ihre Spalte zu erstellen:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. Die folgende Spalte wird im Projektbericht angezeigt und listet alle Aufgaben in jedem Projekt neben ihren primären Beauftragten auf:

   ![Projektbericht mit Aufgaben- und Empfängersammlung](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png){width=400}

1. Klicken Sie auf **Speichern**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicken Sie **Speichern + Schließen**, um den Bericht zu speichern.

#### Die Zeilen einer Sammlungsansicht im Textmodus verstehen

Die Zeilen in einer Textmodusansicht für eine Sammlung sind in der folgenden Tabelle aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Beispielzeile</strong> </th> 
   <th><strong>Beschreibung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Sie können verschiedene Werte für diese Zeile verwenden. Es wird jedoch empfohlen, dass der <code style="font-weight: normal;">valueformat</code> für eine Sammlungsliste <strong>HTML lautet</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Diese Zeile zeigt an, dass die Spalte im Textmodus konfiguriert wurde. Wenn Sie diese Zeile entfernen, fügt Workfront sie standardmäßig wieder hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>Der <code>type</code> einer Liste wird beim Erstellen einer Ansicht immer <code>iterate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Dies ist das Trennzeichen, das verwendet wird, um die Werte in Ihrer Liste zu trennen.<br>Es wird empfohlen, <code>&lt;p&gt;</code> zu verwenden, das einen Zeilenumbruch zwischen den Werten hinzufügt.</p> <p>Sie können auch Folgendes verwenden:</p> <p><code>&zwj;</code> (Joiner mit Nullbreite). Die Werte der Sammlung sind nicht voneinander getrennt.<br><strong>,</strong> =Kommatrennzeichen. Die Werte der Sammlung werden durch ein Komma getrennt, gefolgt von keinem Leerzeichen.<br><strong>/</strong> = Schrägstrich-Trennzeichen. Die Werte der Sammlung werden durch einen Schrägstrich getrennt.<br><strong>-</strong> = Bindestrich-Trennzeichen. Die Werte der Sammlung werden durch einen Bindestrich getrennt.<br>Wenn diese Zeile leer gelassen wird, wird standardmäßig ein Komma gefolgt von einem Leerzeichen zwischen den Werten der Sammlung hinzugefügt.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Spaltenname</em> </td> 
   <td> <p>Ersetzen <strong>Spaltenname</strong> durch den tatsächlichen Namen der neuen Spalte.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Diese Zeile definiert die Sammlung, auf die Sie verweisen.</p> <p>Ersetzen Sie <strong>Sammlungsobjektname</strong> durch den Namen des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie er im <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer) </a>. Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamens.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Diese Zeile definiert, auf welches Feld Sie vom Sammlungsobjekt verweisen.</p> <p>Ersetzen Sie <strong>Feld des Sammlungsobjekts</strong> durch den Namen des Felds des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie es im <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer) </a>.</p> <p>Sie können diese Zeile ersetzen durch:</p> <p><strong>valueExpression</strong>=Feld/Felder des berechneten Sammlungsobjekts</p> <p>Mit <strong>valueExpression</strong> können Sie  Zeigt einen berechneten benutzerdefinierten Ausdruck in der Spalte an.</p> <p>Weitere Informationen zum Formatieren von <strong>valueExpression</strong>-Zeilen finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Textmodus-Syntax</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Einschränkungen einer Sammlungsansicht {#limitations-of-a-collection-view}

Beachten Sie beim Erstellen einer Sammlungsansicht die folgenden Einschränkungen:

* Sie können nicht steuern, in welcher Reihenfolge die Sammlungsdaten angezeigt werden.
* Bedingte Formatierung kann nicht auf eine Sammlungsansicht angewendet werden.
* Sie können ein Objekt in einer Sammlung nicht zu einem anklickbaren Link machen.
* Sie können keine Sammlungsansicht einer anderen Sammlung erstellen.\
  Beispielsweise können Sie nicht alle Bevollmächtigten für jede Aufgabe in einem Projektbericht anzeigen. Sie können den primären Beauftragten nur für jede Aufgabe in einer Projektansicht anzeigen.

### Referenzieren einer Sammlung im Filter eines Berichts {#reference-a-collection-in-the-filter-of-a-report}

Sie können im Filter eines Berichts auf eine Auflistung von Objekten verweisen, um nach den Attributen von Objekten zu filtern, die mit dem Objekt des Berichts verknüpft sind.

Sie können beispielsweise nach Aufgaben- oder Probleminformationen in einem Projektbericht filtern, indem Sie in der Filteranweisung auf die Attribute von Aufgaben oder Problemen des Projekts verweisen.

>[!NOTE]
>
>Wenn der Filter auf Felder angewendet wird, die mehrere Werte enthalten (z. B. eine Sammlung von Notizen innerhalb eines Projekts), bestimmt er die Einbeziehung wie folgt:
>
>* Wenn alle Elemente in einer Sammlung den angegebenen Wert enthalten, wird der gesamte Datensatz aus den Ergebnissen ausgeschlossen.
>* Wenn mindestens ein Element in der Sammlung nicht den angegebenen Wert enthält, bleibt der Datensatz in den Ergebnissen.



So fügen Sie einen Verweis auf eine Sammlung in einem Berichtsfilter hinzu:

1. Klicken Sie auf das **Hauptmenü** (![-](assets/main-menu-icon.png)) und dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie weg von Ihrem Bericht und ermitteln Sie mithilfe des [API-Explorers](../../../wf-api/general/api-explorer.md), welche Sammlungen für das Objekt verfügbar sind, das Sie für Ihren Bericht ausgewählt haben.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen nach Sammlungsobjekten und ihren Feldern im API-Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des -Objekts für die Auflistung.

1. Navigieren Sie mithilfe [API-Explorers](../../../wf-api/general/api-explorer.md) zur Liste der Felder für das Objekt, das Sie in der Sammlung anzeigen möchten.

   Weitere Informationen zum Suchen der Felder des -Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen nach Sammlungsobjekten und ihren Feldern im API-Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich das Feld, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und klicken Sie auf der Registerkarte **Filter** auf **In Textmodus wechseln** und dann **Textmodus bearbeiten**.

1. Fügen **im Bereich Filterregeln für Ihren Bericht** folgenden Code ein:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Ersetzen Sie **Sammlungsobjektname** durch den Namen Ihres Sammlungsobjekts, wie er im [API-Explorer) ](../../../wf-api/general/api-explorer.md). Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamens.

1. Ersetzen Sie **Feld des Sammlungsobjekts** durch den Namen des Felds Ihres Sammlungsobjekts in , wie er im [API-Explorer) ](../../../wf-api/general/api-explorer.md).

1. Ersetzen Sie **Wert des Sammlungsobjekts** durch den Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.
1. Ersetzen Sie **Wert des Modifikators** durch einen gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter [Filter- und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Um beispielsweise einen Projektbericht zu erstellen, der nur Projekte mit Aufgaben anzeigt, deren Name „Marketing“ enthält, verwenden Sie den folgenden Code:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Dieser Bericht zeigt nur Projekte an, die mindestens eine Aufgabe mit dem Wort „Marketing“ in ihrem Namen haben.

   ![Nur Marketing-Aufgaben im Projekt](assets/marketing-only-tasks-in-project-report-nwe-350x309.png){width=400}

1. Verwenden Sie den folgenden Code, um nach dem Namen eines Problems zu filtern:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Beachten Sie, dass Sie `issues` für den Namen des Sammlungsobjekts verwenden müssen, anstatt `optask` zu verwenden, wie Probleme im API-Explorer angezeigt werden.

1. Klicken Sie **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicken Sie **Speichern + Schließen**, um den Bericht zu speichern.

### Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts {#reference-a-collection-in-the-custom-prompt-of-a-report}

Sie können in der benutzerdefinierten Eingabeaufforderung eines Berichts auf eine Auflistung von Objekten verweisen, um die Ergebnisse des Berichts nach den Attributen von Objekten zu filtern, die mit dem Objekt des Berichts verknüpft sind.

Sie können beispielsweise in einem Projektbericht auffordern, Aufgabeninformationen anzugeben, indem Sie in der benutzerdefinierten Eingabeaufforderung des Berichts einen Verweis auf die Attribute von Aufgaben für das Projekt verwenden.

>[!NOTE]
>
>Sie können in einer Standardaufforderung nicht auf Sammlungen verweisen.

Eine benutzerdefinierte Eingabeaufforderung ist ein benutzerdefinierter Filter, bei dem die Anweisungen durch kaufmännische Und-Zeichen verbunden werden. Es wird empfohlen, die Anweisung zunächst in einem Filter zu erstellen und dann die Zeilen der Anweisungen mit kaufmännischen Und-Zeichen zu verbinden.

Weitere Informationen zum Erstellen einer Filteranweisung mit einer Sammlungsreferenz finden Sie im Abschnitt [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel.

So fügen Sie in der benutzerdefinierten Eingabeaufforderung eines Berichts einen Verweis auf eine Sammlung hinzu:

1. Klicken Sie auf das **Hauptmenü** (![-](assets/main-menu-icon.png)) und dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Erstellen Sie einen Filter mit einer Sammlungsreferenz, wie im Abschnitt [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel beschrieben.
1. Klicken Sie **Berichteinstellungen**.
1. Klicken Sie **Eingabeaufforderungen melden**.
1. Klicken Sie **Eingabeaufforderung hinzufügen**.
1. Klicken Sie **Benutzerdefinierte Eingabeaufforderung**.
1. Geben Sie den Namen der Eingabeaufforderung im Feld **field**&#x200B;**name** an.

1. Geben Sie eine **Dropdown-Elementbezeichnung** an.
1. Geben Sie Folgendes im Feld **Bedingung** an:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Optional) Geben Sie an, ob diese Auswahl in der Eingabeaufforderung standardmäßig angezeigt wird.
1. Ersetzen Sie **Sammlungsobjektname** durch den Namen Ihres Sammlungsobjekts, wie er im [API-Explorer) ](../../../wf-api/general/api-explorer.md). Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamens.
1. Ersetzen Sie **Feld des Sammlungsobjekts** durch den Namen des Felds Ihres Sammlungsobjekts, wie es im [API-Explorer) ](../../../wf-api/general/api-explorer.md).
1. Ersetzen Sie **Wert des Sammlungsobjekts** durch den Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.

   Wenn Sie beispielsweise nach Projekten filtern, in denen der Name der Aufgabe „Marketing“ enthält, ersetzen Sie **Sammlungsobjektwert** durch **Marketing**.

1. Ersetzen Sie **Wert des Modifikators** durch einen gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter [Filter- und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Beispiel** Um beispielsweise einen Projektbericht mit einer benutzerdefinierten Eingabeaufforderung zu erstellen, in der Sie nur Projekte anzeigen möchten, denen mindestens eine Aufgabe einem bestimmten Benutzer zugewiesen ist, verwenden Sie den folgenden Code:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens eine Aufgabe zugewiesen ist, deren GUID 57cf1b7a000077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Sie können nicht auf den Namen des primären Verantwortlichen (Feld „Zugewiesen an„) einer Aufgabe verweisen, wie im [API-Explorer](../../../wf-api/general/api-explorer.md) angegeben. Sie können nur auf die ID des primären Verantwortlichen verweisen.

   Um beispielsweise nach Projekten zu filtern, bei denen eines der Projektprobleme einem bestimmten Benutzer zugewiesen ist, verwenden Sie den folgenden Code für Ihre benutzerdefinierte Eingabeaufforderung:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens ein Problem dem Benutzer zugewiesen ist, dessen GUID 57cf1b7a000077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Beachten Sie, dass Sie **Probleme** für den Sammlungsobjektnamen verwenden müssen. Der API-Explorer bietet derzeit keinen Sammlungsobjektnamen für Probleme.

1. Klicken Sie **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicken Sie **Speichern + Schließen**, um den Bericht zu speichern.
