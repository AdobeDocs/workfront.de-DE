---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Konfigurieren Sie die Einstellungen eines Moduls in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Konfigurieren der Einstellungen eines Moduls in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Konfigurieren eines Moduls](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/configure-a-modules-settings.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Sie müssen für jedes Modul, das Sie erstellen, Einstellungen konfigurieren.

Für die Module [[!DNL Dropbox] module](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) müssen Sie beispielsweise den Zielordner angeben, in den Sie Dateien hochladen möchten. Für die [[!UICONTROL E]Mail](../../workfront-fusion/apps-and-their-modules/email-modules.md)-Module müssen Sie die E-Mail-Adresse eingeben, an die die E-Mails gesendet werden sollen.

>[!NOTE]
>
>Neben den Moduleinstellungen können Sie auch Einstellungen für ein Szenario anpassen. Sie können unter anderem Ihr Szenario umbenennen, seinen Zeitplan ändern und zusätzliche Einstellungen angeben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
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

## Konfigurieren der Moduleinstellungen

1. Fügen Sie einem Szenario ein neues Modul hinzu.

   Oder

   Klicken Sie auf das Symbol des Moduls im Szenario-Editor, wie in [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) beschrieben.

1. Erstellen Sie bei Bedarf für das Modul eine **[!UICONTROL Verbindung]** zu Ihrem registrierten Benutzerkonto für diesen bestimmten Dienst, wie in [Verbindungen - Übersicht](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md) beschrieben.
1. Geben Sie in jedes Feld den entsprechenden Text ein.

   Oder

   Klicken Sie **[!UICONTROL Zuordnen]** wenn es rechts neben dem Feld angezeigt wird, und ordnen Sie dann ein Element aus einem anderen Modul in Ihrem Szenario zu.

   Fettgedruckte Parameter sind erforderlich.

   Informationen zu den verschiedenen Elementdatentypen, die [!DNL Workfront Fusion] erkennen können (z. B. Datum, Zahl und Text), finden Sie unter [Elementdatentypen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. (Bedingt) Wenn das Modul über erweiterte Optionen verfügt, die angezeigt und verwendet werden sollen, wählen Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]** aus.
