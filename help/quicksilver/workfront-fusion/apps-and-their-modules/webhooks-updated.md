---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# Webhooks



>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie nun in den Artikeln:
>
>* [Webhooks](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/webhooks-updated.html)
>* [Webhook für einen Webservice ohne Connector konfigurieren](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

Ein Webhook ist ein HTTP-Aufruf, der von einem Ereignis ausgelöst wird. Sie können Webhooks verwenden, um Instant Trigger-Module zu aktivieren. Jede Anwendung, die mit dem Internet verbunden ist und HTTP-Anfragen zulässt, kann Webhooks an Adobe Workfront Fusion senden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Verwenden eines Webhooks in [!DNL Workfront Fusion]

>[!NOTE]
>
>Verwenden Sie eines der HTTP-Module, um einen Webhook eines Drittanbieters (einen ausgehenden Webhook) aufzurufen. Weitere Informationen finden Sie unter [HTTP-Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

So verwenden Sie einen Webhook, um eine App mit [!DNL Workfront Fusion] zu verbinden:

1. Fügen Sie das **[!UICONTROL Webhooks]** > **[!UICONTROL Benutzerdefinierter Webhook]** Instant Trigger-Modul zu Ihrem Szenario hinzu.

1. Klicken Sie **[!UICONTROL Hinzufügen]** neben dem Feld Webhook und geben Sie einen Namen für den neuen Webhook ein.
1. (Optional) Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen]**.
1. Geben Sie **[!UICONTROL Feld IP-]**) eine kommagetrennte Liste der IP-Adressen ein, von denen das Modul Daten akzeptieren kann.
1. Klicken Sie auf **[!UICONTROL Speichern]**

Nachdem Sie einen Webhook erstellt haben, wird eine eindeutige URL angezeigt. Dies ist die Adresse, an die der Webhook Daten sendet. Workfront Fusion validiert die an diese Adresse gesendeten Daten und gibt sie dann zur Verarbeitung im Szenario weiter.

>[!NOTE]
>
>Nachdem Sie einen Webhook erstellt haben, können Sie ihn in mehr als einem Szenario gleichzeitig verwenden.

### Konfigurieren der Datenstruktur des Webhooks {#configure-the-webhook-s-data-structure}

Um die Datenstruktur der eingehenden Payload zu erkennen, analysiert [!DNL Workfront Fusion] Beispieldaten, die Sie an die angezeigte Adresse senden. Sie können die Beispieldaten bereitstellen, indem Sie den Service oder die App ändern, damit dieser Service oder diese App den Webhook aufruft. Sie können beispielsweise eine Datei entfernen.

Sie können auch die folgenden Schritte ausführen, um die Beispieldaten über das Modul [!UICONTROL HTTP] > [!UICONTROL Anfrage stellen] zu senden.

1. Erstellen Sie ein neues Szenario mit dem Modul **[!UICONTROL HTTP]** > **[!UICONTROL Anfrage]**)

1. Konfigurieren Sie das Modul mit den folgenden Werten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Geben Sie die URL des Webhooks ein. Diese URL finden Sie im Modul [!UICONTROL Webhooks], das Sie zum Einrichten des Webhooks verwendet haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Methode] </td> 
      <td><p>[!UICONTROL-POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Texttyp]</td> 
      <td><p> [!UICONTROL Roh]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content-Typ]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Inhalt anfordern]</td> 
      <td><p>Im Webhook wird unformatiertes JSON erwartet</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Öffnen Sie das Szenario mit dem Modul [!UICONTROL Webhooks] in einer separaten Browser-Registerkarte oder einem separaten Fenster.
1. Klicken Sie im Webhooks-Modul auf **[!UICONTROL Datenstruktur neu bestimmen]**.

   Sie müssen die Verknüpfung anderer Module mit dem Webhooks-Modul nicht aufheben.

1. Wechseln Sie mit dem Modul [!UICONTROL HTTP] zum Szenario und führen Sie es aus.
1. Wechseln Sie mit dem Modul Webhooks zurück zum Szenario.

   Eine Meldung [!UICONTROL Erfolgreich ermittelt] bedeutet, dass das Modul die Datenstruktur erfolgreich ermittelt hat.

   ![](assets/successfully-determined-350x175.png)

1. Klicken Sie **[!UICONTROL OK]**, um die Datenstruktur zu speichern.

   Die Elemente des Webhooks sind jetzt im Zuordnungsbereich verfügbar und können mit nachfolgenden Modulen im Szenario verwendet werden.

## Die Webhook-Warteschlange

Wenn ein Webhook Daten empfängt und kein aktives Szenario diese Daten erwartet, werden die Daten in der Warteschlange gespeichert. Nachdem Sie das Szenario aktiviert haben, werden alle Pakete, die in der Warteschlange warten, sequenziell verarbeitet.

>[!IMPORTANT]
>
>Webhook-Warteschlangen werden von Szenarien gemeinsam verwendet, die denselben Webhook verwenden. Wenn eines der Szenarien deaktiviert ist, werden alle eingehenden Daten in der Warteschlange gehalten.

## Unterstützte eingehende Datenformate

[!DNL Workfront Fusion] unterstützt 3 eingehende Datenformate: [!UICONTROL Abfragezeichenfolge], [!UICONTROL Formulardaten] und [!UICONTROL JSON].

[!DNL Workfront Fusion] validiert alle eingehenden Daten anhand der ausgewählten Datenstruktur. Anschließend werden die Daten je nach den Einstellungen des Szenarios entweder zur Verarbeitung in der Warteschlange gespeichert oder sofort verarbeitet.

Wenn ein Teil der Daten die Validierung nicht besteht, gibt [!DNL Workfront Fusion] einen 400-HTTP-Status-Code zurück und gibt im Hauptteil der HTTP-Antwort den Grund an, warum die eingehenden Daten bei den Validierungsprüfungen fehlgeschlagen sind. Wenn die Validierung der eingehenden Daten erfolgreich ist, gibt Workfront Fusion den Status &quot;[!UICONTROL 200 Accepted] zurück.

* [[!UICONTROL Abfragezeichenfolge]](#query-string)
* [[!UICONTROL Formulardaten]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Abfragezeichenfolge]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Formulardaten]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Mehrteilige Formulardaten

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

Um mit `multipart/form-data` codierte Dateien zu erhalten, müssen Sie eine Datenstruktur mit einem Feld vom Typ `collection` konfigurieren, das die verschachtelten Felder `name`, `mime` und `data` enthält. Das Feld `name` ist ein `text` und enthält den Namen der hochgeladenen Datei. Der `mime` ist ein `text` und enthält eine Datei im MIME-Format. Das Feld `data` ist vom `buffer` Typ und enthält Binärdaten für die übertragene Datei.

Weitere Informationen zum MIME-Format finden Sie unter [MIME-Module](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Wenn Sie auf die ursprüngliche JSON zugreifen möchten, aktivieren Sie beim Einrichten des Webhooks JSON-Pass-Through.
>
>1. Klicken Sie **[!UICONTROL Hinzufügen]**, um einen neuen Webhook hinzuzufügen.
>1. Klicken Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
>1. Klicken Sie auf **[!UICONTROL JSON-Pass-Through]**.
>

## Webhook-Kopfzeilen

Um auf die Kopfzeilen des Webhooks zuzugreifen, aktivieren Sie beim Einrichten des Webhooks die Option GET-Anfrage-Kopfzeilen .

1. Klicken Sie **[!UICONTROL Hinzufügen]**, um einen neuen Webhook hinzuzufügen.
1. Klicken Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
1. Klicken Sie **[!UICONTROL Anfrage-Header abrufen]**.

Sie können einen bestimmten Kopfzeilenwert mit der Kombination aus `map()`- und `get()` extrahieren.

>[!INFO]
>
>**Beispiel:**
>
>Das folgende Beispiel zeigt eine Formel, die den Wert der `authorization`-Kopfzeile aus dem `Headers[]`-Array extrahiert. Die Formel wird in einem Filter verwendet, der den extrahierten Wert mit dem angegebenen Text vergleicht, damit nur Webhooks übergeben werden, wenn eine Übereinstimmung vorliegt.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Weitere Informationen zum Abrufen eines Array-Elements mit einem bestimmten Schlüssel finden Sie unter [Zuordnen eines Array-Elements mit einem bestimmten Schlüssel](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) im Artikel [Zuordnen von Informationen von einem Modul zu einem anderen in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Reagieren auf Webhooks

Die Standardantwort auf einen Webhook-Aufruf ist der Text „Accepted“. Die Antwort wird an die App zurückgegeben, die den Webhook während der Ausführung des benutzerdefinierten Webhook-Moduls aufgerufen hat.

* [Testen der Antwort auf einen Webhook](#test-the-response-to-a-webhook)
* Beispiel für eine [HTML-Antwort](#html-response-example)
* [Redirect-Beispiel](#redirect-example)

### Testen der Antwort auf einen Webhook

1. Fügen Sie das **[!UICONTROL Custom Webhook]**-Modul in Ihr Szenario ein.
1. Fügen Sie dem Modul einen neuen Webhook hinzu.
1. Kopieren Sie die Webhook-URL in die Zwischenablage.
1. Führen Sie das Szenario aus.

   Das Blitzsymbol auf dem Modul [!UICONTROL Benutzerdefinierter Webhook] ändert sich in „Drehpunkte“. Dies zeigt an, dass das Modul jetzt auf den Webhook-Aufruf wartet.

1. Öffnen Sie ein neues Browser-Fenster, fügen Sie die kopierte URL in die Adressleiste ein und drücken Sie die **[!UICONTROL Eingabetaste]**.

   Das Modul [!UICONTROL Benutzerdefinierter Webhook] wird ausgelöst und der Browser zeigt eine neue Seite an.

Wenn Sie die Webhook-Antwort anpassen möchten, verwenden Sie das Modul Webhook-Antwort .

Die Konfiguration des Moduls enthält zwei Felder: [!UICONTROL Status] und [!UICONTROL Body].

* Das Feld [!UICONTROL Status] enthält HTTP-Antwort-Status-Codes wie 2xx für Erfolg (z. B. `200` für OK), 3xx für Umleitung (z. B. `307` für temporäre Umleitung), 4xx für Client-Fehler (z. B. `400` für ungültige Anfrage) usw.

* Das Feld [!UICONTROL body] enthält alles, was vom Aufruf des Webhooks akzeptiert wird. Dabei kann es sich um einfachen Text, HTML, XML, JSON usw. handeln.

  >[!TIP]
  >
  >Es wird empfohlen, den `Content-Type`-Header auf den entsprechenden MIME-Typ festzulegen: `text/plain` für Nur-Text, `text/html` für HTML, `application/json` für JSON, `application/xml` für XML usw. Weitere Informationen zu MIME-Typen finden Sie unter [MIME-Module](../../workfront-fusion/apps-and-their-modules/mime.md).

Die maximale Wartezeit für das Senden einer Antwort beträgt 40 Sekunden. Wenn die Antwort innerhalb dieses Zeitraums nicht verfügbar ist, gibt Workfront Fusion den Status „200 akzeptiert“ zurück.

### Beispiel einer HTML-Antwort

>[!INFO]
>
>**Beispiel:**
>
>Konfigurieren Sie [!UICONTROL  Modul ]Webhook-Antwort“ wie folgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>2xx Erfolgs-HTTP-Status-Code, z. B. 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL body] </td> 
&gt;   <td> <p>HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Kopfzeilen]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>key</strong>: Content-Type</li> 
&gt;     <li><strong>Wert</strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Dadurch wird eine HTML-Antwort erzeugt, die in einem Webbrowser angezeigt wird:
>
>![](assets/html-response-350x70.png)

### Redirect-Beispiel

>[!INFO]
>
>**Beispiel:** Konfigurieren Sie das Modul [!UICONTROL Webhook-]) wie folgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>3xx HTTP-Status-Code der Weiterleitung, z. B. 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Kopfzeilen]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL key]</strong>: Speicherort</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: Die URL, zu der Sie umleiten möchten.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook-Deaktiviert

Webhooks werden automatisch deaktiviert, wenn einer der folgenden Punkte zutrifft:

* Der Webhook wurde seit mehr als 5 Tagen mit keinem Szenario verbunden
* Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

Deaktivierte Webhooks werden automatisch gelöscht und von der Registrierung entfernt, wenn sie mit keinem Szenario verbunden sind und sich seit mehr als 30 Tagen im Status Deaktiviert befinden.


## Fehlerbehebung

### Fehlende Elemente im Zuordnungsbereich

Wenn einige Elemente im Zuordnungsbereich bei der Einrichtung der Module nach dem Modul [!UICONTROL Webhooks] > [!UICONTROL Benutzerdefinierter Webhook] fehlen, klicken Sie auf das Modul **[!UICONTROL Webhooks] > [!UICONTROL Benutzerdefinierter Webhook]** , um sein Setup zu öffnen, und klicken Sie auf **[!UICONTROL Datenstruktur neu bestimmen]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Führen Sie dann die Schritte aus, die im Abschnitt [Konfigurieren der Datenstruktur des Webhooks](#configure-the-webhook-s-data-structure) in diesem Artikel beschrieben sind.
