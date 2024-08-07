---
title: Erstellen eines Formelfelds in der Berichtsarbeitsfläche
description: Erstellen eines Formelfelds in der Berichtsarbeitsfläche
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---

# Erstellen eines Formelfelds in der Berichtsarbeitsfläche

Mit dem Feld-Builder auf der Arbeitsfläche für die Berichterstellung können Sie Felder erstellen, die benutzerdefinierte Berechnungen durchführen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Arbeitsfläche für die Berichterstellung Beta: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Erstellen eines Formelfelds

1. Erstellen oder navigieren Sie zu einem Tabellenblock, wie in [Hinzufügen oder Bearbeiten eines Tabellenblocks auf der Berichtsarbeitsfläche](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md) beschrieben.
1. Klicken Sie in der Tabellenüberschrift im Bericht auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Wenn Sie die Tabelle gerade erstellt haben und noch keine Felder hinzugefügt haben, klicken Sie stattdessen in der Tabellenmitte auf die Schaltfläche Bearbeiten .

1. Klicken Sie oben in der Liste **Felder** im rechten Bereich auf **Neu +** .
1. Klicken Sie in der sich öffnenden neuen Seite auf das Symbol **Bearbeiten** neben dem Feldnamen in der oberen linken Ecke, um den Namen des Formelfelds zu ändern.![](assets/edit-icon.png)
1. Ziehen Sie **Funktionen** oder **Felder** aus dem linken Bereich in den Feld-Builder in der Mitte, um sie Ihrem Formelfeld hinzuzufügen.


   >[!TIP]
   >
   >Während Sie Ihr Formelfeld erstellen, zeigt die Vorschau **Feld** rechts Beispiele für das resultierende Feld an.

   Jede Funktion enthält eine Anzahl leerer gepunkteter Rechtecke, die als Argumente für die Berechnung eines Ergebnisses verwendet werden. Diese können durch Eingabe von statischem Text oder statischen Zahlen, Ziehen und Ablegen eines Felds aus dem linken Bereich (unter Verwendung des Feldwerts in der Berechnung) oder durch Ziehen und Ablegen einer anderen Funktion (unter Erstellung einer verschachtelten Funktion) aufgefüllt werden. Mögliche Funktionen sind:

   | Funktion | Beschreibung | Ausgabe |
   |---|---|---|
   | IF | Vergleichen Sie zwei Argumente basierend auf einem ausgewählten Modifikator und führen Sie dann eine bestimmte Aktion basierend auf dem resultierenden Wert True (Is True:) oder False (Is False:) aus. Hinweis: Derzeit kann das zweite Argument kein statischer True- oder False-Wert sein. Stattdessen können Sie eine verschachtelte Funktion wie ISBLANK (Projektname) verwenden, die immer False als Problemumgehung zurückgibt. | True/False, Datum, Zahl oder Zeichenfolge |
   | ZUSAMMENFÜGEN | Führen Sie zwei oder mehr Zeichenfolgen von Anfang bis Ende zusammen, um eine neue Zeichenfolge zu erstellen. | Zeichenfolge |
   | CONTAINS | Überprüfen Sie, ob ein Feld für ein Zeichenfolgenargument (Suchtext) in einem anderen Feld für ein Zeichenfolgenargument (In-Text) enthalten ist. | Wahr/Falsch |
   | IN | Überprüfen Sie, ob der Wert eines Argumentfelds (Find) mit dem Wert mindestens eines anderen Argumentfelds (Within) übereinstimmt. | Wahr/Falsch |
   | ISBLANK | Überprüfen Sie, ob ein Argumentfeld leer ist. | Wahr/Falsch |
   | LEN | Messen Sie die Länge (in Zeichenanzahl) eines Argumentfelds. | Zahl |
   | ROUND | Gibt eine gerundete Zahl basierend auf der ausgewählten Genauigkeit zurück. | Zahl |
   | FLOOR | Gibt die nächste Ganzzahl zurück, abgerundet. | Zahl |
   | ZAHL | Gibt den größten Zeilenumbruch zurück, der kleiner als der Wert eines numerischen Arguments ist (identisch mit einer Floor-Funktion). | Zahl |
   | ZEICHENFOLGE | Konvertiert den Inhalt eines Argumentfelds in einen String | Zeichenfolge |
   | SUBSTR | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die die Zeichen zwischen einer Indexnummer (Start) und einer anderen (Ende) enthält. | Zeichenfolge |
   | LINKS | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die Zeichen enthält, die mit ganz links beginnen und eine Reihe von Zeichen (Länge) rechts zählen. | Zeichenfolge |
   | RECHTS | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die Zeichen enthält, die mit dem ganz rechts beginnenden Zeichen beginnen und eine Anzahl von Zeichen links zählen (Länge). | Zeichenfolge |
   | SUM | Fügen Sie die Werte von zwei oder mehr Argumentfeldern zusammen. | Zahl |
   | SUB | Ziehen Sie die Werte von zwei oder mehr Argumentfeldern ab (in der Reihenfolge von links nach rechts). | Zahl |
   | PROD | Multipliziert die Werte von zwei oder mehr Argumentfeldern. | Zahl |
   | DIV | Teilen Sie den Wert von zwei oder mehr Argumentfeldern (in der Reihenfolge von links nach rechts). | Zahl |
   | MONAT | Gibt eine Zahl zurück, die dem Monatswert eines Datums entspricht. | Zahl |
   | JAHR | Gibt eine Zahl zurück, die dem Wert des Jahres für ein Datum entspricht. | Zahl |
   | DATEDIFF | Berechnet die Gesamtanzahl von Tagen zwischen zwei Daten, auf eine Dezimalstelle gerundet. | Zahl |
   | WEEKDAYDIFF | Berechnet die Anzahl der Wochentage zwischen zwei Daten, auf eine Dezimalstelle gerundet. | Zahl |

   {style="table-layout:auto"}

1. Klicken Sie in der oberen linken Ecke des Bildschirms auf den Pfeil **Zurück** , um zu Ihrer Tabelle zurückzukehren.
