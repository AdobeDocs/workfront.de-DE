---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: HTTP &gt;Andere Module
description: Die  [!DNL Adobe Workfront Fusion] HTTP-App stellt verschiedene Kommunikationsmodule bereit, die auf dem HTTP-Protokoll (Hypertext Transfer Protocol) basieren. HTTP ist die Grundlage der Datenkommunikation für das World Wide Web. Sie können die Module verwenden, um Webseiten und Dateien herunterzuladen, Webhooks und API-Endpunkte aufzurufen usw.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# HTTP > Andere Module

>[!NOTE]
>
>Für [!UICONTROL Adobe Workfront Fusion] ist zusätzlich zu einer [!UICONTROL Adobe Workfront] -Lizenz eine [!UICONTROL Adobe Workfront Fusion] -Lizenz erforderlich.

Die App [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] stellt verschiedene Kommunikationsmodule bereit, die auf dem HTTP-Protokoll (Hypertext Transfer Protocol) basieren. HTTP ist die Grundlage der Datenkommunikation für das World Wide Web. Sie können die Module verwenden, um Webseiten und Dateien herunterzuladen, Webhooks und API-Endpunkte aufzurufen usw.

Die richtige Auswahl des Moduls hängt vom Authentifizierungs-/Autorisierungsmechanismus ab, den die Ressource verwendet, auf die Sie zugreifen möchten. Im Folgenden finden Sie Beispiele für Module

* Anfrage:universelles Modul, das hauptsächlich für Ressourcen bestimmt ist, die keine Authentifizierung/Autorisierung durchführen
* Erstellen einer einfachen Authentifizierungsanfrage:für Ressourcen mit [!DNL HTTP] Standardauthentifizierung (BA)
* Anfrage für OAuth 2.0: für Ressourcen, die das OAuth 2.0-Autorisierungsprotokoll verwenden
* Erstellen Sie eine Client-Zertifikatauthentifizierungsanfrage: für Ressourcen, die ein Autorisierungsprotokoll verwenden, für das ein clientseitiges Zertifikat erforderlich ist.
* Anfrage zur API-Schlüsselautorisierung: für Ressourcen, die API-Schlüssel zur Autorisierung verwenden.

>[!NOTE]
>
>Wenn Sie eine Verbindung zu einem Adobe-Produkt herstellen, das derzeit über keinen dedizierten Connector verfügt, empfehlen wir die Verwendung des Adobe Authenticator-Moduls.
>
>Weitere Informationen finden Sie unter [Adobe Authenticator-Modul](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Anforderungsmodule

Spezifische Anweisungen für Anfragemodule finden Sie in den folgenden Artikeln:

* [[!UICONTROL HTTP] >[!UICONTROL Stellen eines Anfrage-Moduls]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Erstellen eines einfachen Autorisierungsanfragemoduls]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Erstellen eines OAuth 2.0-Anfrage-Moduls]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Erstellen eines Moduls zur Autorisierung von Clientzertifikaten]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Eine API-Schlüsselautorisierungsanforderung stellen]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Andere Aktionsmodule

* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Auflösen einer Ziel-URL]](#resolve-a-target-url)

### [!UICONTROL Datei abrufen]

Dieses Aktionsmodul lädt eine Datei von der angegebenen URL herunter. Nachdem die Datei heruntergeladen wurde, können Sie die Datei weiter verarbeiten (die Dateidaten zuordnen), indem Sie im Szenario andere Module verwenden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Geben Sie die URL der Datei ein oder ordnen Sie sie zu. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Auflösen einer Ziel-URL]

Dieses Aktionsmodul löst eine Kette von HTTP-Weiterleitungen auf und gibt eine Ziel-URL zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Geben Sie die URL ein oder ordnen Sie sie zu, die Sie auflösen möchten, z. B. eine [!DNL bit.ly]-URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode] </td> 
   <td> <p>Wählen Sie aus, ob Sie die [!UICONTROL HEAD]-Methode oder die [!UICONTROL GET]-Methode verwenden möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iterator-Module

### [!UICONTROL Header abrufen]

Dieses Modul gibt jeden Header (Name und Wert) des angegebenen HTTP-Moduls in einem separaten Bundle zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Wählen Sie das Modul aus, aus dem Sie Kopfzeilen abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-Web-Token (JWT) erstellen

Es ist möglich, mithilfe integrierter Funktionen ein JWT-Token zu generieren:

Kopfzeile:

![](assets/jwt-header-350x19.png)

Code für Kopieren und Einfügen:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Nutzlast:

![](assets/jwt-payload-350x17.png)

Code für Kopieren und Einfügen:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Code für Kopieren und Einfügen:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
