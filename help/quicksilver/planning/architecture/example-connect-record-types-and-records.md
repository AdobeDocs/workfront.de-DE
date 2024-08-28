---
title: Beispiel für das Verbinden von Datensatztypen und Datensätzen
description: In diesem Artikel wird ein Beispiel für das Erstellen einer Verbindung zwischen einem Adobe Workfront-Planungs-Datensatztyp und einem Workfront-Projektobjekttyp beschrieben. Außerdem wird beschrieben, wie Sie einen Workfront-Planungsdatensatz mit einem einzelnen Projekt verbinden können.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: a3006a05b7003e638596c2754b77e914083a5643
workflow-type: tm+mt
source-wordcount: '1949'
ht-degree: 0%

---

# Beispiel für das Verbinden von Datensatztypen und Datensätzen

{{planning-important-intro}}

In diesem Artikel wird ein Beispiel für Folgendes beschrieben:

* So erstellen Sie eine Verbindung zwischen zwei Workfront-Planungs-Datensatztypen und zwei Datensätzen.

* Erstellen einer Verbindung zwischen einem Workfront-Planungs-Datensatztyp und einem Workfront-Projektobjekttyp sowie einer Verbindung zwischen einem Datensatz und einem Projekt.

Weitere Informationen finden Sie auch in den folgenden Artikeln:

* [Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md)

## Verbinden von zwei Datensatztypen und Datensätzen in der Workfront-Planung (Beispiel)

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch einen anderen Datensatztyp namens &quot;Produkt&quot;, der über ein Währungsfeld namens &quot;Budget&quot;verfügt.

Sie möchten ein Feld für den Datensatztyp von Campaign erstellen, in dem Sie die Werte des Felds Budget des Datensatztyps Product anzeigen können.

Gehen Sie dazu folgendermaßen vor:

1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp in einem Arbeitsbereich.
1. Klicken Sie auf das Symbol &quot;**+**&quot;in der oberen rechten Ecke der Tabellenansicht, um ein neues Feld hinzuzufügen, klicken Sie dann auf &quot;**Neue Verbindung**&quot;und anschließend im ausgewählten Arbeitsbereich auf &quot;**Produkt**&quot;.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record type**: Product <!--did they change the casing here?-->
   * **Name**: Geben Sie dem neuen Feld einen Namen. Beispiel: &quot;Produktinformationen&quot;. Dies ist der Name des verknüpften Datensatzfelds.
   * **Beschreibung**: Fügen Sie eine Beschreibung für das neue Feld hinzu. Beispiel: &quot;Dies sind die Produkte, mit denen meine Kampagnen verknüpft werden sollen.&quot; Die Beschreibung des Felds wird angezeigt, wenn Sie den Mauszeiger über das Feld in der Spaltenüberschrift bewegen.
   * **Verbindungstyp**: Wählen Sie eine der folgenden Optionen aus:
      * **Viele zu viele**: Benutzer können eine Kampagne mit mehreren Produkten und ein Produkt mit mehreren Kampagnen verbinden.
      * **1:n**: Benutzer können eine Kampagne mit mehreren Produkten und ein Produkt mit einer Kampagne verbinden.
      * **Viele zu eins**: Benutzer können eine Kampagne mit einem Produkt und ein Produkt mit vielen Kampagnen verbinden.
      * **Eins zu eins**: Benutzer können eine Kampagne mit einem Produkt und ein Produkt mit einer Kampagne verbinden.

     >[!NOTE]
     >
     >Die Option **Verbindungstyp** ist beim Verbinden von Datensätzen aus verschiedenen Arbeitsbereichen oder beim Verbinden von Experience Manager-Assets nicht verfügbar. Weitere Informationen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Erscheinungsbild der Aufzeichnung**: Deaktivieren Sie den Umschalter **Titel** , wenn Sie den Namen der Produkte nicht anzeigen möchten, wenn Sie sie zum Feld &quot;Produktinformationen&quot;der Kampagne hinzufügen. Wenn diese Option aktiviert ist, zeigen Datensätze sowohl die Miniaturansicht als auch den Titel an. Der Umschalter ist standardmäßig aktiviert.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird als Nächstes das Feld **Suchfelder hinzufügen** geöffnet, damit Sie Produktfelder mit dem Kampagnen-Datensatztyp verknüpfen können. Sie können auf **Überspringen** klicken, um diesen Schritt zu überspringen und Produktfelder später hinzuzufügen.

   ![](assets/new-connection-with-product-record-type.png)

1. (Bedingt) Wenn Sie im vorherigen Schritt die Option **Suchfelder auswählen** ausgewählt haben, klicken Sie in der Liste der Felder, die mit dem Datensatztyp **Produkt** verknüpft sind, auf das Symbol **+** für das Feld **Budget** und klicken Sie dann auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Budget (aus Produktinformationen)** erstellt, das dem Namen des verknüpften Felds entspricht. Alle Informationen zum Produktbudget werden in diesem Feld für die Kampagnendatensätze angezeigt.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Wenn Sie das Budget aller ausgewählten Produkte als eine Gesamtanzahl anzeigen möchten, wählen Sie im Dropdown-Menü rechts neben dem Feldnamen **SUM** aus. Wenn Benutzer mehrere Produkte im Feld **Produktinformationen** verknüpfter Datensatz auswählen, werden im Feld **Budget (aus Produktinformationen)** alle Budgetwerte hinzugefügt und die Gesamtsumme angezeigt. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie &quot;**None**&quot;anstelle von &quot;**SUM**&quot;auswählen, werden die einzelnen Budgets der ausgewählten Produkte durch Kommas getrennt angezeigt.

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht von Campaign-Datensätzen und auf der Datensatzseite einer Kampagne:

      * **Produktinformationen** (das verknüpfte Datensatzfeld): Zeigt den Namen oder die Namen der Produkte an, wenn Sie sie hinzufügen.
      * **Budget (aus Produktinformationen)** (das verknüpfte Feld): Zeigt die Budgets der im Feld Produktinformationen ausgewählten Produkte an.

   * In der Tabellenansicht &quot;Produktdatensatz&quot;und auf der Seite Produktdatensatz eines Produkts:

      * **Kampagne**: Dies bedeutet, dass der Produktdatensatztyp vom Campaign-Datensatztyp aus verknüpft ist.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Verknüpfte Datensatzfelder erhalten das Beziehungssymbol ![](assets/relationship-field-icon.png).

1. Erstellen Sie in der Tabellenansicht vom Typ **Kampagne** eine Kampagne, indem Sie der Tabelle des Kampagnentyps eine neue Zeile hinzufügen.

1. Doppelklicken Sie in die Spalte **Produktinformationen** der neuen Kampagne.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines verbundenen Produkts, um es dem ausgewählten Datensatz hinzuzufügen. Das Produkt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Produkts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Produkt wird automatisch hinzugefügt.
   * Klicken Sie auf **Alle anzeigen** , um alle Produkte anzuzeigen.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf &quot;**See all**&quot;geklickt haben, wird das Feld **Objekte verbinden** angezeigt.

   ![](assets/connected-objects-table-for-records.png)

1. Geben Sie den Namen eines Produkts in das Suchfeld ein und wählen Sie es aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie die Produktdatensätze aus, die Sie mit den Campaign-Datensätzen verbinden möchten, und klicken Sie dann auf **Objekte verbinden**.

   >[!TIP]
   >
   >    Sie können die Datensatzseite einer Kampagne öffnen, das verknüpfte Datensatzfeld suchen und auf das Symbol **+** im Feld klicken, um Produkte vom verbundenen Produktdatensatztyp hinzuzufügen.

   Die folgenden Spalten werden in der Tabelle vom Typ Campaign-Datensatz ausgefüllt:
   * Das Feld **Produktinformationen** wird für den Campaign-Datensatz mit den ausgewählten Produkten ausgefüllt.
   * **Das Feld Budget (aus Produktinformationen)** wird mit dem Budgetwert für jedes ausgewählte Produkt oder mit einer Gesamtsumme aller Budgets der ausgewählten Produkte ausgefüllt (wenn Sie SUM für Ihren Aggregator ausgewählt haben).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen, werden alle Werte aus den ausgewählten Produkten durch Kommas getrennt angezeigt.

1. Um das Feld **Kampagne** aus der Tabellenansicht **Produkt** auszufüllen, wiederholen Sie die Schritte 5 bis 7, beginnend mit der Tabellenansicht des Produktdatensatzes und wählen Sie Kampagneninformationen aus. Dadurch wird auch das Feld Produktinformationen in der Tabelle des Campaign-Datensatztyps aktualisiert. <!--ensure the step numbers remain correct-->


## Verbinden eines Workfront-Planungs-Datensatztyps mit einem Workfront-Projektobjekttyp und eines Datensatzes mit einzelnen Projekten

>[!IMPORTANT]
>
>    Jeder Benutzer mit der Berechtigung Anzeigen oder höher für den Arbeitsbereich kann die Informationen in den verknüpften Feldern anzeigen, unabhängig von seinen Berechtigungen oder Zugriffsrechten in Workfront.

Sie haben beispielsweise einen Datensatztyp namens Campaign als Ihren ursprünglichen Datensatztyp.

Sie haben auch Projekte in Workfront mit einem Feld namens &quot;Geplanter Umsatz&quot;.

Sie möchten ein Verbindungsfeld für den Kampagnentyp erstellen, in dem Sie die Werte des Felds &quot;Geplanter Umsatz&quot;der Projekte in Workfront anzeigen können, die mit Kampagnen in der Workfront-Planung verbunden sind.

Gehen Sie dazu folgendermaßen vor:

1. Wechseln Sie zu einer Workspace, wo Sie den Campaign-Datensatztyp mit Workfront-Projekten verbinden möchten.
1. Öffnen Sie die Tabellenansicht für den Campaign-Datensatztyp im ausgewählten Arbeitsbereich.
1. Klicken Sie auf das Symbol &quot;**+**&quot;in der oberen rechten Ecke der Tabellenansicht, um ein neues Feld hinzuzufügen, klicken Sie dann auf &quot;**Neue Verbindung**&quot;und dann auf &quot;**Projekt**&quot;im Abschnitt &quot;**Workfront-Objekttypen**&quot;.
1. Fügen Sie die folgenden Informationen hinzu, beispielsweise:

   * **Record type**: Project (aus dem Workfront-Unterabschnitt)
   * **Name**: Geben Sie dem neuen Feld einen Namen, z. B. &quot;Projektinformationen&quot;.
   * **Beschreibung**: Fügen Sie eine Beschreibung für das neue Feld hinzu. Beispiel: &quot;Dies sind die Projekte, mit denen meine Kampagnen verknüpft werden sollen.&quot; Die Beschreibung wird in der Tabellenansicht angezeigt, wenn Sie den Mauszeiger über den Feldnamen in der Spaltenüberschrift bewegen.
   * **Verbindungstyp**: Wählen Sie eine der folgenden Optionen aus:
      * **Viele zu viele**: Benutzer können eine Kampagne mit mehreren Produkten und ein Produkt mit mehreren Kampagnen verbinden.
      * **1:n**: Benutzer können eine Kampagne mit mehreren Produkten und ein Produkt mit einer Kampagne verbinden.
      * **Viele zu eins**: Benutzer können eine Kampagne mit einem Produkt und ein Produkt mit vielen Kampagnen verbinden.
      * **Eins zu eins**: Benutzer können eine Kampagne mit einem Produkt und ein Produkt mit einer Kampagne verbinden.
   * **Nur Objekte verknüpfen, die diesen Kriterien entsprechen**: Wählen Sie ein benutzerdefiniertes Formular aus dem Dropdownmenü **Benutzerdefiniertes Formular** aus. Nur Projekte, die mit den angegebenen Formularen verknüpft sind, können mit Kampagnen verbunden werden. Sie können mehrere Formulare auswählen.
   * **Suchfelder auswählen**: Wenn Sie diese Option ausgewählt lassen, wird als Nächstes das Feld **Suchfelder hinzufügen** geöffnet, damit Sie Projektfelder mit dem Kampagnen-Datensatztyp verknüpfen können. Sie können auf **Überspringen** klicken, um diesen Schritt zu überspringen und die Felder des Projekts später hinzuzufügen.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Bedingt) Wenn Sie im vorherigen Schritt die Option **Suchfelder auswählen** ausgewählt haben, klicken Sie in der Liste der Felder, die mit dem Objekttyp **Projekt** verknüpft sind, auf das Symbol **+** für das Feld **Geplanter Umsatz** und klicken Sie dann auf **Felder hinzufügen**. Dadurch wird ein Feld mit dem Namen **Geplanter Umsatz (aus Projektinformationen)** erstellt, das dem Namen des verknüpften Felds entspricht. Alle Informationen aus dem Feld Geplanter Umsatz des Projekts werden in diesem Feld automatisch für die Kampagneneinträge angezeigt.

   >[!TIP]
   >
   >    Wenn Sie den geplanten Umsatz aller ausgewählten Projekte als eine Gesamtsumme anzeigen möchten, wählen Sie im Dropdown-Menü rechts neben dem Feldnamen **SUM** aus. Wenn Benutzer mehrere Projekte im Feld **Projektinformationen** des verknüpften Objekts auswählen, werden im Feld **Geplanter Umsatz (aus Produktinformationen)** alle zugehörigen Werte hinzugefügt und die Gesamtsumme angezeigt. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Wenn Sie &quot;**None**&quot;anstelle von &quot;**SUM**&quot;auswählen, werden die einzelnen geplanten Umsätze durch Kommas getrennt angezeigt.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Dadurch werden die folgenden Felder generiert:

   * In der Tabellenansicht von Campaign-Datensätzen und auf der Datensatzseite von Campaign:

      * **Projektinformationen** (das verknüpfte Objektfeld): Zeigt den Namen der Projekte an.
      * **Geplanter Umsatz (aus Projektinformationen)** (das verknüpfte Feld): Zeigt die geplanten Umsätze der im Feld Projektinformationen ausgewählten Projekte an.

   >[!TIP]
   >
   >    Verknüpfte Objektfelder erhalten das Beziehungssymbol ![](assets/relationship-field-icon.png).

1. Erstellen Sie in der Tabellenansicht **Kampagnen** eine Kampagne, indem Sie der Tabelle eine neue Zeile hinzufügen.

1. Doppelklicken Sie in die Spalte Projektinformationen** der neuen Kampagne.

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines Projekts, um es dem ausgewählten Datensatz hinzuzufügen. Das Projekt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Projekts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Projekt wird automatisch hinzugefügt.
   * Klicken Sie auf **Alle anzeigen** , um alle Projekte anzuzeigen.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf &quot;**See all**&quot;geklickt haben, wird das Feld **Objekte verbinden** angezeigt.

   ![](assets/connect-projects-larger-box.png)

1. Geben Sie den Namen eines Projekts in das Suchfeld ein und wählen Sie es aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie die Projektdatensätze aus, die Sie mit den Campaign-Datensätzen verbinden möchten, und klicken Sie dann auf **Objekte verbinden**.

   >[!TIP]
   >
   >    Sie können die Seite einer Kampagne öffnen, das verknüpfte Projektfeld suchen und auf das Symbol **+** im Feld klicken, um Projekte aus dem verbundenen Produktdatensatztyp hinzuzufügen.

   Dadurch wird dem ausgewählten Arbeitsbereich Folgendes hinzugefügt:

   * In der Datensatztyp-Tabelle von Campaign:
      * Das Feld **Projektinformationen** wird für den Campaign-Datensatz mit den ausgewählten Projekten ausgefüllt.
      * Das Feld **Geplanter Umsatz (aus Produktinformationen)** wird mit dem Budgetwert für jedes ausgewählte Produkt ausgefüllt. Dies ist ein schreibgeschütztes Feld.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Wenn Sie keinen Aggregator für mehrere Werte auswählen und im objektverknüpften Feld mehrere Objekte auswählen, werden alle Werte durch Kommas getrennt angezeigt.

1. Klicken Sie im Feld &quot;Verbundener Datensatz&quot;auf den Namen eines Projekts.

   Dadurch wird das Projekt in Workfront geöffnet, wenn Sie mindestens über Anzeigeberechtigungen für das Projekt verfügen.
1. (Optional) Aktualisieren Sie die Informationen zum Projekt in Workfront, sofern Sie dazu berechtigt sind.

1. (Optional) Halten Sie in der Tabellenansicht von Campaign den Mauszeiger über die Feldüberschrift **Projektinformationen**, klicken Sie auf den nach unten zeigenden Pfeil und klicken Sie dann auf **Suchfelder bearbeiten** .
1. Klicken Sie für alle Projektfelder, die Sie zum Workfront-Planungdatensatz des Projekts hinzufügen möchten, im Abschnitt **Nicht ausgewählte Felder** auf das Symbol **+** .
1. Klicken Sie für alle Projektfelder, die Sie aus dem Workfront-Projektplanungsdatensatz entfernen möchten, im Abschnitt **Ausgewählte Felder** auf das Symbol **-** .
1. Klicken Sie auf **Speichern**.

   Dem Campaign-Datensatztyp werden zusätzliche verknüpfte Felder hinzugefügt.
