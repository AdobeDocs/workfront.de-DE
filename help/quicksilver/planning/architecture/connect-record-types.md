---
title: Verbinden von Datensatztypen
description: Eine Möglichkeit, die Beziehung zwischen den einzelnen Datensatztypen anzugeben, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Datensatztypen von Adobe Workfront Planning mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und deren Fokus in einer Anwendung zu behalten.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 9bdc36a76393acd2f0617cc5796cfd7279b2c97a
workflow-type: tm+mt
source-wordcount: '2752'
ht-degree: 1%

---


# Verbinden von Datensatztypen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Sie können Datensatztypen miteinander verbinden oder Datensatztypen mit Objekttypen aus anderen Anwendungen verbinden.

Das Verbinden von Datensatztypen ist hilfreich, wenn sich mehrere Typen von Arbeitsobjekten gegenseitig beeinflussen. Sie können beispielsweise mit Kampagnen arbeiten, wobei jede Kampagne mehreren Marken gerecht werden kann. Um diese Beziehung anzugeben, können Sie Kampagnen mit Marken verbinden. Darüber hinaus kann es sein, dass die Arbeit für jede Kampagne in mehreren Projekten in Workfront geplant wird. Um dies anzuzeigen, können Sie die Kampagnen mit den entsprechenden Projekten verbinden. Durch das Verbinden von Datensatztypen und das anschließende Verbinden einzelner Datensätze wird diese Beziehung in Workfront Planning erreicht.

In diesem Artikel wird beschrieben, wie Sie zwei Workfront Planning-Datensatztypen oder einen Workfront Planning-Datensatztyp mit einem Objekt aus einer anderen Anwendung verbinden können.

Nachdem Sie die Verbindung zwischen Datensätzen oder Objekttypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden und Felder aus den verknüpften Datensatz- oder Objekttypen in einem Workfront Planning-Datensatz anzeigen.

Allgemeine Informationen zu Verbindungstypen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Informationen zum Verbinden von Datensätzen oder Datensätzen mit Objekten aus anderen Anwendungen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen und Datensätzen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

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
   <li><p> Adobe Workfront-Planung<p></li>
   <li><p> Adobe Experience Manager Assets, wenn Sie AEM-Assets mit Planungs-Datensatztypen verbinden möchten<p>
   <p>Sie müssen über eine Adobe Experience Manager Assets-Lizenz und eine Integration zwischen AEM Assets und Workfront verfügen.
    Weitere Informationen finden Sie unter <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront für Experience Manager Assets und Assets Essentials: Artikelindex</a>. </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten.</p></td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verbinden von Datensatztypen

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie verbinden möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite „Datensatztyp“ zu öffnen.
1. Klicken Sie oben rechts in der Tabellenansicht auf das Symbol **+** und dann auf die Registerkarte **Neue Verbindung**.

   ![Neue Registerkarte „Verbindung“ mit Workfront AEM-Optionen](assets/new-connection-tab-with-workfront-aem-options.png)

1. Suchen Sie **Feld** Datensatztyp“ nach einem Datensatztyp oder wählen Sie einen der folgenden Typen aus:

   * Ein anderer Datensatztyp aus dem aktuellen Arbeitsbereich

     ![Viele zu viele Verbindungsauswahl](assets/many-to-many-connection-picker.png)

     >[!TIP]
     >
     > 
     >Wenn Sie im ausgewählten Arbeitsbereich keine anderen Datensatztypen haben, wird der Abschnitt Arbeitsbereich nicht angezeigt.


   * Ein Datensatztyp aus einem anderen Arbeitsbereich, der für die Verbindung von anderen Arbeitsbereichen konfiguriert wurde.

     >[!TIP]
     >
     >Die Einstellung **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** muss für einen Datensatztyp auf der Registerkarte **Erweiterte Einstellungen** des Felds **Datensatztyp bearbeiten** aktiviert sein, damit ein Datensatztyp von anderen Arbeitsbereichen aus zugänglich ist. Wenn es keine Datensatztypen gibt, die für die Verbindung von anderen Arbeitsbereichen konfiguriert sind, wird der Abschnitt Arbeitsbereich nicht angezeigt.
     > ![Registerkarte „Erweiterte Einstellungen“ im Feld „Datensatztyp bearbeiten“](assets/edit-record-type-box-advanced-settings-tab.png)

     Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

     ![Neue Verbindung, um mehrere Datensätze zuzulassen](assets/new-connection-allow-multiple-records-box.png)

   * Ein **Projekt, Portfolio, Programm,** oder **Gruppe** aus dem Abschnitt **Workfront** Objekttypen.

     ![Auswahl der Workfront-Projektverbindung](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** im Abschnitt **Adobe-**.

     ![AEM Assets-Verbindungsauswahl](assets/aem-assets-connection-selection.png)

     Für den ausgewählten Datensatz oder Objekttyp wird eine neue Registerkarte Verbindung geöffnet.

1. Aktualisieren Sie das **Name** mit dem Namen des neuen verbundenen Felds, wie es in der Tabellenansicht oder auf der Datensatzseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verbundene Datensatzspalte (oder das verbundene Feld) in der Tabellenansicht des ursprünglichen Datensatztyps erstellt. Standardmäßig ist der Name des Felds der Name des Datensatzes oder Objekts, mit dem Sie eine Verbindung herstellen.

   >[!TIP]
   >
   >Sie können mehrere Verbindungen mit demselben Datensatz oder Objekttyp haben. Wenn Sie den Namen des verbundenen Feldes nicht bearbeiten, fügt Workfront eine Zahl nach dem Namen des verbundenen Datensatzes hinzu, um die Anzahl der verbundenen Datensatztypen mit demselben Namen anzugeben.

1. Aktualisieren Sie **Feld** Beschreibung“, indem Sie Informationen zum verbundenen Datensatzfeld hinzufügen. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. (Bedingt) Wenn Sie Datensatztypen aus zwei verschiedenen Arbeitsbereichen oder einem Datensatz und einem Adobe Experience Manager-Asset-Objekt verbinden, wählen Sie die Option **Mehrere Datensätze zulassen** aus. Wenn Sie diese Option auswählen, können Benutzer mehrere Datensätze hinzufügen, wenn das Feld „Verbundener Datensatztyp“ in den ursprünglichen Datensätzen angezeigt wird. Dies ist standardmäßig ausgewählt.

   ![Neue Verbindung, um mehrere Datensätze zuzulassen](assets/new-connection-allow-multiple-records-box.png)

1. (Bedingt) Wenn Sie Datensatztypen aus demselben Arbeitsbereich oder einen Planning-Datensatztyp mit einem Workfront-Objekttyp verbinden, führen Sie je nach verwendeter Umgebung einen der folgenden Schritte aus:

   * Wählen Sie in der Produktionsumgebung eine der folgenden Optionen **Verbindungstyp** aus, um anzugeben, mit wie vielen Datensätzen Benutzende eine Verbindung herstellen können:

      * Viele-zu-viele
      * Eins zu viele
      * Viele-zu-eins
      * Eins zu eins

     ![Viele zu viele Verbindungsauswahl](assets/many-to-many-connection-picker.png)

   <div class="preview">

   * Gehen Sie in der Vorschau -Umgebung wie folgt vor:
      1. Wählen Sie eine der folgenden Optionen aus:

         * **Mehrfachauswahl**: Wählen Sie diese Option aus, damit ein Datensatz aus dem aktuellen Datensatztyp mit mehreren Datensätzen aus dem Verbindungs-Datensatztyp verbunden werden kann.
         * **Einzelauswahl**: Wählen Sie diese Option aus, damit ein Datensatz aus dem aktuellen Datensatztyp mit einem Datensatz aus dem Verbindungs-Datensatztyp verbunden werden kann.

      2. Aktivieren Sie **entsprechendes Feld für verknüpften Datensatztyp erstellen**. Wenn diese Option aktiviert ist, wird zusätzlich zum Verbindungsfeld, das zum aktuellen Datensatztyp hinzugefügt wird, ein Verbindungsfeld für den Datensatztyp erstellt, mit dem Sie verbunden sind. Dies ist standardmäßig deaktiviert.

         >[!TIP]
         >
         >Es gibt eine Beschränkung von 500 Verbindungen für einen Datensatztyp. Es wird empfohlen, diese Einstellung deaktiviert zu lassen, insbesondere für taxonomische Datensatztypen, um ein Erreichen dieser Grenze zu vermeiden.

      3. (Bedingt) Wenn Sie **Entsprechendes Feld für verknüpften Datensatztyp erstellen** aktiviert haben, wählen Sie eine der folgenden Optionen, um anzugeben, mit wie vielen Datensätzen Benutzende eine Verbindung herstellen können:

         * Viele-zu-viele
         * Eins zu viele
         * Viele-zu-eins
         * Eins zu eins

     </div>

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
   >Ihr Workfront-Administrator kann Workfront Planning-Felder über die Metadatenzuordnung in Workfront Experience Manager Assets-Feldern zuordnen. Weitere Informationen finden Sie unter &quot;[ der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets ](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. (Bedingt) Wenn Sie eine Verbindung zu Experience Manager Assets oder einem Workfront Planning-Datensatztyp herstellen möchten, wählen Sie im Bereich „Erscheinungsbild des Datensatzes **eine der folgenden Optionen**:

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

1. Klicken Sie auf **Erstellen**.

1. (Bedingt) Wenn Sie die Einstellung **Suchfeld auswählen** ausgewählt haben, wird das Feld **Suchfelder hinzufügen** geöffnet.

   Klicken Sie auf das Symbol **+** , um Felder aus dem Bereich **Nicht ausgewählte Felder** hinzuzufügen.

   Oder

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
   > Aggregatoren sind beim Verbinden von Datensatztypen mit Experience Manager Assets nicht verfügbar.

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

   * Wenn Sie Datensatztypen miteinander verknüpfen, wird dem Datensatztyp, mit dem Sie verknüpfen, auch ein verknüpftes Datensatzfeld hinzugefügt <!--<span class="preview">only when you enable the Create corresponding field on linked record type setting.</span>--> Der Name des verknüpften Datensatzfelds im verknüpften Datensatztyp ist der Name des Datensatztyps, mit dem Sie verknüpfen.

     Wenn Sie beispielsweise den Datensatztyp „Produkt“ mit dem Datensatztyp „Kampagne“ verknüpfen und das verbundene Feld der Kampagne als „Verknüpftes Produkt“ benennen, wird für den Datensatztyp „Produkt“ ein verknüpftes Datensatzfeld „Kampagne“ erstellt.

     >[!TIP]
     >
     > Für Objekte aus einem anderen Programm wird kein verknüpftes Datensatzfeld mit dem Datensatztyp erstellt, von dem aus Sie in Workfront Planning verknüpfen. <!--<span class="preview">We recommend not creating links on taxonomical record types, as there is a 500 connection field limit for every record type.</span>-->

   <!--see the span preview text in the TIP above; it might not show up in green-->

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
