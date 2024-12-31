---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Modultypen
description: 'Adobe Workfront Fusion unterscheidet fünf Modultypen: Aktionsmodule, Suchmodule, Trigger-Module, Aggregatoren und Iteratoren. Aggregatoren und Iteratoren sind für fortgeschrittene Szenarien geeignet.'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 0%

---

# Modultypen

In [!UICONTROL Adobe Workfront Fusion] werden fünf Modultypen unterschieden: Aktionsmodule, Suchmodule, Trigger-Module, Aggregatoren und Iteratoren. Aggregatoren und Iteratoren sind für fortgeschrittene Szenarien geeignet.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss Adobe Workfront Fusion sowie Adobe Workfront erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Aktionsmodule

Aktionsmodule sind der häufigste Modultyp. Ein typisches Aktionsmodul gibt ein einzelnes Bundle zurück, das dann zur Verarbeitung an das nächste Modul weitergegeben wird.

Im Gegensatz zu Trigger-Modulen können Aktionsmodule am Anfang, in der Mitte oder am Ende eines Szenarios platziert werden. Szenarien können eine unbegrenzte Anzahl von Aktionsmodulen enthalten.

>[!INFO]
>
>**Beispiele:**
>
>* **[!DNL Workfront]> [!UICONTROL Datei hochladen]** sendet eine Datei an [!DNL Workfront] und gibt deren Kennung zurück.
>* **[!UICONTROL Bild] > [!UICONTROL Größe ändern]** empfängt ein Bild, ändert es in die angegebenen Abmessungen und übergibt das skalierte Bild an die nächste Aktion.

Der Aktionstyp weist vier Untertypen auf: Erstellen, Lesen, Aktualisieren und Löschen. Der Untertyp Aktualisieren ermöglicht die folgenden drei Vorgänge:

* **Inhalt eines Felds löschen**. Dieser Vorgang findet statt, wenn der Inhalt des Felds als Keyword zum Löschen ausgewertet wird (nicht zu verwechseln mit *leer*).

  ![](assets/erase-content-of-field.png)

* **Lassen Sie den Inhalt eines Felds**. Dieser Vorgang findet statt, wenn das Feld leer gelassen wird oder der Inhalt des Felds als leer ausgewertet wird (in JSON durch null dargestellt).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Ersetzen Sie den Inhalt eines Felds**. Dieser Vorgang findet in allen anderen als den beiden oben beschriebenen Fällen statt.

>[!NOTE]
>
>* Wenn das Keyword `erase` im Zuordnungsbereich nicht angezeigt wird, ist das Modul kein Aktualisierungsmodul oder es wurde nicht auf die neuesten Spezifikationen für die App aktualisiert.
>* &quot;[!UICONTROL Empty]&quot; ändert den Feldinhalt nicht. Wenn das Feld gelöscht werden muss, können Sie die folgende Formel verwenden:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Ein Feld unverändert zu lassen, wenn sein Inhalt als leer ausgewertet wird, ist derzeit nicht möglich.

## Suchmodule

Eine typische Suche gibt null, ein oder mehrere Bundles zurück, die dann zur Verarbeitung an das nächste Modul weitergegeben werden.

Sie können Suchen am Anfang, in der Mitte oder am Ende eines Szenarios platzieren.

Szenarien können eine unbegrenzte Anzahl von Suchvorgängen enthalten.

>[!INFO]
>
>**Beispiel:**
>
>**[!DNL Workfront]> [!UICONTROL Verwandte Datensätze lesen]** liest Datensätze, die in einem bestimmten übergeordneten Objekt der angegebenen Suchabfrage entsprechen

## Trigger-Module

Trigger generieren Pakete, wenn eine Änderung an einem bestimmten Service stattgefunden hat. Bei der Änderung kann es sich um die Erstellung neuer Datensätze, das Löschen von Datensätzen, die Aktualisierung von Datensätzen usw. handeln.

Jeder Trigger kann null, ein oder mehrere Bundles zurückgeben, die dann zur Verarbeitung an das nächste Modul weitergegeben werden.

Trigger können nur am Anfang eines Szenarios platziert werden.

Jedes Szenario kann nur einen Trigger enthalten.

[!DNL Workfront Fusion] unterscheidet zwei Typen von Triggern: Abfrage von Triggern und Sofort-Trigger.

### Trigger werden abgerufen

Trigger fragen regelmäßig einen bestimmten Dienst ab, auch wenn seit der vorherigen Ausführung keine Änderung vorgenommen wurde. Es wird empfohlen, ein Szenario mit einem Abrufintervall so zu planen, dass es in regelmäßigen Triggern ausgeführt wird. Bei einer *Änderung* gibt der Trigger Bundles mit Informationen über die Änderung zurück. Wenn keine *Änderung* erfolgt, gibt der Trigger keine Pakete aus. Anweisungen zum Planen eines Szenarios finden Sie unter [Planen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Mit Abfrage-Triggern können Sie das erste Bundle auswählen, das über das Epochenbedienfeld ausgegeben werden soll. Das Bedienfeld wird automatisch angezeigt, nachdem Sie einen Trigger gespeichert oder die Trigger-Einstellungen geändert haben. Weitere Informationen finden Sie unter [Auswählen, wo ein Trigger-Modul in [!UICONTROL Adobe Workfront Fusion beginnt]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Die im Epochenbedienfeld vorgenommenen Einstellungen wirken sich nur auf die erste Ausführung des Moduls aus. Sobald das Modul ausgeführt wird, speichert es das zuletzt ausgegebene Bundle und löscht die über das Epochenbedienfeld vorgenommenen Einstellungen.

>[!INFO]
>
>**Beispiele:**
>
>* **[!DNL Workfront]> [!UICONTROL Datensätze beobachten]** gibt Dateien zurück, die seit der letzten Ausführung des Szenarios neu hinzugefügt wurden
>
>* **[!DNL Google Sheets]> [!UICONTROL Zeilen beobachten]** gibt neue Zeilen zurück, die vom Benutzer seit der letzten Ausführung des Szenarios hinzugefügt wurden

### Sofortige Trigger

Sofortige Trigger ermöglichen es dem Service, [!DNL Workfront Fusion] sofort über eine *Änderung* zu informieren. Es wird empfohlen, ein Szenario mit einem sofortigen Trigger zu planen, der sofort ausgeführt werden soll. Anweisungen finden Sie unter [Planen eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Siehe auch [Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) für Details zur Verarbeitung der eingehenden Daten.

>[!INFO]
>
>**Beispiele:**
>
>* **[!DNL Workfront]> [!UICONTROL Ereignisse beobachten]** gibt Informationen zurück, wenn ein bestimmter Ereignistyp in Workfront auftritt, z. B. bei der Erstellung einer Aufgabe.
>* **[!DNL Google Sheets]> [!UICONTROL Änderungen beobachten]** gibt Informationen zurück, sobald eine Zelle aktualisiert wird.

## Aggregatoren

Ein Aggregator ist ein Modultyp, der mehrere Bundles in einem Bundle sammelt.

Jeder Aggregator gibt nur ein Bundle zurück, das dann zur weiteren Verarbeitung an das nächste Modul übergeben wird.

Aggregatoren können nur in der Mitte eines Szenarios platziert werden.

Szenarien können eine unbegrenzte Anzahl von Aggregatoren enthalten.

>[!INFO]
>
>**Beispiele:**
>
>* **[!UICONTROL Archivieren] > [!UICONTROL Archiv erstellen]** Komprimiert empfangene Dateien in ein ZIP-Archiv
>* **[!UICONTROL CSV] > [!UICONTROL In CSV aggregieren]** führt mehrere Zeichenfolgen aus einer CSV-Datei in einer Zeile zusammen
>* **[!UICONTROL Tools] > [!UICONTROL Text-Aggregator]** kombiniert mehrere Zeichenfolgen zu einer einzigen Zeichenfolge

Weitere Informationen finden Sie unter [Aggregator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteratoren

Ein Iterator ist ein Modultyp, der Arrays in mehrere separate Bundles aufteilt.

Jeder Iterator gibt ein oder mehrere Bundles zurück, die dann zur Verarbeitung an das nächste Modul weitergegeben werden.

Iteratoren können nur in der Mitte eines Szenarios platziert werden.

Szenarien können eine unbegrenzte Anzahl von Iteratoren enthalten.

>[!INFO]
>
>**Beispiel:**
>
>**[!UICONTROL E] > [!UICONTROL Anhänge abrufen]** teilt ein Array von Anhängen in separate Bundles auf

Weitere Informationen finden Sie unter [Iterator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) und [Zuordnen eines Arrays in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
