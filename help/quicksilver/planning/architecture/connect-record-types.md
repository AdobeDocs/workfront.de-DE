---
title: Verbinden von Datensatztypen
description: Eine Möglichkeit, die Beziehung zwischen den einzelnen Datensatztypen anzugeben, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Datensatztypen von Adobe Workfront Planning mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und deren Fokus in einer Anwendung zu behalten.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '2966'
ht-degree: 1%

---


<!--keep the 30 fields limit in yellow till Jan 2026; also the global record type cross-workspace capability information-->

<!--take production and preview references out at prod-->

# Verbinden von Datensatztypen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Sie können Datensatztypen miteinander verbinden oder Datensatztypen mit Objekttypen aus anderen Anwendungen verbinden.

Das Verbinden von Datensatztypen ist hilfreich, wenn sich mehrere Typen von Arbeitsobjekten gegenseitig beeinflussen. Sie können beispielsweise mit Kampagnen arbeiten, wobei jede Kampagne mehreren Marken gerecht werden kann. Um diese Beziehung anzugeben, können Sie Kampagnen mit Marken verbinden. Dadurch wird ein Verbindungsfeld für Marken im Kampagnendatensatz erstellt.

Darüber hinaus kann es sein, dass die Arbeit für jede Kampagne in mehreren Projekten in Workfront geplant wird. Um dies anzuzeigen, können Sie die Kampagnen mit den entsprechenden Projekten verbinden. Dadurch wird ein Verbindungsfeld für Projekte im Kampagnendatensatz erstellt.

Nachdem die Verbindungsfelder erstellt wurden, können Sie einzelne Datensätze zwischen den beiden Datensatz- oder Objekttypen verbinden.

>[!NOTE]
>
>Sie können bis zu 30 Verbindungsfelder für einen Datensatztyp haben.

In diesem Artikel wird beschrieben, wie Sie zwei Workfront Planning-Datensatztypen oder einen Workfront Planning-Datensatztyp mit einem Objekt aus einer anderen Anwendung verbinden können.

Nachdem Sie die Verbindung zwischen Datensätzen oder Objekttypen hergestellt haben, wird ein Verbindungsfeld zu einem Planungs-Datensatztyp hinzugefügt. Im Verbindungsfeld können Sie einzelne Datensätze miteinander verbinden und Felder aus den verknüpften Datensatz- oder Objekttypen in einem Workfront Planning-Datensatz anzeigen.

Allgemeine Informationen zu Verbindungstypen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Informationen zum Verbinden von Datensätzen oder Datensätzen mit Objekten aus anderen Anwendungen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen und Datensätzen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->


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
<p>So verbinden Sie Datensatztypen aus demselben Arbeitsbereich: </p>
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
<li><p>Beliebiger Workflow und beliebiges Planungspaket</li></ul>

<p>So verbinden Sie Datensatztypen aus verschiedenen Arbeitsbereichen:</p>

<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
<tr> 
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Zusätzlich zu Adobe Workfront müssen Sie über Folgendes verfügen, wenn Sie Datensatztypen mit Objekten aus den folgenden Programmen verbinden möchten:</p>
   <ul><li><p>Eine Adobe Experience Manager Assets-Lizenz und eine Integration zwischen AEM Assets und Workfront, um AEM-Assets mit Planungs-Datensatztypen zu verbinden.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront für Experience Manager Assets und Assets Essentials: Artikelindex</a>. </p></li>
   <li><p> Eine Adobe GenStudio for Performance Marketing-Lizenz zum Verbinden von Datensatztypen mit GenStudio Brands</p>
   <p>Weitere Informationen finden Sie <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Erste Schritte mit Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <li><p> Adobe Experience Manager Assets, if you want to connect AEM assets with Planning record types<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p></td> 
  </tr> 
 
</tbody> 
</table> -->

## Verbinden von Datensatztypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie verbinden möchten.

   ODER

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite „Datensatztyp“ zu öffnen.
1. Klicken Sie oben rechts in der Tabellenansicht auf das Symbol **+** und dann auf die Registerkarte **Neue Verbindung**.

   ![Neue Registerkarte „Verbindung“ mit Workfront AEM-Optionen](assets/new-connection-tab-with-workfront-aem-options-no-buttons.png)

1. Nach einem Datensatztyp suchen oder einen der folgenden Typen auswählen:

   * Einen Datensatztyp aus dem aktuellen Arbeitsbereich

     ![Mehrfachauswahl für die Verbindungsauswahl für den Datensatztyp „Same-Workspace“](assets/multi-select-connection-picker-record-type.png)

     >[!TIP]
     >
     > 
     >Wenn Sie im ausgewählten Arbeitsbereich keine anderen Datensatztypen haben, wird der Abschnitt Arbeitsbereich nicht angezeigt.

   * Ein Datensatztyp aus einem anderen Arbeitsbereich, der für die Verbindung von anderen Arbeitsbereichen konfiguriert wurde.

     >[!TIP]
     >
     >Die Einstellung **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** muss für einen Datensatztyp auf der Registerkarte **Arbeitsbereichsübergreifende Einstellungen** des Felds **Datensatztyp bearbeiten** aktiviert sein, damit ein Datensatztyp von anderen Arbeitsbereichen aus zugänglich ist. Wenn es keine Datensatztypen gibt, die für die Verbindung von anderen Arbeitsbereichen konfiguriert sind, wird der Abschnitt Arbeitsbereich nicht angezeigt.
     >
     >Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production-->
     >
     >![Registerkarte „Einstellungen für Workspace-übergreifende Einstellungen“ des Felds „Datensatztyp bearbeiten“](assets/edit-record-type-box-advanced-settings-tab.png)

     <!--Old:
        [!TIP]
        The **Allow connecting to this record type in other workspaces** setting must be enabled for a record type in the **Advanced settings** tab of the **Edit record type** box, for a record type to be accessible from other workspaces. If there are no record types that are configured to connect from other workspaces, the workspace section does not display.
        ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
        -->

   Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

   * Ein **Projekt, Portfolio, Programm,** oder **Gruppe** aus dem Abschnitt **Workfront** Objekttypen.

     ![Auswahl der Workfront-Projektverbindung](assets/multi-select-connection-picker-project.png)

   <div class="preview">

   * Eine **ursprüngliche Anfrage** Objekttyp aus dem Abschnitt **Workfront** Objekttypen.

     Das Feld Ursprüngliche Anfrageverbindung erstellt zeigt den Namen der gesendeten Planning-Anfrage an, die das Objekt erstellt hat. Der Name der Anfrage ist auch im Feld **Betreff** der Anfrage sichtbar.

     >[!NOTE]
     >
     >Sie müssen Anforderungsformulare erstellen und veröffentlichen, um Planungsanfragen zum Erstellen von Datensätzen in Workfront Planning senden zu können.
     >
     >Weitere Informationen finden Sie in den folgenden Artikeln:
     >* [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
     >* [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

     ![Auswahl der ursprünglichen Anfrageverbindung](assets/original-request-connection-selection.png)

   </div>


   * **Experience Manager Assets** im Abschnitt **Adobe-**.

     ![AEM Assets-Verbindungsauswahl](assets/aem-assets-connection-selection.png)

     Für den ausgewählten Datensatz oder Objekttyp wird eine neue Registerkarte Verbindung geöffnet.

   * Eine **Marke** aus Adobe GenStudio for Performance Marketing im Abschnitt **Adobe GenStudio**

     ![Auswahl der GenStudio Brand-Verbindung](assets/brand-genstudio-connection-selection.png)

1. Aktualisieren Sie das **Name** mit dem Namen des neuen verbundenen Felds, wie es in der Tabellenansicht oder auf der Datensatzseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verbundene Datensatzspalte (oder das verbundene Feld) in der Tabellenansicht des ursprünglichen Datensatztyps erstellt. Standardmäßig ist der Name des Felds der Name des Datensatzes oder Objekts, mit dem Sie eine Verbindung herstellen.

   >[!TIP]
   >
   >Sie können mehrere Verbindungen mit demselben Datensatz oder Objekttyp haben. Wenn Sie den Namen des verbundenen Feldes nicht bearbeiten, fügt Workfront eine Zahl nach dem Namen des verbundenen Datensatzes hinzu, um die Anzahl der verbundenen Datensatztypen mit demselben Namen anzugeben.

1. Aktualisieren Sie **Feld** Beschreibung“, indem Sie Informationen zum verbundenen Datensatzfeld hinzufügen. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. (Bedingt) Wenn Sie Datensatztypen aus zwei verschiedenen Arbeitsbereichen, einem Datensatztyp und einem Adobe Experience Manager-Asset-Objekt oder einem Datensatztyp und einer GenStudio-Marke, verbinden, wählen Sie die Option **Mehrere Datensätze zulassen** aus. Wenn Sie diese Option auswählen, können Benutzer mehrere Datensätze hinzufügen, wenn das Feld „Verbundener Datensatztyp“ in den ursprünglichen Datensätzen angezeigt wird. Dies ist standardmäßig ausgewählt.

   ![Neue Verbindung zum Datensatztyp aus einem anderen Arbeitsbereich](assets/new-connection-allow-multiple-records-box.png)

1. (Bedingt) Wenn Sie Datensatztypen aus demselben Arbeitsbereich oder einen Planning-Datensatztyp mit einem Workfront-Objekttyp verbinden, wählen Sie eine der folgenden Optionen aus:

   * **Mehrfachauswahl**: Wählen Sie diese Option aus, damit ein Datensatz aus dem aktuellen Datensatztyp mit mehreren Datensätzen aus dem Verbindungs-Datensatztyp verbunden werden kann.
   * **Einzelauswahl**: Wählen Sie diese Option aus, damit ein Datensatz aus dem aktuellen Datensatztyp mit einem Datensatz aus dem Verbindungs-Datensatztyp verbunden werden kann.

1. Wählen Sie das **Entsprechendes Feld für verknüpften Datensatztyp erstellen**. Wenn diese Option aktiviert ist, wird zusätzlich zum Verbindungsfeld, das zum aktuellen Datensatztyp hinzugefügt wird, ein Verbindungsfeld für den Datensatztyp erstellt, mit dem Sie verbunden sind. Dies ist standardmäßig deaktiviert.

   >[!TIP]
   >
   >* Zusätzlich zu der Beschränkung von 30 Verbindungsfeldern für einen Datensatztyp gibt es eine Beschränkung von 500 Feldern für einen Datensatztyp. Es wird empfohlen, diese Einstellung deaktiviert zu lassen, insbesondere für taxonomische Datensatztypen, um ein Erreichen dieser Grenze zu vermeiden.
   >
   >* Die Auswahl **Felds „Entsprechendes Feld für verknüpften Datensatztyp erstellen** ist eine Voraussetzung für die Erstellung von Hierarchien.

1. (Bedingt) Wenn Sie **Entsprechendes Feld für verknüpften Datensatztyp erstellen** aktiviert haben, wählen Sie eine der folgenden Optionen, um anzugeben, mit wie vielen Datensätzen Benutzende eine Verbindung herstellen können:

   * Viele-zu-viele
   * Eins zu viele
   * Viele-zu-eins
   * Eins zu eins

   Weitere Informationen zu Verbindungstypen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   >[!NOTE]
   >
   >Wenn Sie für den Verbindungstyp Eins-zu-viele oder Eins-zu-Eins auswählen und später einen Datensatz oder ein Objekt verbinden möchten, das bereits an anderer Stelle verbunden ist, erhalten Sie eine Warnung, dass durch erneutes Verbinden der Datensatz oder das Objekt aus der ursprünglichen Verbindung entfernt wird. Sie können das Entfernen zulassen oder einen anderen Datensatz auswählen.

1. (Bedingt und optional) Wenn Sie eine Verbindung zu einem Workfront-Objekt herstellen möchten, wählen Sie ein **benutzerdefiniertes Formular** aus dem Abschnitt **Nur Objekte verknüpfen, die diesen Kriterien**. Nur Objekte, an die die ausgewählten benutzerdefinierten Formulare angehängt sind, können mit dem ausgewählten Datensatztyp verknüpft werden. Sie können mehrere Formulare auswählen.

   >[!NOTE]
   >
   > Sie müssen benutzerdefinierte Formulare in Workfront für die ausgewählten Objekte erstellen, bevor sie in dieser Liste angezeigt werden.

1. (Bedingt) Wenn Sie eine Verbindung zu Experience Manager Assets herstellen möchten, wählen Sie ein Repository aus dem Dropdown-Menü **Experience Manager** im Abschnitt **Verknüpfen von Assets aus dem folgenden Repository** aus. Dies ist ein Pflichtfeld. In diesem Feld werden nur Repositorys angezeigt, auf die Sie in Experience Manager Assets Zugriff haben.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann Workfront Planning-Felder über die Metadatenzuordnung in Workfront Experience Manager Assets-Feldern zuordnen. Weitere Informationen finden Sie unter &quot;[ der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. (Bedingt) Wenn Sie eine Verbindung zu Experience Manager Assets, zu einem Workfront Planning-Datensatztyp oder zu einer GenStudio-Marke herstellen möchten, wählen Sie im Bereich „Erscheinungsbild des **&quot; eine der folgenden Optionen**:

   * **Name und Bild**: Sowohl der Name als auch die Miniaturansicht oder das Symbol der verbundenen Datensätze werden im Feld Verbundener Datensatz angezeigt. Dies ist die Standardoption.
   * **Name**: Im Feld Verbundener Datensatz wird nur der Name der verbundenen Datensätze angezeigt.
   * **Bild**: Im Feld Verbundener Datensatz wird nur die Miniaturansicht oder das Symbol der verbundenen Datensätze angezeigt.

   Bei Datensätzen ohne Miniaturbild wird stattdessen das Symbol für den Datensatztyp angezeigt. Ein Beispiel dafür, wie die verbundenen Datensätze im Bereich **Erscheinungsbild des Datensatzes** angezeigt werden.

   >[!NOTE]
   >
   >* Wenn Sie die Verknüpfung mehrerer Datensätze zulassen, kann die Anzeige nur der Miniaturansicht Platz in kleineren Bereichen sparen, z. B. in Datensatzansichten.
   >
   >* Der Name eines Datensatzes ist das primäre Feld des Datensatzes. Weitere Informationen finden Sie unter [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >* Bei der Auswahl von Workfront-Objekttypen steht das Erscheinungsbild eines Datensatzes nicht zur Verfügung.
   >
   >* Die Auswahl im Bereich Erscheinungsbild des Datensatzes bestimmt, wie die Datensätze in Verbindungen überall im System angezeigt werden, einschließlich aller Ansichten und Detailseiten.

1. Wählen Sie die **Suchfelder auswählen**, um Felder aus dem Datensatztyp hinzuzufügen, mit dem Sie eine Verbindung herstellen. Die Suchfelder sind Felder, die mit dem Datensatz oder Objekttyp verknüpft sind, mit dem Sie eine Verknüpfung herstellen. Durch Verknüpfen werden Informationen des Datensatzes oder Objekts angezeigt, mit dem Sie eine Verknüpfung herstellen, und zwar für den Datensatz, von dem aus eine Verknüpfung hergestellt wird. Dies ist standardmäßig ausgewählt.

   >[!TIP]
   >
   >* Sie können keine Workfront-Felder mit automatischer Textvervollständigung (einschließlich Feldern wie Projektbesitzer oder Projektsponsor) als Suchfelder hinzufügen.
   >
   >* Die Datumsfeldinformationen der Workfront-Objekte werden in Workfront Planning im 24-Stunden-Format angezeigt, unabhängig davon, wie sie in Workfront angezeigt werden.
   >
   >   Wenn beispielsweise das geplante Startdatum eines Projekts in Workfront um 15 :00 angezeigt wird, wird es in Workfront :00 in einem importierten Suchfeld als 15 angezeigt.
   >* In der Produktionsumgebung können Sie keine Personenfelder als Lookup-Felder hinzufügen. <span class="preview">Sie können Personenfelder als Suchfelder in der Vorschau-Umgebung hinzufügen.</span>
   >

1. Klicken Sie auf **Erstellen**.

1. (Bedingt) Wenn Sie die Einstellung **Suchfeld auswählen** ausgewählt haben, wird das Feld **Suchfelder hinzufügen** geöffnet.

   Klicken Sie auf das Symbol **+** , um Felder aus dem Bereich **Nicht ausgewählte Felder** hinzuzufügen.

   ODER

   Klicken Sie auf das Symbol **-** , um Felder aus dem Bereich **Ausgewählte Felder** zu entfernen

   ![Suchfelder für ein Feld eines anderen Datensatztyps hinzufügen](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Die Werte für die verbundenen Felder werden automatisch ausgefüllt, nachdem Sie Datensätze oder Objekte verknüpft haben.

   >[!IMPORTANT]
   >
   >    Alle Personen mit Anzeigen- oder höheren Berechtigungen für den Arbeitsbereich können die Informationen in den verknüpften Feldern anzeigen, unabhängig von ihren Berechtigungen oder Zugriffsebenen bei der Anwendung der verknüpften Objekttypen.

1. (Optional) Klicken Sie auf **Überspringen**, um das Hinzufügen von Feldern aus dem verknüpften Datensatz oder Objekttyp zu überspringen. Der Name oder das Primäre Feld des verknüpften Datensatzes ist das einzige sichtbare Feld in der Tabellenansicht des Datensatztyps, von dem aus Sie eine Verbindung herstellen.

1. Wählen Sie einen Aggregator für die hinzugefügten Suchfelder aus.

   >[!NOTE]
   >
   >Sie können keine Aggregatoren für die folgenden Feldtypen hinzufügen:
   >
   >    * Absatz
   >    * Kontrollkästchen

   Die Werte für die verknüpften Felder werden je nach ausgewähltem Aggregator entweder durch Kommas getrennt oder als zusammengefasster Wert angezeigt, wenn Benutzende mehr als einen verknüpften Datensatz im verknüpften Datensatzfeld auswählen.

   Wenn das Suchfeld mehrere Werte enthält, die nicht zusammengefasst sind, sollten Sie bei der Verwendung des Felds beim Sortieren oder Gruppieren in einer Ansicht Folgendes beachten:

   * Die Sortierung erfolgt nach dem ersten Wert

   * Datensätze werden nach jeder eindeutigen Kombination von Feldwerten gruppiert

   * Die Zeitleisten-Ansicht basiert auf dem ersten Datumswert des verbundenen Datensatztyps, wenn er in der Ansicht angezeigt wird

   >[!IMPORTANT]
   >
   > Sie müssen beim Hinzufügen von Suchdatumsfeldern einen Aggregatorwert auswählen, wenn die Felder verfügbar sein sollen, um als Start- und Enddatum für die Timeline- und Kalenderansichten hinzugefügt werden zu können. Sie können beispielsweise den MAX oder den MIN-Aggregator für ein Suchdatumsfeld auswählen.

   ![Aggregator-Dropdown für verknüpftes Zahlenfeld](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Aggregatoren sind nicht verfügbar, wenn Datensatztypen mit folgenden Elementen verbunden werden:
   >* Experience Manager Assets
   >* GenStudio-Marken.
   >

   Wählen Sie aus den folgenden Optionen aus:

   * **Keine**: Zeigt die Werte an, die aus mehreren durch Kommas getrennten Datensätzen stammen. Dies ist die Standardauswahl.
   * **MAX**: Zeigt den höchsten Wert aus allen Werten an, die aus mehreren Datensätzen stammen, die im Feld Verknüpfter Datensatz ausgewählt wurden.
   * **MIN**: Zeigt den niedrigsten Wert aus allen Werten an, die aus mehreren Datensätzen stammen, die im Feld Verknüpfter Datensatz ausgewählt wurden.
   * **SUM**: Zeigt die Summe aller Werte an, die aus mehreren Datensätzen stammen, die im verknüpften Datensatzfeld ausgewählt wurden.
   * **AVG**: Zeigt den Durchschnitt aller Werte an, die aus mehreren Datensätzen stammen, die im Feld Verknüpfter Datensatz ausgewählt wurden.
   * **UNIQUE**: Entfernt Duplikate aus den Werten der Suchfelder und zeigt nur die eindeutigen Werte an. Dies ist für die folgenden Feldtypen nicht verfügbar:
      * Absatz
      * Kontrollkästchen
      * Personen

   >[!NOTE]
   >
   >Sie können beispielsweise den Produktdatensatz (verknüpfter Datensatz) mit dem Kampagnendatensatz (ursprünglicher Datensatz) verknüpfen und ihm den Namen „Produktfeld“ geben. Sie können auch das Budgetfeld des Produktdatensatzes mit dem Kampagnendatensatz verknüpfen und ihn „Produktbudget“ nennen. Wenn Sie mehrere Datensätze im Feld „Produkt“ auswählen dürfen, können Sie Produkt 1 mit einem Budget von 100.000 US-Dollar und Produkt 2 mit einem Budget von 110.000 US-Dollar und Produkt 3 mit einem Budget von 100.000 US-Dollar auswählen. Je nach ausgewähltem Aggregator können Sie die folgenden Budgetinformationen im verknüpften Feld des ursprünglichen Datensatzes anzeigen:
   >
   >* **None**: $100.000, $110.000, $100.000
   >* **MAX**: 110.000 $
   >* **MIN**: 100.000 $
   >* **SUMME**: 310.000 $
   >* **DURCHSCHN**: 103.000,33 $
   >* **EINDEUTIG**: 100.000 $
   >

1. (Optional) Verwenden Sie das Symbol **Suche** ![Suchsymbol](assets/search-icon.png), um nach einem Feld zu suchen.

1. Klicken Sie auf **Felder hinzufügen**, um Ihre Änderungen zu speichern.

   Die folgenden Punkte werden hinzugefügt:

   * Ein verknüpftes Datensatzfeld für den Datensatztyp, von dem aus Sie eine Verknüpfung herstellen. Im Feld Verknüpfter Datensatz werden einzelne Datensätze aus dem verknüpften Datensatztyp angezeigt, nachdem Sie sie manuell hinzugefügt haben. Informationen zum Hinzufügen von Datensätzen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md). Der Name des verknüpften Datensatzfelds entspricht dem Namen, den Sie in Schritt 6 ausgewählt haben. <!--accurate-->

   * Ein verknüpftes Feld (oder Suchfelder), das Informationen zu einem verknüpften Datensatz oder zu Objekttypen anzeigt, nachdem Sie die Datensätze oder Objekte manuell in das verknüpfte Datensatzfeld eingefügt haben. Suchfelder werden nur erstellt, wenn die Einstellung **Suchfelder auswählen** beim Erstellen der Verbindung ausgewählt ist. Suchfelder werden automatisch nach diesem Muster benannt:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Wenn Sie beispielsweise einen Kampagnendatensatztyp mit dem Programmdatensatztyp verknüpft und das Feld Programmverknüpfte Datensatzinformationen als „Programm“ bezeichnet und dann die Option ausgewählt haben, das Feld Programmbudget auch in der Tabellenansicht der Kampagne anzuzeigen, wird das verknüpfte Feld automatisch in der Tabellenansicht der Kampagne `Budget (from Program information)` benannt.

   * Wenn Sie Datensatztypen miteinander verknüpfen, wird für den Datensatztyp, mit dem Sie verknüpfen, auch ein verknüpftes Datensatzfeld hinzugefügt, allerdings nur, wenn Sie die Einstellung **entsprechendes Feld für verknüpften Datensatztyp erstellen** aktivieren. Der Name des verknüpften Datensatzfelds beim verknüpften Datensatztyp ist der Name des Datensatztyps, von dem aus die Verknüpfung hergestellt wird.

     Wenn Sie beispielsweise den Datensatztyp „Produkt“ mit dem Datensatztyp „Kampagne“ verknüpfen und das verbundene Feld der Kampagne als „Verknüpftes Produkt“ benennen, wird für den Datensatztyp „Produkt“ ein verknüpftes Datensatzfeld „Kampagne“ erstellt.

     >[!TIP]
     >
     > Ein verknüpftes Datensatzfeld wird für Objekte aus einem anderen Programm in den jeweiligen Programmen nicht erstellt.
     > Es wird empfohlen, keine Links zu taxonomischen Datensatztypen zu erstellen, da es zusätzlich zu der Beschränkung von 30 verbundenen Feldern für jeden Datensatztyp eine Beschränkung von 500 Feldern gibt.


1. (Optional und bedingt) Klicken Sie in der Tabellenansicht Ursprünglicher Datensatztyp oder Verknüpfter Datensatztyp auf den nach unten zeigenden Pfeil in der Kopfzeile der verknüpften Datensatzfelder und dann auf eine der folgenden Aktionen:

   * **Feld bearbeiten**: Aktualisieren Sie die **Name** und die **Beschreibung** des Felds.
   * **Suchfelder bearbeiten**: Fügt Felder des verknüpften Datensatzes hinzu oder entfernt sie.

   ![Dropdown-Menü „Feld bearbeiten“ und „Suchfelder“ in der Tabellenspalte](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Um Suchfelder hinzuzufügen oder zu entfernen, folgen Sie den Anweisungen in den Schritten 16-17 oben. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Sie können keine Suchfelder hinzufügen, die zu Datensatztypen gehören, von denen aus Sie Verknüpfungen zu Objekttypen aus einer anderen Anwendung herstellen.
   >
   > Sie können beispielsweise das Suchfeld „Kampagnenstatus“ nicht zu einem Workfront-Projekt hinzufügen, mit dem Sie von den Kampagnen aus eine Verknüpfung herstellen.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil in der Kopfzeile eines verknüpften Datensatzfelds oder in der Kopfzeile eines Suchfelds vom Datensatztyp, von dem aus Sie eine Verknüpfung herstellen, und klicken Sie dann auf **Löschen**.

   Das Datensatzfeld oder das Suchfeld werden gelöscht. Wenn Sie ein Datensatzfeld löschen, werden auch alle mit dem verknüpften Datensatz verknüpften Suchfelder gelöscht.
