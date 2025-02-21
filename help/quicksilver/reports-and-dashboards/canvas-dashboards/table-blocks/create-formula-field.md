---
title: Erstellen eines Formelfelds auf der Reporting-Arbeitsfläche
description: Erstellen eines Formelfelds auf der Reporting-Arbeitsfläche
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 7%

---

# Erstellen eines Formelfelds auf der Reporting-Arbeitsfläche

Mit dem Feld-Builder auf der Reporting-Arbeitsfläche können Sie Felder erstellen, die benutzerdefinierte Berechnungen durchführen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich für die Betaversion der Reporting-Arbeitsfläche registrieren. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Betaversion: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Erstellen eines Formelfelds

1. Erstellen Sie einen Tabellenblock oder navigieren Sie zu diesem, wie in [Hinzufügen oder Bearbeiten eines Tabellenblocks auf der Reporting-Arbeitsfläche](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md) beschrieben.
1. Klicken Sie in der Tabellenkopfzeile im Bericht auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).

   ![Bearbeitungssymbol in der Tabellenkopfzeile](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Wenn Sie die Tabelle gerade erstellt und noch keine Felder hinzugefügt haben, klicken Sie stattdessen auf die Schaltfläche Bearbeiten in der Mitte der Tabelle.

1. Klicken Sie **Neu +** oben in der Liste **Felder** im rechten Bedienfeld.
1. Klicken Sie auf der neu geöffneten Seite **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png) neben dem Feldnamen oben links, um den Namen des Formelfelds zu ändern.
1. Ziehen Sie **Funktionen** oder **Felder** aus dem linken Bereich auf den Feld-Builder in der Mitte, um sie zu Ihrem Formelfeld hinzuzufügen.


   >[!TIP]
   >
   >Beim Erstellen des Formelfelds zeigt die **Feldvorschau** auf der rechten Seite Beispiele für das resultierende Feld an.

   Jede Funktion enthält eine Reihe leerer gepunkteter Rechtecke, die als Argumente bei der Berechnung eines Ergebnisses verwendet werden. Diese können durch Eingabe von statischem Text oder von Zahlen, Ziehen und Ablegen eines Felds aus dem linken Bereich (unter Verwendung des Feldwerts in der Berechnung) oder durch Ziehen und Ablegen einer anderen Funktion (Erstellen einer verschachtelten Funktion) gefüllt werden. Mögliche Funktionen sind:

   | Funktion | Beschreibung | Ausgabe |
   |---|---|---|
   | IF | Vergleichen Sie zwei Argumente basierend auf einem ausgewählten Modifikator und führen Sie dann eine bestimmte Aktion basierend auf dem resultierenden Wert True (Ist wahr:) oder False (Ist falsch:) aus. Hinweis: Derzeit kann das zweite Argument kein statischer Wert vom Typ „True“ oder „False“ sein. Stattdessen können Sie eine verschachtelte Funktion wie ISBLANK (Projektname) verwenden, die als Problemumgehung immer „false“ zurückgibt. | true/false, Datum, Zahl oder Zeichenfolge |
   | ZUSAMMENFÜGEN | Zusammenführen von zwei oder mehr Zeichenfolgen End-to-End, um eine neue Zeichenfolge zu erstellen. | Zeichenfolge |
   | CONTAINS | Auswerten, ob ein Zeichenfolgenargumentfeld (Suchtext) in einem anderen Zeichenfolgenargumentfeld (im Text) enthalten ist. | Wahr/Falsch |
   | IN | Auswerten, ob der Wert eines Argumentfelds (Suchen) mit dem Wert von mindestens einem anderen Argumentfeld (Innerhalb) übereinstimmt | Wahr/Falsch |
   | ISBLANK | Auswerten, ob ein Argumentfeld leer ist. | Wahr/Falsch |
   | LEN | Messen Sie die Länge (in Zeichenanzahl) eines Argumentfelds. | Zahl |
   | ROUND | Gibt eine gerundete Zahl basierend auf der ausgewählten Genauigkeit zurück. | Zahl |
   | FLOOR | Gibt die nächste ganze Zahl zurück, abgerundet. | Zahl |
   | ZAHL | Gibt die größte Ganzzahl zurück, die kleiner ist als der Wert eines numerischen Arguments (identisch mit einer Floor-Funktion). | Zahl |
   | ZEICHENFOLGE | Konvertiert den Inhalt eines Argumentfelds in eine Zeichenfolge. | Zeichenfolge |
   | SUBSTR | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die die Zeichen zwischen einer Indexnummer (Start) und einer anderen (Ende) enthält. | Zeichenfolge |
   | LINKS | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die Zeichen enthält, die mit dem Zeichen beginnen, das am weitesten links beginnt und nach rechts eine bestimmte Anzahl von Zeichen zählt (Länge). | Zeichenfolge |
   | RECHTS | Erstellen Sie eine neue Zeichenfolge aus einer größeren Zeichenfolge, die Zeichen enthält, die mit dem Zeichen beginnen, das am weitesten rechts beginnt, und eine Anzahl von Zeichen links zählt (Länge). | Zeichenfolge |
   | SUM | Fügen Sie die Werte von zwei oder mehr Argumentfeldern hinzu. | Zahl |
   | SUB | Subtrahieren Sie die Werte von zwei oder mehr Argumentfeldern (in der Reihenfolge von links nach rechts). | Zahl |
   | PROD | Multiplizieren Sie die Werte von zwei oder mehr Argumentfeldern. | Zahl |
   | DIV | Dividieren Sie den Wert von zwei oder mehr Argumentfeldern (in der Reihenfolge von links nach rechts). | Zahl |
   | MONAT | Gibt eine Zahl zurück, die dem Monatswert für ein Datum entspricht. | Zahl |
   | JAHR | Gibt eine Zahl zurück, die dem Jahreswert für ein Datum entspricht. | Zahl |
   | DATEDIFF | Berechnet die Gesamtzahl von Tagen zwischen zwei Datumsangaben, gerundet auf eine Dezimalstelle. | Zahl |
   | WEEKDAYDIFF | Berechnet die Anzahl der Wochentage zwischen zwei Datumsangaben, gerundet auf eine Dezimalstelle. | Zahl |

   {style="table-layout:auto"}

1. Klicken Sie auf **Pfeil „Zurück** in der oberen linken Ecke des Bildschirms, um zu Ihrer Tabelle zurückzukehren.
