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
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Verwenden von TLS auf Gegenseitige Weise in HTTP-Modulen in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine [!DNL Adobe Workfront Fusion] -Lizenz.

## Übersicht über TLS für beide Seiten

Wenn Sie Daten über das Internet senden, müssen Sie sicherstellen, dass sie an den richtigen Ort übermittelt werden oder von dort stammen und dass nur der vorgesehene Empfänger sie lesen kann. Wenn TLS aktiviert ist, verwendet der Client (Computer, der Informationen anfordert) Zertifikate, um die Identität des Servers zu überprüfen (Computer, der Informationen bereitstellt). Dadurch werden sichere HTTP-Verbindungen hergestellt.

Durch gegenseitige TLS kann diese Identitätsbestätigung auf beide Arten erfolgen. Wenn der Server sein Zertifikat sendet, um seine Identität an den Client zu überprüfen, fordert er auch das Zertifikat des Clients an. Dadurch wird sichergestellt, dass der Server keine Informationen an eine Site oder einen Benutzer sendet, die sie missbrauchen würden.

>[!INFO]
>
>**Beispiel:**
>
>* **TLS**: Wenn eine Person &quot;MyGreatBank.com&quot;in einen Browser eingibt, möchte sie sicher sein, dass sie zu &quot;My Great Bank&quot;geht, nicht zu einer Website, die ihre Bankinformationen missbrauchen oder verkaufen könnte. Sie wollen auch sicherstellen, dass ihre Bankkontoinformationen verschlüsselt sind.
>
>   Wenn der Browser (der Client) eine Verbindung zu MyGreatBank.com (dem Server) herstellt, erfordert TLS ein Zertifikat von MyGreatBank.com , um seine Identität zu überprüfen. Das Zertifikat wird von einer Zertifizierungsstelle wie [!DNL DigiCert] oder [!DNL Thawte] bereitgestellt. Da der Browser der Zertifizierungsstelle vertraut, ermöglicht er die Verbindung.
>
>* **Mutual TLS**: MySoftware.com ist ein Software-Client, der Informationen von der MyGreatBank.com API benötigt. MyGreatBank ermöglicht es nur vertrauenswürdigen Clients, eine Verbindung zu ihren Servern herzustellen. Zusätzlich zu den regulären TLS, die die Identität von MyGreatBank.com überprüfen, überprüft der TLS-/Zertifikatauthentifizierungsprozess auch die Anfrage von MySoftware.com.

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

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Bereitstellen Ihres öffentlichen [!DNL Workfront Fusion] Zertifikats


Wenn Sie mit einer HTTP-Anforderung eine Verbindung zu einem Webdienst herstellen, erfordert der Webdienst normalerweise ein öffentliches Zertifikat vom Typ &quot;[!DNL Workfront Fusion]&quot; zur Überprüfung. Dadurch kann der Webdienst das in der HTTP-Anforderung angezeigte Zertifikat mit dem in der Datei vergleichen, um sicherzustellen, dass das Zertifikat auf der Zulassungsliste des Webdiensts vorhanden ist.

Anweisungen zum Hochladen des öffentlichen Zertifikats [!DNL Adobe Workfront Fusion] in einen Webdienst finden Sie in der Dokumentation des Webdienstes.

>[!NOTE]
>
>Möglicherweise müssen Sie zusätzlich zum Zertifikat weitere Informationen angeben. Informationen dazu, was ein Webdienst erfordert, finden Sie in der API-Dokumentation des Webdienstes .

Sie können die folgenden Links verwenden, um die öffentlichen Workfront Fusion-Zertifikate herunterzuladen:

### Zertifikate für den 23. April 2023-7. Mai 2024

>[!IMPORTANT]
>
>* Diese öffentlichen [!DNL Workfront Fusion] Zertifikate laufen am 7. Mai 2025 ab. Nach Ablauf Ihrer Gültigkeit müssen Sie ein neues Zertifikat in den Webdienst hochladen. Wir empfehlen Ihnen Folgendes:
>
>   * Notieren Sie sich das Ablaufdatum und erinnern Sie Sie sich daran, das Zertifikat in Ihren Webdienst hochzuladen.
>   * Markieren Sie diese Seite, um die neuen Zertifikate einfach zu finden.
>
>* Dies sind mTLS-Zertifikate ohne Platzhalter.

* [Herunterladen [!DNL Workfront Fusion] Zertifikat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [Herunterladen [!DNL Workfront Fusion] EU-Zertifikat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

  Zur Verwendung in der EU

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## Aktivieren von TLS auf Gegenseitige Weise in [!DNL Workfront Fusion] HTTP-Modulen

Alle [!DNL Workfront Fusion] [!UICONTROL HTTP]-Anforderungsmodule haben die Möglichkeit, gegenseitige TLS zu aktivieren.

So aktivieren Sie gegenseitige TLS in einem [!UICONTROL HTTP]-Anforderungsmodul:

1. Fügen Sie Ihrem Szenario ein [!UICONTROL HTTP]-Anforderungsmodul hinzu.
1. Beginnen Sie mit der Konfiguration des Moduls.

   Anweisungen zum Konfigurieren eines [!UICONTROL HTTP]-Anfragemoduls finden Sie im entsprechenden Artikel unter [[!UICONTROL HTTP] -Module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Aktivieren Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]** am unteren Rand des Moduls.
1. Aktivieren Sie **[!UICONTROL Use Mutual TLS]**.
