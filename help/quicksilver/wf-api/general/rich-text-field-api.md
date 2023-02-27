---
content-type: api
navigation-topic: general-api
title: Rich-Text-Felder in der Adobe Workfront-API
description: Rich-Text-Felder in der Adobe Workfront-API
author: Becky
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Rich-Text-Felder in der Adobe Workfront-API

Einige Objekte in Adobe Workfront ermöglichen die Speicherung von Text mit Rich-Text-Formatierung. In der Workfront-API wird Rich Text mithilfe des Open-Source-Frameworks Draft.js als JSON gespeichert.

## Übersichtsbeispiel

Ein benutzerdefiniertes Feld mit Rich-Text-Formatierung wird als **Feld mit Rich-Text** und können die folgenden Werte zugeordnet sein:

![](assets/rich-text-example-350x158.png)

**Beispiel:** Eine einfache GET-Anfrage zum Abrufen des Werts des benutzerdefinierten Formularfelds. **Feld mit Rich-Text**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Beispiel:** Diese Anfrage gibt den Wert von **Feld mit Rich-Text** in JSON gespeichert im **parameterValue** **DE:Feld mit Rich-Text**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Beispiel:** Dies ist eine formatierte Version der Antwort, die direkt oben in der Abbildung dargestellt wird.

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Blöcke

Die JSON-Objekte, die den Rich-Text-Inhalt speichern, bestehen aus zwei Hauptteilen: **Bausteine** und **entityMaps**.

Ein Block ist ein JSON-Objekt, das eine einzelne Zeile formatierten Texts darstellt. Da ein einzelnes benutzerdefiniertes Feld mehrere Textzeilen haben kann, hat jede Textzeile einen eigenen Block und jeder Block wird als Element in einem übergeordneten Array namens dargestellt **Bausteine**.

**Beispiel:** Hier wird jede Textzeile aus einem benutzerdefinierten Feld einem Blockelement in den Array-Blöcken zugeordnet

![](assets/copy-of-rich-text-mapping-350x159.png)

Da jedes Blockelement auch ein JSON-Objekt ist, besteht jeder Block aus folgenden Elementen: **key**, **text**, **type**, **depth**, **inlineStyleRanges**, **entityRanges** und **data**. Jedes dieser Elemente funktioniert wie folgt:

* **Schlüssel** ist die eindeutige Kennung für diesen Block. Der Schlüssel wird verwendet, um eine Textzeile über entityMaps zuzuordnen. Details zu entityMaps finden Sie im Abschnitt entityMaps dieses Dokuments.
* **Text** ist die Textinhaltszeile, die aus dem benutzerdefinierten Feld gespeichert wird.
* **Typ** beschreibt den Typ des Textes, der dargestellt wird. Eine Textzeile, die beispielsweise in einem Block gespeichert wird, kann Teil einer Liste sein. Wenn diese Textzeile Teil einer ungeordneten Liste ist, wird ihr Typ wie folgt definiert: unordered-list-item.
* Listen werden derzeit nicht unterstützt, sollten aber in Kürze verfügbar sein.
* **Tiefe** Dieser Parameter definiert die Tiefe der Zeile, wenn die Zeile ein verschachtelter Teil einer geordneten oder ungeordneten Liste ist.
* **inlineStyleRanges** ist ein Array, das die Formatierungstypen beschreibt, die auf die Textzeile angewendet wurden, die durch den aktuellen Block dargestellt werden.

**Beispiel:** Im Folgenden finden Sie ein inlineStyleRanges -Array, das jeden Stil auf Zeichenebene beschreibt. In diesem Fall: 9 Zeichen (Länge: 9) ab Index 0 (Versatz: 0) hatte den Stil **Fett** angewendet:

![](assets/copy-of-rich-text-mapping-2-350x136.png)

Wenn mehrere Formatierungstypen auf eine einzelne Zeile angewendet wurden, werden Stile zusätzlichen Elementen im Array** inlineStyleRanges** zugeordnet.

**Beispiel:** So würde ein Block beim Speichern einer Textzeile aussehen, die die gemischte Formatierung enthält: **Fettdruck und kursiv**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Alle Versionen nach Version 20.3 unterstützen Formatierungsoptionen für Fettdruck, Kursiv und Unterstrichen.

## entityMaps und entityRanges

Ein Datenblock kann potenziell Entitäten wie Hyperlinks oder andere Arten von stilisierter Formatierung enthalten, die mit Datenquellen verbunden sind, die sich außerhalb des benutzerdefinierten Textfelds befinden.

## Beispiele

### Abrufen von normalem Text aus JSON

Wenn ein benutzerdefiniertes Feld mit Rich-Text-Formatierung gesendet wird, wird der gesamte Text im Array gespeichert **Bausteine**. Jede Zeile des Volltextes wird jedoch im **Textparameter** innerhalb der einzelnen Blockelemente, aus denen das übergeordnete Array besteht **Bausteine**. Um den Volltext abzurufen, muss also jede separate Textzeile extrahiert und wieder geparst werden. Dies kann erreicht werden, indem alle Elemente in Blöcken in Schleife gehalten und jeder Textparameter miteinander verkettet wird, wobei ein Zeilentrennzeichen (\n) verwendet wird.

**Beispiel:** So könnte Ihr JS aussehen:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Speichern eines Rich-Text-Feldwerts mit der Workfront-API

So speichern Sie die folgenden Werte eines Rich-Text-Felds mithilfe der Workfront-API:
<pre>
		Hallo <strong>Welt</strong>!!
		Das ist meine erste <strong>Rich-Text</strong></pre>

1. Erstellen Sie eine JSON-Datei, die den Wert des Rich-Text-Felds darstellt, das Sie erfassen möchten, indem Sie jede Textzeile in einem Block-Element im Array organisieren. **Bausteine**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Erfassen Sie die Rich-Text-Formatierung mit dem **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Um die zweite Zeile zu erfassen, muss der Text &quot;Rich Text&quot;fett und kursiv formatiert sein.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >Die entityMap-Funktion wird zwar während der ersten Veröffentlichung nicht unterstützt, es ist jedoch dennoch ein erforderliches Feld, um diese JSON in einer Anfrage zu übergeben

1. Verwenden Sie die **stringify** -Methode für die oben beschriebene JSON verwenden, um eine **PUT** Anfordern und Senden von Updates

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
