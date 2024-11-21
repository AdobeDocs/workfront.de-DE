---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: SOAP-Modul
description: Sie können das SOAP-Modul verwenden, um eine Verbindung zu SOAP APIs in Adobe Workfront Fusion herzustellen.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 1%

---

# Modul [!UICONTROL SOAP]

Sie können das Modul [!UICONTROL SOAP] verwenden, um eine Verbindung zu [!UICONTROL SOAP] APIs in [!UICONTROL Adobe Workfront Fusion] herzustellen.

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

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Einschränkungen des Moduls [!UICONTROL SOAP]

>[!NOTE]
>
>Umleitungen werden während des WDSL-Ladens deaktiviert. Dies ist eine Sicherheitsfunktion, kann jedoch bedeuten, dass nicht überprüfte Weiterleitungen blockiert werden, wenn das Modul ausgeführt wird.

Das Modul [!UICONTROL SOAP] befindet sich derzeit in der Beta-Phase und unterstützt nicht:

* Elemente neu definieren
* Einschränkungen für Bruchziffern
* Beschränkungen für die Gesamtanzahl der Stellen
* Leerraumbeschränkungen
* Mehrere Teile in Eingabe- und Ausgabemeldungen. Es werden nur einteilige Nachrichten unterstützt
* Benutzerdefinierte XML-Schemaelemente, die mithilfe von Schemas und Elementen vom Typ [[!UICONTROL SOAP] Kodierung](https://schemas.xmlsoap.org) definiert wurden.

>[!INFO]
>
>**Beispiel:**
>  
>Folgendes wird von [!UICONTROL Workfront Fusion] nicht richtig erkannt:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```
>
>In diesem Beispiel sind die Verweise `soapenc:Array`, `soapenc:arrayType` und `wsdl:arrayType` enthalten, die in [!UICONTROL Workfront Fusion] noch nicht unterstützt werden.

## Workaround

Wenn das Modul [!UICONTROL SOAP] die Verarbeitung der WSDL-Datei ablehnt oder verschiedene Fehler in der Konfiguration des Moduls ausgibt, können Sie stattdessen das universelle Modul **[!UICONTROL HTTP] > [!UICONTROL Anfrage senden]** verwenden:

1. Erstellen Sie in [!DNL Workfront Fusion] ein neues Szenario.
1. Fügen Sie das Modul **[!UICONTROL HTTP] > [!UICONTROL Anfrage stellen]** in das Szenario ein.
1. Öffnen Sie die Konfiguration des Moduls und füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Methode]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Textkörper]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Inhaltstyp]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Aktiviert]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Öffnen Sie ein neues Webbrowser-Fenster oder eine neue Registerkarte.
1. Fügen Sie die WSDL-URL in die Adressleiste des Webbrowsers ein und rufen Sie die XML-Datei ab.

   Die WSDL-URL endet normalerweise mit `?wsdl`, jedoch nicht unbedingt, z. B. `http://voip.ms/api/v1/server.wsdl`.

1. Wenn die WSDL-Datei nicht direkt im Webbrowser angezeigt wird, öffnen Sie die heruntergeladene Datei in einem Texteditor.
1. Suchen Sie nach dem Tag `<service>` oder `<wsdl:service>` :

   ![](assets/service-350x65.png)

1. Kopieren Sie nach dem Speicherort die URL aus dem Attribut `location` .
1. Fügen Sie in [!DNL Workfront Fusion] die URL in das URL-Feld des HTTP-Moduls ein.
1. Öffnen Sie den [Online [!UICONTROL SOAP] Client](https://wsdlbrowser.com/) in einem neuen Webbrowserfenster/-registerkarte.
1. Fügen Sie die WSDL-URL in das Feld WSDL-URL ein.
1. Klicken Sie auf **[!UICONTROL Durchsuchen]**.
1. Wählen Sie aus der Funktionsliste nach links, z. B. `getLanguages`.
1. Kopieren Sie den Inhalt des Textbereichs [!UICONTROL XML anfordern] .
1. Fügen Sie in [!UICONTROL Workfront Fusion] den kopierten Inhalt in das Feld URL des Moduls ein.
1. Geben Sie Werte für ausgewählte Parameter an, indem Sie die Fragezeichen durch tatsächliche Werte ersetzen:

   ![](assets/request-xml-350x172.png)

1. Schließen Sie die Konfiguration des Moduls, indem Sie auf **[!UICONTROL OK]** klicken.
1. Führen Sie das Szenario oder Modul aus.
