---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwaltung von Adobe Workfront Fusion-Vorlagen
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Verwaltung von [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie nun in den Artikeln:
>
>* [Vorlagen für die Registerkarte „Öffentlich“ genehmigen oder nicht genehmigen](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [Vorlagen bearbeiten](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Als Administrator sind Sie berechtigt, von anderen erstellte Vorlagen anzuzeigen, zu ändern, umzubenennen, zu veröffentlichen, zu genehmigen und zu löschen. Sie können diese Aktionen über die Seite [!UICONTROL Vorlagen] im [!DNL Adobe Workfront Fusion Administration] ausführen.

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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront Fusion-Administrator für Ihr Unternehmen sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Anzeigen [!DNL Workfront Fusion] Vorlagen als [!DNL Workfront Fusion]

So zeigen Sie eine Tabelle aller erstellten Vorlagen und ihrer Status an:

1. Klicken Sie **[!UICONTROL linken]** auf „Administration“, um den Bereich [!UICONTROL Administration] zu öffnen.

   >[!NOTE]
   >
   >Der Bereich Administration ist nur für Workfront Fusion-Administratoren sichtbar.

1. Klicken **[!UICONTROL im linken]** auf „Vorlagen“.

Es gibt drei Spalten zum Veröffentlichungsstatus der Vorlagen. Ein Häkchen in einer Spalte weist auf Folgendes hin:

* **[!UICONTROL Veröffentlicht]**: Diese Vorlagen sind derzeit auf der Registerkarte [!UICONTROL Team-Vorlagen] in der Benutzeroberfläche sichtbar.
* **[!UICONTROL Angeforderte Genehmigung]**: Diese Vorlagen warten auf Ihre Genehmigung. Sie sind derzeit auf der Registerkarte [!UICONTROL Teamvorlagen] in der Benutzeroberfläche sichtbar.
* **[!UICONTROL Genehmigt]**: Diese Vorlagen wurden genehmigt. Sie sind derzeit auf der Registerkarte [!UICONTROL Öffentliche Vorlagen] in der Standardbenutzeroberfläche sichtbar.

>[!NOTE]
>
>Vorlagen mit dem Häkchen sowohl in der Spalte [!UICONTROL Angeforderte Genehmigung] als auch in der Spalte [!UICONTROL Genehmigt] wurden bereits genehmigt und veröffentlicht, aber es gibt eine neuere Version davon, die auf Ihre Genehmigung wartet.

## Bearbeiten [!DNL Workfront Fusion] Vorlagen als Admin

1. Klicken Sie **[!UICONTROL linken]** auf „Administration“, um den Bereich [!UICONTROL Administration] zu öffnen.
1. Klicken **[!UICONTROL im linken]** auf „Vorlagen“.
1. Klicken **[!UICONTROL rechts neben]** Vorlage, die Sie bearbeiten möchten, auf „Detail“.

Sie können die Vorlage jetzt bearbeiten, ähnlich wie eine Vorlage als Benutzer ohne Administratorrechte zu bearbeiten. In der [!UICONTROL Optionen] oben rechts gibt es jedoch eine zusätzliche Option - das SVG-Diagramm, das den SVG-Code bereitstellt. Außerdem ist der Veröffentlichungsprozess derselbe wie bei einem Standardbenutzer. Weitere Informationen finden Sie im Abschnitt Veröffentlichungs- und Freigabevorlagen .

Informationen zu den Vorlagenoptionen, die Sie bearbeiten können, finden Sie unter [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Informationen zum Veröffentlichen von Vorlagen finden Sie unter [Publish und share [!DNL Adobe Workfront Fusion] templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## [!DNL Workfront Fusion] genehmigen oder ablehnen

Wenn Sie eine Vorlage validieren, wird sie auf der Registerkarte [!UICONTROL Öffentliche Vorlagen] angezeigt und steht allen Benutzern zur Verfügung. Wenn Sie eine Vorlage ablehnen, wird sie aus der Registerkarte [!UICONTROL Öffentliche Vorlagen] entfernt und nur für das Team verfügbar gemacht, das sie erstellt hat.

1. Klicken Sie **[!UICONTROL linken]** auf „Administration“, um den Bereich [!UICONTROL Administration] zu öffnen.
1. Klicken **[!UICONTROL im linken]** auf „Vorlagen“.
1. Wenn Sie eine Vorlage genehmigen möchten, klicken **[!UICONTROL rechts neben]** Vorlage auf „Genehmigen“.
1. Wenn Sie eine Vorlage nicht genehmigen möchten, klicken **[!UICONTROL rechts neben]** Vorlage auf „Nicht genehmigen“.

>[!NOTE]
>
>Wenn Sie die zuvor genehmigte und dann bearbeitete Vorlage genehmigen, überschreibt Ihre zweite Genehmigung die ursprüngliche Vorlage.

## Klonen eines Szenarios als Vorlage

Als Administrator haben Sie die Möglichkeit, ein Szenario als Vorlage zu klonen.

Anweisungen zum Klonen eines Szenarios als Vorlage finden Sie unter [Erstellen einer Vorlage aus einem Szenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
