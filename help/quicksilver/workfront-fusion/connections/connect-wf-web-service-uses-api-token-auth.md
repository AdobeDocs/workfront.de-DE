---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Verbinden Sie [!DNL Adobe Workfront Fusion] mit einem Webdienst, der die API-Token-Autorisierung verwendet
description: Einige Dienste ermöglichen es Integrationslösungen wie [!DNL Adobe Workfront Fusion] nicht, eine App zu erstellen, die Sie in Ihrem Szenario einfach verwenden können.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Verbinden Sie [!DNL Adobe Workfront Fusion] mit einem Webdienst, der die API-Token-Autorisierung verwendet

Einige Dienste ermöglichen es Integrationslösungen wie [!DNL Adobe Workfront Fusion] nicht, eine App zu erstellen, die Sie in Ihrem Szenario einfach verwenden können.

Es gibt eine Lösung für diese Situation. Sie können den gewünschten Dienst (App) mit [!DNL Workfront Fusion] über das [!UICONTROL HTTP]-Modul von [!DNL Workfront Fusion] verbinden.

In diesem Artikel wird erläutert, wie fast jeder Webdienst mit [!DNL Workfront Fusion] über einen API-Schlüssel/API-Token verbunden werden kann.

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Herstellen einer Verbindung zu einem Webdienst, der ein API-Token verwendet

Die Vorgehensweise zum Verbinden des Dienstes über ein API-Token ist für die meisten Webdienste ähnlich.

1. Erstellen Sie eine Anwendung auf der Website des Webdienstes, wie im Abschnitt [Erstellen einer neuen Anwendung und Abrufen des API-Tokens](#create-a-new-application-and-obtain-the-api-token) in diesem Artikel beschrieben.
1. Rufen Sie den API-Schlüssel oder das API-Token ab.
1. Fügen Sie Ihrem Szenario das Modul [!UICONTROL HTTP] > [!UICONTROL Eine Anforderung stellen] von [!DNL Workfront Fusion] hinzu.
1. Richten Sie das Modul gemäß der API-Dokumentation des Webdienstes ein und führen Sie das Szenario aus, wie im Abschnitt [Einrichten des [!UICONTROL HTTP]-Moduls](#set-up-the-http-module) in diesem Artikel beschrieben.

>[!NOTE]
>
>Wir werden den [!DNL Pushover]-Benachrichtigungsdienst in diesem Artikel als Beispiel verwenden.

## Erstellen einer neuen Anwendung und Abrufen des API-Tokens

>[!NOTE]
>
>Es gibt viele verschiedene Möglichkeiten, wie Webdienste API-Schlüssel oder API-Token erstellen und verteilen. Anweisungen zum Abrufen eines API-Schlüssels und -Tokens für Ihren gewünschten Webdienst finden Sie auf der Website des Diensts und suchen Sie nach &quot;API-Schlüssel&quot;oder &quot;API-Token&quot;.
>
>Wir enthalten Anweisungen zum Abrufen eines Pushover-API-Schlüssels nur als Beispiel dafür, was Sie finden.

1. Melden Sie sich bei Ihrem [!DNL Pushover] -Konto an.
1. Klicken Sie unten auf der Seite auf **[!UICONTROL Erstellen eines Anwendungs-/API-Tokens]** .
1. Füllen Sie die Anwendungsinformationen aus und klicken Sie auf **[!UICONTROL Anwendung erstellen]**.
1. Speichern Sie das bereitgestellte API-Token an einem sicheren Ort. Sie benötigen es, damit das Modul [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Eine Anforderung stellen] eine Verbindung zum gewünschten Webdienst herstellen kann ([!DNL Pushover], in diesem Fall).

## Einrichten des Moduls [!UICONTROL HTTP]

Um einen Webdienst mit Ihrem [!DNL Workfront Fusion]-Szenario zu verbinden, müssen Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] im Szenario verwenden und das Modul gemäß der API-Dokumentation des Webdienstes einrichten.

1. Fügen Sie das Modul [!UICONTROL HTTP] >[!UICONTROL Make a Request] zu Ihrem Szenario hinzu.
1. Um eine Nachricht mit [!DNL Workfront Fusion] zu pushen, richten Sie das HTTP-Modul wie folgt ein.

   >[!NOTE]
   >
   >Diese Moduleinstellungen entsprechen der Dokumentation zur Webdienst-API von [!DNL Pushover] . Die Einstellungen können für andere Webdienste unterschiedlich sein. Beispielsweise kann das API-Token in den [!UICONTROL Header] und nicht in das Feld [!UICONTROL Body] eingefügt werden.

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
      <td> <p>Einige Webdienste können eine Abfragezeichenfolge verwenden, um andere Parameter anzugeben. Dies ist in unserem Beispiel nicht der Fall, da der [!DNL Pushover] -Webdienst [!UICONTROL Body] (siehe unten) für alle Anfragetypen verwendet.</p> </td> 
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
      <td> <p>Geben Sie den Anforderungsinhalt des [!UICONTROL Hauptteils] im JSON-Format ein. Sie können das Modul [!UICONTROL JSON] &gt; [!UICONTROL JSON erstellen] verwenden, wie im Abschnitt "<a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON-Hauptteil, der mithilfe des Moduls [!UICONTROL JSON] &gt; [!UICONTROL JSON erstellen</a>"in diesem Artikel beschrieben wird. Alternativ können Sie den JSON-Inhalt manuell eingeben, wie in <a href="#json-body-entered-manually" class="MCXref xref">Manuell eingegebener JSON-Hauptteil</a> in diesem Artikel beschrieben.</p> <p>Die erforderlichen Parameter für diesen Webdienst finden Sie in der API-Dokumentation des Webdienstes .</p> </td> 
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
   <td> <p>Ihr USER_KEY. Dies finden Sie in Ihrem [!DNL Pushover]-Dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token] </td> 
   <td> <p>Ihr API-Token/API-Schlüssel, der generiert wurde, haben Sie Ihre [!DNL Pushover]-App erstellt.</p> </td> 
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

## JSON-Hauptteil, der mithilfe des Moduls [!UICONTROL JSON] >[!UICONTROL JSON erstellen] zugeordnet wurde

Das Modul [!UICONTROL JSON erstellen] erleichtert die Angabe von JSON. Sie können damit auch Werte dynamisch definieren.

Weitere Informationen zu den JSON-Modulen finden Sie unter [JSON-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Geben Sie die Werte ein oder ordnen Sie sie zu, aus denen JSON erstellt werden soll.

   ![](assets/json-values-350x288.png)

1. Verbinden Sie das Modul [!UICONTROL JSON] > [!UICONTROL JSON erstellen] mit HTTP > Anforderungsmodul.
1. Ordnen Sie die JSON-Zeichenfolge aus dem Modul [!UICONTROL JSON erstellen] dem Feld [!UICONTROL Inhalt anfordern] im Modul [!UICONTROL HTTP] >[!UICONTROL Anfordern] zu.

   Wenn Sie nun das Szenario ausführen, wird die Push-Benachrichtigung an das Gerät gesendet, das in Ihrem [!DNL Pushover] -Konto registriert wurde.
