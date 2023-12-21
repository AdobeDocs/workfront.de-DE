---
title: Felder erstellen
description: In Adobe Maestro können Sie benutzerdefinierte Felder für jeden Betriebsdatentyp oder jede Taxonomie erstellen. Anschließend können Sie das Feld mit Maestro-Datensätzen verknüpfen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '3169'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Formula fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Felder erstellen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro können Sie benutzerdefinierte Felder für betriebliche Datensatztypen oder Taxonomien erstellen. Anschließend können Sie die Felder mit Maestro-Datensätzen verknüpfen, um die Datensatzinformationen zu verbessern.

Sie müssen Datensatztypen erstellen, bevor Sie Felder erstellen können, die mit ihnen verknüpft werden sollen. Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

In Maestro können Sie Felder auf folgende Weise erstellen:

* Neu
* Durch Verbinden von Datensatztypen
* Durch Importieren von Datensatztypen mit Excel- und CSV-Dateien
* Erstellen eines Datensatztyps
* Erstellen eines Arbeitsbereichs aus einer Vorlage

Weitere Informationen zu Maestro-Feldern finden Sie unter [Feldübersicht](../fields/fields-overview.md)

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
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Felder von Grund auf neu erstellen {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen, wählen Sie den Arbeitsbereich aus, für den Sie Felder erstellen möchten, und klicken Sie dann auf den Datensatztyp.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.

   >[!TIP]
   >
   >    Wenn keine Datensätze angezeigt werden, sind möglicherweise noch keine Datensätze vorhanden oder es wird ein Filter angewendet, der die Anzeige auf dem Bildschirm einschränkt.

   Alle vorhandenen Felder, die mit dem Datensatztyp verknüpft sind, werden in den Spalten der Tabellenansicht angezeigt. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Klicken Sie auf **+** rechts oben in der Tabellenansicht, um neue Felder hinzuzufügen.
1. Im **Neues Feld** -Registerkarte nach einem Feldtyp in der **Feldtyp** oder wählen Sie aus den folgenden Feldtypen aus:

   * [Einzeiliger Text](#single-line-text)
   * [Absatz](#paragraph)
   * [Mehrfachauswahl](#multi-select)
   * [Einzelauswahl](#single-select)
   * [Datum](#date)
   * [Zahl](#number)
   * [Prozentsatz](#percentage)
   * [Währung](#currency)
   * [Kontrollkästchen](#checkbox)
   * [Personen](#people)
   * [Erstellt von](#created-by)
   * [Erstellungsdatum](#created-date)
   * [Zuletzt geändert von](#last-modified-by)
   * [Zuletzt geändert am](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Der Feldtyp kann nach dem Speichern nicht mehr geändert werden.

1. Fahren Sie mit dem Hinzufügen der einzelnen Felder fort, wie in den folgenden Abschnitten beschrieben.

### Einzeiliger Text {#single-line-text}

Einzelzeilige Textfelder erfassen begrenzte alphanumerische Informationen. Sie können beispielsweise die Informationen zu Eigentümern, Interessenvertretern, Teams oder Organisationseinheiten in einem einzeiligen Textfeld erfassen. Der Inhalt eines einzeiligen Textfelds kann bis zu 250 Zeichen lang sein. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Einzelzeilentext** Feldtyp.

   ![](assets/single-line-text-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spaltenüberschrift eines Felds in einer Tabelle bewegen.
1. Klicks **Erstellen**.

   Das neue einzeilige Feld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.


### Absatz {#paragraph}

Absatzfelder erfassen zusätzliche alphanumerische Informationen zu einem Datensatz, ähnlich dem Feld Beschreibung .

>[!TIP]
>
>* Der Inhalt eines Absatzfelds kann bis zu 1.000 Zeichen lang sein.
>
>* Sie können die Rich-Text-Formatierung verwenden, um den Inhalt von Absatzfeldern zu verbessern, wenn sie in der Tabellenansicht oder auf der Detailseite eines Datensatzes angezeigt werden.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Absatz** Feldtyp.

   ![](assets/paragraph-field-type.png)


1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. Klicks **Erstellen**.

   Das neue Absatzfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.


### Mehrfachauswahl {#multi-select}

Sie können ein Mehrfachauswahlfeld verwenden, um zusätzliche Informationen in einem beliebigen Format zu erfassen, indem Sie mehrere Optionen aus einem Dropdown-Menü auswählen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Mehrfachauswahl** Feldtyp.

   ![](assets/multi-select-field-type.png)


1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Auswahlmöglichkeiten**: Die Optionen, die nach dem Speichern des Felds aus dem Dropdown-Menü ausgewählt werden können. Sie können sowohl Zahlen als auch Buchstaben für den Namen jeder Wahl haben.
1. Klicks **Auswahl hinzufügen** um so viele Auswahlmöglichkeiten wie nötig hinzuzufügen. Es gibt keine Beschränkung dafür, wie viele Auswahlmöglichkeiten Sie einem Mehrfachauswahlfeld hinzufügen können.
1. (Optional) Ziehen Sie die einzelnen Auswahlmöglichkeiten manuell in die gewünschte Reihenfolge oder wählen Sie die
   **Sortieren von Optionen A-Z** , wenn die Auswahlmöglichkeiten automatisch in alphabetischer Reihenfolge aufgeführt werden sollen. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicken Sie auf **x** rechts von einer Auswahl, um sie zu entfernen.
1. Klicken Sie auf das Farbfeld links neben einer Auswahl, um die Farbauswahl zu erweitern und die Farbe der einzelnen Optionen anzupassen.
1. Klicks **Erstellen**.

   Das neue Mehrfachauswahlfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Einzelauswahl {#single-select}

Felder mit einmaliger Auswahl erfassen zusätzliche Informationen in einem beliebigen Format, indem Sie eine Option aus einem Dropdown-Menü auswählen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Einzelauswahl** Feldtyp.

   ![](assets/single-select-field-type.png)


1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Auswahlmöglichkeiten**: Die Optionen, die nach dem Speichern des Felds aus dem Dropdown-Menü ausgewählt werden können. Sie können sowohl Zahlen als auch Buchstaben für den Namen jeder Wahl haben.

1. Klicks **Auswahl hinzufügen** um so viele Auswahlmöglichkeiten wie nötig hinzuzufügen. Es gibt keine Beschränkung dafür, wie viele Auswahlmöglichkeiten Sie einem Feld mit Einzelauswahl hinzufügen können.
1. (Optional) Ziehen Sie die einzelnen Auswahlmöglichkeiten manuell in die gewünschte Reihenfolge oder wählen Sie die **Sortieren von Optionen A-Z** , wenn die Auswahlmöglichkeiten automatisch in alphabetischer Reihenfolge aufgeführt werden sollen. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicken Sie auf **x** rechts von einer Auswahl, um sie zu entfernen.
1. Klicken Sie auf das Farbfeld links neben einer Auswahl, um die Farbauswahl zu erweitern und die Farbe der einzelnen Optionen anzupassen.
1. Klicks **Erstellen**.

   Das neue Einzelauswahlfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Datum {#date}

Sie können ein Datumsfeld verwenden, um zusätzliche Informationen im Datums- und Uhrzeitformat zu erfassen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Datum** Feldtyp.

   ![](assets/date-field-type.png)


1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Datumsformat**: Der Typ des Datumsformats, das in diesem Feld angezeigt werden soll. <!--update this casing - submitted bug for it-->

     Wählen Sie aus den folgenden Formaten aus:
      * **Gebietsschema**: Entspricht dem Gebietsschema Ihres Browsers.
      * **Standard**: 16.5.2023
      * **Lang**: 16. Mai 2023
      * **europäisch**: 16.5.2023
      * **ISO**: 2023-05-16
   * **Zeitfeld einschließen**: Wählen Sie diese Option, wenn Sie einen Zeitstempel einschließen möchten. Diese Option ist standardmäßig deaktiviert. <!--update this setting name - submitted bug for it to be changed-->

     Wählen Sie aus den folgenden Optionen aus:

      * **24 Stunden**: Beispiel: 18:00
      * **12 Stunden**: Beispiel: 18:00 Uhr

1. Klicks **Erstellen**.

   Das neue Datumsfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Zahl {#number}

Zahlenfeldtypen erfassen Informationen im Zahlenformat.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Zahl** Feldtyp.

   ![](assets/number-field-type.png)
1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird.
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Zahlen in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicks **Erstellen**.

   Das neue Zahlenfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Prozentsatz {#percentage}

Prozentfeldtypen erfassen Informationen in einem Zahlenformat, gefolgt von einem Prozentzeichen.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Prozentsatz** Feldtyp.

   ![](assets/percentage-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird.
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Prozentwerte in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicks **Erstellen**.

   Das neue Prozentfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Währung {#currency}

Währungsfeldtypen erfassen Informationen in einem Zahlenformat, dem ein Währungssymbol vorangestellt ist.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Währung** Feldtyp.

   ![](assets/currency-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Währung**: Der Typ der Währung, die in diesem Feld angezeigt werden soll. Dies ist eine Liste der Währungen gemäß der Internationalen Organisation für Normung (ISO).
   * **Genauigkeit**: Die Anzahl der Dezimalstellen, die für das Feld aufgezeichnet werden sollen. Sie können bis zu 6 Dezimalstellen anzeigen.
   * **Negative Zahlen zulassen**: Wählen Sie diese Option aus, wenn Sie negative Währungswerte in diesem Feld zulassen möchten. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie negative Zahlen zulassen auswählen und negative Werte auf den Datensätzen gespeichert werden, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung in Zukunft nicht mehr aufheben.

1. Klicks **Erstellen**.

   Das neue Währungsfeld wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Kontrollkästchen

Sie können den Feldtyp Kontrollkästchen verwenden, um einem Datensatz eine einzelne Kontrollkästchen-Option hinzuzufügen. Sie können dieses Feld verwenden, um ein bestimmtes Attribut oder einen bestimmten Status für diesen Datensatz anzugeben. Sie können sie beispielsweise als Markierung zum Tracking der Fertigstellung, Genehmigung oder eines anderen Binärattributs für jeden Datensatz verwenden.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Kontrollkästchen** Feldtyp.

   ![](assets/checkbox-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
1. Klicks **Erstellen**.

   Das neue Kontrollkästchen wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Personen

Sie können den Feldtyp Personen verwenden, um einen Benutzer hinzuzufügen <!--, job role, or team--> zu einem Datensatz. Es handelt sich um ein Feld vom Typ voraus, dem nur Benutzer hinzugefügt werden können.<!--, roles, or teams--> die bereits in Workfront vorhanden sind.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Personen** Feldtyp.

   ![](assets/people-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:
   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird.
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Mehrere Werte zulassen**: Wählen Sie diese Option aus, wenn Sie zulassen möchten, dass Benutzer mehr als einen Benutzer in dieses Feld hinzufügen können. Diese Option ist standardmäßig deaktiviert.

   >[!NOTE]
   >
   >    Wenn Sie die Option Mehrere Werte zulassen auswählen und mehrere Benutzer in den Datensätzen gespeichert sind, an die das Feld angehängt ist, können Sie die Auswahl der Einstellung bei der Bearbeitung dieses Felds in Zukunft nicht mehr aufheben.

1. Klicks **Erstellen**.

   Das neue Feld vom Typ Personen wird dem Datensatztyp als Spalte hinzugefügt und seine Werte können Datensätzen zugeordnet werden.

### Erstellt von

Sie können den Feldtyp Erstellt nach verwenden, um den Benutzer, der den Datensatz erstellt hat, einem Datensatz hinzuzufügen. Dies ist ein schreibgeschütztes Feld, in dem automatisch der Name des Benutzers eingetragen wird, der bei der Erstellung des Datensatzes angemeldet war.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Erstellt von** Feldtyp.

   ![](assets/created-by-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.

1. Klicks **Erstellen**.

   Das neue Feld Erstellt nach Typ wird dem Datensatztyp als Spalte hinzugefügt und seine Werte werden mit dem Namen des Benutzers vorausgefüllt, der jeden Datensatz erstellt hat.


### Erstellungsdatum

Mit dem Feldtyp Erstellungsdatum können Sie das Datum der Erstellung eines Datensatzes zu einem Datensatz hinzufügen. Dies ist ein schreibgeschütztes Feld, das automatisch mit dem Datum (und optional mit der Uhrzeit) ausgefüllt wird, an dem der Datensatz erstellt wurde.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Erstellungsdatum** Feldtyp.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Datumsformat**: Wählen Sie aus den folgenden Formaten aus:

      * **Gebietsschema**: Entspricht dem Gebietsschema Ihres Browsers.
      * **Standard**: 16.5.2023
      * **Lang**: 16. Mai 2023
      * **europäisch**: 16.5.2023
      * **ISO**: 2023-05-16
   * **Zeitfeld einschließen**: Wählen Sie diese Option, wenn Sie einen Zeitstempel einschließen möchten. Diese Option ist standardmäßig deaktiviert. <!--submitted a UI text change for this - check the UI-->

     Wählen Sie aus den folgenden Optionen aus:

      * **24 Stunden**: Beispiel: 18:00
      * **12 Stunden**: Beispiel: 18:00 Uhr

1. Klicks **Erstellen**.

   Das neue Feld Erstelltes Datum wird dem Datensatztyp als Spalte hinzugefügt und seine Werte werden mit dem Datum (oder Datum und Uhrzeit) zum Zeitpunkt der Erstellung des Datensatzes vorausgefüllt.


### Zuletzt geändert von

Mit dem Feldtyp Letzte Änderung können Sie den Benutzer, der den Datensatz zuletzt geändert hat, zu einem Datensatz hinzufügen. Dies ist ein schreibgeschütztes Feld, das automatisch mit dem Namen des Benutzers gefüllt wird, der bei der letzten Aktualisierung des Datensatzes angemeldet war.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Zuletzt geändert durch** Feldtyp.

   ![](assets/last-modified-by-field-type.png)

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.

1. Klicks **Erstellen**.

   Das neue Feld Letzte Änderung nach Typ wird dem Datensatztyp als Spalte hinzugefügt und seine Werte werden mit dem Namen des Benutzers vorausgefüllt, der jeden Datensatz zuletzt geändert hat.


### Zuletzt geändert am

Sie können den Feldtyp Letzte Änderung des Datums verwenden, um das Datum hinzuzufügen, an dem ein Datensatz zuletzt in einen Datensatz geändert wurde. Dies ist ein schreibgeschütztes Feld, das automatisch mit dem Datum (und optional mit der Uhrzeit) gefüllt wird, an dem der Datensatz zuletzt geändert wurde.

1. Erstellen Sie ein Feld wie im Abschnitt beschrieben. [Felder von Grund auf neu erstellen](#create-fields-from-scratch) Wählen Sie in diesem Artikel die **Erstellungsdatum** Feldtyp.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Fügen Sie die folgenden Informationen in die **Neues Feld** tab:

   * **Name**: Der Name des Feldtyps, wie er in einer Tabelle oder auf der Detailseite des Datensatzes angezeigt wird. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschreibung**: Zusätzliche Informationen zum Feld. Die Beschreibung eines Felds wird angezeigt, wenn Sie den Mauszeiger über die Spalte eines Felds in einer Tabelle bewegen.
   * **Datumsformat**: Wählen Sie aus den folgenden Formaten aus:

      * **Gebietsschema**: Entspricht dem Gebietsschema Ihres Browsers.
      * **Standard**: 16.5.2023
      * **Lang**: 16. Mai 2023
      * **europäisch**: 16.5.2023
      * **ISO**: 2023-05-16
   * **Zeitfeld einschließen**: Wählen Sie diese Option, wenn Sie einen Zeitstempel einschließen möchten. Diese Option ist standardmäßig deaktiviert. <!--submitted a UI text change for this - check the UI-->

     Wählen Sie aus den folgenden Optionen aus:

      * **24 Stunden**: Beispiel: 18:00
      * **12 Stunden**: Beispiel: 18:00 Uhr

1. Klicks **Erstellen**.

   Das neue Feld Letzte Änderung des Datentyps wird dem Datensatztyp als Spalte hinzugefügt und seine Werte werden mit dem Datum (oder Datum und Uhrzeit) der letzten Änderung des Datensatzes vorausgefüllt.

## Erstellen von Feldern durch Verbinden von Datensatztypen

Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Maestro-Datensatztypen oder einen Datensatztyp und einen Objekttyp aus anderen Anwendungen hinzufügen.

Informationen zum Verbinden von Maestro-Datensatztypen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md)

## Erstellen von Feldern durch Importieren von Datensatztypen mithilfe einer Excel- und CSV-Datei

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

## Erstellen von Feldern durch Erstellung eines Datensatztyps

Beim Erstellen eines Datensatztyps werden standardmäßig auch mehrere mit dem neuen Datensatztyp verknüpfte Felder erstellt. Weitere Informationen finden Sie unter [Erstellen von operationellen Datensatztypen](../architecture/create-record-types.md).

## Erstellen von Feldern durch Erstellen eines Arbeitsbereichs aus einer Vorlage

Maestro erstellt Felder für betriebliche Datensatztypen und Taxonomien, wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen.

Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).