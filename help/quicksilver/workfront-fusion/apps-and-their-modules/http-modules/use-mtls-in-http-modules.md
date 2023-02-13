---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: http-modules
title: Verwenden von TLS auf Gegenseitigkeit in HTTP-Modulen in Adobe Workfront Fusion
description: Sie können in Ihren Adobe Workfront Fusion-HTTP-Modulen "Mutual TLS"verwenden, sodass beide Seiten der Informationstransaktion die Identität des anderen überprüfen können.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 595d6e3e0a7d87240644bf20efd425917f4d953d
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Verwenden von TLS auf Gegenseitigkeit in HTTP-Modulen in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion erfordert eine [!DNL Adobe Workfront Fusion] zusätzlich zu einer Adobe Workfront-Lizenz.

## Übersicht über TLS für beide Seiten

Wenn Sie Daten über das Internet senden, müssen Sie sicherstellen, dass sie an den richtigen Ort übermittelt werden oder von dort stammen und dass nur der vorgesehene Empfänger sie lesen kann. Wenn TLS aktiviert ist, verwendet der Client (Computer, der Informationen anfordert) Zertifikate, um die Identität des Servers zu überprüfen (Computer, der Informationen bereitstellt). Dadurch werden sichere HTTP-Verbindungen hergestellt.

Durch gegenseitige TLS kann diese Identitätsbestätigung auf beide Arten erfolgen. Wenn der Server sein Zertifikat sendet, um seine Identität an den Client zu überprüfen, fordert er auch das Zertifikat des Clients an. Dadurch wird sichergestellt, dass der Server keine Informationen an eine Site oder einen Benutzer sendet, die sie missbrauchen würden.

>[!INFO]
>
>**Beispiel:**
>
>* **TLS**: Wenn eine Person &quot;MyGreatBank.com&quot;in einen Browser eingibt, will sie sicher sein, dass sie zu My Great Bank geht, nicht zu einer Website, die ihre Bankinformationen missbrauchen oder verkaufen könnte. Sie wollen auch sicherstellen, dass ihre Bankkontoinformationen verschlüsselt sind.
   >
   >   Wenn der Browser (der Client) eine Verbindung zu MyGreatBank.com (dem Server) herstellt, benötigt TLS ein Zertifikat von MyGreatBank.com, um seine Identität zu überprüfen. Die Bescheinigung wird von einer Zertifizierungsstelle wie [!DNL DigiCert] oder [!DNL Thawte]. Da der Browser der Zertifizierungsstelle vertraut, ermöglicht er die Verbindung.
>
>* **TLS auf Gegenseitigkeit**: MySoftware.com ist ein Software-Client, der Informationen von der MyGreatBank.com API benötigt. MyGreatBank ermöglicht es nur vertrauenswürdigen Clients, eine Verbindung zu ihren Servern herzustellen. Zusätzlich zu den regulären TLS, die die Identität von MyGreatBank.com überprüfen, überprüft der Prozess der TLS/Certificate Authority auch die Anfrage von MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion für Arbeitsautomatisierung und -integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

&#42;&#42;Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Bereitstellung Ihrer [!DNL Workfront Fusion] öffentliches Zertifikat


Wenn Sie eine Verbindung zu einem Webdienst mit einer HTTP-Anforderung herstellen, erfordert der Webdienst normalerweise eine [!DNL Workfront Fusion] öffentliches Zertifikat zur Überprüfung. Dadurch kann der Webdienst das in der HTTP-Anforderung angezeigte Zertifikat mit dem in der Datei vergleichen, um sicherzustellen, dass das Zertifikat auf der Zulassungsliste des Webdiensts vorhanden ist.

Anweisungen zum Hochladen der [!DNL Adobe Workfront Fusion] ein öffentliches Zertifikat für einen Webdienst verwenden, siehe die Dokumentation des Webdienstes .

>[!NOTE]
>
>Möglicherweise müssen Sie zusätzlich zum Zertifikat weitere Informationen angeben. Informationen dazu, was ein Webdienst erfordert, finden Sie in der API-Dokumentation des Webdienstes .

Sie können die folgenden Links verwenden, um die öffentlichen Workfront Fusion-Zertifikate herunterzuladen:

### Zertifikate für den 14. November 2022 - 15. Juli 2023

>[!IMPORTANT]
>
>Diese [!DNL Workfront Fusion] öffentliche Zertifikate laufen am 15. Juli 2023 aus. Nach Ablauf Ihrer Gültigkeit müssen Sie ein neues Zertifikat in den Webdienst hochladen. Wir empfehlen Ihnen Folgendes:
>
>* Notieren Sie sich das Ablaufdatum und erinnern Sie Sie sich daran, das Zertifikat in Ihren Webdienst hochzuladen.
>* Markieren Sie diese Seite, um die neuen Zertifikate einfach zu finden.
>


* [Download [!DNL Workfront Fusion] Zertifikat 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU-Zertifikat 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   Zur Verwendung in der EU

<!--

Previous US cert

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app_workfrontfusion_com-jul-15-2023.cer)

### Certificates for November 17, 2021 - November 14, 2022

>[!IMPORTANT]
>
>These certificates expire on November 14, 2022. Upload the new certificates to the web service as soon as possible.

* [Download Workfront Fusion Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
* [Download Workfront Fusion EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt)

  For use in the EU

  -->

## Aktivieren der bidirektionalen TLS in [!DNL Workfront Fusion] HTTP-Module

Alle [!DNL Workfront Fusion] [!UICONTROL HTTP] -Anfragemodule haben die Möglichkeit, &quot;Mutual TLS&quot;zu aktivieren.

So aktivieren Sie gegenseitige TLS in einer [!UICONTROL HTTP] Anfragemodul:

1. Hinzufügen einer [!UICONTROL HTTP] -Anfragemodul zu Ihrem Szenario hinzufügen.
1. Beginnen Sie mit der Konfiguration des Moduls.

   Anweisungen zum Konfigurieren eines [!UICONTROL HTTP] Anforderungsmodul, siehe den entsprechenden Artikel unter [[!UICONTROL HTTP] Module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Aktivieren **[!UICONTROL Erweiterte Einstellungen anzeigen]** am unteren Rand des Moduls.
1. Aktivieren **[!UICONTROL Verwenden von TLS auf Gegenseitigkeit]**.
