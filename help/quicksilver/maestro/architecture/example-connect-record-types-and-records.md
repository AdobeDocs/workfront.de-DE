---
title: Beispiel für das Verbinden von Datensatztypen und Datensätzen
description: In diesem Artikel wird ein Beispiel beschrieben, wie Sie eine Verbindung zwischen einem Adobe Workspace-Planungs-Datensatztyp und einem Workfront-Projektobjekttyp herstellen. Außerdem wird beschrieben, wie Sie einen Workfront-Planungsdatensatz mit einem einzelnen Projekt verbinden können.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: 9b1b8d8661917946230033b661ca652f5edef734
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 0%

---

# Beispiel für das Verbinden von Datensatztypen und Datensätzen

{{maestro-important-intro}}

In diesem Artikel wird ein Beispiel für Folgendes beschrieben:

* So erstellen Sie eine Verbindung zwischen zwei Workfront-Planungs-Datensatztypen und zwei Datensätzen.

* Erstellen einer Verbindung zwischen einem Workfront-Planungs-Datensatztyp und einem Workfront-Projektobjekttyp sowie einer Verbindung zwischen einem Datensatz und einem Projekt.

Weitere Informationen finden Sie auch in den folgenden Artikeln:

* [Datensatztypen verbinden](../architecture/connect-record-types.md)
* [Datensätze verbinden](../records/connect-records.md)

## Verbinden von zwei Datensatztypen und Datensätzen in der Workfront-Planung (Beispiel)

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch einen anderen Datensatztyp namens &quot;Produkt&quot;, der über ein Währungsfeld namens &quot;Budget&quot;verfügt.

Sie möchten ein Feld für den Datensatztyp von Campaign erstellen, in dem Sie die Werte des Felds Budget des Datensatztyps Product anzeigen können.

Gehen Sie dazu folgendermaßen vor:

1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp in einem Arbeitsbereich.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht ein neues Feld hinzufügen, und klicken Sie dann auf **Neue Verbindung** Klicken Sie auf **Produkt** im ausgewählten Arbeitsbereich angezeigt.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record Type**: Produkt <!--did they change the casing here?-->
   * **Name**: Benennen Sie das neue Feld. Beispiel: &quot;Produktinformationen&quot;. Dies ist der Name des verknüpften Datensatzfelds.
   * **Beschreibung**: Fügen Sie eine Beschreibung für das neue Feld hinzu. Beispiel: &quot;Dies sind die Produkte, mit denen meine Kampagnen verknüpft werden sollen.&quot; Die Beschreibung des Felds wird angezeigt, wenn Sie den Mauszeiger über das Feld in der Spaltenüberschrift bewegen.
   * **Mehrere Datensätze zulassen**: Wenn Sie diese Option aktiviert lassen, können Benutzer mehrere Datensätze auswählen, wenn das verknüpfte Datensatztyp-Feld (Produktinformationen) in den Originaldatensätzen (Kampagnen) angezeigt wird. In unserem Fall können Benutzer mehrere Produkte auswählen, die mit einer Kampagne verbunden werden sollen.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird die **Suchfelder hinzufügen** wird als Nächstes geöffnet, damit Sie Produktfelder mit dem Campaign-Datensatztyp verknüpfen können. Sie können auf **Überspringen** um diesen Schritt zu überspringen und Produktfelder später hinzuzufügen.

   ![](assets/new-connection-with-product-record-type.png)

1. (Bedingt) Wenn Sie die Option **Option &quot;Suchfelder auswählen&quot;** im vorherigen Schritt aus der Liste der Felder, die mit der **Produkt** Record Type, klicken Sie auf die **+** -Symbol für **Budget** und klicken Sie auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Budget (aus Produktinformationen)**, der Name des verknüpften Felds. Alle Informationen zum Produktbudget werden in diesem Feld für die Campaign-Datensätze angezeigt.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Wenn Sie das Budget aller ausgewählten Produkte als eine Gesamtanzahl anzeigen möchten, wählen Sie **SUM** im Dropdown-Menü rechts neben dem Feldnamen. Wenn Benutzer mehrere Produkte in der **Produktinformationen** verknüpftes Datensatzfeld, das **Budget (aus Produktinformationen)** fügt alle Budgetwerte zusammen und zeigt die Summe an. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie **Keines**, anstelle von **SUM**, werden die einzelnen Budgets der ausgewählten Produkte durch Kommas getrennt angezeigt.

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht von Campaign-Datensätzen und auf der Datensatzseite einer Kampagne:

      * **Produktinformationen** (verknüpftes Datensatzfeld): Zeigt den Namen der Produkte an, wenn Sie sie hinzufügen.
      * **Budget (aus Produktinformationen)** (verknüpftes Feld): Zeigt die Budgets der im Feld Produktinformationen ausgewählten Produkte an.

   * In der Tabellenansicht &quot;Produktdatensatz&quot;und auf der Seite Produktdatensatz eines Produkts:

      * **Kampagne**: Dies gibt an, dass der Produktdatensatztyp vom Campaign-Datensatztyp aus verknüpft ist.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Verknüpfte Datensatzfelder werden durch das Beziehungssymbol gekennzeichnet ![](assets/relationship-field-icon.png).

1. Aus dem **Kampagne** Tabellenansicht des Datensatztyps erstellen, erstellen Sie eine Kampagne, indem Sie in der Tabelle des Kampagnentyps eine neue Zeile hinzufügen.

1. Doppelklicken Sie in die  **Produktinformationen** Spalte der neuen Kampagne.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines verbundenen Produkts, um es dem ausgewählten Datensatz hinzuzufügen. Das Produkt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Produkts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Produkt wird automatisch hinzugefügt.
   * Klicks **Alle anzeigen** , um alle Produkte anzuzeigen.

1. (Bedingt) Wenn Sie auf **Alle anzeigen** im vorherigen Schritt die Variable **Objekte verbinden** angezeigt.

   ![](assets/connected-objects-table-for-records.png)

1. Geben Sie den Namen eines Produkts in das Suchfeld ein und wählen Sie es aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie die Produktdatensätze aus, die Sie mit den Campaign-Datensätzen verbinden möchten, und klicken Sie auf **Objekte verbinden**.

   >[!TIP]
   >
   >    Sie können die Datensatzseite einer Kampagne öffnen, das verknüpfte Datensatzfeld suchen und auf die Schaltfläche **+** im Feld, um Produkte aus dem verbundenen Produktdatensatz-Typ hinzuzufügen.

   Die folgenden Spalten werden in der Tabelle vom Typ Campaign-Datensatz ausgefüllt:
   * Die **Produktinformationen** wird für den Campaign-Datensatz mit den ausgewählten Produkten ausgefüllt.
   * **Das Budget (aus Produktinformationen)** wird mit dem Budgetwert für jedes ausgewählte Produkt oder mit einem Gesamtbudget der ausgewählten Produkte ausgefüllt (wenn Sie SUM für Ihren Aggregator ausgewählt haben).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen, werden alle Werte aus den ausgewählten Produkten durch Kommas getrennt angezeigt.

1. So füllen Sie die **Kampagne** aus dem **Produkt** -Tabellenansicht, wiederholen Sie die Schritte 5 bis 7, angefangen bei der Tabellenansicht vom Typ Produktdatensatz und wählen Sie Kampagneninformationen aus. Dadurch wird auch das Feld Produktinformationen in der Tabelle des Campaign-Datensatztyps aktualisiert. <!--ensure the step numbers remain correct-->


## Verbinden eines Workfront-Planungs-Datensatztyps mit einem Workfront-Projektobjekttyp und eines Datensatzes mit einzelnen Projekten

>[!IMPORTANT]
>
>    Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in Workfront.

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch Projekte in Workfront mit einem Feld namens &quot;Geplanter Umsatz&quot;.

Sie möchten ein Verbindungsfeld für den Kampagnentyp erstellen, in dem Sie die Werte des Felds &quot;Geplanter Umsatz&quot;der Projekte in Workfront anzeigen können, die mit Kampagnen in der Workfront-Planung verbunden sind.

Gehen Sie dazu folgendermaßen vor:

1. Wechseln Sie zu einem Arbeitsbereich, in dem Sie den Campaign-Datensatztyp mit Workfront-Projekten verbinden möchten.
1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp im ausgewählten Arbeitsbereich.
1. Klicken Sie auf **+** in der oberen rechten Ecke der Tabellenansicht ein neues Feld hinzufügen, und klicken Sie dann auf **Neue Verbindung** Klicken Sie auf **Projekt** im **Workfront-Objekttypen** Abschnitt.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record Type**: Projekt (aus dem Workfront-Unterabschnitt)
   * **Name**: Geben Sie dem neuen Feld einen Namen, z. B. &quot;Projektinformationen&quot;.
   * **Beschreibung**: Fügen Sie eine Beschreibung für das neue Feld hinzu. Beispiel: &quot;Dies sind die Projekte, mit denen meine Kampagnen verknüpft werden sollen.&quot; Die Beschreibung wird in der Tabellenansicht angezeigt, wenn Sie den Mauszeiger über den Feldnamen in der Spaltenüberschrift bewegen.
   * 
      * **Mehrere Datensätze zulassen**: Wenn Sie diese Option deaktiviert lassen, können Benutzer mehrere Projekte auswählen, wenn das Feld &quot;Verknüpfter Projekttyp&quot;(Projektinformationen) in den Originaldatensätzen (Kampagnen) angezeigt wird.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird die **Suchfelder hinzufügen** wird als Nächstes geöffnet, damit Sie Projektfelder mit dem Campaign-Datensatztyp verknüpfen können. Sie können auf **Überspringen** , um diesen Schritt zu überspringen und die Projektfelder später hinzuzufügen.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Bedingt) Wenn Sie die Option **Option &quot;Suchfelder auswählen&quot;** im vorherigen Schritt aus der Liste der Felder, die mit der **Projekt** Objekttyp auswählen, klicken Sie auf die **+** -Symbol für **Geplanter Umsatz** und klicken Sie auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Geplanter Umsatz (aus Projektinformationen)**, der Name des verknüpften Felds. Alle Informationen aus dem Feld Geplanter Umsatz des Projekts werden in diesem Feld automatisch für die Kampagneneinträge angezeigt.

   >[!TIP]
   >
   >    Wenn Sie den geplanten Umsatz aller ausgewählten Projekte als eine Gesamtsumme anzeigen möchten, wählen Sie **SUM** im Dropdown-Menü rechts neben dem Feldnamen. Wenn Benutzer mehrere Projekte in der **Projektinformationen** verknüpftes Objektfeld, das **Geplanter Umsatz (aus Produktinformationen)** fügt alle Werte zusammen und zeigt die Summe an. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie **Keines**, anstelle von **SUM**, werden die einzelnen geplanten Umsätze durch Kommas getrennt angezeigt.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht von Campaign-Datensätzen und auf der Datensatzseite von Campaign:

      * **Projektinformationen** (verknüpftes Objektfeld): Zeigt den Namen der Projekte an.
      * **Geplanter Umsatz (aus Projektinformationen)** (verknüpftes Feld): Daraufhin werden die geplanten Umsätze der im Feld Projektinformationen ausgewählten Projekte angezeigt.

   >[!TIP]
   >
   >    Verknüpfte Objektfelder werden durch das Verknüpfungssymbol ![](assets/relationship-field-icon.png).

1. Aus dem **Kampagne** Tabellenansicht des Datensatztyps erstellen Sie eine Kampagne, indem Sie der Tabelle eine neue Zeile hinzufügen.

1. Doppelklicken Sie in die  **Projektinformationen** Spalte der neuen Kampagne.

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines Projekts, um es dem ausgewählten Datensatz hinzuzufügen. Das Projekt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Projekts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Projekt wird automatisch hinzugefügt.
   * Klicks **Alle anzeigen** , um alle Projekte anzuzeigen.

1. (Bedingt) Wenn Sie auf **Alle anzeigen** im vorherigen Schritt die Variable **Objekte verbinden** angezeigt.

   ![](assets/connect-projects-larger-box.png)

1. Geben Sie den Namen eines Projekts in das Suchfeld ein und wählen Sie es aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie die Datensätze des Projekts aus, die Sie mit den Campaign-Datensätzen verbinden möchten, und klicken Sie auf **Objekte verbinden**.

   >[!TIP]
   >
   >    Sie können die Seite einer Kampagne öffnen, das verknüpfte Projektfeld suchen und auf die Schaltfläche **+** im Feld, um Projekte aus dem verbundenen Produktdatensatz-Typ hinzuzufügen.

   Dadurch wird dem ausgewählten Arbeitsbereich Folgendes hinzugefügt:

   * In der Datensatztyp-Tabelle von Campaign:
      * Die **Projektinformationen** wird für den Campaign-Datensatz mit den ausgewählten Projekten gefüllt.
      * Die **Geplanter Umsatz (aus Produktinformationen)** mit dem Budgetwert für jedes ausgewählte Produkt gefüllt. Dies ist ein schreibgeschütztes Feld.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen und im objektverknüpften Feld mehrere Objekte auswählen, werden alle Werte durch Kommas getrennt angezeigt.

1. Klicken Sie im Feld &quot;Verbundener Datensatz&quot;auf den Namen eines Projekts.

   Dadurch wird die Seite des schreibgeschützten Woekfront-Planungsprojekts geöffnet.
Überprüfen Sie die Informationen zum Projekt. Auf der Datensatzseite werden nur ausgewählte Projektfelder angezeigt.

1. Klicks **Zu Quelle wechseln** in der rechten oberen Ecke des Bildschirms, um das Projekt in Workfront zu öffnen, wenn Sie mindestens über Anzeigeberechtigungen für das Projekt verfügen.
1. (Optional) Aktualisieren Sie die Informationen zum Projekt in Workfront, sofern Sie dazu berechtigt sind.

1. (Optional) Bewegen Sie in der Tabellenansicht von Campaign den Mauszeiger über die **Projektinformationen** -Feldüberschrift, klicken Sie auf den nach unten zeigenden Pfeil und klicken Sie dann auf **Suchfelder bearbeiten.**
1. Klicken Sie auf **+** für alle Projektfelder, die Sie dem Workfront-Planungsdatensatz des Projekts hinzufügen möchten, im **Nicht ausgewählte Felder** Abschnitt.
1. Klicken Sie auf **-** für alle Projektfelder, die Sie aus dem Workfront-Projekt-Planungsdatensatz entfernen möchten, im **Ausgewählte Felder** Abschnitt.
1. Klicken Sie auf **Speichern**.

   Dem Campaign-Datensatztyp werden zusätzliche verknüpfte Felder hinzugefügt.
