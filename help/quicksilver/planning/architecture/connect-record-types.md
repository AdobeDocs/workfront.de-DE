---
title: Datensatztypen verbinden
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Adobe Workfront Planning-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu behalten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '2487'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Datensatztypen verbinden

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Sie können Datensatztypen miteinander oder Datensatztypen mit Objektarten aus anderen Anwendungen verbinden.

In diesem Artikel wird beschrieben, wie Sie zwei Workfront Planning-Record-Typen eines Workfront Planning-Datensatztyps mit einem Objekt einer anderen Anwendung verbinden können.

Nachdem Sie die Verbindung zwischen Datensätzen oder Objekttypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden und Felder aus den verknüpften Datensätzen oder Objekttypen in einem Workfront Planning-Datensatz anzeigen.

Informationen zum Verbinden eines Workfront-Planungsprotokolls mit einem Objekt aus einer anderen Anwendung finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen und Datensätzen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Um Adobe Workfront Planning-Record-Typen mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit dem Adobe Unified Experience integriert sein. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p> 
   <p>Aktuell: Plan</p>
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Überlegungen zum Verbinden von Datensatztypen

* Sie können die folgenden Entitäten in der Adobe Workfront-Planung verbinden:

   * Zwei Datensatztypen

     Die Datensatztypen müssen zum selben Arbeitsbereich gehören.
   * Ein Datensatztyp und ein Objekttyp aus einer anderen Anwendung.

* Sie können die Workfront Planning-Datensatztypen mit den folgenden Objekttypen aus den folgenden Anwendungen verbinden:

   * Adobe Workfront:

      * Projekte
      * Portfolios
      * Programme
      * Firmen
      * Gruppen

   * Adobe Experience Manager Assets:

      * Bilder
      * Ordner

     >[!IMPORTANT]
     >
     >Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Workfront Planning-Datensätze mit Adobe Experience Manager Assets zu verbinden.
     >
     >Wenn Sie Fragen zum Einstieg in die Adobe Admin Console haben, lesen Sie den Abschnitt [Häufig gestellte Fragen zu Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nachdem Sie einzelne Datensätze für einen Datensatztyp erstellt haben, können Sie die Datensätze, zu denen Sie eine Verbindung herstellen, aus dem Feld des verknüpften Datensatztyps auswählen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder einem Objekttyp aus einer anderen Anwendung verbunden haben, gibt es folgende Szenarien:

   * **Wenn Sie zwei Datensatztypen verbinden**: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Ein ähnliches verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, mit dem Sie eine Verbindung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Datensatztyp &quot;Produkt&quot;verbinden, wird ein verknüpftes Datensatzfeld, das Sie &quot;Verknüpftes Produkt&quot;nennen, für den Datensatztyp &quot;Kampagne&quot;erstellt und ein verknüpfter Datensatztyp automatisch mit dem Namen &quot;Kampagne&quot;für den Produktdatensatz erstellt.

   * **Wenn Sie einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden**:

      * Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Für den Objekttyp der anderen Anwendung wird kein verknüpftes Datensatzfeld erstellt.

      * Ein neuer schreibgeschützter Workfront-Planungstyp wird nur dann für das Objekt der anderen Anwendung erstellt, wenn die eigentlichen Objekte mit Datensätzen der Workfront-Planung verbunden sind.

        Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

      * Über Workfront-Objekte ist der Zugriff auf die Felder für die Planung von Datensätzen nicht möglich.
      * Die Planung von Datensatzfeldern ist über Experience Manager-Assets verfügbar, wenn der Workfront-Administrator die Metadaten-Zuordnung durch die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Wenn Sie verknüpfte (oder Lookup-) Felder des Datensatzes oder Objekts hinzufügen, zu dem Sie eine Verbindung herstellen**: Sie können Felder vom -Objekt der anderen Anwendung mit dem Datensatztyp für die Workfront-Planung verbinden. Verknüpfte Felder sind schreibgeschützt und zeigen automatisch Informationen aus verbundenen Datensätzen oder Objekten an, wenn Sie die Datensätze oder Objekte verbinden.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit einem Workfront-Projekt verbinden und das Feld &quot;Geplantes Abschlussdatum&quot;des Projekts in den Workfront-Planungsdatensatz übertragen möchten, wird automatisch ein verknüpftes Feld namens &quot;Geplantes Abschlussdatum&quot;(aus Projekt) für die Kampagne erstellt. Sie können dieses verknüpfte Feld nicht manuell bearbeiten. Im Feld Geplantes Abschlussdatum (aus Projekt) wird das geplante Abschlussdatum der verknüpften Projekte angezeigt.

     >[!IMPORTANT]
     >
     >    Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in der Anwendung der verknüpften Objekttypen.

* Verknüpfte Datensatzfelder erhalten ein Beziehungssymbol ![](assets/relationship-field-icon.png).

  Verknüpfte Felder erhalten ein Symbol, das den Feldtyp identifiziert. Verknüpfte (oder Lookup-) Felder weisen beispielsweise Symbole darauf hin, dass es sich bei einem Feld um eine Zahl, einen Absatz oder ein Datum handelt.


## Datensatztypen verbinden

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie verbinden möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht angezeigt, und klicken Sie dann auf die Schaltfläche **Neue Verbindung** Registerkarte.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Im **Record Type** -Feld nach einem Datensatztyp suchen oder eine der folgenden Optionen auswählen:

   * Ein anderer Datensatztyp aus dem ausgewählten Arbeitsbereich

     ![](assets/new-connection-tab-fields-with-another-record-selected.png)

     >[!TIP]
     >
     >Es sind nur Datensatztypen aus dem ausgewählten Arbeitsbereich verfügbar, mit denen eine Verbindung hergestellt werden kann.
     > 
     >Wenn im ausgewählten Arbeitsbereich keine anderen Datensatztypen vorhanden sind, wird der Arbeitsbereich-Bereich nicht angezeigt.

   * A **Projekt, Portfolio, Programm, Firma** oder **Gruppe** aus dem **Workfront-Objekttypen** Abschnitt.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** aus dem **Adobe-Anwendungen** Abschnitt.

     ![](assets/aem-assets-connection-selection.png)

1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Der Name des verbundenen Felds, wie er in der Tabellenansicht oder auf der Datensatzseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verknüpfte Datensatzspalte in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatzfelds für die ursprünglichen Datensätze erstellt. Standardmäßig ist der Name des Felds der Name des Datensatzes oder Objekts, mit dem Sie eine Verbindung herstellen.

   >[!TIP]
   >
   >Sie können mehrere Verbindungen zum selben Datensatz oder Objekttyp haben. Wenn Sie den Namen des verbundenen Felds nicht bearbeiten, fügt Workfront eine Zahl nach dem Namen des verbundenen Datensatzes hinzu, um die Anzahl der verbundenen Datensatztypen mit demselben Namen anzugeben.

   * **Beschreibung**: Zusätzliche Informationen zum verbundenen Datensatzfeld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Mehrere Datensätze zulassen**: Wählen Sie diese Option, um anzugeben, dass Benutzer mehrere Datensätze hinzufügen können, wenn das Feld des verknüpften Datensatztyps in den Originaldatensätzen angezeigt wird. Diese Option ist standardmäßig aktiviert.
   * **Suchfelder auswählen**: Wählen Sie diese Option, um Felder aus dem ausgewählten Datensatztyp hinzuzufügen. Die Suchfelder sind Felder, die mit dem Datensatz oder Objekttyp verknüpft sind, mit dem Sie verknüpft sind. Durch die Verknüpfung werden Informationen aus dem Datensatz oder Objekt angezeigt, mit dem Sie in dem Datensatz verknüpfen, den Sie möchten. Diese Option ist standardmäßig aktiviert.

     >[!TIP]
     >
     > Sie können die folgenden Feldtypen nicht als Suchfelder hinzufügen:
     >
     >    * Personen
     >    * Erstellt von
     >    * Zuletzt geändert von
     >    * Workfront typeahead-Felder (einschließlich Feldern wie Projekteigentümer oder Projektsponsor)

1. (Bedingt und optional) Wenn Sie die Verbindung eines Workfront-Objekts ausgewählt haben, wählen Sie eine **Benutzerdefiniertes Formular** aus dem **Nur Objekte verknüpfen, die diesen Kriterien entsprechen** Abschnitt. Nur Objekte, an die die ausgewählten benutzerdefinierten Formulare angehängt sind, können mit dem ausgewählten Datensatztyp verknüpft werden. Sie können mehrere Formulare auswählen.

   >[!NOTE]
   >
   > Sie müssen benutzerdefinierte Formulare in Workfront für die ausgewählten Objekte erstellen, bevor sie in dieser Liste angezeigt werden.

1. (Bedingt) Wenn Sie die Verbindung zu Experience Manager Assets hergestellt haben, wählen Sie ein Repository aus der **Experience Manager-Repository** Dropdown-Menü im **Verknüpfen von Assets aus dem folgenden Repository** Abschnitt. Dies ist ein erforderliches Feld. In diesem Feld werden nur Repositorys angezeigt, auf die Sie in Experience Manager Assets Zugriff haben.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann Experience Manager Assets-Feldern Planungsfelder über das Metadaten-Mapping in Workfront zuordnen. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Bedingt) Wenn Sie ausgewählt haben, dass eine Verbindung mit Experience Manager Assets oder einem Workfront-Planungs-Datensatztyp hergestellt werden soll, deaktivieren Sie die Option **Titel** Umschalten in der **Anzeige von Datensätzen** -Bereich, wenn Sie nicht möchten, dass der Titel der verbundenen Datensätze oder Assets im verknüpften Feld angezeigt wird. Wenn diese Option deaktiviert ist, werden nur die Miniaturansichten der Datensätze in den verknüpften Feldern angezeigt. Datensätze ohne Miniaturbild zeigen stattdessen ein Bildsymbol an. Der Umschalter ist standardmäßig aktiviert. Ein Beispiel dafür, wie die verbundenen Datensätze in der **Anzeige von Datensätzen** Bereich.

   >[!TIP]
   >
   >    Wenn Sie zulassen, dass mehrere Datensätze verknüpft werden, kann die Anzeige nur der Miniaturansicht in kleineren Bereichen, wie z. B. Datensatzansichten, Platz sparen.
   >
   >Der Titel eines Datensatzes ist das primäre Feld des Datensatzes. Weitere Informationen finden Sie unter [Primäre Feldübersicht](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Klicken Sie auf **Erstellen**.

1. (Bedingt) Wenn Sie die Option **Suchfeld auswählen** -Einstellung, **Suchfelder hinzufügen** wird geöffnet.

   Klicken Sie auf **+** Symbol zum Hinzufügen von Feldern aus dem **Nicht ausgewählte Felder** Bereich.

   Oder

   Klicken Sie auf **-** Symbol zum Entfernen von Feldern aus dem **Ausgewählte Felder** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Die Werte für die verbundenen Felder werden automatisch ausgefüllt, nachdem Sie Datensätze oder Objekte verknüpft haben.

   >[!IMPORTANT]
   >
   >    Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in der Anwendung der verknüpften Objekttypen.


1. (Optional) Klicken Sie auf **Überspringen** , um das Hinzufügen von Feldern aus dem verknüpften Datensatz oder Objekttyp zu überspringen. Die **Name** oder **Titel** des verknüpften Datensatzes ist das einzige sichtbare Feld in der Tabellenansicht des Datensatztyps, von dem Sie eine Verbindung herstellen.

1. (Optional und bedingt) Wenn Sie ein Feld vom Typ Zahl, Währung, Prozentsatz oder Datum verknüpfen möchten, wählen Sie auch einen Aggregatorwert aus. Die Werte der verknüpften Felder werden je nach ausgewähltem Aggregator entweder durch Kommas oder als aggregierter Wert angezeigt, wenn Benutzer im verknüpften Datensatzfeld mehr als einen verknüpften Datensatz auswählen.

   >[!IMPORTANT]
   >
   >    Sie müssen beim Hinzufügen von Suchdatumsfeldern einen Aggregatorwert auswählen, wenn die Felder verfügbar sein sollen, um als Start- und Enddaten für die Timeline- und Kalenderansichten hinzuzufügen. Sie können beispielsweise den MAX- oder MIN-Aggregator für ein Suchdatumsfeld auswählen.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Beim Verbinden von Datensatztypen mit Experience Manager Assets sind keine Aggregatoren verfügbar.

   Wählen Sie aus den folgenden Optionen aus:

   * **Keines**: Zeigt die Werte an, die aus mehreren durch Kommas getrennten Datensätzen stammen. Dies ist die Standardauswahl.
   * **MAX**: Zeigt den höchsten Wert aus allen Werten an, die aus mehreren im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **MIN**: Zeigt den niedrigsten Wert aus allen Werten an, die aus mehreren, im verknüpften Datensatzfeld ausgewählten Datensätzen stammen.
   * **SUM**: Zeigt die Gesamtzahl aller Werte an, die aus mehreren im Feld &quot;Verknüpfter Datensatz&quot;ausgewählten Datensätzen stammen.
   * **AVG**: Zeigt den Durchschnitt aller Werte an, die aus mehreren, im Feld &quot;Verknüpfter Datensatz&quot;ausgewählten Datensätzen stammen.
   * **UNIQUE**: Entfernt Duplikate aus den Suchfeldwerten und zeigt nur die eindeutigen Werte an. Dies ist für die folgenden Feldtypen nicht verfügbar:
      * Absatz
      * Kontrollkästchen
      * Personen

   >[!NOTE]
   >
   >Sie können beispielsweise den Produktdatensatz (verknüpfter Datensatz) aus dem Campaign-Datensatz (Originaldatensatz) verknüpfen und ihn &quot;Produktfeld&quot;nennen. Sie können auch das Feld Budget des Produktdatensatzes aus dem Campaign-Datensatz verknüpfen und es &quot;Produktbudget&quot;nennen. Wenn Sie mehrere Datensätze im Feld &quot;Produkt&quot;auswählen können, können Sie Produkt 1 mit einem Budget von 100.000 $ und Produkt 2 mit einem Budget von 110.000 $ und Produkt 3 mit einem Budget von 100.000 $ auswählen. Je nach ausgewähltem Aggregator können Sie im verknüpften Feld aus dem ursprünglichen Datensatz die folgenden Budgetinformationen anzeigen:
   >
   >* **Keines**: 100.000 $, 110.000 $, 100.000 $
   >* **MAX**: 110.000 $
   >* **MIN**: 100.000 $
   >* **SUM**: 310.000 $
   >* **AVG**: 103.000,33 $
   >* **UNIQUE**: 100.000 $
   >

1. (Optional) Verwenden Sie die **suchen** icon ![](assets/search-icon.png) , um nach einem Feld zu suchen.

1. Klicks **Felder hinzufügen** , um Ihre Änderungen zu speichern.

   Die folgenden Elemente werden hinzugefügt:

   * Ein verknüpftes Datensatzfeld des Datensatztyps, von dem Sie eine Verknüpfung herstellen. Das verknüpfte Datensatzfeld zeigt einzelne Datensätze des verknüpften Datensatztyps an, nachdem Sie sie manuell hinzugefügt haben. Informationen zum Hinzufügen von Datensätzen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md). Der Name des verknüpften Datensatzfelds ist der Name, den Sie in Schritt 7 ausgewählt haben. <!--accurate-->

   * Ein verknüpftes (oder Lookup-) Feld (oder Felder), das Informationen über den verknüpften Datensatz oder die verknüpften Objekttypen anzeigt, nachdem Sie die Datensätze oder Objekte manuell in das verknüpfte Datensatzfeld eingefügt haben. Suchfelder werden nur erstellt, wenn die **Suchfelder auswählen** wird bei der Erstellung der Verbindung ausgewählt. Suchfelder werden automatisch nach folgendem Muster benannt:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Wenn Sie beispielsweise einen Kampagnen-Record-Typ mit einem Programmdatensatz-Typ verknüpft haben und das Feld Programm-verknüpfter Datensatz &quot;Programminformationen&quot;nennen, wählen Sie dann aus, auch das Feld Budget des Programms in der Tabellenansicht der Kampagne anzuzeigen, wird das verknüpfte Feld automatisch benannt. `Budget (from Program information)` in der Tabellenansicht der Kampagne.

   * Wenn Sie Datensatztypen miteinander verknüpfen, wird auch ein verknüpftes Datensatzfeld für den Datensatztyp hinzugefügt, mit dem Sie verknüpft sind. Der Name des verknüpften Datensatzfelds im verknüpften Datensatztyp ist der Name des Datensatztyps, von dem Sie eine Verknüpfung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Produkt&quot;aus dem Datensatztyp &quot;Kampagne&quot;verknüpfen und das verknüpfte Feld der Kampagne &quot;Verknüpftes Produkt&quot;nennen, wird ein mit &quot;Kampagne&quot;verknüpftes Datensatzfeld für den Produktdatensatz-Typ erstellt.

     >[!TIP]
     >
     > Für Objekte aus einer anderen Anwendung wird kein verknüpftes Datensatzfeld erstellt, das dem Datensatztyp entspricht, von dem aus Sie in der Workfront-Planung verknüpfen.

1. (Optional und bedingt) Klicken Sie in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatztyps auf den nach unten zeigenden Pfeil in der Kopfzeile der verknüpften Datensatzfelder und klicken Sie dann auf einen der folgenden Punkte:

   * **Feld bearbeiten**: Sie können die **Name** und **Beschreibung** Informationen zum Feld.
   * **Suchfelder bearbeiten**: Fügt die Felder des verknüpften Datensatzes hinzu oder entfernt sie.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Um Suchfelder hinzuzufügen oder zu entfernen, folgen Sie den Anweisungen in den Schritten 10-14 oben. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Sie können keine Suchfelder hinzufügen, die zu Datensatztypen gehören, von denen Sie Verknüpfungen zu Objektarten aus einer anderen Anwendung erstellen.
   >
   > Sie können beispielsweise das Suchfeld &quot;Kampagnenstatus&quot;nicht zu einem Workfront-Projekt hinzufügen, zu dem Sie über die Kampagnen verknüpfen.

1. (Optional) Klicken Sie in der Kopfzeile eines verknüpften Datensatzfelds auf den nach unten zeigenden Pfeil oder in der Kopfzeile eines Lookup-Felds des Datensatztyps, von dem Sie die Verknüpfung herstellen, und klicken Sie dann auf **Löschen**.

   Das Datensatzfeld oder das Lookup-Feld werden gelöscht. Wenn Sie ein Datensatzfeld löschen, werden auch alle mit dem verknüpften Datensatz verknüpften Suchfelder gelöscht.
