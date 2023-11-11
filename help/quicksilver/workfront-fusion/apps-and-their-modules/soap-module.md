---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: SOAP-Modul
description: Sie können das SOAP-Modul verwenden, um eine Verbindung zu SOAP-APIs in Adobe Workfront Fusion herzustellen.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL SOAP] Modul

Sie können die [!UICONTROL SOAP] Modul zum Herstellen einer Verbindung [!UICONTROL SOAP] APIs in [!UICONTROL Adobe Workfront Fusion].

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verwenden der [!UICONTROL SOAP] Modul

Die [!UICONTROL SOAP] -Modul befindet sich derzeit in der Betaphase und unterstützt nicht:

* Elemente neu definieren
* Einschränkungen für Bruchziffern
* Beschränkungen für die Gesamtanzahl der Stellen
* Leerraumbeschränkungen
* Mehrere Teile in Eingabe- und Ausgabemeldungen. Es werden nur einteilige Nachrichten unterstützt
* Benutzerdefinierte XML-Schemaelemente, die mithilfe von [[!UICONTROL SOAP] Kodierung](https://schemas.xmlsoap.org) Schemas und Elemente.

>[!INFO]
>
>**Beispiel:**
>  
>Folgendes würde nicht richtig erkannt durch [!UICONTROL Workfront Fusion]:
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

Er enthält die `soapenc:Array`, `soapenc:arrayType` und `wsdl:arrayType` -Verweise, die noch nicht unterstützt werden in [!UICONTROL Workfront Fusion].

## Problemumgehung

Wenn die Variable [!UICONTROL SOAP] -Modul weigert sich, die WSDL-Datei zu verarbeiten oder gibt verschiedene Fehler in der Konfiguration des Moduls aus. Sie können versuchen, die universelle **[!UICONTROL HTTP] > [!UICONTROL Anfrage stellen]** -Modul stattdessen:

1. In [!DNL Workfront Fusion], erstellen Sie ein neues Szenario.
1. Fügen Sie die **[!UICONTROL HTTP] > [!UICONTROL Anfrage stellen]** -Modul im Szenario.
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

   Die WSDL-URL endet normalerweise mit `?wsdl`, aber nicht notwendigerweise, zum Beispiel `http://voip.ms/api/v1/server.wsdl`.

1. Wenn die WSDL-Datei nicht direkt im Webbrowser angezeigt wird, öffnen Sie die heruntergeladene Datei in einem Texteditor.
1. Suchen Sie nach `<service>` oder `<wsdl:service>` Tag:

   ![](assets/service-350x65.png)

1. Kopieren Sie nach dem Speicherort die URL aus der `location` -Attribut.
1. In [!DNL Workfront Fusion], fügen Sie die URL in das URL-Feld des HTTP-Moduls ein.
1. Öffnen Sie die [Online [!UICONTROL SOAP] Client](https://wsdlbrowser.com/) in einem neuen Webbrowserfenster/-tab.
1. Fügen Sie die WSDL-URL in das Feld WSDL-URL ein.
1. Klicks **[!UICONTROL Durchsuchen]**.
1. Wählen Sie aus der Funktionsliste nach links, z. B. `getLanguages`.
1. Kopieren Sie den Inhalt der [!UICONTROL XML anfordern] Textbereich.
1. In [!UICONTROL Workfront Fusion], fügen Sie den kopierten Inhalt in das URL-Feld des Moduls ein.
1. Geben Sie Werte für ausgewählte Parameter an, indem Sie die Fragezeichen durch tatsächliche Werte ersetzen:

   ![](assets/request-xml-350x172.png)

1. Schließen Sie die Konfiguration des Moduls, indem Sie auf **[!UICONTROL OK]**.
1. Führen Sie das Szenario oder Modul aus.
