---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: SOAP-Modul
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# [!UICONTROL SOAP]-Modul

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [SOAP-Modul](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/soap-module.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Sie können das Modul [!UICONTROL SOAP] verwenden, um eine Verbindung zu [!UICONTROL SOAP]-APIs in [!UICONTROL Adobe Workfront Fusion herzustellen].

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

## Einschränkungen des [!UICONTROL SOAP]-Moduls

>[!NOTE]
>
>Umleitungen sind beim Laden von WSDL deaktiviert. Dies ist eine Sicherheitsfunktion, kann jedoch bedeuten, dass nicht verifizierte Weiterleitungen blockiert werden, wenn das Modul ausgeführt wird.

Das [!UICONTROL SOAP]-Modul befindet sich derzeit in der Beta-Phase und unterstützt nicht:

* Elemente neu definieren
* Einschränkungen für Bruchziffern
* Einschränkungen für Ziffernstellen insgesamt
* Einschränkungen bei Leerzeichen
* Mehrere Teile in Ein- und Ausgabemeldungen. Es werden nur Einzelteilnachrichten unterstützt
* Benutzerdefinierte XML-Schemaelemente, die mithilfe von [[!UICONTROL SOAP]-Codierung](https://schemas.xmlsoap.org) Schemata und -elementen definiert wurden.

>[!INFO]
>
>**Beispiel:**
>  
>Folgendes würde von [!UICONTROL Workfront Fusion nicht korrekt erkannt]:
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
>Dieses Beispiel enthält die Verweise `soapenc:Array`, `soapenc:arrayType` und `wsdl:arrayType`, die in [!UICONTROL Workfront Fusion noch nicht unterstützt ].

## Abhilfe

Wenn das [!UICONTROL SOAP]-Modul die Verarbeitung der WSDL-Datei ablehnt oder verschiedene Fehler in der Modulkonfiguration auslöst, können Sie stattdessen das Modul Universal **[!UICONTROL HTTP] > [!UICONTROL Anfrage]** verwenden:

1. Erstellen Sie [!DNL Workfront Fusion] ein neues Szenario.
1. Fügen Sie das Modul **[!UICONTROL HTTP] > [!UICONTROL Anfrage stellen]** in das Szenario ein.
1. Öffnen Sie die Konfiguration des Moduls und füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Methode]</td> 
      <td> <p>[!UICONTROL-POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Texttyp]</td> 
      <td> <p>[!UICONTROL Roh]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content-Typ]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL aktiviert]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Öffnen Sie ein neues Webbrowser-Fenster oder eine neue Registerkarte.
1. Fügen Sie die WSDL-URL in die Adressleiste des Webbrowsers ein und rufen Sie die XML-Datei ab.

   Die WSDL-URL endet normalerweise mit `?wsdl`, aber nicht notwendigerweise, z. B. `http://voip.ms/api/v1/server.wsdl`.

1. Wenn die WSDL-Datei nicht direkt im Webbrowser angezeigt wird, öffnen Sie die heruntergeladene Datei in einem Texteditor.
1. Suchen Sie nach dem `<service>`- oder `<wsdl:service>`-Tag:

   ![](assets/service-350x65.png)

1. Kopieren Sie nach dem Auffinden die URL aus dem `location`.
1. Fügen Sie [!DNL Workfront Fusion] die URL in das URL-Feld des HTTP-Moduls ein.
1. Öffnen Sie den [Online [!UICONTROL SOAP]-Client](https://wsdlbrowser.com/) in einem neuen Webbrowser-Fenster/-Registerkarte.
1. Fügen Sie die WSDL-URL in das Feld WSDL-URL ein.
1. Klicken Sie **[!UICONTROL Durchsuchen]**.
1. Wählen Sie aus der Liste der Funktionen links aus, z. B. `getLanguages`.
1. Kopieren Sie den Inhalt des Textbereichs [!UICONTROL Anfrage]XML).
1. Fügen Sie in [!UICONTROL Workfront Fusion] den kopierten Inhalt in das URL-Feld des Moduls ein.
1. Geben Sie Werte für ausgewählte Parameter an, indem Sie die Fragezeichen durch die tatsächlichen Werte ersetzen:

   ![](assets/request-xml-350x172.png)

1. Schließen Sie die Modulkonfiguration, indem Sie auf **[!UICONTROL OK]** klicken.
1. Führen Sie das Szenario oder Modul aus.
