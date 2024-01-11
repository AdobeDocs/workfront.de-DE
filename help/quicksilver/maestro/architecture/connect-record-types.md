---
title: Datensatztypen verbinden
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Maestro-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu halten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Datensatztypen verbinden

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Adobe Maestro verwenden, um vollständig anpassbare Arbeitsbereiche zu entwerfen, die Datensatztypen enthalten, die in Ihrem Unternehmen benötigt werden. Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Maestro-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu halten.

Sie können Folgendes verbinden:

* Maestro-Betriebsaufzeichnungen
* Maestro-Taxonomien zueinander
* Maestro-Betriebsaufzeichentypen und -taxonomien untereinander
* Maestro-Betriebsdatentypen und -taxonomien mit Objekttypen aus anderen Anwendungen.

Auf diese Weise können Sie Felder aus dem verknüpften Datensatz oder Objekttyp in einem anderen Maestro-Datensatz anzeigen.

In diesem Artikel wird beschrieben, wie Sie zwei Maestro-Datensatztypen oder einen Maestro-Datensatztyp mit einem Objekt aus einer anderen Anwendung verbinden können.

Nachdem die Verbindung zwischen Datensatz- oder Objekttypen hergestellt wurde, können Sie einzelne Datensätze miteinander verbinden.

Informationen zum Verbinden eines Maestro-Datensatzes mit einem Objekt aus einer anderen Anwendung finden Sie unter [Datensätze verbinden](../records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](../architecture/example-connect-record-types-and-records.md).

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
   <p> Adobe Workfront</p> <p>Um Maestro-Record-Typen mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Überlegungen zum Verbinden von Datensatztypen

Beachten Sie Folgendes:

* Sie können die folgenden Entitäten in Maestro verbinden:

   * Zwei Betriebsaufzeichentypen
   * Zwei Taxonomien
   * Betriebsaufzeichentyp und Taxonomie
   * Ein operationeller Datensatztyp oder eine Taxonomie und ein Objekttyp aus einer anderen Anwendung.

* Sie können die folgenden Objekte aus den folgenden Anwendungen mit Maestro-Datensatztypen verbinden:

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
     >Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Maestro-Datensätze mit Adobe Experience Manager Assets zu verbinden.
     >
     >Wenn Sie Fragen zum Einstieg in die Adobe Admin Console haben, lesen Sie den Abschnitt [Häufig gestellte Fragen zu Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder einem Objekttyp aus einer anderen Anwendung verbunden haben, gibt es folgende Szenarien:

   * **Wenn Sie zwei Datensatztypen verbinden**: Ein Feld für verknüpfte Datensätze wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Ein ähnliches Feld für verknüpfte Datensätze wird für den Datensatztyp erstellt, mit dem Sie eine Verbindung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Datensatztyp &quot;Produkt&quot;verbinden, wird ein verknüpftes Datensatzfeld, das Sie &quot;Verknüpftes Produkt&quot;nennen, für den Datensatztyp &quot;Kampagne&quot;erstellt und ein verknüpfter Datensatztyp automatisch mit dem Namen &quot;Kampagne&quot;für den Produktdatensatz erstellt.

   * **Wenn Sie einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden**: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, aus dem Sie eine Verbindung herstellen. Für das Anwendungsobjekt der Drittanbieteranwendung wird kein verknüpftes Datensatzfeld automatisch erstellt.

     Für das Anwendungsobjekt eines Drittanbieters wird ein neuer Maestro-Record-Typ erstellt, wenn tatsächliche Objekte mit den Maestro-Datensätzen verbunden sind.

     Weitere Informationen finden Sie unter [Datensätze verbinden](../records/connect-records.md).

   * **Beim Hinzufügen von Suchfeldern aus dem Datensatz oder Objekt, zu dem Sie eine Verbindung herstellen**: Verknüpfte Felder werden dem Datensatz hinzugefügt, aus dem Sie eine Verbindung herstellen. Darin werden die Suchfelder angezeigt, die Sie ausgewählt haben, um den verknüpften Datensatz mit den Datensätzen, von denen Sie eine Verknüpfung herstellen, zu übernehmen. Die Datensatzfelder sind immer schreibgeschützt und werden automatisch mit den Werten des Drittanbieterobjekts gefüllt.

     Wenn Sie beispielsweise den Maestro-Record-Typ &quot;Kampagne&quot;mit einem Workfront-Projekt verbinden und das Feld &quot;Geplantes Abschlussdatum&quot;des Projekts auf den Maestro-Datensatz übertragen möchten, wird automatisch ein verknüpftes Feld namens &quot;Geplantes Abschlussdatum (aus Projekt)&quot;für den Datensatz erstellt, von dem Sie die Verknüpfung herstellen.

* Verknüpfte Datensatzfelder erhalten ein Beziehungssymbol ![](assets/relationship-field-icon.png).

  Verknüpfte Felder erhalten ein Symbol, das den Feldtyp identifiziert. Beispielsweise Symbole, die angeben, dass es sich bei einem Feld um eine Zahl, einen Absatz oder ein Datum handelt.

* Nachdem Sie einzelne Datensätze für einen Datensatztyp erstellt haben, können Sie die Datensätze, zu denen Sie eine Verbindung herstellen, aus dem Feld des verknüpften Datensatztyps auswählen. Weitere Informationen finden Sie unter [Datensätze verbinden](../records/connect-records.md).

## Datensatztypen verbinden

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensatztypen verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht angezeigt, und klicken Sie dann auf die Schaltfläche **Neue Verbindung** Registerkarte.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Im **Record Type** -Feld nach einem Datensatztyp suchen oder eine der folgenden Optionen auswählen: <!--is the field name spelled right? lowercase "t"?-->

   * Ein anderer betrieblicher Datensatztyp oder eine Taxonomie aus dem ausgewählten Arbeitsbereich

     >[!TIP]
     >
     >Es sind nur Datensatztypen und Taxonomien aus dem ausgewählten Arbeitsbereich verfügbar, mit denen eine Verbindung hergestellt werden kann.
     > 
     >Wenn im ausgewählten Arbeitsbereich keine anderen Datensatztypen vorhanden sind, wird der Workspace-Name nicht angezeigt.

   * A **Projekt, Portfolio, Programm, Firma** oder **Gruppe** aus dem **Workfront-Objekttypen** Abschnitt.
   * **Experience Manager Assets** aus dem **Adobe-Anwendungen** Abschnitt.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Der Name des verbundenen Felds, wie er in der Tabellenansicht oder auf der Detailseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verknüpfte Datensatzspalte in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatzfelds für die ursprünglichen Datensätze erstellt. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >Es wird empfohlen, den Namen des Datensatzes, zu dem Sie die Verknüpfung herstellen, in den Namen des verbundenen Datensatzfelds einzuschließen, um zu erfassen, von welchem Datensatztyp das neue Feld stammt. Der Name des verknüpften Datensatzes ist im neuen verknüpften Datensatzfeld oder in den verknüpften Feldern nicht sichtbar.

   * **Beschreibung**: Zusätzliche Informationen zum verbundenen Datensatzfeld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Mehrere Datensätze zulassen**: Wählen Sie diese Option, um anzugeben, dass Benutzer mehrere Datensätze hinzufügen können, wenn das Feld des verknüpften Datensatztyps in den Originaldatensätzen angezeigt wird. Diese Option ist standardmäßig aktiviert.
   * **Suchfelder auswählen**: Wählen Sie diese Option, um Felder aus dem ausgewählten Datensatztyp hinzuzufügen. Diese Option ist standardmäßig aktiviert.

1. (Bedingt und optional) Wenn Sie die Verbindung eines Workfront-Objekts ausgewählt haben, wählen Sie eine **Benutzerdefiniertes Formular** aus dem **Nur Projekte verknüpfen, die diesen Kriterien entsprechen** Abschnitt. <!--this needs to be updated for each object when they fix this UI.--> Nur Objekte, an die die ausgewählten benutzerdefinierten Formulare angehängt sind, können mit dem ausgewählten Maestro-Datensatztyp verknüpft werden. Sie können mehrere Formulare auswählen.

   ![](assets/workfront-project-connection-selection.png)

1. (Bedingt) Wenn Sie die Verbindung zu Experience Manager Assets hergestellt haben, wählen Sie ein Repository aus der **Experience Manager-Repository** Dropdown-Menü im **Verknüpfen von Assets aus dem folgenden Repository** Abschnitt. Dies ist ein erforderliches Feld. In diesem Feld werden nur Repositorys angezeigt, auf die Sie in Experience Manager Assets Zugriff haben.

   ![](assets/aem-assets-connection-selection.png)

1. Klicks **Erstellen**.

1. (Bedingt) Wenn Sie die Option **Suchfeld auswählen** -Einstellung, **Suchfelder hinzufügen** wird geöffnet.

   Klicken Sie auf **+** Symbol zum Hinzufügen von Feldern aus dem **Nicht ausgewählte Felder** Bereich.

   Oder

   Klicken Sie auf **-** Symbol zum Entfernen von Feldern aus dem **Ausgewählte Felder** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)


1. (Optional) Klicken Sie auf **Überspringen** und fügen keine Felder aus dem verknüpften Datensatz oder Objekt hinzu. Die **Name** des verknüpften Datensatzes ist das einzige sichtbare Feld in der Tabellenansicht des ursprünglichen Datensatzes.

1. (Optional und bedingt) Wenn Sie ein Feld vom Typ Zahl, Währung, Prozentsatz oder Datum verknüpfen möchten, wählen Sie auch einen Aggregatorwert aus. Die Werte der verknüpften Felder werden je nach ausgewähltem Aggregator entweder durch Kommas oder als aggregierter Wert angezeigt, wenn Benutzer im verknüpften Datensatzfeld mehr als einen verknüpften Datensatz auswählen.

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

   >[!NOTE]
   >
   >Sie können beispielsweise den Produktdatensatz (verknüpfter Datensatz) aus dem Campaign-Datensatz (Originaldatensatz) verknüpfen und ihn &quot;Produktfeld&quot;nennen. Sie können auch das Feld Budget des Produktdatensatzes aus dem Campaign-Datensatz verknüpfen und es &quot;Produktbudget&quot;nennen. Wenn Sie mehrere Datensätze im Feld &quot;Produkt&quot;auswählen konnten, können Sie Produkt 1 mit einem Budget von 120.000 $ und Produkt 2 mit einem Budget von 100.000 $ auswählen. Je nach ausgewähltem Aggregator können Sie im verknüpften Feld aus dem ursprünglichen Datensatz die folgenden Budgetinformationen anzeigen:
   >
   >* **Keines**: 120.000 $, 100.000 $
   >* **MAX**: 120.000 $
   >* **MIN**: 100.000 $
   >* **SUM**: 220.000 $
   >* **AVG**: 110.000 $
   >

1. (Optional) Verwenden Sie die **suchen** icon ![](assets/search-icon.png) , um nach einem Feld zu suchen.

1. Klicks **Felder hinzufügen** , um Ihre Änderungen zu speichern.

   Die folgenden Elemente werden hinzugefügt:

   * Das verknüpfte Datensatzfeld, das die Datensätze des verknüpften Datensatztyps anzeigt, nachdem Sie sie manuell hinzugefügt haben. Der Name des verknüpften Datensatzfelds ist der Name, den Sie in Schritt 5 ausgewählt haben. <!--accurate-->

   * Das verknüpfte Feld (oder die verknüpften Felder), das bzw. die Informationen aus den Feldern des verknüpften Datensatztyps anzeigt, nachdem Sie die Datensätze manuell in das verknüpfte Datensatzfeld eingefügt haben. Die verknüpften Felder werden nur erstellt, wenn die Variable **Suchfelder auswählen** wird bei der Erstellung der Verbindung ausgewählt. Die verknüpften Felder werden nach folgendem Muster benannt:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Wenn Sie Maestro-Datensatztypen miteinander verknüpfen, wird auch ein verknüpftes Datensatzfeld für den Datensatztyp hinzugefügt, mit dem Sie verknüpfen. Der Name des verknüpften Datensatzfelds im verknüpften Datensatztyp ist der Name des Datensatztyps, von dem Sie eine Verknüpfung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Produkt&quot;aus dem Datensatztyp &quot;Kampagne&quot;verknüpfen und das verknüpfte Feld der Kampagne &quot;Verknüpftes Produkt&quot;nennen, wird ein mit &quot;Kampagne&quot;verknüpftes Datensatzfeld für den Produktdatensatz-Typ erstellt.

1. (Optional) Klicken Sie in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatztyps auf den nach unten zeigenden Pfeil in der Kopfzeile der verknüpften Datensatzfelder und klicken Sie dann auf einen der folgenden Punkte:

   * **Feld bearbeiten**: Sie können nur die **Name** und **Beschreibung** Informationen zum Feld.
   * **Suchfelder bearbeiten**: Fügt die Felder des verknüpften Datensatzes hinzu oder entfernt sie.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Um Suchfelder hinzuzufügen oder zu entfernen, folgen Sie den Anweisungen in den Schritten 9 bis 13 oben. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Sie können die Suchfelder des Datensatzes, von dem Sie eine Verknüpfung herstellen, nicht zum verknüpften Datensatztyp hinzufügen, der ein Objekt in einer Drittanbieteranwendung anzeigt.
   >
   > Beispielsweise können Sie das Suchfeld eines Maestro-Objekts &quot;Kampagne&quot;nicht aus dem Feld &quot;Kampagne&quot;hinzufügen, das im Datensatztyp &quot;Maestro-Projekt&quot;angezeigt wird, wenn Sie eine Verknüpfung zu Workfront-Projekten herstellen.


1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil in der Kopfzeile des verknüpften Datensatzfelds vom Typ, von dem Sie die Verknüpfung herstellen, und klicken Sie dann auf **Löschen**.

   Das Datensatzfeld und alle zusätzlichen verknüpften Lookup-Felder werden gelöscht und die Felder und ihre Informationen können nicht wiederhergestellt werden.

   >[!TIP]
   >
   >    Das verknüpfte Datensatzfeld des Datensatztyps, zu dem Sie eine Verknüpfung herstellen, wird nicht gelöscht. <!-- is this still accurate?! -->
