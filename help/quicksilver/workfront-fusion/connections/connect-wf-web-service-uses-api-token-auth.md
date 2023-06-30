---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] zu einem Webdienst hinzu, der die API-Token-Autorisierung verwendet
description: Einige Dienste ermöglichen keine Integrationslösungen wie [!DNL Adobe Workfront Fusion] , um eine App zu erstellen, die Sie in Ihrem Szenario einfach verwenden können.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] zu einem Webdienst hinzu, der die API-Token-Autorisierung verwendet

Einige Dienste ermöglichen keine Integrationslösungen wie [!DNL Adobe Workfront Fusion] , um eine App zu erstellen, die Sie in Ihrem Szenario einfach verwenden können.

Es gibt eine Lösung für diese Situation. Sie können den gewünschten Dienst (App) mit [!DNL Workfront Fusion] using [!DNL Workfront Fusion]s [!UICONTROL HTTP] -Modul.

In diesem Artikel wird erläutert, wie fast jeder Webdienst mit [!DNL Workfront Fusion] Verwendung eines API-Schlüssels/API-Tokens.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Herstellen einer Verbindung zu einem Webdienst, der ein API-Token verwendet

Die Vorgehensweise zum Verbinden des Dienstes über ein API-Token ist für die meisten Webdienste ähnlich.

1. Erstellen Sie eine Anwendung auf der Website des Webdienstes, wie im Abschnitt beschrieben. [Erstellen einer neuen Anwendung und Abrufen des API-Tokens](#create-a-new-application-and-obtain-the-api-token) in diesem Artikel.
1. Rufen Sie den API-Schlüssel oder das API-Token ab.
1. Hinzufügen [!DNL Workfront Fusion]s [!UICONTROL HTTP] > [!UICONTROL Anfordern] -Modul zu Ihrem Szenario hinzu.
1. Richten Sie das Modul gemäß der API-Dokumentation des Webdienstes ein und führen Sie das Szenario wie im Abschnitt beschrieben aus. [Richten Sie die [!UICONTROL HTTP] Modul](#set-up-the-http-module) in diesem Artikel.

>[!NOTE]
>
>Wir werden die [!DNL Pushover] Benachrichtigungsdienst als Beispiel in diesem Artikel.

## Erstellen einer neuen Anwendung und Abrufen des API-Tokens

>[!NOTE]
>
>Es gibt viele verschiedene Möglichkeiten, wie Webdienste API-Schlüssel oder API-Token erstellen und verteilen. Anweisungen zum Abrufen eines API-Schlüssels und -Tokens für Ihren gewünschten Webdienst finden Sie auf der Website des Diensts und suchen Sie nach &quot;API-Schlüssel&quot;oder &quot;API-Token&quot;.
>
>Wir enthalten Anweisungen zum Abrufen eines Pushover-API-Schlüssels nur als Beispiel dafür, was Sie finden.

1. Melden Sie sich bei Ihrer [!DNL Pushover] -Konto.
1. Klicken **[!UICONTROL Erstellen eines Anwendungs-/API-Tokens]** unten auf der Seite.
1. Füllen Sie die Anwendungsinformationen aus und klicken Sie auf **[!UICONTROL Erstellen einer Anwendung]**.
1. Speichern Sie das bereitgestellte API-Token an einem sicheren Ort. Sie benötigen sie für die [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Anfordern] -Modul, um eine Verbindung zum gewünschten Webdienst herzustellen ([!DNL Pushover], in diesem Fall).

## Richten Sie die [!UICONTROL HTTP] Modul

So verbinden Sie einen Webdienst mit Ihrem [!DNL Workfront Fusion] -Szenario verwenden, müssen Sie die [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] -Modul im Szenario ein und richten Sie das -Modul gemäß der API-Dokumentation des Webdienstes ein.

1. Fügen Sie die [!UICONTROL HTTP] >[!UICONTROL Anfordern] -Modul zu Ihrem Szenario hinzu.
1. So senden Sie eine Nachricht über [!DNL Workfront Fusion], richten Sie das HTTP-Modul wie folgt ein.

   >[!NOTE]
   >
   >Diese Moduleinstellungen entsprechen dem [!DNL Pushover] Webdienst-API-Dokumentation. Die Einstellungen können für andere Webdienste unterschiedlich sein. Beispielsweise kann das API-Token zum [!UICONTROL Kopfzeile] und nicht [!UICONTROL body] -Feld.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Das Feld URL enthält den Endpunkt, den Sie in der API-Dokumentation des Webdienstes finden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Methode]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>Die verwendete Methode hängt vom entsprechenden Endpunkt ab. Der Pushover-Endpunkt zum Pushen von Nachrichten verwendet die POST-Methode.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Header]</p> </td> 
      <td> <p>Einige Webdienste können Kopfzeilen verwenden, um die API-Token-Authentifizierung oder andere Parameter anzugeben. Dies ist in unserem Beispiel nicht der Fall, da der Pushover-Endpunkt zum Pushover-Senden von Nachrichten für alle Anfragetypen den Hauptteil verwendet (siehe unten).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Abfragezeichenfolge]</p> </td> 
      <td> <p>Einige Webdienste können eine Abfragezeichenfolge verwenden, um andere Parameter anzugeben. Dies ist in unserem Beispiel nicht der Fall, da die Variable [!DNL Pushover] Der Webdienst verwendet [!UICONTROL Body] (siehe unten) für alle Anfragetypen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Textkörper]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Mit dieser Einstellung können Sie den JSON-Inhaltstyp im unten stehenden Feld [!UICONTROL Inhaltstyp] auswählen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON ist der erforderliche Inhaltstyp für die [!UICONTROL Pushover]-App. Dies kann sich von anderen Webdiensten unterscheiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Anforderungsinhalt]</p> </td> 
      <td> <p>Geben Sie den Anforderungsinhalt des [!UICONTROL Hauptteils] im JSON-Format ein. Sie können das Modul [!UICONTROL JSON] &gt; [!UICONTROL JSON erstellen, wie hier beschrieben: <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON-Hauptteil, der mithilfe des Moduls [!UICONTROL JSON] &gt; [!UICONTROL JSON erstellen zugeordnet wurde</a> in diesem Artikel. Alternativ können Sie den JSON-Inhalt manuell eingeben, wie hier beschrieben: <a href="#json-body-entered-manually" class="MCXref xref">Manuelles Eingeben des JSON-Hauptteils</a> in diesem Artikel.</p> <p>Die erforderlichen Parameter für diesen Webdienst finden Sie in der API-Dokumentation des Webdienstes .</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Manuelles Eingeben des JSON-Hauptteils

Geben Sie Parameter und Werte im JSON-Format an.

>[!INFO]
>
>**Beispiel:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Benutzer]</p> </td> 
   <td> <p>Ihr USER_KEY. Diese finden Sie in Ihrer [!DNL Pushover] Dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token] </td> 
   <td> <p>Ihr API-Token/API-Schlüssel, der von Ihnen generiert wurde [!DNL Pushover] App.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>Der Textinhalt der Push-Benachrichtigung, die an das Gerät/die Geräte gesendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Optional) Der Titel Ihrer Nachricht. Wenn kein Wert eingegeben wird, wird der Name Ihrer App verwendet. </p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-Hauptteil, der mithilfe der [!UICONTROL JSON] >[!UICONTROL JSON erstellen] Modul

Die [!UICONTROL JSON erstellen] -Modul vereinfacht die Angabe von JSON. Sie können damit auch Werte dynamisch definieren.

Weitere Informationen zu den JSON-Modulen finden Sie unter [JSON-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Geben Sie die Werte ein oder ordnen Sie sie zu, aus denen JSON erstellt werden soll.

   ![](assets/json-values-350x288.png)

1. Verbinden Sie die [!UICONTROL JSON] > [!UICONTROL JSON erstellen] -Modul zum HTTP > Anforderungsmodul hinzufügen.
1. Ordnen Sie die JSON-Zeichenfolge aus der [!UICONTROL JSON erstellen] -Modul [!UICONTROL Inhalt anfordern] im Feld [!UICONTROL HTTP] >[!UICONTROL Anfordern] -Modul.

   Wenn Sie nun das Szenario ausführen, wird die Push-Benachrichtigung an das Gerät gesendet, das in Ihrer [!DNL Pushover] -Konto.
