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

Weitere Informationen zum Erstellen eines Berichts in Workfront finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Berechtigungen für Ansichten, Filter oder Gruppierungen verwalten </p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
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

Weitere Informationen zum Erstellen eines Berichts in der standardmäßigen Berichterstellung finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Weitere Informationen zum Erstellen eines Berichts mithilfe der Textmodus-Oberfläche finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Überblick über häufige Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Übersicht über die Syntax der Textmodi](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Suchen von Sammlungsobjekten und ihren Feldern im API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Es können nicht alle Sammlungen in Berichten aufgeführt werden.

Um zu verstehen, welche Objekte mit einer Sammlung anderer Objekte verknüpft werden können, müssen Sie den API Explorer verwenden.\
Weitere Informationen zur API Explorer-Tabelle finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

Um herauszufinden, über welche Sammlungen berichtet werden kann, gehen Sie folgendermaßen vor:

1. Wechseln Sie zum [API-Explorer](../../../wf-api/general/api-explorer.md).
1. Suchen Sie das Objekt Ihres Berichts.
1. Wählen Sie die Registerkarte **Sammlungen** aus.

   >[!NOTE]
   >
   >Nur die auf dieser Registerkarte aufgelisteten Objekte können in einem Bericht für das ausgewählte Objekt als Sammlung dargestellt werden.

1. Erweitern Sie das Objekt Ihrer Sammlung, indem Sie darauf klicken.
1. Klicken Sie auf den angezeigten Link, um zum Objekt Ihrer Sammlung zu gelangen.\
   Dadurch wird die Registerkarte **fields** für das Objekt Ihrer Sammlung geöffnet.

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
* [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report)
* [Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Referenzieren einer Sammlung in der Berichtansicht {#reference-a-collection-in-the-view-of-a-report}

Sie können in der Ansicht eines Berichts auf eine Sammlung von Objekten verweisen, um Attribute von Objekten anzuzeigen, die mit dem Objekt des Berichts verknüpft sind.

Beispielsweise können Sie in einem Projektbericht Aufgaben- oder Probleminformationen anzeigen, indem Sie eine Kollektionsspalte für Aufgaben oder Probleme in der Berichtansicht erstellen.

Sie können Informationen zu Aufgaben oder Problemen wie Namen, Daten, primäre Zuweisung, prozentuale Abschlüsse usw. in der Sammlungsansicht anzeigen.

Die Ansicht zeigt Aufgaben- oder Probleminformationen in einem Listenformat an, wobei jede Zeile der Liste Informationen über eine Aufgabe oder ein Problem darstellt. Die Liste der Aufgaben oder Probleme und ihre Felder werden in derselben Zeile angezeigt wie das Projekt, zu dem die Aufgaben oder Probleme gehören.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Hinzufügen einer Sammlungsspalte in einer Berichtsansicht](#add-a-collection-column-in-a-report-view)
* [Grundlegendes zu den Zeilen einer Sammlungsansicht im Textmodus](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Einschränkungen einer Sammlungsansicht](#limitations-of-a-collection-view)

### Hinzufügen einer Kollektionsspalte in einer Berichtsansicht {#add-a-collection-column-in-a-report-view}

So fügen Sie eine Kollektionsspalte in einer Berichtsansicht hinzu:

1. Klicken Sie auf das Menü **Main** und dann auf **Berichte**.![](assets/main-menu-icon.png)
1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie von Ihrem Bericht weg und bestimmen Sie mithilfe des [API Explorer](../../../wf-api/general/api-explorer.md), welche Sammlungen für das für Ihren Bericht ausgewählte Objekt verfügbar sind.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und deren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.\
   Notieren Sie sich den Namen des Objekts für die Sammlung.

1. Rufen Sie mit dem [API Explorer](../../../wf-api/general/api-explorer.md) die Liste der Felder für das Objekt auf, das in der Sammlung angezeigt werden soll.

   Weitere Informationen zum Suchen der Felder des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und deren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des Felds, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und klicken Sie auf der Registerkarte **Spalten (Ansicht)** auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Bewegen Sie den Mauszeiger über das Dialogfeld und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Wählen Sie den gesamten Text im Dialogfeld **Textmodus** aus und entfernen Sie ihn. Fügen Sie dann den folgenden Code ein, wenn Sie auf ein Feld des Sammlungsobjekts verweisen:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Ersetzen Sie **Spaltenname** durch den Namen Ihrer Spalte in der Zeile `displayname` .
1. Ersetzen Sie **den Sammlungsobjektnamen** durch den Namen Ihres Sammlungsobjekts in der Zeile `listmethod`, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird.

1. Ersetzen Sie **das Sammlungsobjektfeld** durch den Namen des Felds Ihres Sammlungsobjekts in der Zeile `valuefield`, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird.

   Sie können **valueField** durch **valueExpression** ersetzen, wenn Sie einen benutzerdefinierten Ausdruck in Ihrer Ansicht erstellen möchten.

   Weitere Informationen zu berechneten benutzerdefinierten Ausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Beispiel: Sie möchten eine Liste der Aufgaben in einem Projektbericht anzeigen. Diese Sammlung verwendet eine Zeile `valuefield` , um auf die Namen der Aufgaben zu verweisen.

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

     Beachten Sie, dass Sie in einer Sammlung für die Zeile **listmethod** **issues** anstelle von **opTasks** verwenden müssen, der Datenbankname für Probleme ist. Informationen dazu, wann **Problem** verwendet werden soll und wann **opTask** verwendet werden soll, wenn auf Probleme verwiesen wird, finden Sie unter [Verwenden von &quot;opTask&quot;und &quot;issue&quot;beim Referenzieren von Problemen](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Wenn Sie eine Liste der Aufgaben in einem Projektbericht zusammen mit ihrem primären Verantwortlichen anzeigen möchten, verwenden Sie eine Zeile mit dem Wert **valueExpression** , um auf die Namen der Aufgaben zu verweisen, die an die Namen ihrer primären Verantwortlichen angrenzen, anstatt auf **valueField**.

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

   Klicken Sie auf **Speichern + Schließen** , um den Bericht zu speichern.

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
   <td> <p>Sie können für diese Zeile verschiedene Werte verwenden. Wir empfehlen jedoch, <code style="font-weight: normal;">valueformat</code> für eine Sammlungsliste <strong>HTML zu verwenden.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Diese Zeile zeigt an, dass die Spalte im Textmodus konfiguriert wurde. Wenn Sie diese Zeile entfernen, fügt Workfront sie standardmäßig wieder hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>Die <code>type</code> einer Liste ist immer <code>iterate</code>, wenn eine Ansicht erstellt wird.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Dies ist das Trennzeichen, mit dem die Werte in Ihrer Liste getrennt werden.<br>Wir empfehlen die Verwendung von <code>&lt;p&gt;</code> , wodurch ein Zeilenumbruch zwischen den Werten hinzugefügt wird.</p> <p>Sie können auch Folgendes verwenden:</p> <p><code>&amp;zwj;</code> (Joiner mit Nullbreite). Die Werte der Kollektion unterscheiden sich nicht zwischen ihnen.<br><strong>,</strong> =Kommatrennzeichen. Die Werte der Kollektion werden durch Kommas getrennt, gefolgt von Leerzeichen.<br><strong>/</strong> = Schrägstrich-Trennzeichen. Die Werte der Kollektion werden durch einen Schrägstrich getrennt.<br><strong>-</strong> = Bindestrich-Trennzeichen. Die Werte der Kollektion werden durch einen Bindestrich voneinander getrennt.<br>Wenn Sie diese Zeile leer lassen, wird standardmäßig ein Komma und danach ein Leerzeichen zwischen den Werten der Sammlung hinzugefügt.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Spaltenname</em> </td> 
   <td> <p>Ersetzen Sie <strong>Spaltenname</strong> durch den tatsächlichen Namen Ihrer neuen Spalte.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Diese Zeile definiert die Sammlung, auf die Sie verweisen.</p> <p>Ersetzen Sie <strong>den Namen des Sammlungsobjekts</strong> durch den Namen des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie er im <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a> angezeigt wird. Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Diese Zeile definiert, auf welches Feld Sie vom Kollektionsobjekt verweisen.</p> <p>Ersetzen Sie <strong>das Sammlungsobjektfeld</strong> durch den Namen des Felds des Objekts, auf das Sie in Ihrer Sammlung verweisen, wie er im <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a> angezeigt wird.</p> <p>Sie können diese Zeile durch Folgendes ersetzen:</p> <p><strong>valueExpression</strong>=calculated collection object field/ fields</p> <p>Mit <strong>valueExpression</strong> können Sie  einen berechneten benutzerdefinierten Ausdruck in der Spalte anzeigen.</p> <p>Weitere Informationen zum Formatieren von Zeilen mit <strong>Werteausdruck</strong> finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Syntax im Textmodus</a>.</p> </td> 
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

1. Klicken Sie auf das Menü **Main** und dann auf **Berichte**.![](assets/main-menu-icon.png)
1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Navigieren Sie von Ihrem Bericht weg und bestimmen Sie mithilfe des [API Explorer](../../../wf-api/general/api-explorer.md), welche Sammlungen für das für Ihren Bericht ausgewählte Objekt verfügbar sind.

   Weitere Informationen zum Auswählen des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und deren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich den Namen des Objekts für die Sammlung.

1. Rufen Sie mit dem [API Explorer](../../../wf-api/general/api-explorer.md) die Liste der Felder für das Objekt auf, das in der Sammlung angezeigt werden soll.

   Weitere Informationen zum Suchen der Felder des Objekts Ihrer Sammlung finden Sie im Abschnitt [Suchen von Sammlungsobjekten und deren Feldern im API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) in diesem Artikel.

   Notieren Sie sich das Feld, das Sie in der Sammlung anzeigen möchten.

1. Navigieren Sie zurück zu Ihrem Bericht und klicken Sie auf der Registerkarte **Filter** auf **In den Textmodus wechseln**.

1. Fügen Sie im Bereich **Filterregeln für Ihren Bericht festlegen** den folgenden Code ein:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Ersetzen Sie **den Sammlungsobjektnamen** durch den Namen Ihres Sammlungsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird. Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.

1. Ersetzen Sie **das Sammlungsobjektfeld** durch den Namen des Felds Ihres Sammlungsobjekts in , wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird.

1. Ersetzen Sie **den Wert des Sammlungsobjekts** durch den Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.
1. Ersetzen Sie den **Wert des Modifikators** durch einen gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
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
   >Beachten Sie, dass Sie für den Namen des Sammlungsobjekts &quot;`issues`&quot;anstelle von &quot;`optask`&quot;verwenden müssen, da Probleme im API Explorer angezeigt werden.

1. Klicken Sie auf **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicken Sie auf **Speichern + Schließen** , um den Bericht zu speichern.

### Referenzieren einer Sammlung in der benutzerdefinierten Eingabeaufforderung eines Berichts {#reference-a-collection-in-the-custom-prompt-of-a-report}

Sie können in der benutzerdefinierten Eingabeaufforderung eines Berichts auf eine Sammlung von Objekten verweisen, um die Ergebnisse des Berichts nach den Attributen der Objekte zu filtern, die mit dem Objekt des Berichts verknüpft sind.

Beispielsweise können Sie in einem Projektbericht zur Eingabe von Aufgabeninformationen auffordern, indem Sie in der benutzerdefinierten Eingabeaufforderung des Berichts einen Verweis auf die Attribute der Aufgaben im Projekt verwenden.

>[!NOTE]
>
>In einer Standardaufforderung können Sie nicht auf Sammlungen verweisen.

Eine benutzerdefinierte Eingabeaufforderung ist ein benutzerdefinierter Filter, bei dem die Anweisungen durch kaufmännische Und-Zeichen verbunden werden. Es wird empfohlen, dass Sie Ihre Anweisung in einem Filter erstellen und dann zunächst die Zeilen der Anweisungen mit Und-Zeichen verbinden.

Weitere Informationen zum Erstellen einer Filteranweisung mit einem Sammlungsverweis finden Sie im Abschnitt [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel.

So fügen Sie in der benutzerdefinierten Eingabeaufforderung eines Berichts einer Sammlung einen Verweis hinzu:

1. Klicken Sie auf das Menü **Main** und dann auf **Berichte**.![](assets/main-menu-icon.png)
1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie das Objekt Ihres Berichts aus.
1. Erstellen Sie einen Filter mit einer Sammlungsreferenz, wie im Abschnitt [Referenzieren einer Sammlung im Filter eines Berichts](#reference-a-collection-in-the-filter-of-a-report) in diesem Artikel beschrieben.
1. Klicken Sie auf **Berichtseinstellungen**.
1. Klicken Sie auf **Berichtaufforderungen**.
1. Klicken Sie auf **Aufforderung hinzufügen**.
1. Klicken Sie auf **Benutzerdefinierte Aufforderung**.
1. Geben Sie den Namen der Eingabeaufforderung im Feld **Feld***name** an.

1. Geben Sie eine **Bezeichnung für Dropdown-Elemente** an.
1. Geben Sie Folgendes im Feld **Bedingung** an:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Optional) Geben Sie an, ob diese Auswahl in der Eingabeaufforderung standardmäßig angezeigt wird.
1. Ersetzen Sie **den Sammlungsobjektnamen** durch den Namen Ihres Sammlungsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird. Dieser Wert ist normalerweise die Pluralform des Sammlungsobjektnamen.
1. Ersetzen Sie **das Sammlungsobjektfeld** durch den Namen des Felds Ihres Sammlungsobjekts, wie er im [API-Explorer](../../../wf-api/general/api-explorer.md) angezeigt wird.
1. Ersetzen Sie **den Wert des Sammlungsobjekts** durch den Wert des Sammlungsobjekts, wie er in Workfront angezeigt wird.

   Wenn Sie beispielsweise nach Projekten filtern, in denen der Name der Aufgabe &quot;Marketing&quot;enthält, ersetzen Sie den Wert des Kollektionsobjekts **durch den Wert** marketing **.**

1. Ersetzen Sie den **Wert des Modifikators** durch einen gültigen Modifikator.

   Eine Liste der Modifikatoren finden Sie unter  [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Beispiel:** Um beispielsweise einen Projektbericht mit einer benutzerdefinierten Eingabeaufforderung zu erstellen, in dem Sie nur Projekte anzeigen möchten, denen mindestens eine Aufgabe zugewiesen ist, verwenden Sie den folgenden Code:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens eine Aufgabe zugewiesen ist, deren GUID 57cf1b7a00077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Gemäß dem [API Explorer](../../../wf-api/general/api-explorer.md) können Sie nicht auf den Namen des primären Verantwortlichen ( Feld &quot;Zugeordnet zu&quot;) einer Aufgabe verweisen. Sie können nur auf die ID des primären Verantwortlichen verweisen.

   Um beispielsweise nach Projekten zu filtern, bei denen einem bestimmten Benutzer eines der Projektprobleme zugewiesen ist, verwenden Sie den folgenden Code für Ihre benutzerdefinierte Eingabeaufforderung:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Dadurch wird ein Bericht generiert, in dem allen aufgelisteten Projekten mindestens ein Problem zugewiesen ist, dessen GUID 57cf1b7a00077c9f02f66cb09c8f86c lautet.

   >[!NOTE]
   >
   >Beachten Sie, dass Sie **issues** für den Sammlungsobjektnamen verwenden müssen. Der API Explorer  bietet derzeit keinen Sammlungsobjektnamen für Probleme.

1. Klicken Sie auf **Fertig**.
1. (Optional) Fahren Sie mit der Bearbeitung des Berichts fort.

   Oder

   Klicken Sie auf **Speichern + Schließen** , um den Bericht zu speichern.
