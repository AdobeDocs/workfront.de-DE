---
title: Datensatztypen verbinden
description: Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Maestro-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu halten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '1742'
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
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Adobe Maestro verwenden, um vollständig anpassbare Arbeitsbereiche zu entwerfen, die Datensatztypen enthalten, die in Ihrem Unternehmen benötigt werden. Eine Möglichkeit, anzugeben, wie sich einzelne Datensatztypen zueinander verhalten, besteht darin, sie miteinander zu verbinden. Außerdem können Sie Maestro-Record-Typen mit Objekttypen aus anderen Anwendungen verbinden, um das Benutzererlebnis zu verbessern und den Fokus in einer Anwendung zu halten.

Sie können Folgendes verbinden:

* Betriebsaufzeichentypen von Maestro
* Maestro-Betriebsaufzeichentypen zu Taxonomiedatensatztypen
* Maestro-Betriebsdatentypen und -objekttypen aus anderen Anwendungen.

Auf diese Weise können Sie Felder aus dem verknüpften Datensatz oder Objekttyp in einem anderen Maestro-Datensatz anzeigen.

In diesem Artikel wird beschrieben, wie Sie zwei Maestro-Datensatztypen oder einen Maestro-Datensatztyp mit einem Objekt aus einer anderen Anwendung verbinden können.

Nachdem die Verbindung zwischen Datensatz- oder Objekttypen hergestellt wurde, können Sie einzelne Datensätze miteinander verbinden.

Informationen zum Verbinden eines Maestro-Datensatzes mit einem Objekt aus einer anderen Anwendung finden Sie unter [Datensätze verbinden](../records/connect-records.md).

Ein Beispiel für das Verbinden von Datensatztypen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](../architecture-and-fields/example-connect-record-types-and-records.md).

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
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Beliebig</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Beliebig</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
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

* Sie können die folgenden Entitäten in Maestro verbinden:

   * Zwei Betriebsaufzeichentypen
   * Zwei Taxonomien
   * Betriebsaufzeichentyp und Taxonomie
   * Ein operationeller Datensatztyp und ein Objekttyp aus einer anderen Anwendung.

     >[!TIP]
     >
     >    Ein Taxonomie-Record-Typ kann nicht von einer anderen Anwendung aus mit einem operationellen Record-Typ oder einem Objekttyp verbunden werden.

* Sie können die folgenden Objekte aus den folgenden Anwendungen mit Maestro-Datensatztypen verbinden:

   * Adobe Workfront:

      * Projekte
      * Portfolios
      * Programme
      * Firmen
      * Gruppen

* Nachdem Sie einen Datensatztyp mit einem anderen Datensatztyp oder einem Objekttyp aus einer anderen Anwendung verbunden haben, gibt es folgende Szenarien:

   * Wenn Sie zwei Datensatztypen verbinden: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, von dem Sie eine Verbindung herstellen. Ein ähnliches Feld für verknüpfte Datensätze wird für den Datensatztyp erstellt, mit dem Sie eine Verbindung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Datensatztyp &quot;Produkt&quot;verbinden, wird ein verknüpftes Datensatzfeld, das Sie &quot;Verknüpftes Produkt&quot;nennen, für den Datensatztyp &quot;Kampagne&quot;erstellt und ein verknüpfter Datensatztyp automatisch mit dem Namen &quot;Kampagne&quot;für den Produktdatensatz erstellt.

   * Wenn Sie ein Feld vom Typ Datensatz mit einer Taxonomie verbinden: Ein verknüpftes Datensatzfeld wird für den Typ erstellt, aus dem Sie eine Verbindung herstellen. Für die Taxonomie, mit der Sie eine Verbindung herstellen, wird kein verknüpftes Datensatzfeld erstellt.

     Wenn Sie beispielsweise den Datensatztyp &quot;Kampagne&quot;mit dem Taxonomiedatensatz &quot;Zielgruppe&quot;verbinden, wird ein verknüpftes Datensatzfeld erstellt, das Sie &quot;Verknüpfte Zielgruppe&quot;nennen, und zwar im Datensatztyp &quot;Kampagne&quot;. Es wird kein verknüpftes Datensatzfeld mit dem Namen &quot;Kampagne&quot;für den Datensatztyp der Zielgruppe-Taxonomie erstellt. <!--this might be temporary-->

   * Wenn Sie ein Feld vom Typ Datensatz mit einem Objekttyp aus einer anderen Anwendung verbinden: Ein verknüpftes Datensatzfeld wird für den Datensatztyp erstellt, von dem aus Sie eine Verbindung herstellen. Für das Workfront-Projekt in Workfront wird kein verknüpftes Datensatzfeld automatisch erstellt. Ein verknüpftes Datensatzfeld wird nur dann für den Workfront-Objektdatensatz erstellt, wenn die eigentlichen Objekte mit den Maestro-Datensätzen verbunden sind.

     Weitere Informationen finden Sie unter [Datensätze verbinden](../records/connect-records.md).

* Nachdem Sie die Datensatztypen verbunden haben, können Sie mehrere Felder von einem Datensatztyp zu einem anderen Datensatztyp verbinden. Diese Felder werden als &quot;verknüpfte Felder&quot;oder &quot;Lookup-Felder&quot;bezeichnet.
* Verknüpfte Datensatzfelder erhalten ein Beziehungssymbol ![](assets/relationship-field-icon.png).
* Nachdem Sie einzelne Datensätze für einen Datensatztyp erstellt haben, können Sie die Datensätze, zu denen Sie eine Verbindung herstellen, aus dem Feld des verknüpften Datensatztyps auswählen. Weitere Informationen finden Sie unter [Datensätze verbinden](../records/connect-records.md).
* Sie können die Informationen der verknüpften Felder des Datensatztyps, aus dem Sie die Relation herstellen, nicht bearbeiten, da sie automatisch aus dem ursprünglichen Datensatztyp, zu dem sie gehören, gefüllt werden, sobald Sie die verknüpften Datensätze auswählen.

## Datensatztypen verbinden

<!--when changes here, also update the article for "Connect records"-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensatztypen verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht angezeigt, und klicken Sie dann auf die Schaltfläche **Neue Verbindung** Registerkarte.

   ![](assets/new-connection-tab-with-workfront-option.png)
1. Im **Record Type** wählen Sie eines der folgenden Elemente aus: <!--is the field name spelled right? lowercase "t"?-->

   * Sonstige betriebliche Datensatzart
   * Taxonomie
   * Ein Workfront-Projekt, ein Portfolio, ein Programm, ein Unternehmen oder eine Gruppe.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)

   >[!TIP]
   >
   > Nur Datensatztypen und Taxonomien aus dem ausgewählten Arbeitsbereich können ausgewählt werden.

1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Der Name des verbundenen Felds, wie er in der Tabellenansicht oder auf der Detailseite des ursprünglichen Datensatztyps angezeigt wird. Dadurch wird die verknüpfte Datensatzspalte in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatzfelds für die ursprünglichen Datensätze erstellt. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >Es wird empfohlen, den Namen des Datensatzes, zu dem Sie die Verknüpfung herstellen, in den Namen des verbundenen Datensatzfelds einzuschließen, um zu erfassen, von welchem Datensatztyp das neue Feld stammt. Der Name des verknüpften Datensatzes ist im neuen verknüpften Datensatzfeld oder in den verknüpften Feldern nicht sichtbar.

   * **Beschreibung**: Zusätzliche Informationen zum verbundenen Datensatzfeld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Mehrere Datensätze zulassen**: Wählen Sie diese Option, um anzugeben, dass Benutzer mehrere Datensätze hinzufügen können, wenn das Feld des verknüpften Datensatztyps in den Originaldatensätzen angezeigt wird. Diese Option ist standardmäßig aktiviert.
   * **Suchfelder auswählen**: Wählen Sie diese Option, um Felder aus dem ausgewählten Datensatztyp hinzuzufügen. Diese Option ist standardmäßig aktiviert.

1. Klicken Sie auf **Erstellen**.

1. (Bedingt) Wenn Sie im vorherigen Schritt die Einstellung Suchfeld auswählen ausgewählt haben, wird die **Suchfelder hinzufügen** wird geöffnet.

   Klicken Sie auf **+** Symbol zum Hinzufügen von Feldern aus dem **Nicht ausgewählte Felder** Bereich.

   Oder

   Klicken Sie auf **-** Symbol zum Entfernen von Feldern aus dem **Ausgewählte Felder** area

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!NOTE]
   >
   >Wenn Sie keines der Felder auswählen, wird die **Name** des verknüpften Datensatzes ist das einzige sichtbare Feld in der Tabellenansicht des ursprünglichen Datensatzes. Die **Name** -Feld kann nicht entfernt werden.

1. (Optional und bedingt) Wenn Sie ein Feld vom Typ Zahl, Währung, Prozentsatz oder Datum verknüpfen möchten, wählen Sie auch einen Aggregatorwert aus. Die Werte der verknüpften Felder werden je nach ausgewähltem Aggregator entweder durch Kommas oder als aggregierter Wert angezeigt, wenn Benutzer im verknüpften Datensatzfeld mehr als einen verknüpften Datensatz auswählen.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

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

1. (Optional) Klicken Sie auf **Überspringen** , wenn Sie keine Felder aus dem verbundenen Datensatztyp hinzufügen möchten.

1. Klicks **Felder hinzufügen** , um Ihre Änderungen zu speichern.

   Folgendes wird hinzugefügt:

   * Das verknüpfte Datensatzfeld, das die Datensätze des verknüpften Datensatztyps anzeigt, nachdem Sie sie manuell hinzugefügt haben. Der Name des verknüpften Datensatzfelds ist der Name, den Sie in Schritt 6 ausgewählt haben. <!-- ensure this is still accurate-->

   * Das verknüpfte Feld (oder die verknüpften Felder), das Informationen aus den Feldern des verknüpften Datensatztyps anzeigt, nachdem Sie die Datensätze manuell in das verknüpfte Datensatzfeld eingefügt haben. Die verknüpften Felder werden nur erstellt, wenn die Variable **Suchfelder auswählen** wird bei der Erstellung der Verbindung ausgewählt. Die verknüpften Felder werden nach folgendem Muster benannt:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Ein verknüpftes Datensatzfeld des Datensatztyps, mit dem Sie verknüpft sind. Der Name des verknüpften Datensatzfelds im verknüpften Datensatztyp ist der Name des Datensatztyps, von dem Sie eine Verknüpfung herstellen.

     Wenn Sie beispielsweise den Datensatztyp &quot;Produkt&quot;aus dem Datensatztyp &quot;Kampagne&quot;verknüpfen und das verknüpfte Feld der Kampagne &quot;Verknüpftes Produkt&quot;nennen, wird ein mit &quot;Kampagne&quot;verknüpftes Feld für den Produktdatensatztyp erstellt.

     <!--is the statement in the note below still accurate?? they were working on removing this from taxonomies-->

     >[!NOTE]
     >
     >Das verknüpfte Datensatzfeld, das den von Ihnen verknüpften Datensatztyp anzeigt, wird nicht zu Datensatztypen hinzugefügt, wenn Sie einen Datensatztyp mit folgendem Element verbinden: <!--is this temporary for taxonomies??-->
     >        
     >   * Eine Taxonomie.
     >   * Ein Objekttyp aus einer anderen Anwendung.

1. (Optional) Klicken Sie in der Tabellenansicht des ursprünglichen Datensatztyps oder des verknüpften Datensatztyps auf das Dropdown-Menü rechts neben dem verknüpften Datensatzfeld und klicken Sie dann auf eine der folgenden Optionen:

   * **Feld bearbeiten**: Sie können nur die **Name** und **Beschreibung** Informationen zum Feld.
   * **Suchfelder bearbeiten**: Fügt die Felder des verknüpften Datensatzes hinzu oder entfernt sie.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Um Felder hinzuzufügen oder zu entfernen, folgen Sie den Anweisungen in den Schritten 7 bis 12. <!--ensure these step numbers stay accurate-->

1. (Optional) Klicken Sie in der Kopfzeile des verknüpften Datensatzes oder der verknüpften Felder auf den nach unten zeigenden Pfeil und dann auf **Löschen**.

   Das Datensatzfeld und alle zusätzlichen Lookup-Felder werden gelöscht und die Felder und ihre Informationen können nicht wiederhergestellt werden.

   >[!TIP]
   >
   >    Das verknüpfte Datensatzfeld im Datensatz, der mit dem ursprünglichen Datensatz verknüpft ist, wird nicht gelöscht. <!-- is this still accurate?! -->

