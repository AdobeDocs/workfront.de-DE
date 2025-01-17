---
title: Verschlüsseler
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Verschlüsseler

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Encryptor](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/encryptor-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

[!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor]-Module ermöglichen die Verschlüsselung von Textdaten. Sie unterstützen derzeit die Nachrichtenverschlüsselung über AES256 und PGP ([!UICONTROL OpenPGP]).

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Nachrichtenverschlüsselung und -entschlüsselung mit PGP

Beim Ver- und Entschlüsseln mit PGP muss ein Schlüsselbund verwendet und ein privater oder öffentlicher Schlüssel (oder beides) erstellt werden.

Weitere Informationen zu öffentlichen und privaten Schlüsseln finden Sie unter [Allgemeine Begriffe in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Weitere Informationen zu Schlüsselbändern finden Sie unter [Schlüssel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Encryptor]-Module und ihre Felder

Beim Konfigurieren von [!UICONTROL Encryptor]-Modulen werden die folgenden Felder angezeigt. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

### Verschlüsseln einer PGP-Nachricht

Dieses Modul ermöglicht die Verschlüsselung von Nachrichten mit öffentlichen und privaten Schlüsseln.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Privater Schlüssel]</td>
        <td>Geben Sie den privaten Schlüssel des Absenders ein. Dadurch kann die Identität des Absenders authentifiziert werden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Öffentlicher Schlüssel]</td>
        <td>Geben Sie den öffentlichen Schlüssel des Empfängers ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nachricht]</td>
        <td>Geben Sie die Nachricht ein, die Sie verschlüsseln möchten.</td>
    </tr>

### Entschlüsseln einer PGP-Nachricht

Mit diesem Modul können Sie eine Nachricht mit öffentlichen und privaten Schlüsseln entschlüsseln.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Privater Schlüssel]</td>
        <td>Geben Sie den privaten Schlüssel des Empfängers ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Öffentlicher Schlüssel]</td>
        <td>Geben Sie den öffentlichen Schlüssel des Empfängers ein. Dadurch kann die Identität des Absenders authentifiziert werden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nachricht]</td>
        <td>Ordnen Sie die Nachricht zu, die Sie entschlüsseln möchten.</td>
    </tr>
</table>
