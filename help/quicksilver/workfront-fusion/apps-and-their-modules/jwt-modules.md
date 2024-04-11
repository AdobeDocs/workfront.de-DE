---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT-Module
description: Die [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app stellt ein Modul bereit, das JWT-Token basierend auf dem bereitgestellten Algorithmus erstellt.
author: Becky
feature: Workfront Fusion
source-git-commit: 121aef2ee55597fee2e2adc8250dd0651ea86f17
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] Modul

Die [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app stellt ein Modul bereit, das JWT-Token basierend auf dem bereitgestellten Algorithmus erstellt.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JWT-Modul und seine Felder

### JWT generieren

Dieses Modul generiert eine JWT auf Grundlage des ausgewählten Algorithmus.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithm]</td> 
   <td> <p>Wählen Sie den Algorithmus aus, mit dem Sie die JWT generieren möchten.</p> <ul>
   <li><b>HS256</b>: HMAC mit SHA-256-Hash-Algorithmus</li>
   <li><b>HS384</b>: HMAC mit SHA-384-Hash-Algorithmus</li>
   <li><b>HS512</b>: HMAC mit SHA-512-Hash-Algorithmus</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 mit SHA-256-Hash-Algorithmus</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 mit SHA-384-Hash-Algorithmus</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 mit SHA-512-Hash-Algorithmus</li>
   <li><b>PS256</b>: RSASSA-PSS mit SHA-256-Hash-Algorithmus (nur Knoten ^6.12.0 ODER &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS mit SHA-384-Hash-Algorithmus (nur Knoten ^6.12.0 ODER &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS mit SHA-512-Hash-Algorithmus (nur Knoten ^6.12.0 ODER &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA mit P-256-Kurve und SHA-256-Hash-Algorithmus</li>
   <li><b>ES384</b>: ECDSA mit P-384-Kurve und SHA-384-Hash-Algorithmus</li>
   <li><b>ES512</b>: ECDSA mit P-521-Kurve und SHA-512-Hash-Algorithmus</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>Klicken Sie für jedes Payload-Element, das Sie hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und den Wert des Elements ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optionen] </td> 
   <td> <p>Klicken Sie für jedes hinzuzufügende Optionselement auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und den Wert des Elements ein.</p> <p>Die folgenden Schlüssel sind verfügbar:
   <ul>
   <li><b>Algorithmus</b>: (Standard: RS256)</li>
   <li><b>expiresIn</b>: Wird in Sekunden oder einer Zeichenfolge ausgedrückt, die eine Zeitspanne beschreibt (z. B. 2 Tage, 10 Stunden, 7 Tage). Ein numerischer Wert wird als Anzahl der Sekunden interpretiert. Wenn Sie eine Zeichenfolge verwenden, stellen Sie sicher, dass Sie die Zeiteinheiten (Tage, Stunden usw.) angeben. Andernfalls wird standardmäßig die Einheit in Millisekunden verwendet (120 ist gleich 120 ms).</li>
   <li><b>notBefore</b>: Wird in Sekunden oder einer Zeichenfolge ausgedrückt, die eine Zeitspanne beschreibt (z. B. 2 Tage, 10 Stunden, 7 Tage). Ein numerischer Wert wird als Anzahl der Sekunden interpretiert. Wenn Sie eine Zeichenfolge verwenden, stellen Sie sicher, dass Sie die Zeiteinheiten (Tage, Stunden usw.) angeben. Andernfalls wird standardmäßig die Einheit in Millisekunden verwendet (120 ist gleich 120 ms).
</li>
   <li><b>audience</b></li>
   <li><b>Emittent</b></li>
   <li><b>jwtid</b></li>
   <li><b>subject</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: Wenn <code>true</code>, ändert die Zeichenfunktion das Payload-Objekt direkt. Dies ist nützlich, wenn Sie einen Rohverweis auf die Payload benötigen, nachdem die Ansprüche darauf angewendet wurden, aber bevor sie in ein Token kodiert wurden.</li>
   <li><b>allowInsecureKeySizes</b>: Wenn <code>true</code>ermöglicht die Verwendung privater Schlüssel mit einem Modul unter 2048 für RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: Wenn <code>true</code>erlaubt asymmetrische Schlüssel, die nicht mit dem angegebenen Algorithmus übereinstimmen. Diese Option dient nur der Abwärtskompatibilität und sollte vermieden werden.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


