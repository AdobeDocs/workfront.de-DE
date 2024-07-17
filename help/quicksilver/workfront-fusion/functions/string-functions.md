---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Zeichenfolgenfunktionen in Adobe Workfront Fusion
description: Die folgenden Zeichenfolgen-Funktionen sind im Zuordnungsbereich für Adobe Workfront Fusion verfügbar.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0b286e43ed77669329fbee25618394ee5641e428
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Zeichenfolgen-Funktionen in [!DNL Adobe Workfront Fusion]

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Alle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p> 
   <p>Oder</p> 
   <p>Veraltet: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL length (text oder buffer)]

Gibt die Länge der Textzeichenfolge (Anzahl der Zeichen) oder des Binärpuffers (Puffergröße in Byte) zurück.

>[!INFO]
>
>**Beispiel:**
>
>`length( hello )`
>
>Gibt Folgendes zurück: 5

## [!UICONTROL lower (text)]

Konvertiert alle Buchstaben eines Textzeichenders in Kleinbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`lower( Hello )`
>
>Gibt Folgendes zurück: hello

## [!UICONTROL großschreiben (text)]

Konvertiert das erste Zeichen in einer Textzeichenfolge in Großbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`capitalize( workfront )`
>
>Gibt Folgendes zurück: [!DNL Workfront]

## [!UICONTROL startcase (text)]

Großschreibung des ersten Buchstabens jedes Wortes und Kleinschreibung aller anderen Buchstaben.

>[!INFO]
>
>**Beispiel:**
>`startcase( hello WORLD )`
>
>Gibt Folgendes zurück: [!UICONTROL Hello World]

## [!UICONTROL ascii (text; [diakritics entfernen])]

Entfernt alle nichtascii-Zeichen aus einer Textzeichenfolge.

>[!INFO]
>
>**Beispiele:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   Gibt Folgendes zurück: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   Gibt Folgendes zurück: [!UICONTROL escrz]



## [!UICONTROL replace (text;search string; replacement string)]

Ersetzt die Suchzeichenfolge durch die neue Zeichenfolge.

>[!INFO]
>
>**Beispiel:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Gibt Folgendes zurück: [!UICONTROL Hi World]

Reguläre Ausdrücke (in `/.../` eingeschlossen) können als Suchzeichenfolge mit einer Kombination von Flags (wie `g`, `i`, `m`) verwendet werden:

>[!INFO]
>
>**Beispiel:**
>
>![](assets/replace---1-350x31.png)
>
>Alle diese Zahlen X X X X X werden durch X ersetzt

Die Ersatzzeichenfolge kann die folgenden speziellen Ersatzmuster enthalten:

* `$&` Fügt die übereinstimmende Unterzeichenfolge ein.
* `$n` Wenn n eine positive Ganzzahl kleiner als 100 ist, wird die n. in Klammern eingeschlossene Unterübereinstimmungszeichenfolge eingefügt. Dies ist 1-indiziert.

>[!INFO]
>
>**Beispiele:**
>
>![](assets/variable-value-350x63.png)
>
>Gibt Folgendes zurück: Telefonnummer `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Gibt Folgendes zurück: Telefonnummer: `+420777111222`

>[!CAUTION]
>
>Verwenden Sie keine benannten Erfassungsgruppen wie `/ is (?<number>\d+)/` im Ersetzungszeichenfolgenargument. Dies führt zu einem Fehler.

Weitere Informationen zu regulären Ausdrücken finden Sie unter [Text-Parser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL trim (text)]

Entfernt Leerzeichen am Anfang oder Ende des Textes.

## [!UICONTROL upper (text)]

Konvertiert alle Buchstaben einer Textzeichenfolge in Großbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`upper( Hello )`
>
>Gibt Folgendes zurück: [!UICONTROL HELLO]

## [!UICONTROL substring (text; start; end)]

Gibt einen Teil einer Textzeichenfolge zwischen der Position &quot;Start&quot;und der Position &quot;Ende&quot;zurück.

>[!INFO]
>
>**Beispiele:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Gibt Folgendes zurück: Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Gibt Folgendes zurück: el

## [!DNL indexOf (string; value; [start])]

Gibt die Position des ersten Vorkommens eines angegebenen Werts in einer Zeichenfolge zurück. Diese Methode gibt &quot;-1&quot;zurück, wenn der gesuchte Wert nicht vorhanden ist. Der Startwert gibt an, wo in der Zeichenfolge die Suche beginnen soll.

>[!INFO]
>
>**Beispiele:**
>
>* `indexOf( Workfront ; o )`
>
>   Gibt Folgendes zurück: 1
>
>* `indexOf( Workfront ; x )`
>
>   Gibt Folgendes zurück: -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   Gibt Folgendes zurück: 6

## [!UICONTROL toBinary (value)]

Konvertiert jeden Wert in Binärdaten.

Sie können auch die Kodierung als zweites Argument angeben, um binäre Konversionen von Hex oder base64 auf Binärdaten anzuwenden.

>[!INFO]
>
>**Beispiele:**
>
>* `toBinary( Workfront )`
>
>   Gibt Folgendes zurück: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Gibt Folgendes zurück: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (value)]

Konvertiert jeden Wert in eine Zeichenfolge.

## [!UICONTROL encodeURL (text)]

Kodiert Sonderzeichen in einem Text in eine gültige URL-Adresse.

## [!UICONTROL decodeURL (text)]

Dekodiert Sonderzeichen in einer URL in Text.

>[!INFO]
>
>**Beispiel:**
>`decodeURL( Automate%20your%20workflow )`
>
>Gibt Folgendes zurück: [!UICONTROL Automatisieren des Workflows]

## [!UICONTROL escapeHTML (text)]

Schließt alle HTML-Tags im Text aus.

>[!INFO]
>
>**Beispiel:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Gibt Folgendes zurück: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Schließt alle Markdown-Tags im Text aus.

>[!INFO]
>
>**Beispiel:**
>
>`escapeMarkdown( # Header )`
>
>Gibt Folgendes zurück: `&#35; Header`

## [!UICONTROL streifenHTML (text)]

Entfernt alle HTML-Tags aus Text.

>[!INFO]
>
>**Beispiel:**
>
>`stripHTML( <b>Hello</b> )`
>
>Gibt Folgendes zurück: Hallo

## contains (text, search string)

Überprüft, ob Text die Suchzeichenfolge enthält.

>[!INFO]
>
>**Beispiele:**
>
>* `contains( Hello World ; Hello )`
>
>   Gibt Folgendes zurück: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Gibt Folgendes zurück: [!UICONTROL false]

## [!UICONTROL split (text; separator)]

Teilt eine Zeichenfolge in ein Zeichenfolgen-Array, indem die Zeichenfolge in Teilzeichenfolgen unterteilt wird.

>[!INFO]
>
>**Beispiel:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (text)]

Berechnet den md5-Hash einer Zeichenfolge.

>[!INFO]
>
>**Beispiel:**
>
>`md5( Workfront )`
>
>Gibt Folgendes zurück: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (text; [encoding]; [key])]

Berechnet den SHA1-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben ist, wird stattdessen SHA1-HMAC-Hash zurückgegeben. Unterstützte Kodierungen: &quot;hex&quot;(Standard), &quot;base64&quot;oder &quot;latin1&quot;.

>[!INFO]
>
>**Beispiel:**
>
>`sha1( workfront )`
>
>Gibt Folgendes zurück: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [encoding]; [key])]

Berechnet den sha256-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben ist, wird stattdessen der HMAC-Hash sha256 zurückgegeben. Unterstützte Kodierungen: &quot;hex&quot;(Standard), &quot;base64&quot;oder &quot;latin1&quot;.>

>[!INFO]
>
>**Beispiel:**
>
>`sha256( workfront )`
>
>Gibt Folgendes zurück: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bc

## [!UICONTROL sha512 (Text; [Ausgabekodierung]; [Schlüssel]; [Schlüsselkodierung])]

Berechnet den SHA512-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben ist, wird stattdessen der HMAC-Hash sha512 zurückgegeben.

Unterstützte Kodierungen:

* &quot;[!UICONTROL hex]&quot;(Standard)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Unterstützte Schlüsselkodierungen:

* &quot;[!UICONTROL text]&quot; (Standard)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot;oder &quot;[!UICONTROL binary]&quot;

Bei Verwendung der Schlüsselkodierung &quot;[!UICONTROL binary]&quot; muss ein Schlüssel ein Puffer sein, kein String.

>[!INFO]
>
>**Beispiel:**
>
>`sha512(workfront)`
>
>Gibt Folgendes zurück: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd11119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (text)]

Wandelt Text in base64 um.

>[!INFO]
>
>**Beispiel:**
>
>`base64( workfront )`
>
>Gibt Folgendes zurück: d29ya2Zyb250===
