---
product-area: reporting
navigation-topic: text-mode-reporting
title: Bearbeiten einer Ansicht im Textmodus
description: '"HINWEIS: fügen Sie in diesem Artikel einen Abschnitt hinzu: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Entwerfen Sie diesen Bereich auch im Artikel Textmodus-Übersicht )'''
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# Bearbeiten einer Ansicht im Textmodus

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Sie können eine Ansicht in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die nicht in der Standardoberfläche verfügbar sind, und komplexere Ansichten zu erstellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichterstellungselemente in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Ansichten in einem Bericht verwalten</p> <p>Berechtigungen für eine Ansicht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie mit der Verwendung des Textmodus in einem Bericht oder einer Liste beginnen, sollten Sie stets sicherstellen, dass Sie mit der Syntax des Workfront-Textmodus vertraut sind.

Weitere Informationen finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die Syntax der Textmodi](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Beispiele für benutzerdefinierte Ansicht, Filter und Gruppierung](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Textmodus in einer Ansicht bearbeiten

Die Bearbeitung einer Ansicht im Textmodus ist für Berichte und Listen identisch. Der Zugriff auf die Ansicht erfolgt über einen Bericht oder eine Liste.

>[!TIP]
>
>Es wird empfohlen, möglichst viele Ansichten im Standardmodus zu erstellen und sie dann in den Textmodus zu konvertieren, um sie zu bearbeiten.

Informationen zum Erstellen von Ansichten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Führen Sie einen der folgenden Schritte aus:

   1. Um von einem Bericht aus auf die Ansicht zuzugreifen, rufen Sie den Bericht auf und klicken Sie auf **Berichtaktionen** > **Bearbeiten** > **Spalten (Ansicht)** Registerkarte.
   1. Um von einer Liste aus auf die Ansicht zuzugreifen, navigieren Sie zur Liste und wählen Sie die **Ansicht** Dropdown-Menü, bewegen Sie den Mauszeiger über die Ansicht, die Sie ändern möchten, und klicken Sie auf **Bearbeiten** icon ![](assets/edit-icon.png).

      Der Ansichtsgenerator wird geöffnet.

1. Wählen Sie eine Spalte in der Ansicht aus.

   Oder

   Wählen Sie die **Spalten (Ansicht)** und wählen Sie eine Spalte aus.

   >[!TIP]
   >
   >Um eine Ansicht im Textmodus zu bearbeiten, müssen Sie jeweils eine Spalte bearbeiten.

1. Klicken **In den Textmodus wechseln** in der rechten oberen Ecke des Builders.

   >[!NOTE]
   >
   >Wenn Sie eine Spalte im Textmodus bearbeiten, fügt Workfront die `textmode=true` Codezeile zur Spalte hinzu. Dies bedeutet, dass die Spalte im Textmodus geändert wird.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   In der folgenden Tabelle werden die wichtigsten Zeilen in einer Textmodus-Ansicht beschrieben:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Beispielzeile</th> 
      <th>Beschreibung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valueField</strong>=</p> </td> 
      <td> <p>Dies ist der Name des Objekts oder des Felds, wie es in der Datenbank angezeigt wird. Weitere Informationen dazu, wie Objekte und Felder in der Datenbank angezeigt werden, finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> <p>Die folgenden Szenarien existieren:</p> 
       <ol> 
        <li value="1"> <p> Wenn der Name des angezeigten Felds eine Wortgruppe und nicht ein einzelnes Substantiv ist, müssen Sie für die <code>valuefield</code>. Für das geplante Startdatum einer Aufgabe lautet der Code beispielsweise: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Wenn Sie ein benutzerdefiniertes Feld anzeigen möchten, wird die <code>valuefield</code> -Wert ist der tatsächliche Name des Felds, wie er in der Benutzeroberfläche angezeigt wird. Für ein benutzerdefiniertes Feld mit dem Namen "Weitere Informationen"lautet der Code beispielsweise:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Wenn Sie Objekte anzeigen möchten, die mit anderen Objekten in einer Ansicht verbunden sind, verwenden Sie die <code>valuefield</code> Codezeile: Die Objektnamen und -attribute werden durch Doppelpunkte getrennt. </p> <p>Beispielsweise hat eine Spalte in einer Aufgabenansicht, die den Namen des Eigentümers des Portfolios anzeigen würde, den folgenden Wert für die Wertefeldzeile:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Dies bedeutet, dass Sie vom Objekt des Berichts (Aufgabe) aus auf das nächste verwandte Objekt (Projekt) zugreifen können. Von dort aus können Sie auf das folgende verwandte Objekt aus Projekt (Portfolio) zugreifen, dann auf den Portfolioinhaber (Eigentümer) und dann auf dessen Namen (Name). </p> </li> 
       </ol> <p>Informationen dazu, wie Objekte miteinander verbunden werden, finden Sie im Abschnitt <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Abhängigkeit und Hierarchie von Objekten</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in Adobe Workfront verstehen</a>.</p> <p>Hinweis: Wenn Sie ein Feld im Textmodus auswählen, das in der Standardschnittstelle nicht gültig ist, können Sie nicht zur Standardschnittstelle in der Spalte zurückkehren.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueFormat=</strong> </td> 
      <td> <p>Diese Zeile stellt das Format dar, das zum Anzeigen der <code>valuefield</code>. Die <code>valueformat</code> gibt an, ob ein Objekt oder Feld als Text, Zahl, Prozentsatz oder Datum angezeigt wird.</p> <p>Wir empfehlen, <code>HTML</code> für Ihre <code>valueformat</code>, insbesondere bei Verwendung von <code>valueexpression</code>, um eine möglichst genaue Anzeige Ihrer Informationen sicherzustellen. </p> <p>Weitere Informationen zu zusätzlichen Werten für diese Zeile finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Bedingte Formatierung im Textmodus verwenden</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueExpression=</strong> </p> </td> 
      <td> <p>Sie können diese Zeile hinzufügen, um <code>valuefield</code>, wenn Sie ein berechnetes Feld in der Spalte anzeigen möchten.</p> <p>Sie müssen die <code>valuefield</code> der Objekte in geschweiften Klammern jedes Mal, wenn Sie sie in einer <code>valueexpression</code>.</p> <p>Die folgenden Szenarien existieren: </p> 
       <ol> 
        <li value="1"> <p>Wenn Sie ein Feld in einer Spalte in Großbuchstaben anzeigen möchten, können Sie Folgendes verwenden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>Die <code>valuefield</code> des Objekts wird so geschrieben, wie es im API Explorer angezeigt wird. </p> </li> 
        <li value="2">Wenn Sie mehrere <code>valuefields</code> indem Sie sie zusammenreißen, müssen Sie sie durch einen Punkt trennen.</li> 
        <li value="3"> <p>Wenn Sie beispielsweise den Namen des Primären Verantwortlichen einer Aufgabe anzeigen möchten, indem Sie <code>valueexpression</code>verwenden:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Wenn Sie ein benutzerdefiniertes Feld in einem <code>valueexpression</code> Zeile, der Sie dem Feldnamen voranstellen müssen durch <code>DE:</code> um anzugeben, dass es sich um ein benutzerdefiniertes Feld handelt. Der Name des Felds wird so geschrieben, wie er in der Benutzeroberfläche angezeigt wird. </p> <p>Wichtig: Wenn Sie ein benutzerdefiniertes Feld verwenden, das in einem benutzerdefinierten Formularabschnitt platziert wird, der eingeschränkte Berechtigungen für einige Benutzer hat, ist die Berechnung des Werteausdrucks leer, wenn diese Benutzer diese Berechnung in einem Bericht anzeigen. Informationen zum Anpassen von Berechtigungen für benutzerdefinierte Formularabschnitte finden Sie unter <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a></span>.</p> <p>Wenn Sie beispielsweise ein benutzerdefiniertes Feld mit der Bezeichnung "Entwicklername"haben und dieses Feld in Großbuchstaben in einer Spalte anzeigen möchten, können Sie Folgendes verwenden: <code>valueexpression</code> um dies anzugeben:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds vom Typ "TypeAhead"den folgenden Ausdruck, um auf den Namen des Objekts zu verweisen, das in einem Feld mit der Bezeichnung "Entwicklername"ausgewählt wurde:</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Diese Zeile definiert den Text einer QuickInfo, wenn Sie den Mauszeiger über den Namen der Spalte bewegen. In diesem Fall wird ein Schlüssel verwendet, um den Namenswert im Beschreibungstext zu übersetzen. Wenn Sie die Beschreibung ändern möchten, ändern Sie diese Zeile in: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>nameKey= / name=</strong> </td> 
      <td> <p>Diese Zeile definiert den Spaltentitel. In diesem Fall wird der abgekürzte Wert basierend auf dem Schlüssel verwendet.</p> <p>Wenn Sie den Spaltennamen ändern möchten, können Sie diesen Wert wie folgt ändern: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> ermöglicht die Eingabe von Text für den Spaltennamen, während<code>namekey</code> erfordert die Eingabe eines Schlüssels, der zur Übersetzung des Spaltennamens verwendet wird.</p> <p>Um den Spaltennamen zu ändern, können Sie auch die <code>displayname </code>, wenn keine vorhanden ist.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayName =</strong> </td> 
      <td> <p>Sie können die folgende Zeile hinzufügen, um den Namen einer Spalte zu ändern, wodurch die <code>namekey/name</code> Wert:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Diese Zeile definiert, wie die Ergebnisse beim Klicken auf die Spaltenüberschrift sortiert werden. Wenn die Spalte nicht vorhanden ist, kann sie nach der Ausführung des Berichts nicht mehr sortiert werden.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Diese Zeile stellt die Anzahl der Pixel dar, die für die Spalte verwendet werden. Wenn die Zeile weggelassen oder auf 0 (null) gesetzt wird, wird die Spalte nicht in der Ansicht angezeigt.</p> <p>Wenn Sie dieses Feld manuell im Textmodus ändern, müssen Sie auch die <code>usewidths=true</code> -Wert in Ihre Spalte eingeben.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Sie müssen diese Zeile zusätzlich zum <code>width=</code> beim Anpassen der Breite einer Spalte. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Diese Zeile definiert, ob der in einer Spalte angezeigte Wert inline editierbar ist oder nicht. Wenn diese Zeile gleich <strong>true</strong>, ist der Wert in der Spalte inline editierbar. Wenn diese Zeile gleich <code>false</code>festgelegt ist, kann der Wert in der Spalte nicht inline bearbeitet werden.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueField=</strong> </td> 
      <td> <p>Fügen Sie diese Zeile nur ein, wenn der Wert in einer Spalte mit dem zugehörigen Objekt verknüpft werden soll. Der Link öffnet die Detailseite des Objekts. Dieser Wert sollte mit dem Wert <code>valuefield=</code> Linie. Wenn Sie dies einfügen, müssen Sie auch die <code>link.valueformat=</code> Linie. </p> <p> Sie können beispielsweise <code>link.valuefield=priority</code> in einer Problemansicht angezeigt und die Priorität des Problems als Link angezeigt. Wenn Sie auf diesen Link klicken, wird die Seite Problem geöffnet.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueFormat=</strong> </td> 
      <td> <p>Fügen Sie diese Zeile nur ein, wenn Sie die <code>link.valuefield</code> zum Hinzufügen eines Links zum Wert in einer Spalte. Der Link öffnet die Detailseite des Objekts. Dieser Wert sollte mit dem Wert <code>valueformat=</code> und gibt das Format an, das zum Anzeigen der <code>valuefield</code>. </p> <p>Wichtig: Beim Anzeigen des Textmodus in einer integrierten Spalte, die auch einen Link enthält, werden mehrere Zeilen angezeigt, die auf den Link verweisen. Einige dieser Zeilen werden möglicherweise nicht mehr unterstützt oder sind nicht erforderlich, wenn Sie eine eigene benutzerdefinierte Spalte im Textmodus erstellen und die Link-Anweisungen hinzufügen. Die Zeilen, die beim Hinzufügen eines verknüpften Werts erforderlich sind, sind<code> link.valuefield</code> und <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Dies bezieht sich darauf, wie die Werte der einzelnen Spalten zusammengefasst werden. Es gibt mehrere Zeilen, die mit beginnen <code>aggregator.</code> und alle beziehen sich auf den Aggregator, der die Ergebnisse der Spalte zusammenfasst. </p> <p>Im Allgemeinen wird die <code>aggregator.</code> -Zeilen entsprechen denen des Spaltenobjekts. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Beispiel: </b></span></span> 
        <p>Die Spalte Geplante Stunden in einem nach Summe zusammengefassten Aufgabenbericht kann wie folgt aussehen: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valueField=workRequired</pre>
         <pre>valueFormat=composite</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        Die <code>aggregator. </code>-Zeilen <code>valuefield </code>oder <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Anwenden** , wenn Sie Ihre Änderungen speichern und mit der Bearbeitung der Ansicht fortfahren möchten.
1. Klicken **Speichern und schließen** , um Ihren Bericht zu speichern.

   Oder

   Klicken **Ansicht speichern** , um die Ansicht in einer Liste zu speichern.
