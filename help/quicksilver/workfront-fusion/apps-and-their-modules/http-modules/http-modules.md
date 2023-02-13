---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Sonstige Module
description: Die [!DNL Adobe Workfront Fusion] Die HTTP-App bietet verschiedene Kommunikationsmodule, die auf dem HTTP-Protokoll (Hypertext Transfer Protocol) basieren. HTTP ist die Grundlage der Datenkommunikation für das World Wide Web. Sie können die Module verwenden, um Webseiten und Dateien herunterzuladen, Webhooks und API-Endpunkte aufzurufen usw.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > Andere Module

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] erfordert [!UICONTROL Adobe Workfront Fusion] zusätzlich zu einer [!UICONTROL Adobe Workfront] Lizenz.

Die [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] app stellt verschiedene Kommunikationsmodule für das HTTP-Protokoll (Hypertext Transfer Protocol) bereit. HTTP ist die Grundlage der Datenkommunikation für das World Wide Web. Sie können die Module verwenden, um Webseiten und Dateien herunterzuladen, Webhooks und API-Endpunkte aufzurufen usw.

Die richtige Auswahl des Moduls hängt vom Authentifizierungs-/Autorisierungsmechanismus ab, den die Ressource verwendet, auf die Sie zugreifen möchten. Im Folgenden finden Sie Beispiele für Module

* Anfrage:universelles Modul, das hauptsächlich für Ressourcen bestimmt ist, die keine Authentifizierung/Autorisierung durchführen
* Erstellen einer einfachen Authentifizierungsanfrage:für Ressourcen, die [!DNL HTTP] Standardauthentifizierung (BA)
* Erstellen Sie eine OAuth 2.0-Anfrage: für Ressourcen, die das OAuth 2.0-Autorisierungsprotokoll verwenden
* Erstellen Sie eine Client-Zertifikatauthentifizierungsanforderung: für Ressourcen, die ein Autorisierungsprotokoll verwenden, für das ein clientseitiges Zertifikat erforderlich ist.
* Stellen Sie eine API-Schlüsselautorisierungsanfrage: für Ressourcen, die API-Schlüssel zur Autorisierung verwenden.

## Anforderungsmodule

Spezifische Anweisungen für Anfragemodule finden Sie in den folgenden Artikeln:

* [[!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] Modul](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Einfache Genehmigungsanfrage stellen] Modul](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0-Anfrage stellen] Modul](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Anforderung einer Client-Zertifikatautorisierung stellen] Modul](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL API-Schlüsselautorisierungsanfrage stellen]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

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
   <td> <p>Geben Sie die URL der Datei ein, die Sie herunterladen möchten, oder ordnen Sie sie zu. </p> </td> 
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
   <td> <p>Geben Sie die URL ein oder ordnen Sie sie zu, die Sie auflösen möchten, z. B. eine [!DNL bit.ly] URL.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Quellmodul]</td> 
   <td> <p> Wählen Sie das Modul aus, aus dem Sie Kopfzeilen abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-Web-Token (JWT) erstellen

Es ist möglich, mithilfe integrierter Funktionen ein JWT-Token zu generieren:

Header:

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
