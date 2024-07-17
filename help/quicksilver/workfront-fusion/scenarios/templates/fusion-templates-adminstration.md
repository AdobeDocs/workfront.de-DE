---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwaltung von Adobe Workfront-Fusionsvorlagen
description: Wenn Sie Administrator sind, sind Sie berechtigt, von anderen Benutzern erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die Seite [!UICONTROL Vorlagen] im Bereich  [!DNL Adobe Workfront Fusion Administration]  durchführen.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 2b67b5fb951b5ae7867144c444411ebd1c299e75
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Vorlagenverwaltung

Wenn Sie Administrator sind, sind Sie berechtigt, von anderen Benutzern erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die Seite [!UICONTROL Vorlagen] im Bereich [!DNL Adobe Workfront Fusion Administration] durchführen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront Fusion-Administrator für Ihr Unternehmen sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Anzeigen von [!DNL Workfront Fusion]-Vorlagen als [!DNL Workfront Fusion]-Administrator

So zeigen Sie eine Tabelle aller erstellten Vorlagen und deren Status an:

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Administration]** , um den Bereich [!UICONTROL Administration] zu öffnen.

   >[!NOTE]
   >
   >Der Bereich Administration ist nur für Administratoren von Workfront Fusion sichtbar.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Vorlagen]** .

Es gibt drei Spalten zum Veröffentlichungsstatus der Vorlagen. Ein Häkchen in einer Spalte zeigt Folgendes an:

* **[!UICONTROL Veröffentlicht]**: Diese Vorlagen sind derzeit auf der Registerkarte [!UICONTROL Teamvorlagen] in der Benutzeroberfläche sichtbar.
* **[!UICONTROL Beantragte Genehmigung]**: Diese Vorlagen warten auf Ihre Genehmigung. Sie sind derzeit auf der Registerkarte [!UICONTROL Team templates] in der Benutzeroberfläche sichtbar.
* **[!UICONTROL Genehmigt]**: Diese Vorlagen wurden genehmigt. Sie sind derzeit in der Standardbenutzeroberfläche auf der Registerkarte [!UICONTROL Öffentliche Vorlagen] sichtbar.

>[!NOTE]
>
>Vorlagen mit dem Häkchen sowohl in der Spalte [!UICONTROL Beantragte Genehmigung] als auch in der Spalte [!UICONTROL Genehmigt] wurden bereits genehmigt und veröffentlicht. Es gibt jedoch eine neuere Version davon, die auf Ihre Genehmigung wartet.

## Bearbeiten von [!DNL Workfront Fusion]-Vorlagen als Administrator

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Administration]** , um den Bereich [!UICONTROL Administration] zu öffnen.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Vorlagen]** .
1. Klicken Sie rechts neben der Vorlage, die Sie bearbeiten möchten, auf **[!UICONTROL Detail]** .

Sie können die Vorlage jetzt bearbeiten, ähnlich wie eine Vorlage als Benutzer ohne Administratorrechte zu bearbeiten. In der oberen rechten Ecke von [!UICONTROL Options] gibt es jedoch eine zusätzliche Option - das SVG-Diagramm, das Ihnen den SVG-Code bereitstellt. Der Veröffentlichungsprozess entspricht dem für einen Standardbenutzer. Weitere Informationen finden Sie im Abschnitt Veröffentlichungs- und Freigabevorlagen .

Informationen zu bestimmten Vorlagenoptionen, die Sie bearbeiten können, finden Sie unter [Erstellen neuer Vorlagen in  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Informationen zu Veröffentlichungsvorlagen finden Sie unter [Publish und share [!DNL Adobe Workfront Fusion] templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## [!DNL Workfront Fusion]-Vorlagen genehmigen oder ablehnen

Wenn Sie eine Vorlage genehmigen, wird sie auf der Registerkarte [!UICONTROL Öffentliche Vorlagen] sichtbar und für alle Benutzer verfügbar. Wenn Sie eine Vorlage ablehnen, wird sie aus dem Tab [!UICONTROL Öffentliche Vorlagen] entfernt und nur dem Team zur Verfügung gestellt, das sie erstellt hat.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Administration]** , um den Bereich [!UICONTROL Administration] zu öffnen.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Vorlagen]** .
1. Wenn Sie eine Vorlage genehmigen möchten, klicken Sie rechts neben der Vorlage auf **[!UICONTROL Genehmigen]** .
1. Wenn Sie eine Vorlage ablehnen möchten, klicken Sie rechts neben der Vorlage auf **[!UICONTROL Ablehnen]** .

>[!NOTE]
>
>Wenn Sie die Vorlage validieren, die zuvor genehmigt und dann bearbeitet wurde, überschreibt Ihre zweite Validierung die ursprüngliche Vorlage.

## Ein Szenario als Vorlage klonen

Als Administrator haben Sie die Möglichkeit, ein Szenario als Vorlage zu klonen.

Anweisungen zum Klonen eines Szenarios als Vorlage finden Sie unter [Erstellen einer Vorlage aus einem Szenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Erstellen neuer Vorlagen in  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
