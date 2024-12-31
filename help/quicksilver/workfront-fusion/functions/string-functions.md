---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Zeichenfolgen-Funktionen in Adobe Workfront Fusion
description: Die folgenden Zeichenfolgenfunktionen sind im Bedienfeld "Adobe Workfront Fusion-Zuordnung“ verfügbar.
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

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Beliebig</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p> 
   <p>Oder</p> 
   <p>Legacy: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL length (Text oder Puffer)]

Gibt die Länge der Textzeichenfolge (Anzahl der Zeichen) oder des Binärpuffers (Puffergröße in Byte) zurück.

>[!INFO]
>
>**Beispiel:**
>
>`length( hello )`
>
>Gibt zurück: 5

## [!UICONTROL lower (Text)]

Konvertiert alle alphabetischen Zeichen in einer Textzeichenfolge in Kleinbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`lower( Hello )`
>
>Gibt zurück: hallo

## [!UICONTROL großschreiben (Text)]

Konvertiert das erste Zeichen in einer Textzeichenfolge in Großbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`capitalize( workfront )`
>
>Gibt zurück: [!DNL Workfront]

## [!UICONTROL startCase (Text)]

Großschreibung des ersten Buchstaben jedes Wortes und Kleinschreibung aller anderen Buchstaben.

>[!INFO]
>
>**Beispiel:**
>`startcase( hello WORLD )`
>
>Gibt zurück: [!UICONTROL Hello World]

## [!UICONTROL ASCII (Text; [diakritische Zeichen entfernen])]

Entfernt alle Nicht-ASCII-Zeichen aus einer Textzeichenfolge.

>[!INFO]
>
>**Beispiele:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   Gibt zurück: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   Gibt zurück: [!UICONTROL escrz]



## [!UICONTROL replace (Text;Suchzeichenfolge; Ersatzzeichenfolge)]

Ersetzt die Suchzeichenfolge durch die neue Zeichenfolge.

>[!INFO]
>
>**Beispiel:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Gibt zurück: [!UICONTROL Hi World]

Reguläre Ausdrücke (in `/.../` eingeschlossen) können als Suchzeichenfolge verwendet werden, an die eine Kombination von Flags (z. B. `g`, `i`, `m`) angehängt wird:

>[!INFO]
>
>**Beispiel:**
>
>![](assets/replace---1-350x31.png)
>
>Alle diese Zahlen X X X X werden durch X ersetzt

Die Ersatzzeichenfolge kann die folgenden speziellen Ersetzungsmuster enthalten:

* `$&` Fügt die übereinstimmende Teilzeichenfolge ein.
* `$n` Wobei n eine positive Ganzzahl kleiner als 100 ist, wird die n-te, in Klammern eingeschlossene Teilübereinstimmungszeichenfolge eingefügt. Dies ist 1-indiziert.

>[!INFO]
>
>**Beispiele:**
>
>![](assets/variable-value-350x63.png)
>
>Gibt zurück: Telefonnummer `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Gibt zurück: Telefonnummer: `+420777111222`

>[!CAUTION]
>
>Verwenden Sie keine benannten Capture-Gruppen wie `/ is (?<number>\d+)/` im Argument der Ersatzzeichenfolge. Dies führt zu einem Fehler.

Weitere Informationen zu regulären Ausdrücken finden Sie unter [Text-Parser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL trim (Text)]

Entfernt Leerzeichen am Anfang oder Ende des Textes.

## [!UICONTROL upper (Text)]

Konvertiert alle alphabetischen Zeichen in einer Textzeichenfolge in Großbuchstaben.

>[!INFO]
>
>**Beispiel:**
>
>`upper( Hello )`
>
>Gibt zurück: [!UICONTROL HELLO]

## [!UICONTROL Teilzeichenfolge (Text; Start;Ende)]

Gibt einen Teil einer Textzeichenfolge zwischen der „Start“-Position und der „Ende“-Position zurück.

>[!INFO]
>
>**Beispiele:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Rückgabe: Hilfe
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Gibt zurück: el

## [!DNL indexOf (string; value; [start])]

Gibt die Position des ersten Vorkommens eines angegebenen Werts in einer Zeichenfolge zurück. Diese Methode gibt &#39;-1&#39; zurück, wenn der gesuchte Wert nicht vorhanden ist. Der Startwert gibt an, wo in der Zeichenfolge die Suche beginnen soll.

>[!INFO]
>
>**Beispiele:**
>
>* `indexOf( Workfront ; o )`
>
>   Gibt zurück: 1
>
>* `indexOf( Workfront ; x )`
>
>   Gibt zurück: -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   Gibt zurück: 6

## [!UICONTROL toBinary (Wert)]

Konvertiert einen beliebigen Wert in Binärdaten.

Sie können auch Codierung als zweites Argument angeben, um binäre Konvertierungen von hex- oder base64-Binärdaten anzuwenden.

>[!INFO]
>
>**Beispiele:**
>
>* `toBinary( Workfront )`
>
>   Rückgabe: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Rückgabe: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (value)]

Konvertiert einen beliebigen Wert in eine Zeichenfolge.

## [!UICONTROL encodeURL (text)]

Codiert Sonderzeichen in Text in eine gültige URL-Adresse.

## [!UICONTROL decodeURL (text)]

Decodiert Sonderzeichen in einer URL zu Text.

>[!INFO]
>
>**Beispiel:**
>`decodeURL( Automate%20your%20workflow )`
>
>Rückgabe: [!UICONTROL Workflow automatisieren]

## [!UICONTROL escapeHTML (text)]

Alle HTML-Tags im Text werden maskiert.

>[!INFO]
>
>**Beispiel:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Gibt zurück: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Alle Markdown-Tags im Text werden mit Escape-Zeichen versehen.

>[!INFO]
>
>**Beispiel:**
>
>`escapeMarkdown( # Header )`
>
>Gibt zurück: `&#35; Header`

## [!UICONTROL stripHTML (text)]

Entfernt alle HTML-Tags aus dem Text.

>[!INFO]
>
>**Beispiel:**
>
>`stripHTML( <b>Hello</b> )`
>
>Gibt zurück: hallo

## enthält (Text; Suchzeichenfolge)

Prüft, ob der Text die Suchzeichenfolge enthält.

>[!INFO]
>
>**Beispiele:**
>
>* `contains( Hello World ; Hello )`
>
>   Gibt zurück: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Gibt zurück: [!UICONTROL false]

## [!UICONTROL split (Text; Trennzeichen)]

Teilt eine Zeichenfolge in ein Array von Zeichenfolgen, indem die Zeichenfolge in Unterzeichenfolgen aufgeteilt wird.

>[!INFO]
>
>**Beispiel:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL MD5 (Text)]

Berechnet den MD5-Hash einer Zeichenfolge.

>[!INFO]
>
>**Beispiel:**
>
>`md5( Workfront )`
>
>Gibt zurück: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL SHA1 (Text; [Encoding]; [key])]

Berechnet den SHA1-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben wird, wird stattdessen ein sha1-HMAC-Hash zurückgegeben. Unterstützte Codierungen: „hex“ (Standard), „base64“ oder „latin1“.

>[!INFO]
>
>**Beispiel:**
>
>`sha1( workfront )`
>
>Gibt zurück: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL SHA256 (Text; [Encoding]; [key])]

Berechnet den SHA256-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben wird, wird stattdessen ein sha256-HMAC-Hash zurückgegeben. Unterstützte Kodierungen: „hex“ (Standard), „base64“ oder „latin1“.>

>[!INFO]
>
>**Beispiel:**
>
>`sha256( workfront )`
>
>Gibt zurück: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL SHA512 (Text; [Ausgabekodierung]; [Schlüssel]; [Schlüsselkodierung])]

Berechnet den SHA512-Hash einer Zeichenfolge. Wenn das Schlüsselargument angegeben wird, wird stattdessen ein sha512-HMAC-Hash zurückgegeben.

Unterstützte Kodierungen:

* &quot;[!UICONTROL hex]&quot; (Standard)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL Latin1]&quot;

Unterstützte Schlüsselcodierungen:

* &quot;[!UICONTROL text]&quot; (Standard)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; oder &quot;[!UICONTROL binary]&quot;

Bei Verwendung der [!UICONTROL binären] Schlüsselkodierung muss ein Schlüssel ein Puffer sein, keine Zeichenfolge.

>[!INFO]
>
>**Beispiel:**
>
>`sha512(workfront)`
>
>Gibt zurück: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (Text)]

Transformiert Text in base64.

>[!INFO]
>
>**Beispiel:**
>
>`base64( workfront )`
>
>Gibt zurück: d29ya2zyb250==
