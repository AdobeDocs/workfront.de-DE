---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Veröffentlichen und freigeben [!DNL Adobe Workfront Fusion] templates
description: Wenn Sie eine Vorlage erstellen, wird Ihre Vorlage für alle Teammitglieder verfügbar. Wenn Sie die Vorlage für eine Person außerhalb Ihres Teams freigeben möchten, müssen Sie sie zuerst veröffentlichen.
author: Becky
feature: Workfront Fusion
exl-id: aaa59a1e-aa16-41f5-9f56-ce0615c1b685
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Veröffentlichen und freigeben [!DNL Adobe Workfront Fusion] templates

Wenn Sie eine Vorlage erstellen, wird Ihre Vorlage für alle Teammitglieder verfügbar. Wenn Sie die Vorlage für eine Person außerhalb Ihres Teams freigeben möchten, müssen Sie sie zuerst veröffentlichen.

Informationen zum Erstellen einer Vorlage finden Sie unter [Erstellen neuer Vorlagen in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Eine Vorlage muss erstellt werden, bevor sie freigegeben werden kann.

## Veröffentlichen eines [!DNL Adobe Workfront Fusion] template

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Vorlagen]**.
1. Klicken Sie auf **[!UICONTROL Team-Vorlagen]** Registerkarte.
1. Klicken Sie auf den Namen Ihrer Vorlage.
1. Klicken Sie auf **[!UICONTROL Veröffentlichen]** in der oberen rechten Ecke des Bildschirms.

## Freigeben von [!DNL Workfront Fusion] template

Nachdem Sie eine Vorlage veröffentlicht haben, können Sie sie freigeben.

1. (Bedingt) Wenn Sie einen freigebbaren Link erstellen möchten, klicken Sie auf **[!UICONTROL Öffentlichen Link freigeben]**.

   >[!NOTE]
   >
   >Sie können diesen Link für jeden freigeben, den Sie möchten. Die Vorlage selbst bleibt im [!UICONTROL Team-Vorlagen] und ist nicht öffentlich.

1. (Bedingt) Wenn die Vorlage veröffentlicht werden soll, senden Sie sie zur Genehmigung an Ihren Administrator, indem Sie auf **[!UICONTROL Genehmigung anfordern]**.

   >[!NOTE]
   >
   >* Sobald die Vorlage genehmigt wurde, wird sie öffentlich. [!UICONTROL Öffentliche Vorlagen] sind im [!UICONTROL Öffentliche Vorlagen] für alle [!DNL Workfront Fusion] Benutzer, unabhängig von der Organisation oder dem Team.
   >* Ihr Administrator wird nicht über den Erhalt der Vorlage informiert, die per E-Mail geprüft werden soll. Wenn die Validierung dringend erforderlich ist, wenden Sie sich direkt an den Administrator.



## Vorlagenstatus

Sie können den Status auf Ihrer Vorlagenseite unter dem Vorlagennamen überprüfen

Die folgenden Status sind verfügbar:

* **[!UICONTROL Privat]**: Diese Vorlage ist nur für den Vorlagenautor und sein Team sichtbar.
* **[!UICONTROL Veröffentlicht]**: Diese Vorlage ist nur für den Vorlagenautor und sein Team sichtbar. Sie können veröffentlichte Vorlagen zur Genehmigung senden und einen freigebbaren Link kopieren.
* **[!UICONTROL Genehmigt]**: Diese Vorlage ist für alle Benutzer von Workfront Fusion im [!UICONTROL Öffentliche Vorlagen] Registerkarte. Sie können einen freigebbaren Link kopieren, indem Sie auf [!UICONTROL Optionen] in der oberen rechten Ecke des Bildschirms.

Sie können den Status auch über die [!UICONTROL Team-Vorlagen] Registerkarte. Wenn eine Vorlage veröffentlicht wird, wird sie über ein Symbol rechts neben dem Vorlagennamen verfügen.

* **Augensymbol**: Die Vorlage wird veröffentlicht, sie ist nur für das Team sichtbar und die Genehmigungsanfrage wurde nicht gesendet.
* **Gelbes Häkchen-Symbol**: Die Vorlage wird veröffentlicht, sie ist nur für das Team sichtbar und die Genehmigungsanfrage wurde gesendet.
* **Symbol für grünes Häkchen**: Die Vorlage ist veröffentlicht und öffentlich. Sie ist für alle Workfront Fusion-Benutzer im [!UICONTROL Öffentliche Vorlagen] Registerkarte. Sie ist auch weiterhin im [!UICONTROL Team-Vorlagen] und der Vorlagenautor oder sein Team-Mitglied sie weiterhin bearbeiten kann.

Vorlagen ohne Symbole haben [!UICONTROL Privat] Status. Sie werden nicht veröffentlicht und sind nur für das Team sichtbar.
