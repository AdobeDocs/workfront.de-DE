---
title: Dateitypen verbinden
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Adobe Workfront Planning-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu behalten.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 7b5441b2aa17b22f0fd54cfe4921aa5dab2e0461
workflow-type: tm+mt
source-wordcount: '2222'
ht-degree: 1%

---


# Datensatztypen verbinden

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Sandbox-Umgebung verfügbar.</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Sie können Datensatztypen miteinander verbinden oder Sie können Datensatztypen mit Objekttypen aus anderen Anwendungen verbinden.

In diesem Artikel wird beschrieben, wie Sie zwei Datensatztypen der Workfront-Planung oder einen Datensatztyp der Workfront-Planung mit einem Objekt aus einer anderen Anwendung verbinden können.

Nachdem Sie die Verbindung zwischen Datensätzen oder Objekttypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden und Felder aus den verknüpften Datensätzen oder Objekttypen in einem Workfront Planning-Datensatz anzeigen.

Allgemeine Informationen zu Verbindungstypen finden Sie unter [Übersicht über Connected Record Types](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Informationen zum Verbinden von Datensätzen oder Datensätzen mit Objekten aus anderen Anwendungen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen und Datensätzen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Standard</p> 
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Datensatztypen verbinden

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie verbinden möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Klicken Sie oben rechts in der Tabellenansicht auf das Symbol **+** und dann auf die Registerkarte **Neue Verbindung** .

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Suchen Sie im Feld **Record type** nach einem Datensatztyp oder wählen Sie einen der folgenden Typen aus:

   * Ein anderer Datensatztyp aus dem aktuellen Arbeitsbereich

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >Wenn im ausgewählten Arbeitsbereich keine anderen Datensatztypen vorhanden sind, wird der Arbeitsbereich-Bereich nicht angezeigt.


   * Ein Datensatztyp aus einem anderen Arbeitsbereich, der für die Verbindung von anderen Arbeitsbereichen konfiguriert wurde. Weitere Informationen finden Sie unter [Bearbeiten von Datensatztypen](/help/quicksilver/planning/architecture/edit-record-types.md).

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >Wenn keine Datensatztypen konfiguriert sind, um eine Verbindung mit anderen Arbeitsbereichen herzustellen, wird der Arbeitsbereich-Abschnitt nicht angezeigt.


   * Ein **Projekt, Portfolio, Programm, Firma** oder **Gruppe** aus dem Abschnitt **Workfront-Objekttypen** .

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** aus dem Abschnitt **Adobe-Anwendungen**.

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Der Name des verbundenen Felds, wie er in der Tabellenansicht oder auf der Datensatzseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verknüpfte Datensatzspalte in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatzfelds für die ursprünglichen Datensätze erstellt. Standardmäßig ist der Name des Felds der Name des Datensatzes oder Objekts, mit dem Sie eine Verbindung herstellen.

   >[!TIP]
   >
   >Sie können mehrere Verbindungen zum selben Datensatz oder Objekttyp haben. Wenn Sie den Namen des verbundenen Felds nicht bearbeiten, fügt Workfront eine Zahl nach dem Namen des verbundenen Datensatzes hinzu, um die Anzahl der verbundenen Datensatztypen mit demselben Namen anzugeben.

   * **Beschreibung**: Zusätzliche Informationen zum verbundenen Datensatzfeld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Mehrere Datensätze zulassen**: Wählen Sie diese Option, um anzugeben, dass Benutzer mehrere Datensätze hinzufügen dürfen, wenn das Feld des verknüpften Datensatztyps in den Originaldatensätzen angezeigt wird. Diese Option ist standardmäßig aktiviert.

     Diese Option ist nur verfügbar, wenn Datensätze aus zwei verschiedenen Arbeitsbereichen oder einem Datensatz und einem Adobe Experience Manager-Asset-Objekt verbunden werden.

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **Verbindungstyp**: Wählen Sie eine der folgenden Optionen aus, um anzugeben, mit wie vielen Datensätzen sie eine Verbindung herstellen können:

      * Viele-zu-viele
      * Eins-zu-viele
      * Viele-zu-eins
      * Eins-zu-eins

     Diese Option ist nur verfügbar, wenn Datensätze aus demselben Arbeitsbereich, einem Datensatz und einem Workfront-Objekttyp verbunden werden.

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     Weitere Informationen zu Verbindungstypen finden Sie unter [Übersicht über Connected Record Types](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Suchfelder auswählen**: Wählen Sie diese Option, um Felder aus dem ausgewählten Datensatztyp hinzuzufügen. Die Suchfelder sind Felder, die mit dem Datensatz oder Objekttyp verknüpft sind, mit dem Sie verknüpft sind. Die Verknüpfung zeigt Informationen aus dem Datensatz oder Objekt an, mit dem Sie in dem Datensatz verknüpfen, von dem Sie die Verknüpfung herstellen. Diese Option ist standardmäßig aktiviert.

     >[!TIP]
     >
     > Sie können die folgenden Feldtypen nicht als Suchfelder hinzufügen:
     >
     >    * Personen
     >    * Erstellt von
     >    * Zuletzt geändert von
     >    * Workfront typeahead-Felder (einschließlich Feldern wie Projekteigentümer oder Projektsponsor)

1. (Bedingt und optional) Wenn Sie die Verbindung eines Workfront-Objekts ausgewählt haben, wählen Sie ein **Benutzerdefiniertes Formular** aus dem Abschnitt **Nur Objekte verknüpfen, die diesen Kriterien entsprechen** . Nur Objekte, an die die ausgewählten benutzerdefinierten Formulare angehängt sind, können mit dem ausgewählten Datensatztyp verknüpft werden. Sie können mehrere Formulare auswählen.

   >[!NOTE]
   >
   > Sie müssen benutzerdefinierte Formulare in Workfront für die ausgewählten Objekte erstellen, bevor sie in dieser Liste angezeigt werden.

1. (Bedingt) Wenn Sie ausgewählt haben, dass eine Verbindung mit Experience Manager Assets hergestellt werden soll, wählen Sie ein Repository aus dem Dropdownmenü **Experience Manager-Repository** im Abschnitt **Verknüpfen von Assets aus dem folgenden Repository** aus. Dies ist ein erforderliches Feld. In diesem Feld werden nur Repositorys angezeigt, auf die Sie in Experience Manager Assets Zugriff haben.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann Experience Manager Assets-Feldern Planungsfelder über das Metadaten-Mapping in Workfront zuordnen. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Bedingt) Wenn Sie die Verbindung mit Experience Manager Assets oder einem Workfront-Planungs-Datensatztyp hergestellt haben, wählen Sie eine der folgenden Optionen im Bereich **Erscheinungsbild von Datensätzen** aus:

   * <span class="preview">**Name und Bild**: Sowohl der Name als auch die Miniaturansicht oder das Symbol der verbundenen Datensätze werden im Feld des verbundenen Datensatzes angezeigt. Dies ist die Standardoption. </span>
   * <span class="preview">**Name**: Nur der Name der verbundenen Datensätze wird im Feld des verbundenen Datensatzes angezeigt.</span>
   * <span class="preview">**Bild**: Nur die Miniaturansicht oder das Symbol der verbundenen Datensätze wird im Feld des verbundenen Datensatzes angezeigt.</span>

   Datensätze ohne Miniaturbild zeigen stattdessen das Symbol des Datensatztyps an. Ein Beispiel dafür, wie die verbundenen Datensätze im Bereich **Erscheinungsbild eines Datensatzes** angezeigt werden.

   >[!NOTE]
   >
   >* Wenn Sie zulassen, dass mehrere Datensätze verknüpft werden, kann die Anzeige nur der Miniaturansicht in kleineren Bereichen, wie z. B. Datensatzansichten, Platz sparen.
   >
   >* Der Name eines Datensatzes ist das primäre Feld des Datensatzes. Weitere Informationen finden Sie unter [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >* Die Auswahl eines Datensatzaussehens ist bei der Auswahl von Workfront-Objekttypen nicht möglich.
   >
   >* Was Sie im Anzeigebereich &quot;Datensatz&quot;auswählen, bestimmt, wie die Datensätze in allen Verbindungen des Systems angezeigt werden, einschließlich aller Ansichten und Detailseiten.

1. Klicken Sie auf **Erstellen**.

1. (Bedingt) Wenn Sie die Einstellung **Suchfeld auswählen** ausgewählt haben, wird das Feld **Suchfelder hinzufügen** geöffnet.

   Klicken Sie auf das Symbol **+** , um Felder aus dem Bereich **Nicht ausgewählte Felder** hinzuzufügen.

   Oder

   Klicken Sie auf das Symbol **-** , um Felder aus dem Bereich **Ausgewählte Felder** zu entfernen.

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Die Werte für die verbundenen Felder werden automatisch ausgefüllt, nachdem Sie Datensätze oder Objekte verknüpft haben.

   >[!IMPORTANT]
   >
   >    Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in der Anwendung der verknüpften Objekttypen.


1. (Optional) Klicken Sie auf **Überspringen** , um das Hinzufügen von Feldern aus dem verknüpften Datensatz oder Objekttyp zu überspringen. Der Name oder das Primäre Feld des verknüpften Datensatzes ist das einzige sichtbare Feld in der Tabellenansicht des Datensatztyps, von dem Sie eine Verbindung herstellen.

1. (Optional und bedingt) Wenn Sie ein Feld vom Typ Zahl, Währung, Prozentsatz oder Datum verknüpfen möchten, wählen Sie auch einen Aggregatorwert aus, um mehrere Werte zusammenzufassen. Die Werte der verknüpften Felder werden entweder durch Kommas getrennt oder als zusammengefasster Wert entsprechend dem ausgewählten Aggregator angezeigt, wenn Benutzer im verknüpften Datensatzfeld mehr als einen verknüpften Datensatz auswählen.

   Wenn das Suchfeld mehrere Werte enthält, die nicht zusammengefasst sind, sollten Sie Folgendes beachten, wenn Sie das Feld bei der Sortierung oder Gruppierung in einer Ansicht verwenden:

   * Die Sortierung erfolgt durch den ersten Wert.

   * Datensätze werden nach jeder eindeutigen Kombination von Feldwerten gruppiert

   * Die Timeline-Ansicht basiert auf dem ersten Datumswert

   >[!IMPORTANT]
   >
   >    Sie müssen beim Hinzufügen von Suchdatumsfeldern einen Aggregatorwert auswählen, wenn die Felder verfügbar sein sollen, um als Start- und Enddaten für die Timeline- und Kalenderansichten hinzuzufügen. Sie können beispielsweise den MAX- oder MIN-Aggregator für ein Suchdatumsfeld auswählen.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Beim Verbinden von Datensatztypen mit Experience Manager Assets sind keine Aggregatoren verfügbar.

   Wählen Sie aus den folgenden Optionen aus:

   * **None**: Zeigt die Werte an, die aus mehreren durch Kommas getrennten Datensätzen stammen. Dies ist die Standardauswahl.
   * **MAX**: Zeigt den höchsten Wert aus allen Werten an, die aus mehreren im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **MIN**: Zeigt den niedrigsten Wert aus allen Werten an, die aus mehreren im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **SUM**: Zeigt die Summe aller Werte an, die aus mehreren im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **AVG**: Zeigt den Durchschnitt aller Werte an, die aus mehreren im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **UNIQUE**: Entfernt Duplikate aus den Suchfeldwerten und zeigt nur die eindeutigen Werte an. Dies ist für die folgenden Feldtypen nicht verfügbar:
      * Absatz
      * Kontrollkästchen
      * Personen

   >[!NOTE]
   >
   >Sie können beispielsweise den Produktdatensatz (verknüpfter Datensatz) aus dem Campaign-Datensatz (Originaldatensatz) verknüpfen und ihn &quot;Produktfeld&quot;nennen. Sie können auch das Feld Budget des Produktdatensatzes aus dem Campaign-Datensatz verknüpfen und es &quot;Produktbudget&quot;nennen. Wenn Sie mehrere Datensätze im Feld &quot;Produkt&quot;auswählen konnten, können Sie Produkt 1 mit einem Budget von 100.000 $ und Produkt 2 mit einem Budget von 110.000 $ und Produkt 3 mit einem Budget von 100.000 $ auswählen. Je nach ausgewähltem Aggregator können Sie im verknüpften Feld aus dem ursprünglichen Datensatz die folgenden Budgetinformationen anzeigen:
   >
   >* **Keine**: 100.000 $, 110.000 $, 100.000 $
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SUM**: 310.000 $
   >* **AVG**: $103.000.33
   >* **UNIQUE**: $100.000
   >

1. (Optional) Verwenden Sie das Symbol **search** ![](assets/search-icon.png), um nach einem Feld zu suchen.

1. Klicken Sie auf **Felder hinzufügen** , um Ihre Änderungen zu speichern.

   Die folgenden Elemente werden hinzugefügt:

   * Ein verknüpftes Datensatzfeld des Datensatztyps, von dem Sie eine Verknüpfung herstellen. Das verknüpfte Datensatzfeld zeigt einzelne Datensätze des verknüpften Datensatztyps an, nachdem Sie sie manuell hinzugefügt haben. Informationen zum Hinzufügen von Datensätzen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md). Der Name des verknüpften Datensatzfelds ist der in Schritt 6 ausgewählte Name. <!--accurate-->

   * Ein verknüpftes (oder Lookup-) Feld (oder Felder), das Informationen über den verknüpften Datensatz oder die verknüpften Objekttypen anzeigt, nachdem Sie die Datensätze oder Objekte manuell in das verknüpfte Datensatzfeld eingefügt haben. Suchfelder werden nur erstellt, wenn bei der Erstellung der Verbindung die Einstellung **Suchfelder auswählen** ausgewählt ist. Suchfelder werden automatisch nach folgendem Muster benannt:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Wenn Sie beispielsweise einen Kampagnen-Record-Typ mit einem Programmdatensatz-Typ verknüpft haben und das Feld Programm-verknüpfter Datensatz &quot;Programminformationen&quot;nennen und dann ausgewählt haben, um auch das Feld Budget des Programms in der Tabellenansicht der Kampagne anzuzeigen, erhält das verknüpfte Feld automatisch den Namen `Budget (from Program information)` in der Tabellenansicht der Kampagne.

   * Wenn Sie Datensatztypen miteinander verknüpfen, wird auch ein verknüpftes Datensatzfeld für den Datensatztyp hinzugefügt, mit dem Sie verknüpft sind. Der Name des verknüpften Datensatzfelds im verknüpften Datensatztyp ist der Name des Datensatztyps, von dem Sie eine Verknüpfung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Produkt&quot;aus dem Datensatztyp &quot;Kampagne&quot;verknüpfen und das verknüpfte Feld der Kampagne &quot;Verknüpftes Produkt&quot;nennen, wird ein mit &quot;Kampagne&quot;verknüpftes Datensatzfeld für den Produktdatensatz-Typ erstellt.

     >[!TIP]
     >
     > Für Objekte aus einer anderen Anwendung wird kein verknüpftes Datensatzfeld erstellt, das dem Datensatztyp entspricht, von dem aus Sie in der Workfront-Planung verknüpfen.

1. (Optional und bedingt) Klicken Sie in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatztyps auf den nach unten zeigenden Pfeil in der Kopfzeile der verknüpften Datensatzfelder und klicken Sie dann auf einen der folgenden Punkte:

   * **Feld bearbeiten**: Aktualisieren Sie die **Name** und die **Beschreibung** des Felds.
   * **Suchfelder bearbeiten**: Fügen Sie eines der Felder des verknüpften Datensatzes hinzu oder entfernen Sie es.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Um Suchfelder hinzuzufügen oder zu entfernen, folgen Sie den Anweisungen in den Schritten 16 bis 17 oben. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Sie können keine Suchfelder hinzufügen, die zu Datensatztypen gehören, von denen Sie Verknüpfungen zu Objektarten aus einer anderen Anwendung erstellen.
   >
   > Sie können beispielsweise das Suchfeld &quot;Kampagnenstatus&quot;nicht zu einem Workfront-Projekt hinzufügen, zu dem Sie über die Kampagnen verknüpfen.

1. (Optional) Klicken Sie in der Kopfzeile eines verknüpften Datensatzfelds auf den nach unten zeigenden Pfeil oder in der Kopfzeile eines Lookup-Felds des Datensatztyps, von dem Sie die Verknüpfung herstellen, und klicken Sie dann auf **Löschen**.

   Das Datensatzfeld oder das Lookup-Feld werden gelöscht. Wenn Sie ein Datensatzfeld löschen, werden auch alle mit dem verknüpften Datensatz verknüpften Suchfelder gelöscht.
