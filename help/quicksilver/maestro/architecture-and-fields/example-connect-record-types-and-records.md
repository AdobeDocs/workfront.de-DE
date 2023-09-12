---
title: Beispiel für das Verbinden von Datensatztypen und Datensätzen
description: In diesem Artikel wird ein Beispiel für das Erstellen einer Verbindung zwischen einem Adobe Maestro-Record-Typ und einem Workfront-Projektobjekttyp beschrieben. Außerdem wird beschrieben, wie Sie einen Maestro-Datensatz mit einem einzelnen Projekt verbinden können.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 0%

---


# Beispiel für das Verbinden von Datensatztypen und Datensätzen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines geschlossenen Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In diesem Artikel wird ein Beispiel für Folgendes beschrieben:

* Erstellen einer Verbindung zwischen zwei Maestro-Datensatztypen und zwei Maestro-Datensätzen.

* Erstellen einer Verbindung zwischen einem Adobe Maestro-Record-Typ und einem Workfront-Projektobjekttyp sowie einer Verbindung zwischen einem Maestro-Datensatz und einem Projekt.

Weitere Informationen finden Sie auch in den folgenden Artikeln:

* [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md)
* [Datensätze verbinden](../records/connect-records.md)

## Verbinden von zwei Maestro-Datensatztypen und -Datensätzen (Beispiel)

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch einen anderen Datensatztyp namens &quot;Produkt&quot;, der über ein Währungsfeld namens &quot;Budget&quot;verfügt.

Sie möchten ein Feld für den Datensatztyp von Campaign erstellen, in dem Sie die Werte des Felds Budget für den Typ Produkt anzeigen können.

Gehen Sie dazu folgendermaßen vor:

1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht ein neues Feld hinzufügen, und klicken Sie dann auf **Neue Verbindung**.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record Type**: Produkt <!--did they change the casing here?-->
   * **Name**: Produktinformationen. Dies ist der Name des verknüpften Datensatzfelds.
   * **Beschreibung**: Dies sind die Produkte, mit denen meine Kampagnen verknüpft werden sollen.
   * **Mehrere Datensätze zulassen**: Wenn Sie diese Option aktiviert lassen, können Benutzer mehrere Datensätze auswählen, wenn das verknüpfte Datensatztyp-Feld (Produktinformationen) in den Originaldatensätzen (Kampagnen) angezeigt wird. In unserem Fall können sie mehrere Produkte auswählen, die mit einer Kampagne verbunden werden sollen.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird die **Suchfelder hinzufügen** wird als Nächstes geöffnet, damit Sie Produktfelder mit dem Campaign-Datensatztyp verknüpfen können. Sie können diesen Schritt überspringen und Produktfelder später hinzufügen.

   ![](assets/new-connection-with-product-record-type.png)

1. (Bedingt) Wenn Sie die Option **Option &quot;Suchfelder auswählen&quot;** im vorherigen Schritt aus der Liste der Felder, die mit der **Produkt** Record Type, klicken Sie auf die **+** -Symbol für **Budget** und klicken Sie auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Budget (aus Produktinformationen)**, der Name des verknüpften Felds. Alle Informationen zum Produktbudget werden in diesem Feld für die Campaign-Datensätze angezeigt.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Wenn Sie das Budget aller ausgewählten Produkte als eine Gesamtanzahl anzeigen möchten, wählen Sie **SUM** im Dropdown-Menü rechts neben dem Feldnamen. Wenn Benutzer mehrere Produkte in der **Produktinformationen** verknüpftes Datensatzfeld, das **Budget (aus Produktinformationen)** fügt alle Budgetwerte zusammen und zeigt die Summe an. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie **Keines**, anstelle von **SUM**, werden die einzelnen Budgets durch Kommas getrennt angezeigt.

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht der Kampagnentabelle und auf der Seite Details einer Kampagne:

      * **Produktinformationen** (verknüpftes Datensatzfeld): Zeigt den Namen der Produkte an.
      * **Budget (aus Produktinformationen)** (verknüpftes Feld): Zeigt die Budgets der im Feld Produktinformationen ausgewählten Produkte an.

   * In der Tabellenansicht des Produktdatensatzes und auf der Seite &quot;Details&quot;eines Produkts:

      * **Kampagne**: Dies gibt an, dass der Produktdatensatztyp vom Campaign-Datensatztyp aus verknüpft ist.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Verknüpfte Datensatzfelder werden durch das Beziehungssymbol gekennzeichnet ![](assets/relationship-field-icon.png).

1. So füllen Sie die **Produktinformationen** aus dem **Kampagne** Tabellenansicht des Datensatztyps erstellen, erstellen Sie eine Kampagne, indem Sie in der Tabelle des Kampagnentyps eine neue Zeile hinzufügen.
1. Klicken Sie auf **+** -Symbol in  **Produktinformationen** Spalte der neuen Kampagne. Die **Objekte verbinden** angezeigt. Der Name des Datensatztyps, mit dem Sie (Produkt) verknüpfen, wird in der linken oberen Ecke des Felds angezeigt.

   ![](assets/connect-objects-box-to-select-other-maestro-records-example-for-product-record.png)

1. Wählen Sie die Produktdatensätze aus, die Sie mit den Campaign-Datensätzen verbinden möchten, und klicken Sie auf **Objekte verbinden**.

   Die folgenden Spalten werden in der Tabelle vom Typ Campaign-Datensatz ausgefüllt:
   * Die **Produktinformationen** wird für den Campaign-Datensatz mit den ausgewählten Produkten ausgefüllt.
   * **Das Budget (aus Produktinformationen)** mit dem Budgetwert für jedes ausgewählte Produkt oder mit einer Gesamtsumme aller Budgets der ausgewählten Produkte gefüllt.

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen, werden alle Werte durch Kommas getrennt angezeigt.

1. So füllen Sie die **Kampagne** aus dem **Produkt** -Tabellenansicht, wiederholen Sie die Schritte 5 bis 7, angefangen bei der Tabellenansicht vom Typ Produktdatensatz und wählen Sie Kampagneninformationen aus. Dadurch wird auch das Feld Produktinformationen in der Tabelle des Campaign-Datensatztyps aktualisiert. <!--ensure the step numbers remain correct-->


## Verbinden eines Maestro-Datensatztyps mit einem Workfront-Projektobjekttyp und einem Datensatz mit einzelnen Projekten

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch Projekte in Workfront mit dem Feld &quot;Geplanter Umsatz&quot;.

Sie möchten ein Verbindungsfeld für den Datensatztyp von Campaign erstellen, in dem Sie die Werte des Felds &quot;Geplanter Umsatz&quot;im Projekt in Workfront für bestimmte Kampagnen anzeigen können.

Gehen Sie dazu folgendermaßen vor:

1. Wechseln Sie zu einem Arbeitsbereich, in dem Sie den Campaign-Datensatztyp mit Workfront-Projekten verbinden möchten.
1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp im ausgewählten Arbeitsbereich.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht ein neues Feld hinzufügen, und klicken Sie dann auf **Neue Verbindung**.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record Type**: Workfront-Projekt (aus dem Workfront-Unterabschnitt) <!--did they change the casing here for the field label and did they take "Workfront" out of the name of the object?-->
   * **Name**: Projektinformationen. Dies ist der Name des verknüpften Objektfelds.
   * **Beschreibung**: Dies sind die Projekte, mit denen meine Kampagnen verknüpft werden sollen.
   * 
      * **Mehrere Datensätze zulassen**: Wenn Sie diese Option aktiviert lassen, können Benutzer mehrere Objekte auswählen, wenn das Feld &quot;Verknüpfter Objekttyp&quot;(Projektinformationen) in den Originaldatensätzen (Kampagnen) angezeigt wird.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird die **Suchfelder hinzufügen** wird als Nächstes geöffnet, damit Sie Projektfelder mit dem Campaign-Datensatztyp verknüpfen können. Sie können diesen Schritt überspringen und zu einem späteren Zeitpunkt Projektfelder hinzufügen.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Bedingt) Wenn Sie die Option **Option &quot;Suchfelder auswählen&quot;** im vorherigen Schritt aus der Liste der Felder, die mit der **Projekt** Objekttyp auswählen, klicken Sie auf die **+** -Symbol für **Geplanter Umsatz** und klicken Sie auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Geplanter Umsatz (aus Projektinformationen)**, der Name des verknüpften Felds. Alle Informationen aus dem Feld Projektumsatz werden in diesem Feld für die Campaign-Datensätze angezeigt.

   >[!TIP]
   >
   >    Wenn Sie den geplanten Umsatz aller ausgewählten Projekte als eine Gesamtsumme anzeigen möchten, wählen Sie **SUM** im Dropdown-Menü rechts neben dem Feldnamen. Wenn Benutzer mehrere Projekte in der **Projektinformationen** verknüpftes Objektfeld, das **Geplanter Umsatz (aus Produktinformationen)** fügt alle Werte zusammen und zeigt die Summe an. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie **Keines**, anstelle von **SUM**, werden die einzelnen geplanten Umsätze durch Kommas getrennt angezeigt.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht der Kampagnentabelle und auf der Seite Details einer Kampagne:

      * **Projektinformationen** (verknüpftes Objektfeld): Zeigt den Namen der Projekte an.
      * **Geplanter Umsatz (aus Projektinformationen)** (verknüpftes Feld): Daraufhin werden die geplanten Umsätze der im Feld Projektinformationen ausgewählten Projekte angezeigt.

   >[!TIP]
   >
   >    Verknüpfte Objektfelder werden durch das Verknüpfungssymbol ![](assets/relationship-field-icon.png).

1. So füllen Sie die **Projektinformationen** aus dem **Kampagne** Tabellenansicht des Datensatztyps erstellen Sie eine Kampagne, indem Sie der Tabelle eine neue Zeile hinzufügen.
1. Klicken Sie auf **+** -Symbol in  **Projektinformationen** Spalte der neuen Kampagne. Die **Objekte verbinden** angezeigt. Der Name des Objekttyps, mit dem Sie (Workfront-Projekt) verknüpfen, wird in der linken oberen Ecke des Felds angezeigt.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Wählen Sie das Projekt bzw. die Projekte aus, mit denen Sie eine Verbindung herstellen möchten, und klicken Sie auf **Objekte verbinden**.

   Dem ausgewählten Arbeitsbereich werden folgende Elemente hinzugefügt:

   * In der Datensatztyp-Tabelle von Campaign:
      * Die **Projektinformationen** wird für den Campaign-Datensatz mit den ausgewählten Projekten gefüllt.
      * Die **Geplanter Umsatz (aus Produktinformationen)** mit dem Budgetwert für jedes ausgewählte Produkt gefüllt. Dies ist ein schreibgeschütztes Feld.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen und im objektverknüpften Feld mehrere Objekte auswählen, werden alle Werte durch Kommas getrennt angezeigt.

   * Ein schreibgeschützter Workfront-Projektdatensatz für den ausgewählten Arbeitsbereich.

1. Klicken Sie in der Kopfzeile der Seite auf den Pfeil nach links neben dem Datensatznamen, um zum zu aktualisierenden Arbeitsbereich zu gelangen.
1. Öffnen Sie die **Workfront-Projekt** Record Type-Karte, um die Seite vom Typ Datensatz zu öffnen.

   Beachten Sie Folgendes für die Seite mit dem Workfront-Projekt-Datensatztyp:

   * Dies ist ein schreibgeschützter Maestro-Record-Typ, den Sie weder löschen noch aktualisieren können.
   * Die Projekte, die Sie für die Verbindung mit Kampagnen ausgewählt haben, werden auf der Datensatztyp-Seite des Workfront-Projekts als separate Datensätze angezeigt. Die Projektdatensätze sind ebenfalls schreibgeschützt und ihre Informationen werden automatisch aktualisiert, wenn Projekte in Workfront aktualisiert werden. Sie müssen weitere Projekte aus dem verbundenen Maestro-Datensatz hinzufügen, um sie im Workfront-Projekt-Datensatztyp anzuzeigen.
   * Das Feld Kampagnenverknüpfter Datensatz wird mit den Namen der Kampagnen gefüllt, die mit Projekten verbunden sind, ausgehend von der Seite Kampagnentyps .

1. (Optional) Klicken Sie auf die **Mehr** icon ![](assets/more-menu.png) rechts neben dem Workfront Project Record Type-Namen und klicken Sie auf **Umbenennen** , um den Datensatztyp umzubenennen.

   >[!TIP]
   >
   >Sie können einen Namen eines Datensatztyps umbenennen, indem Sie auf den Namen in der Kopfzeile des Datensatztyps klicken.

1. Klicken Sie auf das Symbol Felder hinzufügen . ![](assets/add-fields-icon.png) in der oberen rechten Ecke der Workfront Project Record Type-Tabelle, um dem Workfront Project Maestro-Datensatztyp weitere Projektfelder hinzuzufügen.
1. Klicken Sie auf **+** für alle Projektfelder, die Sie zum Workfront Project Maestro-Datensatz hinzufügen möchten, im **Nicht ausgewählte Felder** Abschnitt.
1. Klicken Sie auf **-** für alle Projektfelder, die Sie aus dem Workfront Project Maestro-Datensatz entfernen möchten, im **Ausgewählte Felder** Abschnitt.
1. Klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >    Die Felder, die Sie zum Workfront Project Maestro-Datensatz hinzufügen, werden nur auf der Seite Workfront-Projekt hinzugefügt und nicht der Seite Campaign-Record Type als verknüpfte Felder hinzugefügt. Sie müssen die Projektfelder aus dem Feld Projektinformationen, verbunden mit Objekt des Datensatztyps Campaign hinzufügen, um sie für Kampagnen anzuzeigen.

1. (Optional und bedingt) Wenn Sie mindestens zwei Datumsfelder für Projekte angezeigt haben, klicken Sie auf die Schaltfläche **Ansicht** Dropdown-Menü in der Workfront-Datensatztyp-Tabelle &quot;Projekt&quot;und **Ansicht erstellen** > **Timeline** > **Erstellen** , um eine Timeline-Ansicht zu erstellen und die Projekte in einer Timeline anzuzeigen.



