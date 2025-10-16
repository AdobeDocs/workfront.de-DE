---
product-area: reporting
navigation-topic: text-mode-reporting
title: Bearbeiten einer Gruppierung im Textmodus
description: Sie können eine Gruppierung in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die in der Standardbenutzeroberfläche nicht verfügbar sind, und komplexere Gruppierungen zu erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 1%

---

# Bearbeiten einer Gruppierung im Textmodus

<!-- Audited: 1/2025 -->

Sie können eine Gruppierung in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die in der Standardbenutzeroberfläche nicht verfügbar sind, und komplexere Gruppierungen zu erstellen.

>[!TIP]
>
>Es wird empfohlen, die Gruppierung so häufig wie möglich im Standardmodus zu erstellen und sie dann in den Textmodus zu konvertieren, um sie zu bearbeiten.

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
     <p>Standard</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Gruppierungen in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berichtsberechtigungen zum Bearbeiten von Gruppierungen in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Gruppierung, um sie zu bearbeiten</p></td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie mit der Verwendung des Textmodus in einem Bericht oder einer Liste beginnen, stellen Sie immer sicher, dass Sie mit der Workfront-Textmodussyntax vertraut sind.

Weitere Informationen finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die Textmodus-Syntax](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Beispiele für benutzerdefinierte Ansichten, Filter und Gruppierungen: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Bearbeiten einer Gruppierung im Textmodus

Das Bearbeiten einer Gruppierung im Textmodus ist für Berichte und Listen identisch. Der Zugriff auf die Gruppierung über einen Bericht oder eine Liste unterscheidet sich.

>[!NOTE]
>
>Gruppierungen sind ein obligatorisches Berichtselement zum Erstellen von Diagrammen in Berichten. Textmodusgruppierungen werden in Diagrammen nicht unterstützt. Informationen zum Hinzufügen von Diagrammen zu Berichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Weitere Informationen zum Erstellen von Gruppierungen finden Sie unter [Gruppierungen in Adobe Workfront erstellen](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Führen Sie einen der folgenden Schritte aus:

   1. Um über einen Bericht auf die Gruppierung zuzugreifen, gehen Sie zum Bericht und klicken Sie auf **Berichtsaktionen** > **Bearbeiten** > **Gruppierungen**.
   1. Um auf die Gruppierung über eine Liste zuzugreifen, gehen Sie zur Liste und klicken Sie **Dropdown-Menü** Gruppierung mit der Maus auf die Gruppierung, die Sie ändern möchten, und klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png).

      Der Gruppierungs-Builder wird geöffnet.

1. Klicken Sie **Gruppierung hinzufügen** um die Gruppierungen hinzuzufügen, klicken Sie in der oberen rechten Ecke **Builders auf** In Textmodus wechseln und klicken Sie dann auf **Textmodus bearbeiten**.

   >[!TIP]
   >
   >Sie können in der Standardschnittstelle bis zu drei Gruppierungen hinzufügen. Sie können eine vierte Gruppierung nur im Textmodus hinzufügen und Sie können in Workfront nicht mehr als vier Gruppierungsebenen haben.

1. Geben Sie den Namen eines Felds ein, nach dem Sie gruppieren möchten.

   Wählen Sie den Namen des Felds aus, wenn es in der Liste angezeigt wird.

1. Klicken **oben rechts** Builder auf „Zum Textmodus wechseln“.

   Die Gruppierung wird dann im Textmodus angezeigt.

   Wenn Sie eine Gruppierung im Textmodus bearbeiten, fügt Workfront die

   ```
   textmode=true
   ```

   Codezeile zur Gruppierung. Dies bedeutet, dass die Gruppierung im Textmodus geändert wird.

   **Beispiel** Um eine Liste von Aufgaben nach Projektname und dann nach dem Namen des Primären Verantwortlichen zu gruppieren, sollte die Gruppierung im Textmodus wie folgt aussehen:

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Die fett gedruckten Zeilen sind obligatorisch.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Jedes Feld in der Gruppierung verfügt über mehrere Codezeilen, die sich auf dieses Feld beziehen.

   In der folgenden Tabelle sind die Schlüsselzeilen in einer Textmodusgruppierung aufgeführt.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >Die Schlüsselzeilen in einer Textmodusgruppierung ähneln den Zeilen, die zum Erstellen von Textmodusansichten erforderlich sind.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

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
      <td><strong>Gruppe.&lt;number&gt;.</strong> </td> 
      <td> <p>Jeder Codezeile wird dieser Text vorangestellt. Die Codezeilen, die sich auf dasselbe in der Gruppierung ausgewählte Feld beziehen, sind mit derselben Nummer wie folgt nummeriert:</p> 
       <ul> 
        <li>Die erste Gruppierung des Berichts weist die Gruppennummer 0 auf. Alle Zeilen, die sich auf die erste Gruppierung beziehen, beginnen mit <code>group.0</code>.</li> 
        <li>Die zweite Gruppierung des Berichts hat die Gruppennummer 1. Alle Zeilen, die sich auf die zweite Gruppierung beziehen, beginnen mit <em><code>group.1</code></em>.</li> 
        <li>Die dritte Gruppe des Berichts ist die Gruppe 2. Alle Zeilen, die sich auf die dritte Gruppierung beziehen, beginnen mit <em><code>group.2</code></em>.</li> 
        <li>Nur im Textmodus können Sie eine Gruppennummer von 3 für eine vierte Gruppierung hinzufügen. Alle Zeilen, die sich auf die vierte Gruppierung beziehen, beginnen mit <em><code>group.3</code></em>.</li> 
       </ul> <p>Hinweis: 4 Gruppierungen werden im Builder nicht unterstützt. Sie werden nur im Textmodus unterstützt. Workfront unterstützt nicht mehr als vier Gruppierungsebenen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueField</strong>=</p> </td> 
      <td> <p>Dies ist der Name des Objekts oder Felds, wie er in der Datenbank angezeigt wird. Weitere Informationen zur Darstellung von Objekten und Feldern in der Datenbank finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> <p>Die folgenden Szenarien sind vorhanden:</p> 
       <ol> 
        <li value="1"> <p> Wenn der Name des angezeigten Felds eine Phrase anstelle eines einzelnen Substantivs ist, müssen Sie für das <code>valuefield</code> die Binnenmajuskeln-Syntax verwenden. Für das geplante Startdatum einer Aufgabe lautet der Code beispielsweise:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Wenn Sie ein benutzerdefiniertes Feld anzeigen möchten, ist der <code>valuefield</code> Wert der tatsächliche Name des Felds, wie er in der Benutzeroberfläche angezeigt wird. Für ein benutzerdefiniertes Feld mit dem Namen „Weitere Informationen“ lautet der Code beispielsweise:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Wenn Sie nach Objekten gruppieren möchten, die sich auf andere Objekte beziehen, indem Sie die <code>valuefield</code> Codezeile verwenden, werden die Objektnamen und Attribute durch Doppelpunkte getrennt.</p> <p>Beispielsweise hat eine Gruppierung nach Portfolio-Name für eine Aufgabenliste den folgenden Wert für die Zeile valueField :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Dies bedeutet, dass Sie über das Objekt des Berichts (Aufgabe) auf das nächste zugehörige Objekt (Projekt) zugreifen können. Von dort aus können Sie auf das folgende zugehörige Objekt über Projekt (Portfolio) zugreifen. Anschließend können Sie auf den Portfolionamen (Namen) zugreifen.</p> </li> 
       </ol> <p>Informationen dazu, wie Objekte miteinander verbunden werden, finden Sie im Abschnitt <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependenz und Hierarchie von Objekten</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in Adobe Workfront verstehen</a>.</p> <p>Hinweis: Wenn Sie ein Feld im Textmodus auswählen, das in der Standardschnittstelle nicht gültig ist, und zur Standardschnittstelle wechseln, wird die Gruppierung gelöscht.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueFormat=</strong> </td> 
      <td> <p>Diese Linie stellt das Format dar, das zum Anzeigen der <code>valuefield</code> verwendet wird. Die <code>valueformat</code> gibt an, ob ein Objekt oder Feld als Text, Zahl, Prozentsatz oder Datum angezeigt wird.</p> <p>Es wird empfohlen, <code>HTML</code> für Ihre <code>valueformat</code> zu verwenden, insbesondere bei der Verwendung von <code>valueexpression</code>, um eine möglichst genaue Anzeige Ihrer Informationen zu gewährleisten.</p> <p>Weitere Informationen zu zusätzlichen Werten für diese Zeile finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Verwenden der bedingten Formatierung im Textmodus</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueExpression=</strong> </p> </td> 
      <td> <p>Sie können diese Zeile hinzufügen, um <code>valuefield</code> zu ersetzen, wenn Sie Ihre Liste durch eine Berechnung zwischen mehreren Feldern gruppieren möchten.</p> <p>Sie müssen die <code>valuefield</code> der Objekte jedes Mal in geschweiften Klammern einschließen, wenn Sie sie in einer <code>valueexpression</code> verwenden.</p> <p>Die folgenden Szenarien sind vorhanden:</p> 
       <ol> 
        <li value="1"> <p>Wenn Sie den Namen einer Gruppierung in Großbuchstaben anzeigen möchten, verwenden Sie Folgendes:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>Die <code>valuefield</code> des -Objekts wird so geschrieben, wie es im API-Explorer angezeigt wird.</p> </li> 
        <li value="2">Wenn Sie mehrere <code>valuefields</code> hinzufügen möchten, indem Sie sie in einer Zeile <code>valueexpression </code>, müssen Sie sie durch einen Punkt trennen.<p>Wenn Sie beispielsweise den Namen des Portfolios in einer Aufgabenliste in Großbuchstaben anzeigen möchten, würden Sie den folgenden Code in der <code>valueexpression</code> verwenden:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Wenn Sie ein benutzerdefiniertes Feld in einer <code>valueexpression</code> verwenden möchten, müssen Sie dem Namen des Felds <code>DE:</code> voranstellen, um anzugeben, dass es sich um ein benutzerdefiniertes Feld handelt. Der Name des Felds wird so geschrieben, wie er in der Benutzeroberfläche angezeigt wird.</p><p>Wichtig: <span>Wenn Sie ein benutzerdefiniertes Feld verwenden, das in einem benutzerdefinierten Formularabschnitt platziert wird, der für einige Benutzer eingeschränkte Berechtigungen hat, ist die Berechnung des <code>valueexpression </code> leer, wenn diese Benutzer diese Berechnung in einem Bericht anzeigen. Informationen zum Anpassen von Berechtigungen für benutzerdefinierte Formularabschnitte finden Sie unter</span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a></span>.</p><p>Wenn Sie beispielsweise ein benutzerdefiniertes Feld mit der Bezeichnung „Entwicklername“ haben und Sie nach diesem Feld gruppieren und es in Großbuchstaben anzeigen möchten, können Sie die folgende <code>valueexpression</code> verwenden, um dies anzugeben:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds mit automatischer Textvervollständigung den folgenden Ausdruck, um auf den Namen des in einem Feld mit der Bezeichnung „Entwicklername“ ausgewählten Objekts zu verweisen:</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>nameKey= / name=</strong> </td> 
      <td> <p>Diese Zeile definiert den Gruppierungstitel. In diesem Fall wird der abgekürzte Wert auf Grundlage des Schlüssels verwendet.</p> <p>Wenn Sie den Gruppierungsnamen ändern möchten, können Sie diesen Wert wie folgt ändern:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> Ermöglicht die Eingabe eines beliebigen Textes für den Gruppierungsnamen, während <code>namekey</code> die Eingabe eines Schlüssels zur Übersetzung des Namens einer Gruppierung erfordert.</p> <p>Um den Gruppierungsnamen zu ändern, können Sie auch die <code>displayname </code>Zeile hinzufügen, falls noch kein Gruppierungsname vorhanden ist.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayName =</strong> </td> 
      <td> <p>Sie können die folgende Zeile hinzufügen, um den Namen einer Spalte zu ändern, wodurch der <code>namekey/name</code> überschrieben wird:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Es wird empfohlen, beim Umbenennen einer Gruppierung alle <code>name </code> enthaltenen Zeilen zu entfernen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fügen Sie einer Gruppierung eine der folgenden Codezeilen hinzu, um anzugeben, ob die Ergebnisse in der Gruppierung in einer erweiterten oder reduzierten Liste angezeigt werden sollen. Standardmäßig werden Gruppierungen erweitert angezeigt:


   ```
   group.0.iscollapsed=true
   ```

   Wenn die Gruppierung mit ausgeblendeten Ergebnissen angezeigt werden soll

   ```
   group.0.iscollapsed=false
   ```

   Wenn die Gruppierung mit erweiterten Ergebnissen angezeigt werden soll

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* Wenn Sie beim Anzeigen einer Liste Gruppierungen manuell anpassen, speichert Workfront Ihre manuellen Einstellungen, bis Sie sich abmelden. Beim erneuten Anmelden wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert angezeigt, nachdem über ein Diagrammelement darauf zugegriffen wurde.

1. Klicken Sie **Fertig**, wenn Sie Ihre Änderungen speichern und die Gruppierung oder den Bericht weiter bearbeiten möchten.
1. Klicken Sie **Gruppierung speichern** in einer Liste oder **Speichern + schließen** um Ihren Bericht zu speichern.
