---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwaltung von Adobe Workfront Fusion-Vorlagen
description: Als Administrator sind Sie berechtigt, von anderen erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die [!UICONTROL Vorlagen] Seite in der [!DNL Adobe Workfront Fusion Administration] Bereich.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 2b67b5fb951b5ae7867144c444411ebd1c299e75
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Verwaltung von Vorlagen

Als Administrator sind Sie berechtigt, von anderen erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die [!UICONTROL Vorlagen] Seite in der [!DNL Adobe Workfront Fusion Administration] Bereich.

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
    <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
    <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderung: Nein [!DNL Workfront Fusion] Lizenzanforderung.</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] für die Automatisierung von Arbeiten]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über die [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss Folgendes kaufen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] enthalten [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss kaufen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront Fusion-Administrator für Ihr Unternehmen sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Um herauszufinden, über welchen Plan, Lizenztyp oder Zugriff Sie verfügen, wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Für Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Ansicht [!DNL Workfront Fusion] Vorlagen als [!DNL Workfront Fusion] Verwalter

So zeigen Sie eine Tabelle aller erstellten Vorlagen und ihrer Status an:

1. Klick **[!UICONTROL Administration]** Öffnen Sie im linken Navigationsbereich das [!UICONTROL Administration] Bereich.

   >[!NOTE]
   >
   >Der Bereich Administration ist nur für Workfront Fusion-Administratoren sichtbar.

1. Klick **[!UICONTROL Vorlagen]** Im linken Navigationsbereich.

Es gibt drei Spalten zum Veröffentlichungsstatus der Vorlagen. Ein Häkchen in einer Spalte weist auf Folgendes hin:

* **[!UICONTROL Veröffentlicht]**: Diese Vorlagen sind derzeit in der [!UICONTROL Teamvorlagen] in der Benutzeroberfläche.
* **[!UICONTROL Genehmigung angefordert]**: Diese Vorlagen warten auf Ihre Genehmigung. Sie sind derzeit in der [!UICONTROL Teamvorlagen] in der Benutzeroberfläche.
* **[!UICONTROL Genehmigt]**: Diese Vorlagen wurden genehmigt. Sie sind derzeit in der [!UICONTROL Öffentliche Vorlagen] die Tabulatortaste in der Standardbenutzeroberfläche.

>[!NOTE]
>
>Vorlagen mit dem Häkchen in beiden [!UICONTROL Genehmigung angefordert] Spalte und in der [!UICONTROL Genehmigt] Spalten wurden bereits genehmigt und veröffentlicht, aber es gibt eine neuere Version davon, die auf Ihre Genehmigung wartet.

## Bearbeiten [!DNL Workfront Fusion] Vorlagen als Administrator

1. Klick **[!UICONTROL Administration]** Öffnen Sie im linken Navigationsbereich das [!UICONTROL Administration] Bereich.
1. Klick **[!UICONTROL Vorlagen]** Im linken Navigationsbereich.
1. Klick **[!UICONTROL Detail]** rechts neben der Vorlage, die Sie bearbeiten möchten.

Sie können die Vorlage jetzt bearbeiten, ähnlich wie eine Vorlage als Benutzer ohne Administratorrechte zu bearbeiten. In der [!UICONTROL Optionen] Oben rechts gibt es eine zusätzliche Option - das SVG-Diagramm, das den SVG-Code bereitstellt. Außerdem ist der Veröffentlichungsprozess derselbe wie bei einem Standardbenutzer. Weitere Informationen finden Sie im Abschnitt Veröffentlichungs- und Freigabevorlagen .

Informationen zu den Vorlagenoptionen, die Sie bearbeiten können, finden Sie unter [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Informationen zu Veröffentlichungsvorlagen finden Sie unter [Veröffentlichen und freigeben [!DNL Adobe Workfront Fusion] Vorlagen](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Genehmigen oder ablehnen [!DNL Workfront Fusion] Vorlagen

Wenn Sie eine Vorlage validieren, wird sie in der [!UICONTROL Öffentliche Vorlagen] und für alle Benutzer verfügbar. Wenn Sie eine Vorlage ablehnen, wird sie aus der [!UICONTROL Öffentliche Vorlagen] und stellt sie nur dem Team zur Verfügung, das sie erstellt hat.

1. Klick **[!UICONTROL Administration]** Öffnen Sie im linken Navigationsbereich das [!UICONTROL Administration] Bereich.
1. Klick **[!UICONTROL Vorlagen]** Im linken Navigationsbereich.
1. Wenn Sie eine Vorlage genehmigen möchten, klicken Sie auf **[!UICONTROL Genehmigen]** rechts neben der Vorlage.
1. Wenn Sie eine Vorlage ablehnen möchten, klicken Sie auf **[!UICONTROL missbilligen]** rechts neben der Vorlage.

>[!NOTE]
>
>Wenn Sie die zuvor genehmigte und dann bearbeitete Vorlage genehmigen, überschreibt Ihre zweite Genehmigung die ursprüngliche Vorlage.

## Klonen eines Szenarios als Vorlage

Als Administrator haben Sie die Möglichkeit, ein Szenario als Vorlage zu klonen.

Anweisungen zum Klonen eines Szenarios als Vorlage finden Sie unter [Erstellen einer Vorlage aus einem Szenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
