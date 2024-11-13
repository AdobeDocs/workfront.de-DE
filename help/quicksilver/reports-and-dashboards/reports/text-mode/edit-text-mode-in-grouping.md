---
product-area: reporting
navigation-topic: text-mode-reporting
title: Textmodus in einer Gruppierung bearbeiten
description: "HINWEIS: Alle FVG-Artikel für die Bearbeitung im Textmodus gleich machen"
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 0%

---

# Textmodus in einer Gruppierung bearbeiten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

Sie können eine Gruppierung in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die nicht in der Standardoberfläche verfügbar sind, und komplexere Gruppierungen zu erstellen.

>[!TIP]
>
>Es wird empfohlen, möglichst viele Gruppierungen im Standardmodus zu erstellen und sie dann in den Textmodus zu konvertieren, um sie zu bearbeiten.

## Zugriffsanforderungen

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
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Gruppierungen in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Gruppierungen in einem Bericht verwalten</p> <p>Berechtigungen für eine Gruppierung verwalten, um sie zu bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie mit der Verwendung des Textmodus in einem Bericht oder einer Liste beginnen, sollten Sie stets sicherstellen, dass Sie mit der Syntax des Workfront-Textmodus vertraut sind.

Weitere Informationen finden Sie unter

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die Syntax im Textmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Beispiele für benutzerdefinierte Ansicht, Filter und Gruppierung: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Textmodus in einer Gruppierung bearbeiten

Die Bearbeitung einer Gruppierung im Textmodus ist für Berichte und Listen identisch. Der Zugriff auf die Gruppierung erfolgt über einen Bericht oder eine Liste.

>[!NOTE]
>
>Gruppierungen sind ein obligatorisches Berichterstellungselement für Grafiken in Berichten. Gruppierungen im Textmodus werden in Diagrammen nicht unterstützt. Weitere Informationen zum Hinzufügen von Diagrammen zu Berichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Weitere Informationen zum Erstellen von Gruppierungen finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Führen Sie einen der folgenden Schritte aus:

   1. Um von einem Bericht aus auf die Gruppierung zuzugreifen, gehen Sie zum Bericht und klicken Sie dann auf die Registerkarte **Berichtaktionen** > **Bearbeiten** > **Gruppierungen** .
   1. Um von einer Liste aus auf die Gruppierung zuzugreifen, gehen Sie zur Liste und bewegen Sie im Dropdown-Menü **Gruppierung** den Mauszeiger über die zu ändernde Gruppierung und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

      Der Gruppierungs-Builder wird geöffnet.

1. Klicken Sie auf **Gruppierung hinzufügen** , um die Gruppierungen hinzuzufügen, und klicken Sie dann oben rechts im Builder auf **In Textmodus wechseln** .

   >[!TIP]
   >
   >Sie können bis zu 3 Gruppierungen in der Standardschnittstelle hinzufügen. Sie können eine vierte Gruppierung nur im Textmodus hinzufügen. In Workfront sind maximal vier Gruppierungsebenen zulässig.

1. Beginnen Sie mit der Eingabe des Namens eines Felds, nach dem Sie eine Gruppe bilden möchten.

   Wählen Sie den Namen des Felds aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie oben rechts im Builder auf **In den Textmodus wechseln** .

   Die Gruppierung wird dann im Textmodus angezeigt.

   Wenn Sie eine Gruppierung im Textmodus bearbeiten, fügt Workfront die

   ```
   textmode=true
   ```

   Codezeile zur Gruppierung hinzu. Dies bedeutet, dass die Gruppierung im Textmodus geändert wird.

   **Beispiel:** Um eine Aufgabenliste nach Projektname und dann nach dem Namen des Primären Verantwortlichen zu gruppieren, sollte Ihre Gruppierung im Textmodus wie folgt aussehen:

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Die fettgedruckten Zeilen sind zwingend erforderlich.

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

   Jedes Feld in der Gruppierung hat mehrere Codezeilen, die auf dieses Feld verweisen.

   In der folgenden Tabelle sind die wichtigsten Zeilen einer Textmodusgruppierung aufgeführt.

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
      <td><strong>Gruppe.&lt;Zahl&gt;.</strong> </td> 
      <td> <p>Jeder Codezeile ist dieser Text vorangestellt. Die Codezeilen, die sich auf dasselbe in der Gruppierung ausgewählte Feld beziehen, werden wie folgt mit derselben Nummer nummeriert:</p> 
       <ul> 
        <li>Die erste Gruppierung des Berichts hat die Gruppennummer 0. Alle Zeilen, die auf die erste Gruppierung verweisen, beginnen mit <code>group.0</code>.</li> 
        <li>Die zweite Gruppierung des Berichts hat die Gruppennummer 1. Alle Zeilen, die auf die zweite Gruppierung verweisen, beginnen mit <em><code>group.1</code></em>.</li> 
        <li>Die dritte Gruppierung des Berichts besteht aus der 2. Alle Zeilen, die auf die dritte Gruppierung verweisen, beginnen mit <em><code>group.2</code></em>.</li> 
        <li>Nur im Textmodus können Sie die Gruppennummer 3 für eine vierte Gruppierung hinzufügen. Alle Zeilen, die auf die vierte Gruppierung verweisen, beginnen mit <em><code>group.3</code></em>.</li> 
       </ul> <p>Hinweis: 4 Gruppierungen werden im Builder nicht unterstützt. Sie werden nur bei Verwendung des Textmodus unterstützt. Workfront unterstützt nicht mehr als vier Gruppierungsebenen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueField</strong>=</p> </td> 
      <td> <p>Dies ist der Name des Objekts oder des Felds, wie es in der Datenbank angezeigt wird. Weitere Informationen dazu, wie Objekte und Felder in der Datenbank angezeigt werden, finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> <p>Die folgenden Szenarien existieren:</p> 
       <ol> 
        <li value="1"> <p> Wenn der Name des angezeigten Felds eine Wortgruppe und nicht ein einzelnes Substantiv ist, müssen Sie die Binnenmajuskel-Groß-/Kleinschreibung für die <code>valuefield</code> verwenden. Für das geplante Startdatum einer Aufgabe lautet der Code beispielsweise:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Wenn Sie ein benutzerdefiniertes Feld anzeigen möchten, ist der Wert <code>valuefield</code> der tatsächliche Name des Felds, wie er in der Benutzeroberfläche angezeigt wird. Für ein benutzerdefiniertes Feld mit dem Namen "Weitere Informationen"lautet der Code beispielsweise:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Wenn Sie mithilfe der Codezeile <code>valuefield</code> Objekte gruppieren möchten, die mit anderen Objekten verbunden sind, werden die Objektnamen und -attribute durch Doppelpunkte getrennt.</p> <p>Beispielsweise hat eine Gruppierung nach Portfolio für eine Aufgabenliste den folgenden Wert für die Wertefeldzeile:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Dies bedeutet, dass Sie vom Objekt des Berichts (Aufgabe) aus auf das nächste verwandte Objekt (Projekt) zugreifen können. Von dort aus können Sie auf das folgende verwandte Objekt aus Projekt (Portfolio) zugreifen und dann den Portfolionamen (Namen).</p> </li> 
       </ol> <p>Informationen dazu, wie Objekte miteinander verbunden werden, finden Sie im Abschnitt <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependenz und Hierarchie von Objekten</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in Adobe Workfront verstehen</a>.</p> <p>Hinweis: Wenn Sie ein Feld im Textmodus auswählen, das in der Standardoberfläche nicht gültig ist, und zur Standardoberfläche wechseln, wird die Gruppierung gelöscht.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueFormat=</strong> </td> 
      <td> <p>Diese Zeile stellt das Format dar, das zum Anzeigen des <code>valuefield</code> verwendet wird. Der Wert <code>valueformat</code> gibt an, ob ein Objekt oder Feld als Text, Zahl, Prozentsatz oder Datum angezeigt wird.</p> <p>Es wird empfohlen, <code>HTML</code> für Ihre <code>valueformat</code> zu verwenden, insbesondere bei Verwendung von <code>valueexpression</code>, um eine möglichst genaue Anzeige Ihrer Informationen sicherzustellen.</p> <p>Weitere Informationen zu zusätzlichen Werten für diese Zeile finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Bedingte Formatierung im Textmodus verwenden</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueExpression=</strong> </p> </td> 
      <td> <p>Sie können diese Zeile hinzufügen, um <code>valuefield</code> zu ersetzen, wenn Sie Ihre Liste durch eine Berechnung zwischen mehreren Feldern gruppieren möchten.</p> <p>Sie müssen die <code>valuefield</code> der Objekte jedes Mal, wenn Sie sie in einem <code>valueexpression</code> verwenden, in geschweifte Klammern setzen.</p> <p>Die folgenden Szenarien existieren:</p> 
       <ol> 
        <li value="1"> <p>Wenn Sie den Namen einer Gruppierung in Großbuchstaben anzeigen möchten, verwenden Sie:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>Die <code>valuefield</code> des Objekts wird so geschrieben, wie es im API Explorer angezeigt wird.</p> </li> 
        <li value="2">Wenn Sie mehrere <code>valuefields</code> hinzufügen möchten, indem Sie sie in einer <code>valueexpression </code> -Zeile zusammenführen, müssen Sie sie durch einen Punkt trennen.<p>Wenn Sie beispielsweise den Namen des Portfolios in Großbuchstaben in einer Aufgabenliste anzeigen möchten, verwenden Sie den folgenden Code in der Zeile <code>valueexpression</code> :</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Wenn Sie ein benutzerdefiniertes Feld in einer Zeile <code>valueexpression</code> verwenden möchten, müssen Sie dem Feldnamen durch <code>DE:</code> vorangehen, um anzugeben, dass es sich um ein benutzerdefiniertes Feld handelt. Der Name des Felds wird so geschrieben, wie er in der Benutzeroberfläche angezeigt wird.</p><p>Wichtig: <span>Wenn Sie ein benutzerdefiniertes Feld verwenden, das in einem benutzerdefinierten Formularabschnitt platziert wird, der eingeschränkte Berechtigungen für einige Benutzer hat, ist die Berechnung des <code>valueexpression </code> leer, wenn diese Benutzer diese Berechnung in einem Bericht anzeigen. Informationen zum Anpassen von Berechtigungen für benutzerdefinierte Formularabschnitte finden Sie unter</span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a></span>.</p><p>Wenn Sie beispielsweise ein benutzerdefiniertes Feld mit der Bezeichnung "Entwicklername"haben und nach diesem Feld gruppieren und es in Großbuchstaben anzeigen möchten, können Sie dies mit dem folgenden <code>valueexpression</code> angeben:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Verwenden Sie beim Referenzieren eines benutzerdefinierten Felds vom Typ "TypeAhead"den folgenden Ausdruck, um auf den Namen des Objekts zu verweisen, das in einem Feld mit der Bezeichnung "Entwicklername"ausgewählt wurde:</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Diese Zeile definiert den Gruppierungstitel. In diesem Fall wird der abgekürzte Wert basierend auf dem Schlüssel verwendet.</p> <p>Wenn Sie den Gruppierungsnamen ändern möchten, können Sie diesen Wert wie folgt ändern:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> ermöglicht die Eingabe von beliebigem Text für den Gruppierungsnamen, während für <code>namekey</code> die Eingabe eines Schlüssels erforderlich ist, der zur Übersetzung des Gruppierungsnamens verwendet wird.</p> <p>Um den Gruppierungsnamen zu ändern, können Sie auch die Zeile <code>displayname </code>hinzufügen, falls keine vorhanden ist.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayName =</strong> </td> 
      <td> <p>Sie können die folgende Zeile hinzufügen, um den Namen einer Spalte zu ändern, wodurch der Wert <code>namekey/name</code> überschrieben wird:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Es wird empfohlen, beim Umbenennen einer Gruppierung alle Zeilen zu entfernen, die "<code>name </code>enthalten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fügen Sie einer beliebigen Gruppierung eine der folgenden Codezeilen hinzu, um anzugeben, ob die Ergebnisse in der Gruppierung in einer erweiterten oder reduzierten Liste angezeigt werden sollen. Standardmäßig werden Gruppierungen erweitert:


   ```
   group.0.iscollapsed=true
   ```

   wenn die Gruppierung mit reduzierten Ergebnissen angezeigt werden soll

   ```
   group.0.iscollapsed=false
   ```

   wenn die Gruppierung mit erweiterten Ergebnissen angezeigt werden soll

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* Wenn Sie Gruppierungen bei der Anzeige einer Liste manuell anpassen, behält sich Workfront Ihre manuellen Voreinstellungen vor, bis Sie sich abmelden. Wenn Sie sich wieder anmelden, wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert, nachdem sie über ein Diagrammelement aufgerufen wurden.

1. Klicken Sie auf **Fertig** , wenn Sie Ihre Änderungen speichern und mit der Bearbeitung der Gruppierung oder des Berichts fortfahren möchten.
1. Klicken Sie in einer Liste auf **Gruppierung speichern** oder auf **Speichern + Schließen** , um den Bericht zu speichern.
