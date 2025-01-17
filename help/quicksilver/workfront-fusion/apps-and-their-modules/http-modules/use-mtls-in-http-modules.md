---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: http-modules
title: Verwenden von gegenseitigem TLS in HTTP-Modulen in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# Verwenden von gegenseitigem TLS in HTTP-Modulen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Verwenden von gegenseitigem TLS in HTTP-Modulen in Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/use-mtls-in-http-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

>[!NOTE]
>
>Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine [!DNL Adobe Workfront Fusion].

## Gegenseitige TLS - Übersicht

Wenn Sie Daten über das Internet senden, müssen Sie sicherstellen, dass sie an den richtigen Ort gesendet werden oder von dort stammen und dass nur die vorgesehene Empfängerin oder der vorgesehene Empfänger sie lesen kann. Bei aktiviertem TLS verwendet der Client (Computer, der Informationen anfordert) Zertifikate, um die Identität des Servers zu überprüfen (Computer, der Informationen bereitstellt). Dadurch werden sichere HTTP-Verbindungen hergestellt.

Das gegenseitige TLS ermöglicht es, dass diese Identitätsbestätigung in beide Richtungen funktioniert. Wenn der Server sein Zertifikat sendet, um seine Identität zum Client zu überprüfen, fordert er auch das Zertifikat des Clients an. Dadurch wird sichergestellt, dass der Server keine Informationen an eine Website oder einen Benutzer sendet, die bzw. der sie missbrauchen würde.

>[!INFO]
>
>**Beispiel:**
>
>* **TLS**: Wenn eine Person „MyGreatBank.com“ in einen Browser eingibt, möchte sie sicherstellen, dass sie zu „My Great Bank“ geht und nicht zu einer Website, die ihre Bankinformationen missbrauchen oder verkaufen könnte. Sie möchten auch sicherstellen, dass ihre Bankkontoinformationen verschlüsselt sind.
>
>   Wenn der Browser (der Client) eine Verbindung zu MyGreatBank.com (dem Server) herstellt, erfordert TLS ein Zertifikat von MyGreatBank.com, um seine Identität zu überprüfen. Das Zertifikat wird von einer Zertifizierungsstelle wie [!DNL DigiCert] oder [!DNL Thawte] bereitgestellt. Da der Browser der Zertifizierungsstelle vertraut, lässt er die Verbindung zu.
>
>* **Mutual TLS**: MySoftware.com ist ein Software-Client, der Informationen von der MyGreatBank.com API benötigt. MyGreatBank erlaubt nur vertrauenswürdigen Kunden eine Verbindung zu ihren Servern herzustellen. Zusätzlich zum regulären TLS, das die Identität von MyGreatBank.com überprüft, überprüft der Prozess für TLS-/Zertifizierungsstellen auch die Anfrage von MySoftware.com.

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

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Bereitstellen Ihres [!DNL Workfront Fusion] öffentlichen Zertifikats


Wenn Sie über eine HTTP-Anfrage eine Verbindung zu einem Webdienst herstellen, benötigt der Webdienst in der Regel ein [!DNL Workfront Fusion] öffentliches Zertifikat zur Überprüfung. Auf diese Weise kann der Webdienst das in der HTTP-Anfrage dargestellte Zertifikat mit dem in der Datei enthaltenen vergleichen, um sicherzustellen, dass sich das Zertifikat auf der Zulassungsliste des Webdienstes befindet.

Anweisungen zum Hochladen des [!DNL Adobe Workfront Fusion] öffentlichen Zertifikats auf einen Webdienst finden Sie in der Dokumentation zum Webdienst.

>[!NOTE]
>
>Zusätzlich zum Zertifikat müssen Sie möglicherweise weitere Informationen angeben. Informationen dazu, was für einen Webdienst erforderlich ist, finden Sie in der API-Dokumentation des Webdienstes.

Über die folgenden Links können Sie die öffentlichen Workfront Fusion-Zertifikate herunterladen:

### Zertifikate für den 23. April 2023-7. Mai 2024

>[!IMPORTANT]
>
>* Diese [!DNL Workfront Fusion] öffentlichen Zertifikate laufen am 7. Mai 2025 ab. Nach Ablauf Ihres müssen Sie ein neues Zertifikat in den Webservice hochladen. Wir empfehlen Ihnen Folgendes:
>
>   * Notieren Sie sich das Ablaufdatum und legen Sie eine Erinnerung fest, damit Sie das Zertifikat in Ihren Webservice hochladen können.
>   * Setzen Sie ein Lesezeichen für diese Seite, um die neuen Zertifikate leicht zu finden.
>
>* Hierbei handelt es sich um Nicht-Platzhalter-TLS-Zertifikate.

* [download [!DNL Workfront Fusion] certificate 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [Download [!DNL Workfront Fusion] EU-Zertifikat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

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

## Aktivieren von gegenseitigem TLS in [!DNL Workfront Fusion] HTTP-Modulen

Alle [!DNL Workfront Fusion] [!UICONTROL HTTP]-Anfragemodule haben die Möglichkeit, gegenseitiges TLS zu aktivieren.

So aktivieren Sie gegenseitiges TLS in einem [!UICONTROL HTTP]-Anfragemodul:

1. Fügen Sie Ihrem [!UICONTROL  ein ]HTTP“-Anfragemodul hinzu.
1. Starten Sie die Konfiguration des Moduls.

   Anweisungen zum Konfigurieren eines [!UICONTROL HTTP]-Anfragemoduls finden Sie im entsprechenden Artikel unter [[!UICONTROL HTTP]-Module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Aktivieren Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]** unten im Modul.
1. Aktivieren **[!UICONTROL Gegenseitige TLS verwenden]**.
