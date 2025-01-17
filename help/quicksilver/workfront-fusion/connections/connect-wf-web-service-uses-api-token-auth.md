---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbindung  [!DNL Adobe Workfront Fusion]  einem Webdienst herstellen, der API-Token-Autorisierung verwendet
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Verbinden von [!DNL Adobe Workfront Fusion] mit einem Webservice, der die API-Token-Autorisierung verwendet

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Verbinden Sie Adobe Workfront Fusion mit einem Webservice, der die API-Token-Autorisierung verwendet](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Einige Services erlauben keine Integrationslösungen wie [!DNL Adobe Workfront Fusion], um eine App zu erstellen, die Sie in Ihrem Szenario einfach verwenden können.

Es gibt eine Problemumgehung für diese Situation. Sie können den gewünschten Dienst (die App) mit [!DNL Workfront Fusion] über das [!DNL Workfront Fusion]-Modul [!UICONTROL HTTP] verbinden.

In diesem Artikel wird erläutert, wie Sie mithilfe eines API-Schlüssels/API-Tokens nahezu jeden Webservice mit [!DNL Workfront Fusion] verbinden.

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

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Herstellen einer Verbindung zu einem Webdienst, der ein API-Token verwendet

Die Vorgehensweise beim Verbinden des Service über ein API-Token ist bei den meisten Web-Services ähnlich.

1. Erstellen Sie eine Anwendung auf der Website des Webservices, wie im Abschnitt [Erstellen einer neuen Anwendung und Abrufen des API-Tokens](#create-a-new-application-and-obtain-the-api-token) in diesem Artikel erläutert.
1. Abrufen des API-Schlüssels oder API-Tokens.
1. [!DNL Workfront Fusion] Fügen Sie das Modul [!UICONTROL HTTP] > [!UICONTROL Anfrage ] Ihrem Szenario hinzu.
1. Richten Sie das Modul gemäß der API-Dokumentation des Web-Services ein und führen Sie das Szenario aus, wie im Abschnitt [Einrichten des [!UICONTROL HTTP]-Moduls](#set-up-the-http-module) in diesem Artikel beschrieben.

>[!NOTE]
>
>In diesem Artikel werden wir den [!DNL Pushover]-Benachrichtigungsdienst als Beispiel verwenden.

## Erstellen eines neuen Programms und Abrufen des API-Tokens

>[!NOTE]
>
>Es gibt viele verschiedene Möglichkeiten, wie Web-Services API-Schlüssel oder API-Token erstellen und verteilen. Anweisungen zum Abrufen eines API-Schlüssels und eines Tokens für Ihren gewünschten Webservice finden Sie auf der Website des Services nach „API-Schlüssel“ oder „API-Token“.
>
>Wir enthalten Anweisungen zum Abrufen eines Pushover-API-Schlüssels nur als Beispiel für das, was Sie möglicherweise finden.

1. Melden Sie sich bei Ihrem [!DNL Pushover] an.
1. Klicken **[!UICONTROL unten auf der Seite auf &quot;]**/API-Token erstellen“.
1. Füllen Sie die Informationen aus und klicken Sie auf **[!UICONTROL Anwendung erstellen]**.
1. Bewahren Sie das bereitgestellte API-Token an einem sicheren Ort auf. Sie benötigen es für das [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen]-Modul, um eine Verbindung zum gewünschten Webservice herzustellen ([!DNL Pushover] in diesem Fall).

## Einrichten des [!UICONTROL HTTP]-Moduls

Um einen Webservice mit Ihrem [!DNL Workfront Fusion] Szenario zu verbinden, müssen Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] im Szenario verwenden und das Modul gemäß der API-Dokumentation des Webservices einrichten.

1. Fügen Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] zu Ihrem Szenario hinzu.
1. Um eine Nachricht mithilfe von [!DNL Workfront Fusion] zu pushen, richten Sie das HTTP-Modul wie folgt ein.

   >[!NOTE]
   >
   >Diese Moduleinstellungen entsprechen der Dokumentation zur [!DNL Pushover]-Webservice-API. Die Einstellungen für andere Webdienste können sich unterscheiden. Beispielsweise kann das API-Token in den [!UICONTROL Header“ und ] in das Feld [!UICONTROL Body] eingefügt werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Das URL-Feld enthält den Endpunkt, den Sie in der API-Dokumentation des Webservices finden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Methode]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>Die verwendete Methode hängt vom entsprechenden Endpunkt ab. Der Pushover-Endpunkt für das Pushen von Nachrichten verwendet die POST -Methode.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL-Kopfzeilen]</p> </td> 
      <td> <p>Einige Webdienste verwenden möglicherweise Kopfzeilen, um das API-Token oder andere Parameter für die Authentifizierung anzugeben. Dies ist in unserem Beispiel nicht der Fall, da der Endpunkt des Pushover für das Pushen von Nachrichten den Hauptteil (siehe unten) für alle Anfragetypen verwendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Abfragezeichenfolge]</p> </td> 
      <td> <p>Einige Webdienste verwenden möglicherweise eine Abfragezeichenfolge, um andere Parameter anzugeben. Dies ist in unserem Beispiel nicht der Fall, da der [!DNL Pushover]-Webdienst [!UICONTROL Body] (siehe unten) für alle Anfragetypen verwendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Texttyp]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Mit dieser Einstellung können Sie den JSON-Inhaltstyp im Feld [!UICONTROL Content Type] unten auswählen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON ist der erforderliche Inhaltstyp der [!UICONTROL Pushover]-App. Dies kann sich von anderen Web-Services unterscheiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Inhalt anfordern]</p> </td> 
      <td> <p>Geben Sie den Inhalt der [!UICONTROL Body]-Anfrage im JSON-Format ein. Sie können das Modul [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] verwenden, wie in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON-Hauptteil zugeordnet mit dem Modul [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] beschrieben</a> in diesem Artikel. Sie können den JSON-Inhalt auch manuell eingeben, wie in <a href="#json-body-entered-manually" class="MCXref xref">JSON-Text manuell eingegeben</a> in diesem Artikel beschrieben.</p> <p>Die erforderlichen Parameter für diesen Webdienst finden Sie in der API-Dokumentation des Webdienstes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Manuell eingegebener JSON-Text

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
   <td role="rowheader"> <p>[!UICONTROL-Benutzer]</p> </td> 
   <td> <p>Ihr USER_KEY. Diese finden Sie in Ihrem [!DNL Pushover]-Dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token] </td> 
   <td> <p>Ihr API-Token/API-Schlüssel, der generiert wurde, als Sie Ihre [!DNL Pushover] App erstellt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachricht] </td> 
   <td> <p>Der Textinhalt der Push-Benachrichtigung, die an das/die Gerät(e) gesendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Optional) Der Titel Ihrer Nachricht. Wenn kein Wert eingegeben wird, wird der Name Ihrer App verwendet. </p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-Text, der mithilfe des Moduls [!UICONTROL JSON] >[!UICONTROL Create JSON] zugeordnet wird

Das [!UICONTROL Create JSON]-Modul erleichtert die Angabe von JSON. Außerdem haben Sie die Möglichkeit, Werte dynamisch zu definieren.

Weitere Informationen zu den JSON-Modulen finden Sie unter [JSON-](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Geben Sie die Werte ein, aus denen Sie JSON erstellen möchten, oder ordnen Sie sie zu.

   ![](assets/json-values-350x288.png)

1. Verbinden Sie das Modul [!UICONTROL JSON] > [!UICONTROL JSON erstellen] mit dem Modul HTTP > Anfrage stellen .
1. Ordnen Sie die JSON-Zeichenfolge aus dem Modul [!UICONTROL JSON erstellen] dem Feld [!UICONTROL Inhalt anfordern] im Modul [!UICONTROL HTTP] >[!UICONTROL Anfrage erstellen] zu.

   Wenn Sie das Szenario jetzt ausführen, wird die Push-Benachrichtigung an das Gerät gesendet, das in Ihrem [!DNL Pushover]-Konto registriert wurde.
