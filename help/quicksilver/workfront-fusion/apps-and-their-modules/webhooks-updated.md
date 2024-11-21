---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Ein Webhook ist ein HTTP-Aufruf, der durch ein Ereignis ausgelöst wird. Sie können Webhooks verwenden, um Instant Trigger Module zu aktivieren. Jede Anwendung, die mit dem Internet verbunden ist und HTTP-Anfragen zulässt, kann Webhooks an Adobe Workfront Fusion senden.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Webhooks



<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

Ein Webhook ist ein HTTP-Aufruf, der durch ein Ereignis ausgelöst wird. Sie können Webhooks verwenden, um Instant Trigger Module zu aktivieren. Jede Anwendung, die mit dem Internet verbunden ist und HTTP-Anfragen zulässt, kann Webhooks an Adobe Workfront Fusion senden.

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
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Webhook in [!DNL Workfront Fusion] verwenden

>[!NOTE]
>
>Um einen Drittanbieter-Webhook (einen ausgehenden Webhook) aufzurufen, verwenden Sie eines der HTTP-Module. Weitere Informationen finden Sie unter [HTTP-Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

So verwenden Sie einen Webhook, um eine App mit [!DNL Workfront Fusion] zu verbinden:

1. Fügen Sie das Instant-Trigger-Modul **[!UICONTROL Webhooks]** >**[!UICONTROL Benutzerspezifischer Webhook]** zu Ihrem Szenario hinzu.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem Webhook-Feld und geben Sie einen Namen für den neuen Webhook ein.
1. (Optional) Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen]**.
1. Geben Sie im Feld **[!UICONTROL IP-Beschränkungen]** eine kommagetrennte Liste der IP-Adressen ein, von denen das Modul Daten akzeptieren kann.
1. Klicken Sie auf **[!UICONTROL Speichern]**

Nachdem Sie einen Webhook erstellt haben, wird eine eindeutige URL angezeigt. Dies ist die Adresse, an die der Webhook Daten sendet. Workfront Fusion validiert die an diese Adresse gesendeten Daten und gibt sie dann zur Verarbeitung im Szenario weiter.

>[!NOTE]
>
>Nachdem Sie einen Webhook erstellt haben, können Sie ihn in mehreren Szenarien gleichzeitig verwenden.

### Datenstruktur des Webhooks konfigurieren {#configure-the-webhook-s-data-structure}

Um die Datenstruktur der eingehenden Payload zu erkennen, analysiert [!DNL Workfront Fusion] Beispieldaten, die Sie an die angezeigte Adresse senden. Sie können die Beispieldaten bereitstellen, indem Sie eine Änderung im Dienst oder in der App vornehmen, die dazu führt, dass dieser Dienst oder diese App den Webhook aufruft. Sie können beispielsweise eine Datei entfernen.

Sie können auch die folgenden Schritte ausführen, um die Beispieldaten über das Modul [!UICONTROL HTTP] > [!UICONTROL Anfrage stellen] zu senden.

1. Erstellen Sie ein neues Szenario mit dem Modul **[!UICONTROL HTTP]** > **[!UICONTROL Anfrage stellen]** .

1. Konfigurieren Sie das Modul mit den folgenden Werten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Geben Sie die URL des Webhooks ein. Sie finden diese URL im Modul [!UICONTROL Webhooks], das Sie zum Einrichten des Webhooks verwendet haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Methode] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Textkörper]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Inhaltstyp]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anforderungsinhalt]</td> 
      <td><p>Rohe JSON im Webhook erwartet</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Öffnen Sie das Szenario mit dem Modul [!UICONTROL Webhooks] in einer separaten Browser-Registerkarte oder einem separaten Fenster.
1. Klicken Sie im webhooks-Modul auf **[!UICONTROL Datenstruktur neu bestimmen]**.

   Sie müssen die Verknüpfung anderer Module nicht vom Webhooks-Modul aufheben.

1. Wechseln Sie mit dem Modul [!UICONTROL HTTP] zum Szenario und führen Sie es aus.
1. Wechseln Sie mit dem Webhooks-Modul zurück zum Szenario.

   Die Meldung &quot;[!UICONTROL Erfolgreich bestimmt]&quot; bedeutet, dass das Modul die Datenstruktur erfolgreich ermittelt hat.

   ![](assets/successfully-determined-350x175.png)

1. Klicken Sie auf **[!UICONTROL OK]** , um die Datenstruktur zu speichern.

   Die Elemente des Webhooks sind jetzt im Zuordnungsbereich für die Verwendung mit nachfolgenden Modulen im Szenario verfügbar.

## Die Webhook-Warteschlange

Wenn ein Webhook Daten erhält und kein aktives Szenario mit diesen Daten verbunden ist, werden die Daten in der Warteschlange gespeichert. Nachdem Sie das Szenario aktiviert haben, werden alle Pakete, die in der Warteschlange warten, nacheinander verarbeitet.

>[!IMPORTANT]
>
>Webhook-Warteschlangen werden unter Szenarien freigegeben, die denselben Webhook verwenden. Wenn eines der Szenarien deaktiviert ist, werden alle eingehenden Daten in der Warteschlange gespeichert.

## Unterstützte eingehende Datenformate

[!DNL Workfront Fusion] unterstützt 3 eingehende Datenformate: [!UICONTROL Abfragezeichenfolge], [!UICONTROL Formulardaten] und [!UICONTROL JSON].

[!DNL Workfront Fusion] validiert alle eingehenden Daten mit der ausgewählten Datenstruktur. Anschließend werden die Daten je nach den Einstellungen des Szenarios entweder zur Verarbeitung in der Warteschlange gespeichert oder sofort verarbeitet.

Wenn ein Teil der Daten die Validierung nicht besteht, gibt [!DNL Workfront Fusion] einen 400-HTTP-Statuscode zurück und gibt im Text der HTTP-Antwort den Grund an, warum die eingehenden Daten bei den Validierungsprüfungen fehlgeschlagen sind. Wenn die Validierung der eingehenden Daten erfolgreich ist, gibt Workfront Fusion den Status &quot;[!UICONTROL 200 Akzeptiert]&quot;zurück.

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

#### Formulardaten mit mehreren Elementen

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

Um mit `multipart/form-data` kodierte Dateien zu erhalten, müssen Sie eine Datenstruktur mit einem Feld vom Typ `collection` konfigurieren, das die verschachtelten Felder `name`, `mime` und `data` enthält. Das Feld `name` ist ein `text`-Typ und enthält den Namen der hochgeladenen Datei. Die `mime` ist ein `text` -Typ und enthält eine Datei im MIME-Format. Das Feld `data` ist ein `buffer` -Typ und enthält Binärdaten für die zu übertragende Datei.

Weitere Informationen zum MIME-Format finden Sie unter [MIME-Module](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Wenn Sie auf die ursprüngliche JSON-Datei zugreifen möchten, aktivieren Sie die JSON-Weitergabe beim Einrichten des Webhooks.
>
>1. Klicken Sie auf **[!UICONTROL Hinzufügen]** , um einen neuen Webhook hinzuzufügen.
>1. Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
>1. Klicken Sie auf **[!UICONTROL JSON-Pass-Through]**.
>

## Webhook-Header

Um auf die Header des Webhooks zuzugreifen, aktivieren Sie beim Einrichten des Webhooks die Option Anforderungsheader abrufen .

1. Klicken Sie auf **[!UICONTROL Hinzufügen]** , um einen neuen Webhook hinzuzufügen.
1. Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
1. Klicken Sie auf **[!UICONTROL Anforderungsheader abrufen]**.

Sie können einen bestimmten Kopfzeilenwert mit der Kombination von `map()` - und `get()` -Funktionen extrahieren.

>[!INFO]
>
>**Beispiel:**
>
>Das folgende Beispiel zeigt eine Formel, die den Wert der Kopfzeile `authorization` aus dem Array `Headers[]` extrahiert. Die Formel wird in einem Filter verwendet, der den extrahierten Wert mit dem angegebenen Text vergleicht, um nur Webhooks zu übergeben, wenn eine Übereinstimmung vorliegt.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Weitere Informationen zum Abrufen des Elements eines Arrays mit einem bestimmten Schlüssel finden Sie unter [Ordnen Sie das Element eines Arrays mit einem bestimmten Schlüssel zu](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) im Artikel [Informationen von einem Modul einem anderen in Adobe Workfront Fusion zuordnen](../../workfront-fusion/mapping/map-information-between-modules.md).

## Antworten auf Webhooks

Die Standardantwort auf einen Webhook-Aufruf ist der Text &quot;Akzeptiert&quot;. Die Antwort wird während der Ausführung des Benutzerspezifischen Webhook-Moduls an die App zurückgegeben, die den Webhook aufgerufen hat.

* [Testen der Antwort auf einen Webhook](#test-the-response-to-a-webhook)
* [HTML Response example](#html-response-example)
* [Beispiel einer Umleitung](#redirect-example)

### Testen der Antwort auf einen Webhook

1. Schließen Sie das Modul **[!UICONTROL Benutzerspezifischer Webhook]** in Ihr Szenario ein.
1. Fügen Sie dem Modul einen neuen Webhook hinzu.
1. Kopieren Sie die Webhook-URL in die Zwischenablage.
1. Führen Sie das Szenario aus.

   Das Blitzsymbol im Modul [!UICONTROL Benutzerspezifischer Webhook] ändert sich in Drehpunkte. Dies zeigt, dass das Modul jetzt auf den Webhook-Aufruf wartet.

1. Öffnen Sie ein neues Browser-Fenster, fügen Sie die kopierte URL in die Adressleiste ein und drücken Sie **[!UICONTROL Enter]**.

   Das Modul [!UICONTROL Benutzerspezifischer Webhook] wird ausgelöst und der Browser zeigt eine neue Seite an.

Wenn Sie die Webhook-Antwort anpassen möchten, wenden Sie das Modul Webhook Response an.

Die Konfiguration des Moduls umfasst zwei Felder: [!UICONTROL Status] und [!UICONTROL Textkörper].

* Das Feld [!UICONTROL Status] enthält HTTP-Antwortstatus-Codes wie 2xx für Erfolg (z. B. `200` für OK), 3xx für Umleitung (z. B. `307` für temporäre Umleitung), 4xx für Client-Fehler (z. B. `400` für fehlerhafte Anfragen) usw.

* Das Feld [!UICONTROL Hauptteil] enthält alles, was vom Webhook-Aufruf akzeptiert wird. Dabei kann es sich um einfachen Text, HTML, XML, JSON usw. handeln.

  >[!TIP]
  >
  >Es wird empfohlen, die Kopfzeile `Content-Type` auf den entsprechenden MIME-Typ festzulegen: `text/plain` für Klartext, `text/html` für HTML, `application/json` für JSON, `application/xml` für XML usw. Weitere Informationen zu MIME-Typen finden Sie unter [MIME-Module](../../workfront-fusion/apps-and-their-modules/mime.md).

Die Zeitüberschreitung für das Senden einer Antwort beträgt 40 Sekunden. Wenn die Antwort innerhalb dieses Zeitraums nicht verfügbar ist, gibt Workfront Fusion den Status &quot;200 Akzeptiert&quot;zurück.

### HTML-Antwortbeispiel

>[!INFO]
>
>**Beispiel:**
>
>Konfigurieren Sie das Modul [!UICONTROL Webhook Response] wie folgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>2xx Erfolg HTTP-Status-Code, z. B. 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>HTML-Code</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Kopfzeilen]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Schlüssel</strong>: Content-Typ</li> 
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

### Beispiel einer Umleitung

>[!INFO]
>
>**Beispiel:** Konfigurieren Sie das Modul [!UICONTROL Webhook Response] wie folgt:
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>3xx-Weiterleitungs-HTTP-Status-Code, z. B. 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Kopfzeilen]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Schlüssel]</strong>: Speicherort</li> 
&gt;     <li><strong>[!UICONTROL Wert]</strong>: Die URL, zu der Sie umleiten möchten.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook-Deaktivierung

Webhooks werden automatisch deaktiviert, wenn eine der folgenden Aktionen zutrifft:

* Der Webhook ist seit mehr als 5 Tagen mit keinem Szenario verbunden
* Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

Deaktivierte Webhooks werden automatisch gelöscht und abgemeldet, wenn sie mit keinem Szenario verbunden sind und seit über 30 Tagen den Status deaktiviert haben.


## Fehlerbehebung

### Fehlende Elemente im Zuordnungsbereich

Wenn im Mapping-Bedienfeld bei der Einrichtung der Module einige Elemente fehlen, die dem Modul [!UICONTROL Webhooks] > [!UICONTROL Benutzerspezifischer Webhook] folgen, klicken Sie auf das Modul **[!UICONTROL Webhooks] > [!UICONTROL Benutzerspezifischer Webhook]** , um dessen Einrichtung zu öffnen, und klicken Sie auf **[!UICONTROL Datenstruktur neu bestimmen]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Führen Sie dann die im Abschnitt [Datenstruktur des Webhooks konfigurieren](#configure-the-webhook-s-data-structure) in diesem Artikel beschriebenen Schritte aus.
