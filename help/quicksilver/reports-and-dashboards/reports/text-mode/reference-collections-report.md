---
product-area: reporting
navigation-topic: text-mode-reporting
title: Referenzieren von Sammlungen in einem Bericht
description: Referenzieren von Sammlungen in einem Bericht
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# Referenzieren von Sammlungen in einem Bericht

Wenn Sie einen Bericht in Adobe Workfront erstellen, können Sie eine Reihe von Objekten, Feldern oder verknüpften Objekten in einer Liste, einem Raster oder einem Diagrammformat anzeigen.

Weitere Informationen zum Erstellen eines Berichts in Workfront finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Berechtigungen für Ansichten, Filter oder Gruppierungen verwalten </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Sammlungen

Eine Sammlung ist eine Liste von Objekten, die mit einem anderen Objekt verknüpft sind.

Sie haben die folgenden beiden Beziehungen zwischen Objekten in Workfront:

* **Eins-zu-Eins-Beziehung**: Ein Objekt kann jeweils nur mit einem anderen Objekt verknüpft werden.\
  Beispielsweise kann ein Projekt nur jeweils mit einem Portfolio verknüpft werden.

* **Eins-zu-viele-Beziehung**: Ein Objekt kann mit mehreren anderen Objekten gleichzeitig verknüpft werden.\
  Ein Projekt kann beispielsweise mehrere Aufgaben haben. In diesem Fall bildet die Aufgabenliste eine Sammlung für das Projekt.

>[!IMPORTANT]
>
>Mithilfe des standardmäßigen ReportBuilder können Sie einen Bericht erstellen, der die Eins-zu-Eins-Beziehung zwischen Objekten anzeigt. Sie können jedoch nur einen Bericht erstellen, der die Eins-zu-viele-Beziehung zwischen Objekten anzeigt, indem Sie die Textmodus-Oberfläche in ReportBuilder verwenden.

Weitere Informationen zum Erstellen eines Berichts in der standardmäßigen Berichterstellung finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Weitere Informationen zum Erstellen eines Berichts mithilfe der Textmodus-Oberfläche finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die häufigsten Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Übersicht über die Syntax der Textmodi](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Suchen von Sammlungsobjekten und ihren Feldern im API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Es können nicht alle Sammlungen in Berichten aufgeführt werden.

Um zu verstehen, welche Objekte mit einer Sammlung anderer Objekte verknüpft werden können, müssen Sie den API Explorer verwenden.\
Weitere Informationen zur Tabelle &quot;API Explorer&quot;finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).

Um herauszufinden, über welche Sammlungen berichtet werden kann, gehen Sie folgendermaßen vor:

1. Navigieren Sie zu [API-Explorer](../../../wf-api/general/api-explorer.md).
1. Suchen Sie das Objekt Ihres Berichts.
1. Wählen Sie die **Sammlungen** Registerkarte.

   >[!NOTE]
   >
   >Nur die auf dieser Registerkarte aufgelisteten Objekte können in einem Bericht für das ausgewählte Objekt als Sammlung dargestellt werden.

1. Erweitern Sie das Objekt Ihrer Sammlung, indem Sie darauf klicken.
1. Klicken Sie auf den angezeigten Link, um zum Objekt Ihrer Sammlung zu gelangen.\
   Dadurch wird die **fields** -Registerkarte für das Objekt Ihrer Sammlung.

   >[!NOTE]
   >
   >Nur die auf dieser Registerkarte aufgelisteten Felder können im Erfassungsbericht referenziert werden oder die Felder, die mit den auf dieser Registerkarte aufgelisteten Objekten verknüpft sind.

## Referenzsammlungen in Berichten

Sie können in den folgenden Berichterstellungselementen auf Objekte aus einer Sammlung verweisen:

* Ansichten
* Filter
* Prompts

Sie können in den folgenden Berichterstellungselementen nicht auf Objekte aus einer Sammlung verweisen:

* Gruppierungen
* Diagramm

Sie können beispielsweise auf die Aufgabe oder Problemkollektionen aus einem Projektbericht verweisen, um Aufgaben- oder Probleminformationen auf Projektebene anzuzeigen.

* [Referenzieren einer Sammlung in der Berichtansicht](#reference-a-collection-in-the-view-of-a-report)
* [Referenzieren einer Kollektion im Berichtsfilter](#reference-a-collection-in-the-filter-of-a-report)
* [Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Referenzieren einer Sammlung in der Berichtansicht {#reference-a-collection-in-the-view-of-a-report}

Sie können in der Ansicht eines Berichts auf eine Sammlung von Objekten verweisen, um Attribute von Objekten anzuzeigen, die mit dem Objekt des Berichts verknüpft sind.

Beispielsweise können Sie in einem Projektbericht Aufgaben- oder Probleminformationen anzeigen, indem Sie eine Kollektionsspalte für Aufgaben oder Probleme in der Berichtansicht erstellen.

Sie können Informationen zu Aufgaben oder Problemen wie Namen, Daten, primäre Zuweisung, prozentuale Abschlüsse usw. in der Sammlungsansicht anzeigen.

Die Ansicht zeigt Aufgaben- oder Probleminformationen in einem Listenformat an, wobei jede Zeile der Liste Informationen über eine Aufgabe oder ein Problem darstellt. Die Liste der Aufgaben oder Probleme und ihre Felder werden in derselben Zeile angezeigt wie das Projekt, zu dem die Aufgaben oder Probleme gehören.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Hinzufügen einer Kollektionsspalte in einer Berichtsansicht](#add-a-collection-column-in-a-report-view)
* [Machen Sie sich mit den Zeilen einer Sammlungsansicht im Textmodus vertraut](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Einschränkungen einer Sammlungsansicht](#limitations-of-a-collection-view)

### Hinzufügen einer Kollektionsspalte in einer Berichtsansicht {#add-a-collection-column-in-a-report-view}

So fügen Sie eine Kollektionsspalte in einer Berichtsansicht hinzu:

1. Klicken Sie auf **Main** Menü ![](assets/main-menu-icon.png)Klicken Sie auf **Berichte**.
1. Klicks **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie weg von Ihrem Bericht und verwenden Sie die [API-Explorer](../../../wf-api/general/api-explorer.md)bestimmen, welche Sammlungen für das Objekt verfügbar sind, das Sie für den Bericht ausgewählt haben.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt . [Suchen von Sammlungsobjekten und ihren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.\
   Notieren Sie sich den Namen des Objekts für die Sammlung.

1. Verwenden der [API-Explorer](../../../wf-api/general/api-explorer.md), navigieren Sie zur Liste der Felder für das Objekt, das Sie in der Sammlung anzeigen möchten.

   Weitere Informationen zum Suchen der Felder des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und ihren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des Felds, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und im **Spalten (Ansicht)** Registerkarte, klicken **Spalte hinzufügen**.
1. Klicks **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über das Dialogfeld und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Wählen Sie den gesamten Text im **Textmodus** und entfernen Sie es. Fügen Sie dann den folgenden Code ein, wenn Sie auf ein Feld des Sammlungsobjekts verweisen:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Ersetzen **Spaltenname** mit dem Namen Ihrer Spalte im `displayname` Linie.
1. Ersetzen **Sammlungsobjektname** mit dem Namen Ihres Sammlungsobjekts im `listmethod` in der [API-Explorer](../../../wf-api/general/api-explorer.md).

1. Ersetzen **Sammlungsobjektfeld** mit dem Namen des Felds des Kollektionsobjekts im `valuefield` in der [API-Explorer](../../../wf-api/general/api-explorer.md).

   Sie können **valueField** mit **valueExpression**, wenn Sie einen benutzerdefinierten Ausdruck in Ihrer Ansicht erstellen möchten.

   Weitere Informationen zu berechneten benutzerdefinierten Ausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Beispiel: Sie möchten eine Liste der Aufgaben in einem Projektbericht anzeigen. Diese Sammlung verwendet eine `valuefield` -Zeile, um auf die Namen der Aufgaben zu verweisen.

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

     Beachten Sie, dass Sie in einer Sammlung **issues** für die **listmethod** Zeile anstatt **opTasks** : der Datenbankname für Probleme. Informationen darüber, wann **Problem** und wann **opTask** Wenn Sie auf Probleme verweisen, lesen Sie [Verwenden Sie &quot;opTask&quot;und &quot;issue&quot;, wenn Sie auf Probleme verweisen](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Wenn Sie eine Liste der Aufgaben in einem Projektbericht zusammen mit ihrem primären Verantwortlichen anzeigen möchten, verwenden Sie eine **valueExpression** -Zeile für die Referenzierung der Namen der Aufgaben, die an die Namen ihrer primären Bevollmächtigten angrenzen, anstelle von **valueField**.

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

1. Die folgende Spalte wird im Projektbericht angezeigt und listet alle Aufgaben in den einzelnen Projekten zusammen mit ihren primären Verantwortlichen auf:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Klicken Sie auf **Speichern**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicks **Speichern und schließen** , um den Bericht zu speichern.

#### Machen Sie sich mit den Zeilen einer Sammlungsansicht im Textmodus vertraut

Die Zeilen in einer Textmodus-Ansicht für eine Sammlung sind in der folgenden Tabelle aufgeführt:

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
   <td> <p>Sie können für diese Zeile verschiedene Werte verwenden. Es wird jedoch empfohlen, <code style="font-weight: normal;">valueformat</code> für eine Sammlungsliste <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Diese Zeile zeigt an, dass die Spalte im Textmodus konfiguriert wurde. Wenn Sie diese Zeile entfernen, fügt Workfront sie standardmäßig wieder hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>Die <code>type</code> einer Liste <code>iterate</code>beim Erstellen einer Ansicht.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Dies ist das Trennzeichen, mit dem die Werte in Ihrer Liste getrennt werden.<br>Wir empfehlen, <code>&lt;p&gt;</code> fügt einen Zeilenumbruch zwischen den Werten hinzu.</p> <p>Sie können auch Folgendes verwenden:</p> <p><code>&amp;zwj;</code> (Joiner mit Nullbreite). Die Werte der Kollektion unterscheiden sich nicht zwischen ihnen.<br><strong>,</strong> =Kommatrennzeichen. Die Werte der Kollektion werden durch Kommas getrennt, gefolgt von Leerzeichen.<br><strong>/</strong> = Schrägstrich. Die Werte der Kollektion werden durch einen Schrägstrich getrennt.<br><strong>-</strong> = Bindestrich. Die Werte der Kollektion werden durch einen Bindestrich voneinander getrennt.<br>Wenn Sie diese Zeile leer lassen, wird standardmäßig ein Komma und danach ein Leerzeichen zwischen den Werten der Kollektion hinzugefügt.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Spaltenname</em> </td> 
   <td> <p>Ersetzen <strong>Spaltenname</strong> mit dem tatsächlichen Namen Ihrer neuen Spalte.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Diese Zeile definiert die Sammlung, auf die Sie verweisen.</p> <p>Ersetzen <strong>Sammlungsobjektname</strong> mit dem Namen des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie er in der <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>. Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Diese Zeile definiert, auf welches Feld Sie vom Kollektionsobjekt verweisen.</p> <p>Ersetzen <strong>Sammlungsobjektfeld</strong> mit dem Namen des Felds des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie er in der <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> <p>Sie können diese Zeile durch Folgendes ersetzen:</p> <p><strong>valueExpression</strong>=berechnetes Sammlungsobjektfeld/-felder</p> <p>Verwenden <strong>valueExpression</strong>können Sie einen berechneten benutzerdefinierten Ausdruck in der Spalte anzeigen.</p> <p>Weitere Informationen zum Formatieren <strong>valueExpression</strong> Zeilen, siehe <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Syntax der Textmodi</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Einschränkungen einer Sammlungsansicht {#limitations-of-a-collection-view}

Beachten Sie beim Erstellen einer Sammlungsansicht die folgenden Einschränkungen:

* Die Reihenfolge, in der die Kollektionsdaten angezeigt werden, lässt sich nicht steuern.
* Sie können eine Sammlungsansicht nicht mit bedingter Formatierung versehen.
* Sie können ein Objekt in einer Sammlung nicht zu einem anklickbaren Link machen.
* Sie können keine Sammlungsansicht einer anderen Sammlung erstellen.\
  Sie können beispielsweise nicht alle Bevollmächtigten für jede Aufgabe in einem Projektbericht anzeigen. Sie können den primären Verantwortlichen nur für jede Aufgabe in einer Projektansicht anzeigen.

### Referenzieren einer Kollektion im Berichtsfilter {#reference-a-collection-in-the-filter-of-a-report}

Sie können eine Sammlung von Objekten im Filter eines Berichts referenzieren, um nach Attributen von Objekten zu filtern, die mit dem Objekt des Berichts verknüpft sind.

Beispielsweise können Sie in einem Projektbericht nach Aufgaben- oder Probleminformationen filtern, indem Sie in der Filteranweisung einen Verweis auf die Attribute von Aufgaben oder Problemen im Projekt verwenden.

So fügen Sie einer Sammlung in einem Berichtsfilter einen Verweis hinzu:

1. Klicken Sie auf **Main** Menü ![](assets/main-menu-icon.png)Klicken Sie auf **Berichte**.
1. Klicks **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie weg von Ihrem Bericht und verwenden Sie die [API-Explorer](../../../wf-api/general/api-explorer.md)bestimmen, welche Sammlungen für das Objekt verfügbar sind, das Sie für den Bericht ausgewählt haben.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt . [Suchen von Sammlungsobjekten und ihren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des Objekts für die Sammlung.

1. Verwenden der [API-Explorer](../../../wf-api/general/api-explorer.md), navigieren Sie zur Liste der Felder für das Objekt, das Sie in der Sammlung anzeigen möchten.

   Weitere Informationen zum Suchen der Felder des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und ihren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich das Feld, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und im **Filter** Registerkarte, klicken **In den Textmodus wechseln**.

1. Im **Festlegen von Filterregeln für Ihren Bericht** den folgenden Code einfügen:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Ersetzen **Sammlungsobjektname** mit dem Namen Ihres Sammlungsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md). Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.

1. Ersetzen **Sammlungsobjektfeld** mit dem Namen des Felds Ihres Sammlungsobjekts in , wie er in der [API-Explorer](../../../wf-api/general/api-explorer.md).

1. Ersetzen **Sammlungsobjektwert** mit dem Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.
1. Ersetzen **Wert des Modifikators** mit einem gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Verwenden Sie beispielsweise den folgenden Code, um einen Projektbericht zu erstellen, der nur Projekte mit Aufgaben anzeigt, deren Name &quot;Marketing&quot;enthält:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Dieser Bericht zeigt nur Projekte an, deren Name mindestens eine Aufgabe enthält, deren Name das Wort &quot;Marketing&quot;enthält.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Verwenden Sie den folgenden Code, um nach dem Namen eines Problems zu filtern:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Beachten Sie, dass Sie `issues` für den Sammlungsobjektnamen anstelle von `optask` So werden Probleme im API Explorer angezeigt.

1. Klicks **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicks **Speichern und schließen** , um den Bericht zu speichern.

### Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts {#reference-a-collection-in-the-custom-prompt-of-a-report}

Sie können in der benutzerdefinierten Eingabeaufforderung eines Berichts auf eine Sammlung von Objekten verweisen, um die Ergebnisse des Berichts nach den Attributen der Objekte zu filtern, die mit dem Objekt des Berichts verknüpft sind.

Beispielsweise können Sie in einem Projektbericht zur Eingabe von Aufgabeninformationen auffordern, indem Sie in der benutzerdefinierten Eingabeaufforderung des Berichts einen Verweis auf die Attribute der Aufgaben im Projekt verwenden.

>[!NOTE]
>
>In einer Standardaufforderung können Sie nicht auf Sammlungen verweisen.

Eine benutzerdefinierte Eingabeaufforderung ist ein benutzerdefinierter Filter, bei dem die Anweisungen durch kaufmännische Und-Zeichen verbunden werden. Es wird empfohlen, dass Sie Ihre Anweisung in einem Filter erstellen und dann zunächst die Zeilen der Anweisungen mit Und-Zeichen verbinden.

Weitere Informationen zum Erstellen einer Filteranweisung mit einem Sammlungsverweis finden Sie im Abschnitt [Referenzieren einer Kollektion im Berichtsfilter](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel.

So fügen Sie in der benutzerdefinierten Eingabeaufforderung eines Berichts einer Sammlung einen Verweis hinzu:

1. Klicken Sie auf **Main** Menü ![](assets/main-menu-icon.png)Klicken Sie auf **Berichte**.
1. Klicks **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Erstellen Sie einen Filter mit einem Sammlungsverweis, wie im Abschnitt beschrieben. [Referenzieren einer Kollektion im Berichtsfilter](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel.
1. Klicks **Berichtseinstellungen**.
1. Klicks **Berichtsaufforderungen**.
1. Klicks **Eingabeaufforderung hinzufügen**.
1. Klicks **Benutzerdefinierte Aufforderung**.
1. Geben Sie den Namen der Aufforderung im **Feld***name** -Feld.

1. Geben Sie eine **Dropdown-Elementbeschriftung**.
1. Geben Sie Folgendes in der **Bedingung** -Feld:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Optional) Geben Sie an, ob diese Auswahl in der Eingabeaufforderung standardmäßig angezeigt wird.
1. Ersetzen **Sammlungsobjektname** mit dem Namen Ihres Sammlungsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md). Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.
1. Ersetzen **Sammlungsobjektfeld** mit dem Namen des Felds des Kollektionsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md).
1. Ersetzen **Sammlungsobjektwert** mit dem Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.

   Wenn Sie beispielsweise nach Projekten filtern, in denen der Name der Aufgabe &quot;Marketing&quot;enthält, ersetzen Sie **Sammlungsobjektwert** mit **Marketing**.

1. Ersetzen **Wert des Modifikators** mit einem gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter  [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Beispiel:** Um beispielsweise einen Projektbericht mit einer benutzerdefinierten Eingabeaufforderung zu erstellen, in der Sie nur Projekte anzeigen möchten, denen mindestens eine Aufgabe zugewiesen ist, verwenden Sie den folgenden Code:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens eine Aufgabe zugewiesen ist, deren GUID 57cf1b7a00077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Sie können den Namen des primären Verantwortlichen (&quot;Zugeordnetes Feld&quot;) einer Aufgabe nicht referenzieren, entsprechend dem [API-Explorer](../../../wf-api/general/api-explorer.md). Sie können nur auf die ID des primären Verantwortlichen verweisen.

   Um beispielsweise nach Projekten zu filtern, bei denen einem bestimmten Benutzer eines der Projektprobleme zugewiesen ist, verwenden Sie den folgenden Code für Ihre benutzerdefinierte Eingabeaufforderung:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens ein Problem zugewiesen ist, dessen GUID 57cf1b7a00077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Beachten Sie, dass Sie **issues** für den Sammlungsobjektnamen. Der API Explorer bietet derzeit keinen Sammlungsobjektnamen für Probleme.

1. Klicks **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicks **Speichern und schließen** , um den Bericht zu speichern.
