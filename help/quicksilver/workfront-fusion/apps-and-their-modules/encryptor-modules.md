---
title: Encryptor
description: Mit den Adobe Workfront Fusion Encryptor-Modulen können Sie alle Textdaten verschlüsseln. Sie unterstützen derzeit die Verschlüsselung von Nachrichten über AES256 und PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Encryptor

Mit den Modulen [!DNL Adobe Workfront Fusion] [!UICONTROL Verschlüsseler] können Sie alle Textdaten verschlüsseln. Sie unterstützen derzeit die Verschlüsselung von Nachrichten über AES256 und PGP ([!UICONTROL OpenPGP]).

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Nachrichtenverschlüsselung und -entschlüsselung mithilfe von PGP

Beim Verschlüsseln und Entschlüsseln über PGP muss eine Schlüsselkette verwendet und ein privater oder öffentlicher Schlüssel (oder beides) erstellt werden.

Weitere Informationen zu öffentlichen und privaten Schlüsseln finden Sie unter [Grundlegende Begriffe in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Weitere Informationen zu Schlüsselketten finden Sie unter [Schlüssel in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Verschlüsseler] -Module und ihre Felder

Beim Konfigurieren von Modulen des Typs [!UICONTROL Verschlüsseler] werden die folgenden Felder angezeigt. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

### PGP-Nachricht verschlüsseln

Mit diesem Modul können Sie eine Nachricht mit öffentlichen und privaten Schlüsseln verschlüsseln.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Privater Schlüssel]</td>
        <td>Geben Sie den privaten Schlüssel des Absenders ein. Dadurch kann die Identität des Absenders authentifiziert werden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Geben Sie den öffentlichen Schlüssel des Empfängers ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nachricht]</td>
        <td>Geben Sie die Nachricht ein, die Sie verschlüsseln möchten.</td>
    </tr>

### PGP-Nachricht entschlüsseln

Mit diesem Modul können Sie eine Nachricht mit öffentlichen und privaten Schlüsseln entschlüsseln.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Privater Schlüssel]</td>
        <td>Geben Sie den privaten Schlüssel des Empfängers ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Geben Sie den öffentlichen Schlüssel des Empfängers ein. Dadurch kann die Identität des Absenders authentifiziert werden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nachricht]</td>
        <td>Ordnen Sie die Nachricht zu, die Sie entschlüsseln möchten.</td>
    </tr>
</table>
