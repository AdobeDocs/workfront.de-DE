---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: '"Kick-Starts-Szenario: Importieren von benutzerdefinierten Feldern mit mehreren Optionen in Workfront'''
description: Mit der Kick-Start-Funktion können Sie benutzerdefinierte Felder mit mehreren Optionen in Adobe Workfront importieren.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 0%

---


# Kick-Starts-Szenario: Benutzerdefinierte Felder mit mehreren Optionen in Workfront importieren

Mit der Kick-Start-Funktion können Sie benutzerdefinierte Felder mit mehreren Optionen in Adobe Workfront importieren.

Beispiele für benutzerdefinierte Felder mit mehreren Optionen:

* Mehrfachauswahl-Dropdown
* Dropdown
* Kontrollkästchen
* Optionsschaltflächen

Diese Felder können manchmal viele (manchmal Hunderte) Optionen haben. Durch den Import mit der Kick-Start-Funktion sparen Sie als Workfront-Administrator viel Zeit und vermeiden Fehler.

>[!IMPORTANT]
>
>Führen Sie die in den folgenden Abschnitten beschriebenen Schritte aus, um benutzerdefinierte Felder mit mehreren Optionen mithilfe eines Schnellstarts zu importieren:
>
>1. Exportieren vorhandener benutzerdefinierter Daten aus Workfront (optionaler Schritt)
>1. Exportieren der Kick-Start-Vorlage für benutzerdefinierte Daten
>1. Füllen der Excel Kick-Start-Tabelle
>1. Hochladen der Excel-Tabelle in Workfront



## Exportieren vorhandener benutzerdefinierter Daten aus Workfront (optionaler Schritt)

Wenn Sie nicht mit der Workfront-Datenbankstruktur vertraut sind oder nicht mit der Schnellstartdatei vertraut sind, die Workfront zum Importieren von Informationen benötigt, empfehlen wir Ihnen, zunächst eine Schnellstartdatei aus Workfront mit vorhandenen Informationen zu exportieren, die den Feldern ähneln, die Sie importieren möchten.

Wenn Sie beispielsweise benutzerdefinierte Formulare oder benutzerdefinierte Felder importieren möchten, müssen Sie zuerst eine Schnellstartdatei mit vorhandenen benutzerdefinierten Daten exportieren.

Durch den Export vorhandener Daten können Sie diese zunächst überprüfen und feststellen, wie Ihre neuen Daten formatiert werden müssen.

Wenn Sie die Workfront-Datenbankobjekte und -struktur gut verstehen, können Sie mit dem folgenden Abschnitt fortfahren.

So exportieren Sie vorhandene Daten aus Workfront:

1. Klicken **Hauptmenü > Einrichtung** in der oberen rechten Ecke der Workfront-Benutzeroberfläche.
1. Erweitern Sie die **System** Menü links, und klicken Sie dann auf **Daten exportieren (Kick-Starts)**.

   ![](assets/export-data-kick-starts-link-in-setup.png)

1. Auswählen **Benutzerdefinierte Daten** im **Was soll eingeschlossen werden?** Abschnitt.

   ![](assets/existing-custom-data-box-checked-kick-starts.png)

1. Auswählen **.xlsx-Datei** im **Download-Format** Abschnitt.

   >[!TIP]
   >
   >    Je nachdem, wie viele benutzerdefinierte Daten Sie in Ihrem System haben, kann dies lange dauern.

   ![](assets/download-button-for-kick-starts.png)

1. Klicken **Download**. Eine .xlsx-Datei wird auf Ihren Computer heruntergeladen. Navigieren Sie zu und öffnen Sie es.

   ![](assets/existing-data-excel-parameter-sheet.png)

1. Überprüfen Sie die heruntergeladene Datei und beachten Sie die folgenden Details:

   * Die Datei enthält mehrere Blätter. Möglicherweise müssen Sie die Informationen nicht in jedem Blatt kennen, aber Sie werden einige der Tabellen verwenden, um Ihre Informationen zu importieren. Nehmen Sie sich Zeit, um sich mit ihrem Inhalt und insbesondere mit dem Format des Inhalts in den einzelnen Blättern vertraut zu machen.
   * Achten Sie besonders auf die Spaltennamen und das Format, in dem die Daten in den einzelnen Spalten angezeigt werden.
   * Die Spaltenbezeichnungen und -reihenfolge dürfen in keiner der Tabellen geändert werden. Die Spaltenüberschriften geben die Felder an, die Sie mit Ihren Informationen ausfüllen müssen (in jeder Zeile). Wenn die Spaltenüberschrift fettgedruckt angezeigt wird, ist es ein erforderliches Feld. Daher müssen Informationen in dieser Spalte vorhanden sein.
   >[!IMPORTANT]
   >
   >Einige Spaltenüberschriften werden möglicherweise nicht fettgedruckt angezeigt, sind aber möglicherweise trotzdem erforderlich.

   * Behalten Sie die heruntergeladene Datei für künftige Referenzzwecke bei und fahren Sie mit dem folgenden Abschnitt fort.


## Exportieren der Kick-Start-Vorlage für benutzerdefinierte Daten

Nachdem Sie die Informationen zu vorhandenen benutzerdefinierten Feldern in Ihrem System durchsucht haben, können Sie eine neue Schnellstartvorlage für Ihren Import herunterladen.

1. Klicken **Hauptmenü > Einrichtung** in der oberen rechten Ecke der Workfront-Benutzeroberfläche.

1. Erweitern Sie die **System** Menü links.

1. Klicken **Daten importieren (Kick-Starts)**.

   ![](assets/import-data-kick-starts-link-in-setup.png)

1. Im **Leere Kick-Start-Tabelle herunterladen** Bereich, wählen Sie die **Benutzerdefinierte Daten** Kontrollkästchen und klicken Sie auf **Download**.

   ![](assets/blank-custom-data-option-checked-kick-starts.png)

   Eine leere Schnellstartdatei wird auf Ihren Computer heruntergeladen.

   >[!NOTE]
   >
   >Die Anzahl der Blätter in der Datei, ihre Namen sowie die Anzahl und Namen der Spalten in den einzelnen Blättern sollten mit denen aus dem im obigen Abschnitt heruntergeladenen Kick-Start identisch sein, der Ihre vorhandenen benutzerdefinierten Daten enthielt.

## Füllen der Excel Kick-Start-Tabelle

Laden Sie vor dem Ausfüllen der Excel-Tabelle die Kick-Start-Vorlage wie im obigen Abschnitt beschrieben herunter.

>[!IMPORTANT]
>
>Versuchen Sie nicht, Informationen mithilfe einer Ad-hoc-Excel-Tabelle zu importieren. Alle Tabellen zum Importieren von Informationen in Workfront mithilfe der Schnellstartfunktion müssen mit dem Inhalt der Dateien übereinstimmen, die Sie von Workfront herunterladen und in diesem Artikel beschrieben haben.

So füllen Sie das Excel-Arbeitsblatt mit Informationen für die neuen benutzerdefinierten Felder aus:

1. Öffnen Sie die Excel-Tabelle, die Sie im vorherigen Abschnitt heruntergeladen haben, und beachten Sie eine Reihe von Arbeitsblättern. Jedes Blatt stellt ein Objekt in der Anwendung dar.

   >[!INFO]
   >
   >Beispiel: **Parameter** (bezieht sich auf &quot;Benutzerdefiniertes Feld&quot;), **Parameteroption**(bezieht sich auf die Option &quot;Benutzerdefiniertes Feld&quot;), **Kategorie** (bezieht sich auf &quot;Benutzerdefiniertes Formular&quot;).
   >
   >Sie müssen die Namen der Objekte und deren Attribute in dem von der Workfront-Datenbank unterstützten Format schreiben.
   >
   >Weitere Informationen zur Bedeutung dieser Objekte finden Sie unter [Glossar zu Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
   >
   >Informationen zu den Namen der Objekte in der Workfront-Datenbank finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).
   >
   >![](assets/sheets-included-in-custom-data-export-kick-start-file.png)





1. Stellen Sie sicher, dass die folgenden Informationen korrekt formatiert sind:

   * Die erste Zeile eines jeden Arbeitsblatts muss leer bleiben, da andernfalls beim Import ein Fehler auftritt.
   * Die Spaltenüberschriften in jedem Blatt stellen Attribute der Objekte dar, die während eines Imports festgelegt werden können. Alle Spaltenüberschriften müssen beim Exportieren des Blatts in der gleichen Reihenfolge wie die Spaltenüberschriften bleiben und können nicht umbenannt werden.
   * Die fett gedruckten Spaltenüberschriften sind erforderliche Felder und müssen einen Wert enthalten.

      >[!TIP]
      >
      >Einige Spalten sind erforderlich, sind jedoch nicht fett gedruckt. Beispiel: die `isNew` und `ID` -Spalten sind nicht fett formatiert, aber es handelt sich um erforderliche Felder.

1. Wählen Sie die `**PARAM Parameter`** Blatt und fügen Sie Informationen über die neuen benutzerdefinierten Felder in den folgenden erforderlichen Spalten hinzu:

   * **`isNew`** = enter **`TRUE`** in dieser Spalte für jede Zeile, die ein neues benutzerdefiniertes Feld darstellt. Dies bedeutet, dass das Feld neu ist und nicht in Workfront existiert.

      >[!TIP]
      >
      >    Wenn eine Zeile ein vorhandenes Feld in Workfront darstellt, geben Sie **`isNew`** = **`FALSE`**.

   * **`ID`** = muss eine eindeutige Zahl für jede Zeile sein, die ein neues Feld darstellt. Sie können eine beliebige Zahl verwenden, die mit 1 beginnt, solange jedes neue Feld eine eindeutige Nummer aufweist.
   * **`setDataType`** = für jede Zeile, die ein neues Feld darstellt, geben Sie den Datentyp ein, den das Feld unterstützt. Der Datentyp muss so eingegeben werden, wie er in der Datenbank angezeigt wird. Wählen Sie aus den folgenden Datentypen aus:
      * **`NMBR`** für Zahl
      * **`CURC`** für Währung
      * **`TEXT`** für Text
   * `**setDisplaySize**`= Anzeigegröße (&#39;**setDisplaySize**&#39;) für mehrere Optionen ist benutzerdefinierte Felder immer 0.
   * **`setDisplayType`** = für jede Zeile, die ein neues Feld darstellt, geben Sie den Anzeigetyp des Felds ein. Der Anzeigetyp muss so eingegeben werden, wie er in der Datenbank angezeigt wird.

      Wählen Sie für benutzerdefinierte Felder mit mehreren Optionen aus den folgenden Optionen:

      * **`MULT`** für Dropdown-Liste mit Mehrfachauswahl
      * **`SLCT`** für Dropdown
      * **`RDIO`** für Optionsfelder
      * **`CHCK`** für Kontrollkästchen
      >[!TIP]
      >
      >Informationen zu Datentyp und Anzeigetyp finden Sie im Abschnitt [API-Explorer](../../../wf-api/general/api-explorer.md), erweitern Sie die **Parameter** -Objekt und suchen Sie nach diesen Attributen unter dem **fields** Registerkarte.

   * **`setName`** = geben Sie den Namen der benutzerdefinierten Felder ein, wie er in Workfront angezeigt werden soll.

      >[!INFO]
      >
      >Beispielsweise können wir zwei benutzerdefinierte Felder importieren, die _Marke_, ein Kontrollkästchen und _Medien_, ein Optionsfeld.

   * Die **`setName`** und **`setValue`** -Spalten enthalten in der Regel dieselben Informationen und sollten die Namen widerspiegeln, die in der Workfront-Benutzeroberfläche für Ihr neues Feld gewünscht werden.
   Der Wert eines Felds ist der Name, der beispielsweise in Berichten angezeigt wird, während der Name in den benutzerdefinierten Formularen angezeigt wird, die an Objekte angehängt sind.

   Weitere Informationen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

   ![](assets/parameter-sheet-filled-out-kick-starts.png)

1. Wählen Sie die **`POPT Parameter Options`** und fügen Sie Informationen zu den Optionen der einzelnen benutzerdefinierten Felder in den folgenden erforderlichen Spalten hinzu:

   * **`isNew`** = enter **`TRUE`** in dieser Spalte für jede Zeile, die eine neue Feldoption darstellt.

      >[!TIP]
      >
      >    Wenn eine Zeile eine vorhandene Option darstellt, geben Sie **`isNew`** = **`FALSE`**.

   * **`ID`** = muss eine eindeutige Zahl für jede Zeile sein, die eine neue Option darstellt. Sie können eine beliebige Zahl verwenden, die mit 1 beginnt, solange jede neue Option eine eindeutige Zahl aufweist.
   * **`setIsDefault`** = enter `TRUE` für die Optionen, die standardmäßig angezeigt werden sollen, und `FALSE` für alle anderen Optionen für jedes Feld.  Beispielsweise möchten wir _Nike_ als Standardoption für _Marke_ und _Drucken_ als Standardoption für _Medien_.

      >[!TIP]
      >
      >Für jedes Feld kann nur eine Standardoption verwendet werden.

   * **`setParameterID`** = die Optionen, die dem _Marke_ benutzerdefiniertes Feld enthält eine **`setParameterID`** von 1 und den Optionen, die dem _Medien_ über ein ** verfügen`setParameterID`**von 2. Die `PARAM` und `POPT` Tabellen verweisen einander, um anzugeben, welche Optionen zu welchem benutzerdefinierten Feld gehören.
   * **`setDisplayOrder`**= Die Anzeigereihenfolge -Spalte gibt die Reihenfolge an, in der die Optionen in Ihrem benutzerdefinierten Feld angezeigt werden. Sie können mit 1 beginnen und für alle Optionen in aufsteigender Reihenfolge fortfahren, unabhängig davon, zu welchen Feldern sie gehören. Wichtig ist hier, dass für jede Option eindeutige Zahlen vorliegen.
   * Die **`setLabel`** und `**setValue`** -Spalten enthalten in der Regel dieselben Informationen und sollten die in der Workfront-Benutzeroberfläche gewünschten Namen widerspiegeln. Der Wert einer Option ist der Name, der beispielsweise in Berichten angezeigt wird, während der Titel in den benutzerdefinierten Formularen angezeigt wird, wenn er an ein Objekt angehängt wird. Weitere Informationen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
   * **`setIsHidden`** = enter `TRUE` , wenn eine der Optionen ausgeblendet werden soll.
   ![](assets/parameter-option-sheet-filled-out-kick-starts.png)


1. (Optional) Wenn Sie auch ein benutzerdefiniertes Formular erstellen möchten, in das Sie die neuen Felder später einfügen können, wählen Sie die  **`CTGY Category`** und aktualisieren Sie die folgenden erforderlichen Spalten für die benutzerdefinierten Formulardaten:

   * **`isNew`** = enter **`TRUE`** in dieser Spalte für jede Zeile, die ein neues benutzerdefiniertes Formular darstellt.
   * **`ID`** = geben Sie für jede Zeile, die ein neues Formular darstellt, eine eindeutige Nummer ein. Sie können eine beliebige Zahl verwenden, die mit 1 beginnt, solange jede neue Option oder Zeile eine eindeutige Zahl aufweist.
   * **`setGroupID`** = Fügen Sie die Gruppen-ID für Ihre Home Group oder eine andere Gruppe im System hinzu, deren Mitglieder Zugriff auf dieses Formular erhalten sollen. Dies ist ein Pflichtfeld.
   So finden Sie heraus: `ID` einer Gruppe können Sie entweder einen Gruppenbericht erstellen und die `ID` in der Ansicht oder navigieren Sie zu einer Gruppe und suchen Sie nach der URL für die Gruppe. Die Gruppen-ID befindet sich in der URL der Seite der Gruppe. Wenn beispielsweise die URL der Gruppe `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members`, lautet die Gruppen-ID . `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode` **= dies ist der Objektcode für den Objekttyp, für den das Formular erstellt werden soll. Geben Sie einen Code aus den folgenden Optionen ein:
      * **`CMPY`** für Unternehmen
      * **`TASK`** für Aufgabe
      * **`PROJ`** für Projekt
      * **`PORT`** für Portfolio
      * **`PRGM`** für das Programm
      * **`USER`** für Benutzer
      * **`DOCU`** für Dokument
      * **`OPTASK`** für Problem
      * **`EXPNS`** für Ausgaben
      * **`ITRN`** zur Iteration
      * **`BILL`** für Rechnungsdatensätze
      * **`GROUP`** für Gruppe
      >[!NOTE]
      >
      >Geben Sie bei Formularen mit mehreren Objekten das erste Objekt ein, das Sie beim Erstellen eines Formulars in der Benutzeroberfläche auswählen würden. Legen Sie beispielsweise die `setCatObjCode` nach `TASK`, wenn Sie &quot;Aufgabe&quot;in der Workfront-Benutzeroberfläche und dann &quot;Problem&quot;, &quot;Portfolio&quot;usw. auswählen, das Formular aber nicht für Projekte verfügbar sein soll.

   * **`setName`** = dies ist der Name des benutzerdefinierten Formulars, wie er in der Workfront-Benutzeroberfläche angezeigt werden soll.

      ![](assets/category-sheet-filled-out-kick-starts.png)



1. Speichern Sie die Tabelle als .xls- oder .xlsx-Datei auf Ihrem Computer. Ihre Excel-Tabelle ist ausgefüllt und kann jetzt in Workfront importiert werden.


## Hochladen der Excel-Tabelle in Workfront

Nachdem Sie die in den vorherigen Abschnitten beschriebenen Schritte ausgeführt haben, fahren Sie mit den folgenden Schritten fort, um die neuen Felder und Formulare in Workfront hochzuladen:

1. Klicken **Daten importieren** **(Kick-Starts) **unter dem **Hauptmenü > Setup > System** Menü.

1. Klicken **Datei auswählen** unter dem Abschnitt **Hochladen von Daten mit der Kick-Start-Tabelle**.

1. Suchen Sie auf Ihrem Computer nach der von Ihnen vorbereiteten Excel-Tabelle und wählen Sie sie aus, wenn Sie sie finden.  Wenn die Datei von Workfront erkannt wird, wird die Schaltfläche Hochladen blau.
1. Klicken **Hochladen.**

   ![](assets/kick-start-file-selected-and-upload-blue-button.png)

1. Es wird eine Benachrichtigung angezeigt, dass der Import erfolgreich war. Je nachdem, wie viele Informationen Sie importieren, kann dieser Schritt einige Sekunden bis zu einer Minute dauern.

   ![](assets/kick-start-successful.png)

   Die neuen benutzerdefinierten Felder und Formulare befinden sich jetzt in Ihrem Workfront-System. Sie finden sie im Bereich Benutzerdefinierte Forms der Einrichtung.

   >[!NOTE]
   >
   >Die neuen Formulare und die importierten Felder sind noch nicht verknüpft. Das Formular wird ohne benutzerdefinierte Felder importiert. Sie müssen die Felder manuell zum neuen benutzerdefinierten Formular oder zu einem anderen vorhandenen benutzerdefinierten Formular hinzufügen.


   Informationen zum Hinzufügen von Feldern zu benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. (Bedingt) Wenn der Import nicht erfolgreich war, erhalten Sie eine Fehlermeldung mit dem Problem. Versuchen Sie, das Feld, das Blatt und die Zeilennummer, in der das Problem aufgetreten ist, zu identifizieren und die Informationen in der Excel-Datei zu korrigieren. Versuchen Sie dann erneut, die Datei zu importieren.

   ![](assets/kick-start-error.png)

1. (Bedingt) Je nachdem, was das Problem ist, wie in der Fehlermeldung angegeben, können einige Informationen bereits importiert werden. Führen Sie einen der folgenden Schritte aus, bevor Sie das Blatt erneut importieren können:

   * Löschen Sie die Informationen, die erfolgreich aus Workfront importiert wurden, aus dem Bereich &quot;Benutzerdefinierte Forms&quot;, und führen Sie dann die von der Fehlermeldung angegebene Korrektur durch.
   * Geben Sie an, dass ein Feld oder Formular bereits im System für die bereits importierten Felder oder Formulare enthalten ist, und korrigieren Sie dann die Datei.
Um anzugeben, dass sich ein Feld oder ein benutzerdefiniertes Formular bereits in Workfront befindet, müssen Sie sicherstellen, dass die Variable `inNew` als `FALSE` in Tabellen mit Informationen zum Formular (`CTGY`) oder dem Feld (`PARAM`) auf dem Kick-Start-Importblatt.
