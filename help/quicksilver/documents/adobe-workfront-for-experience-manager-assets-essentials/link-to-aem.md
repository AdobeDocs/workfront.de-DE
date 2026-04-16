---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Inhalten und Ordnern mit Content Advisor auf Basis von Experience Manager Assets
description: Sie können Content Advisor verwenden, um Inhalte oder Ordner aus Experience Manager Assets mit jedem Adobe Workfront-Objekt zu verknüpfen, das Dokumente unterstützt. Content Advisor bringt intelligente, kontextbezogene Erkennung direkt in Workfront und hilft Ihnen, relevante, genehmigte Inhalte schnell zu finden.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 5%

---

# Verknüpfen von Inhalten und Ordnern mit dem Content Advisor von Experience Manager Assets

Content Advisor bringt intelligente, kontextbezogene Erkennung direkt in Workfront, sodass Sie relevante, genehmigte Inhalte schnell kontextbasiert finden können. Mit Funktionen wie Smart Suggestions, Dynamic Media-Ausgabedarstellungen und detaillierten Asset-Metadaten können Sie Inhalte effizient bewerten und wiederverwenden, ohne Workfront verlassen zu müssen, was die Inhaltserstellung beschleunigt und gleichzeitig die Markenkonsistenz wahrt.

Sie können Content Advisor verwenden, um Inhalte und Ordner von Experience Manager Assets mit Workfront zu verknüpfen. Nach der Verknüpfung können Sie den Inhalt in Workfront anzeigen und verwalten. Alle Änderungen am Inhalt in Experience Manager Assets werden in Workfront übernommen.

>[!IMPORTANT]
>
>Wenn Ihr Unternehmen die Unterzeichnung der GenAI-Reitervereinbarung ablehnt, können Sie weiterhin Content Advisor verwenden, um Assets und Ordner in Experience Manager Assets auszuwählen, Sie haben jedoch keinen Zugriff auf KI-gestützte Funktionen wie KI-Suchen, Smart-Vorschläge oder die Analyse von Kampagnenbeschreibungen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-Berechtigungen</td> 
    <td>Sie müssen Schreibzugriff auf den Ordner haben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen:

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Um die Funktion „Smart Suggestions“ oder „Campaign Briefs“ verwenden zu können, müssen Sie einen GenAI Rider signieren. Weitere Informationen finden Sie unter [Verwenden von Content Advisor für den Zugriff auf AEM-Inhalte in Adobe-Programmen](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Verknüpfen von Inhalten aus Experience Manager Assets mit Content Advisor

Sie können jetzt Content Advisor verwenden, um Inhalte von Experience Manager Assets direkt in Workfront zu verknüpfen. Der Inhaltsratgeber ist nicht für Assets Essentials verfügbar.

So verknüpfen Sie Inhalte:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets möglicherweise nicht explizit erwähnt wird.

1. Mit Content Advisor können Sie:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Suchen nach Assets mithilfe von KI-Suchen.</strong> Verwenden Sie eine KI-gestützte Suche, die Bedeutung und Absicht hinter Abfragen versteht und mehrere Sprachen, Tippfehler und Synonyme unterstützt.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">KI-Suchen für die intelligentere Asset-Erkennung</a>.</td>
      </tr>
      <tr>
         <td><strong>Anzeigen von Smart-Vorschlägen basierend auf Kontext und Absicht.</strong> Entdecken Sie Assets, die Ihren Inhaltsanforderungen entsprechen, mithilfe von kontextabhängigen Empfehlungen aus der Adobe-Hostanwendung.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Intelligente Vorschläge basierend auf Kontext und Absicht</a>.</td>
      </tr>
      <tr>
         <td><strong>Laden Sie eine Kampagnenbeschreibung hoch, um relevante Assets zu finden.</strong> Hochladen eines PDF-, DOCX- oder TXT-Kampagnendokuments, damit Content Advisor es analysieren und relevante Assets empfehlen kann.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Kampagnenbeschreibungen zur Ermittlung relevanter Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Anzeigen und Auswählen von Dynamic Media-Asset-Ausgabedarstellungen.</strong> Durchsuchen Sie kanaloptimierte Ausgabedarstellungen, einschließlich Bildvorgaben, smartem Zuschneiden und Formattypen, und wenden Sie Dynamic Media-Modifikatoren an, um Anpassungen in Echtzeit in der Vorschau anzuzeigen.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Für Dynamic Media-Assets verfügbare Ausgabedarstellungen</a>.</td>
      </tr>
      <tr>
         <td><strong>Anwenden von Dynamic Media-Modifikatoren auf Ausgabedarstellungen.</strong> Fügen Sie Modifikatoren hinzu, um Asset-Ausgabedarstellungen in Echtzeit umzuwandeln und eine Vorschau der Ergebnisse anzuzeigen, bevor Sie eine Ausgabedarstellung für Ihre Hostanwendung auswählen.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Für Dynamic Media-Assets verfügbare Ausgabedarstellungen</a>.</td>
      </tr>
      <tr>
         <td><strong>Entdecken und Durchsuchen von Inhaltsfragmenten.</strong> Inhaltsfragmente zu durchsuchen, Live-Miniaturansichten anzuzeigen, den Status (Entwurf, Geändert oder Veröffentlicht) zu überprüfen und detaillierte Eigenschaften, Verweise und Varianten zu überprüfen.</td>
         <td>Weitere Informationen finden Sie <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Erkennung von Inhaltsfragmenten</a>.</td>
      </tr>
      <tr>
         <td><strong>Zugriff auf Asset-Metadaten.</strong> Überprüfen von Asset-Eigenschaften wie Titel, Beschreibung, Format, Größe und anderen Metadaten-Registerkarten (Produkt, Kampagne, Tags), die mit der Assets-Ansicht übereinstimmen.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Zugriff auf Asset-Metadaten, die der Assets-Ansicht entsprechen</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtern Sie Assets mithilfe vordefinierter Filter.</strong> Verfeinern von Asset-Ergebnissen mithilfe von Filtern wie Dateityp, Dateiformat, Asset-Status, Dateigröße, Bildbreite, Bildhöhe, Änderungsdatum und Erstellungsdatum.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Zugriff auf Filter, die der Assets-Ansicht entsprechen</a>.</td>
      </tr>
      <tr>
         <td><strong>Speichern und Wiederverwenden von Suchen.</strong> Erstellen Sie gespeicherte Suchen, indem Sie einen Suchbegriff und Filteroptionen angeben und diese dann in Experience Manager Assets und anderen Adobe-Programmen wiederverwenden.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Zugreifen auf und Wiederverwenden von kürzlich durchgeführten und gespeicherten Suchen</a>.</td>
      </tr>
      <tr>
         <td><strong>Suchen nach Assets in und innerhalb von Sammlungen.</strong> Suche nach Assets oder Sammlungen in allen Sammlungen oder Suche auf eine bestimmte Sammlung beschränken.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Suchen nach Assets in und innerhalb von Sammlungen</a>.</td>
      </tr>
   </tbody>
   </table>


### Verknüpfen einer neuen Version aus Experience Manager Assets mit dem Inhaltsratgeber

Sie können neue Inhalte aus Experience Manager Assets oder Assets Essentials abrufen und sie als neue Version einem vorhandenen Asset hinzufügen. Wenn das Dokument bereits verknüpft ist und in Experience Manager Assets oder Assets Essentials eine neue Version hinzugefügt wird, wird die neue Version automatisch in Workfront angezeigt.

Verknüpfen einer neuen Version:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Wählen Sie **Neu hinzufügen** > **Version** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets möglicherweise nicht explizit erwähnt wird.

1. Wählen Sie den Inhalt aus, den Sie verknüpfen möchten:

   * Wählen Sie die Registerkarte Assets aus, um Assets, Ordner oder Sammlungen in Experience Manager Assets oder Assets Essentials zu durchsuchen.

     ![Inhaltsratgeber](assets/content-advisor-full.png)

   * Inhaltsfragmente unterstützen keine Versionen. Wenn Sie ein Inhaltsfragment auswählen, ersetzt die neue Version das vorhandene Inhaltsfragment, anstatt eine neue Version zu erstellen.

1. Klicken Sie auf **Auswählen**.

## Verknüpfen von Ordnern aus Experience Manager Assets mit Content Advisor

Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners sind von Experience Manager Assets-Berechtigungen abhängig.

So verknüpfen Sie einen Ordner:

1. Wechseln Sie zum **Dokumente** in Workfront, in dem Sie den Ordner ablegen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets möglicherweise nicht explizit erwähnt wird.

1. Klicken Sie auf **** > **Dateien und Ordner**.

1. Klicken Sie auf **Filter**-Symbol und wählen Sie dann im Abschnitt **Asset-Typ** die Option **Ordner**.

1. Wählen Sie den Ordner aus, den Sie verknüpfen möchten.

1. Klicken Sie auf **Auswählen**.

## Zu beachten

* Die Funktion „Content Advisor“ ist nicht für Objekte verfügbar, die Adobe Enterprise-Speicher verwenden. Wenn Ihr Unternehmen Adobe Enterprise Storage verwendet, können Sie weiterhin Assets und Ordner aus Experience Manager Assets oder Assets Essentials verknüpfen, haben jedoch keinen Zugriff auf Content Advisor-Funktionen wie KI-Suchen, Smart Suggestions oder Dynamic Media-Ausgabedarstellungen. Weitere Informationen finden Sie unter [Verwenden von Adobe Experience Manager mit der Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Die Funktion „Inhaltsratgeber“ ist für Assets Essentials nicht verfügbar. Informationen zum Verknüpfen von Assets und Ordnern aus Assets Essentials finden Sie unter [Verknüpfen von Assets und Ordnern aus Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets senden. Wenn Ihr Workfront-Administrator die Synchronisierung von Objektmetadaten aktiviert hat, bleiben die Felder auf dem neuesten Stand, wenn sie in einer der Anwendungen geändert werden.
