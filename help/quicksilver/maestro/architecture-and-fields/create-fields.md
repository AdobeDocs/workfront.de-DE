---
title: Felder erstellen
description: In Adobe Maestro können Sie benutzerdefinierte Felder für jeden Betriebsdatentyp oder jede Taxonomie erstellen. Anschließend können Sie das Feld mit Maestro-Datensätzen verknüpfen.
hidefromtoc: true
hide: true
source-git-commit: 62c67c8db01c9fc40f530a83162476dd0972f464
workflow-type: tm+mt
source-wordcount: '2556'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Felder erstellen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines geschlossenen Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro können Sie benutzerdefinierte Felder für betriebliche Datensatztypen oder Taxonomien erstellen. Anschließend können Sie die Felder mit Maestro-Datensätzen verknüpfen, um die Datensatzinformationen zu verbessern.

Sie müssen Datensatztypen erstellen, bevor Sie Felder erstellen können, die mit ihnen verknüpft werden sollen. Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
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

## Überlegungen zu Maestro-Feldern

* Sie können Felder nur aus der Tabellenansicht einer Seite vom Typ Datensatz erstellen. Felder werden in der Tabellenansicht als Spalten angezeigt.

  Informationen zum Verwalten von Tabellenspalten (oder Datensatzfeldern) finden Sie unter [Tabellenansicht verwalten](../views/manage-the-table-view.md).

  Weitere Informationen zum Verwalten von Feldern finden Sie in den folgenden Artikeln:

   * [Felder bearbeiten](../architecture-and-fields/edit-fields.md)
   * [Felder löschen](./delete-fields.md)

* Die mit einem Datensatztyp verknüpften Felder können allen Datensätzen dieses Typs zugeordnet werden. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Felder, die einem Datensatztyp zugeordnet sind, können keinem anderen Datensatztyp hinzugefügt werden. <!-- this will change when they open the Field library tab when creating a field-->

* Sie können Felder manuell oder automatisch wie folgt erstellen:

   * Manuell:

      * Durch Hinzufügen von Spalten in der Tabellenansicht einer Seite vom Typ Datensatz. Die Spalten der Tabelle sind die Felder, die dem Datensatztyp zugeordnet sind. Es handelt sich dabei um dieselben Felder, die auf der Detailseite eines Datensatzes angezeigt werden.

        Auf der Detailseite eines Datensatzes können keine Felder erstellt werden.

        In diesem Artikel wird beschrieben, wie Sie Felder manuell erstellen.

      * Durch Verknüpfung von Datensatztypen. Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Maestro-Datensatztypen oder einem Datensatztyp und einem Objekttyp aus anderen Anwendungen hinzufügen.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Weitere Informationen zum Verbinden von Maestro-Datensatztypen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

      * Durch Import von Datensatztypen mithilfe einer Excel- oder CSV-Datei. Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

   * Automatisch:

      * Standardmäßig jedes Mal, wenn Sie einen Datensatztyp erstellen.

        Die folgenden Standardfelder werden standardmäßig für jeden neuen operationellen Datensatztyp erstellt:

         * Name
         * Beschreibung
         * Startdatum
         * Enddatum
         * Status. Die Standardwerte für den Datensatzstatus sind:
            * Entwicklung
            * Geplant
            * Aktiv
            * Abgeschlossen
            * Zurückgestellt

           Sie können weitere Werte hinzufügen oder die vorhandenen umbenennen.

        Im Folgenden finden Sie die Standardfelder, die standardmäßig für jeden neuen Taxonomiedatensatztyp erstellt werden:

         * Name <!--will more be added? If not, consider rephrasing this bullet-->

      * Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen. Maestro erstellt Felder für betriebliche Datensatztypen und Taxonomien, wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).



* Sie können die Einstellungen für die Felder anzeigen und aktualisieren, die Sie oder ein anderer Benutzer erstellt haben. <!--this will change with access/ permissions-->

* Sie können bis zu 500 Felder für einen Datensatztyp haben.

* Feldnamen können bis zu 250 Zeichen enthalten.

* Beim Löschen eines Datensatztyps, einer Taxonomie oder eines Arbeitsbereichs werden auch alle Felder, die mit ihnen verknüpft sind, und die Werte der Felder gelöscht und können nicht wiederhergestellt werden. <!-- this might change with a possible recycle bin solution?!-->


## Felder von Grund auf neu erstellen {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen, wählen Sie den Arbeitsbereich aus, für den Sie Felder erstellen möchten, und klicken Sie dann auf den Datensatztyp.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.

   >[!TIP]
   >
   >    Wenn keine Datensätze angezeigt werden, sind möglicherweise noch keine Datensätze vorhanden oder es wird ein Filter angewendet, der die Anzeige auf dem Bildschirm einschränkt.

   Alle vorhandenen Felder, die mit dem Datensatztyp verknüpft sind, werden in den Spalten der Tabellenansicht angezeigt. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Klicken Sie auf **+** rechts oben in der Tabellenansicht, um neue Felder hinzuzufügen.
1. Im **Neues Feld** wählen Sie aus den folgenden Feldtypen aus:

   * [Einzeiliger Text](#single-line-text)
   * [Absatz](#paragraph)
   * [Mehrfachauswahl](#multi-select)
   * [Einzelauswahl](#single-select)
   * [Datum](#date)
   * [Zahl](#number)
   * [Prozentsatz](#percentage)
   * [Währung](#currency)
   * [Kontrollkästchen](#checkbox)

   >[!IMPORTANT]
   >
   >    Der Feldtyp kann nach dem Speichern nicht mehr geändert werden.

1. Fahren Sie mit dem Hinzufügen der einzelnen Felder fort, wie in den folgenden Abschnitten beschrieben.

### Einzeiliger Text {#single-line-text}

Einzelzeilige Textfelder erfassen begrenzte alphanumerische Informationen. Sie können beispielsweise die Informationen zu Eigentümern, Interessenvertretern, Teams oder Organisationseinheiten in einem einzeiligen Textfeld erfassen. Der Inhalt eines einzeiligen Textfelds kann bis zu 250 Zeichen lang sein. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Einzelzeilentext** Feldtyp.

   ![](assets/single-line-text-field-type.png)

1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spaltenüberschrift eines Felds in einer Tabelle bewegen.
1. Klicken Sie auf **Erstellen**.

   Das neue einzeilige Feld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.


### Absatz {#paragraph}

Absatzfelder erfassen zusätzliche alphanumerische Informationen zu einem Datensatz, ähnlich dem Feld Beschreibung . Der Inhalt eines Absatzfelds kann bis zu 1.000 Zeichen lang sein.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Absatz** Feldtyp.

   ![](assets/paragraph-field-type.png)


1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. Klicken Sie auf **Erstellen**.

   Das neue Absatzfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.


### Mehrfachauswahl {#multi-select}

Sie können ein Mehrfachauswahlfeld verwenden, um zusätzliche Informationen in einem beliebigen Format zu erfassen, indem Sie mehrere Optionen aus einem Dropdown-Menü auswählen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Mehrfachauswahl** Feldtyp.

   ![](assets/multi-select-field-type.png)


1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Auswahlmöglichkeiten**: Die Optionen, die nach dem Speichern des Felds aus dem Dropdown-Menü ausgewählt werden können. Sie können sowohl Zahlen als auch Buchstaben für den Namen jeder Wahl haben.
1. Klicks **Auswahl hinzufügen** um so viele Auswahlmöglichkeiten wie nötig hinzuzufügen. Es gibt keine Beschränkung dafür, wie viele Auswahlmöglichkeiten Sie einem Mehrfachauswahlfeld hinzufügen können.
1. (Optional) Ziehen Sie die einzelnen Auswahlmöglichkeiten manuell in die gewünschte Reihenfolge oder wählen Sie die
   **Sortieren von Optionen A-Z** , wenn die Auswahlmöglichkeiten automatisch in alphabetischer Reihenfolge aufgeführt werden sollen. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicken Sie auf **x** rechts von einer Auswahl, um sie zu entfernen.
1. Klicken Sie auf das Farbfeld links neben einer Auswahl, um die Farbauswahl zu erweitern und die Farbe der einzelnen Optionen anzupassen.
1. Klicken Sie auf **Erstellen**.

   Das neue Mehrfachauswahlfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Einzelauswahl {#single-select}

Felder mit einmaliger Auswahl erfassen zusätzliche Informationen in einem beliebigen Format, indem Sie eine Option aus einem Dropdown-Menü auswählen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Einzelauswahl** Feldtyp.

   ![](assets/single-select-field-type.png)


1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Auswahlmöglichkeiten**: Die Optionen, die nach dem Speichern des Felds aus dem Dropdown-Menü ausgewählt werden können. Sie können sowohl Zahlen als auch Buchstaben für den Namen jeder Wahl haben.

1. Klicks **Auswahl hinzufügen** um so viele Auswahlmöglichkeiten wie nötig hinzuzufügen. Es gibt keine Beschränkung dafür, wie viele Auswahlmöglichkeiten Sie einem Feld mit Einzelauswahl hinzufügen können.
1. (Optional) Ziehen Sie die einzelnen Auswahlmöglichkeiten manuell in die gewünschte Reihenfolge oder wählen Sie die **Sortieren von Optionen A-Z** , wenn die Auswahlmöglichkeiten automatisch in alphabetischer Reihenfolge aufgeführt werden sollen. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicken Sie auf **x** rechts von einer Auswahl, um sie zu entfernen.
1. Klicken Sie auf das Farbfeld links neben einer Auswahl, um die Farbauswahl zu erweitern und die Farbe der einzelnen Optionen anzupassen.
1. Klicken Sie auf **Erstellen**.

   Das neue Einzelauswahlfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Datum {#date}

Sie können ein Datumsfeld verwenden, um zusätzliche Informationen im Datums- und Uhrzeitformat zu erfassen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Datum** Feldtyp.

   ![](assets/date-field-type.png)


1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Datumsformat**: Der Typ des Datumsformats, das in diesem Feld angezeigt werden soll.

     Wählen Sie aus den folgenden Formaten aus:
      * **Gebietsschema**: Entspricht dem Gebietsschema Ihres Browsers.
      * **Standard**: 16.5.2023
      * **Lang**: 16. Mai 2023
      * **europäisch**: 16.5.2023
      * **ISO**: 2023-05-16
   * **Zeitfeld einschließen**: Wählen Sie diese Option, wenn Sie einen Zeitstempel einschließen möchten. Diese Option ist standardmäßig deaktiviert.

     Wählen Sie aus den folgenden Optionen aus:

      * **24 Stunden**: Beispiel: 18:00
      * **12 Stunden**: Beispiel: 18:00 Uhr

1. Klicken Sie auf **Erstellen**.

   Das neue Datumsfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Zahl {#number}

Zahlenfeldtypen erfassen Informationen im Zahlenformat.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Zahl** Feldtyp.

   ![](assets/number-field-type.png)
1. Fügen Sie die folgenden Informationen hinzu:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird.
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Zahlen in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicken Sie auf **Erstellen**.

   Das neue Zahlenfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Prozentsatz {#percentage}

Prozentfeldtypen erfassen Informationen in einem Zahlenformat, gefolgt von einem Prozentzeichen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Prozentsatz** Feldtyp.

   ![](assets/percentage-field-type.png)

1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird.
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Prozentwerte in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicken Sie auf **Erstellen**.

   Das neue Prozentfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Währung {#currency}

Währungsfeldtypen erfassen Informationen in einem Zahlenformat, dem ein Währungssymbol vorangestellt ist.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Währung** Feldtyp.

   ![](assets/currency-field-type.png)

1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Währung**: Der Typ der Währung, die in diesem Feld angezeigt werden soll. Dies ist eine Liste der Währungen gemäß der Internationalen Organisation für Normung (ISO).
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Währungswerte in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicken Sie auf **Erstellen**.

   Das neue Währungsfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

### Kontrollkästchen

Sie können den Feldtyp Kontrollkästchen verwenden, um einem Datensatz eine einzelne Kontrollkästchen-Option hinzuzufügen. Sie können dieses Feld verwenden, um ein bestimmtes Attribut oder einen bestimmten Status für diesen Datensatz anzugeben. Sie können sie beispielsweise als Markierung zum Tracking der Fertigstellung, Genehmigung oder eines anderen Binärattributs für jeden Datensatz verwenden.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Kontrollkästchen** Feldtyp.

   ![](assets/checkbox-field-type.png)

1. Fügen Sie die folgenden Informationen hinzu:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. Klicken Sie auf **Erstellen**.

   Das neue Kontrollkästchen wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden. Das Feld wird auch auf der Detailseite eines Datensatzes angezeigt.

## Erstellen von Feldern durch Verknüpfung von Datensatztypen

Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Maestro-Datensatztypen oder einem Datensatztyp und einem Objekttyp aus anderen Anwendungen hinzufügen.

Informationen zum Verbinden von Maestro-Datensatztypen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).

## Erstellen von Feldern durch Importieren von Datensatztypen mithilfe einer Excel- und CSV-Datei

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

## Erstellen von Feldern durch Erstellung eines Datensatztyps

Beim Erstellen eines Datensatztyps werden standardmäßig auch mehrere mit dem neuen Datensatztyp verknüpfte Felder erstellt. Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

## Erstellen von Feldern durch Erstellen eines Arbeitsbereichs aus einer Vorlage

Maestro erstellt Felder für betriebliche Datensatztypen und Taxonomien, wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen.

Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).



