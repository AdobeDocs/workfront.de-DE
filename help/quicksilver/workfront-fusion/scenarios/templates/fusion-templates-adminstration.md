---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwaltung von Adobe Workfront-Fusionsvorlagen
description: Wenn Sie Administrator sind, sind Sie berechtigt, von anderen Benutzern erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die [!UICONTROL Vorlagen] in der [!DNL Adobe Workfront Fusion Administration] Bereich.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Vorlagenverwaltung

Wenn Sie Administrator sind, sind Sie berechtigt, von anderen Benutzern erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die [!UICONTROL Vorlagen] in der [!DNL Adobe Workfront Fusion Administration] Bereich.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront Fusion-Administrator für Ihr Unternehmen sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ansicht [!DNL Workfront Fusion] Vorlagen als Administrator

So zeigen Sie eine Tabelle aller erstellten Vorlagen und deren Status an:

1. Klicken **[!UICONTROL Administration]** im linken Navigationsbereich, um die [!UICONTROL Administration] Bereich.
1. Klicken **[!UICONTROL Vorlagen]** im linken Navigationsbereich.

Es gibt drei Spalten zum Veröffentlichungsstatus der Vorlagen. Ein Häkchen in einer Spalte zeigt Folgendes an:

* **[!UICONTROL Veröffentlicht]**: Diese Vorlagen sind derzeit im [!UICONTROL Team-Vorlagen] in der Benutzeroberfläche.
* **[!UICONTROL Beantragte Genehmigung]**: Diese Vorlagen warten auf Ihre Validierung. Sie sind derzeit im [!UICONTROL Team-Vorlagen] in der Benutzeroberfläche.
* **[!UICONTROL Genehmigt]**: Diese Vorlagen wurden genehmigt. Sie sind derzeit im [!UICONTROL Öffentliche Vorlagen] in der Standard-Benutzeroberfläche.

>[!NOTE]
>
>Vorlagen mit dem Häkchen in beiden [!UICONTROL Beantragte Genehmigung] und in der Spalte [!UICONTROL Genehmigt] -Spalte wurde bereits genehmigt und veröffentlicht, aber es gibt eine neuere Version davon, die auf Ihre Genehmigung wartet.

## Bearbeiten [!DNL Workfront Fusion] Vorlagen als Administrator

1. Klicken **[!UICONTROL Administration]** im linken Navigationsbereich, um die [!UICONTROL Administration] Bereich.
1. Klicken **[!UICONTROL Vorlagen]** im linken Navigationsbereich.
1. Klicken **[!UICONTROL Detail]** rechts neben der Vorlage, die Sie bearbeiten möchten.

Sie können die Vorlage jetzt bearbeiten, ähnlich wie eine Vorlage als Benutzer ohne Administratorrechte zu bearbeiten. Im [!UICONTROL Optionen] oben rechts gibt es eine zusätzliche Option - das SVG-Diagramm, das Ihnen den SVG-Code bereitstellt. Der Veröffentlichungsprozess entspricht dem für einen Standardbenutzer. Weitere Informationen finden Sie im Abschnitt Veröffentlichungs- und Freigabevorlagen .

Informationen zu bestimmten Vorlagenoptionen, die Sie bearbeiten können, finden Sie unter [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Informationen zu Veröffentlichungsvorlagen finden Sie unter [Veröffentlichen und freigeben [!DNL Adobe Workfront Fusion] templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Genehmigen oder ablehnen [!DNL Workfront Fusion] templates

Wenn Sie eine Vorlage validieren, wird sie im [!UICONTROL Öffentliche Vorlagen] und für alle Benutzer verfügbar sein. Wenn Sie eine Vorlage deaktivieren, wird sie aus dem [!UICONTROL Öffentliche Vorlagen] und stellt sie nur dem Team zur Verfügung, das sie erstellt hat.

1. Klicken **[!UICONTROL Administration]** im linken Navigationsbereich, um die [!UICONTROL Administration] Bereich.
1. Klicken **[!UICONTROL Vorlagen]** im linken Navigationsbereich.
1. Wenn Sie eine Vorlage genehmigen möchten, klicken Sie auf **[!UICONTROL Genehmigen]** rechts neben der Vorlage.
1. Wenn Sie eine Vorlage ablehnen möchten, klicken Sie auf **[!UICONTROL Ablehnen]** rechts neben der Vorlage.

>[!NOTE]
>
>Wenn Sie die Vorlage validieren, die zuvor genehmigt und dann bearbeitet wurde, überschreibt Ihre zweite Validierung die ursprüngliche Vorlage.

## Ein Szenario als Vorlage klonen

Als Administrator haben Sie die Möglichkeit, ein Szenario als Vorlage zu klonen.

Anweisungen zum Klonen eines Szenarios als Vorlage finden Sie unter [Erstellen einer Vorlage aus einem Szenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
