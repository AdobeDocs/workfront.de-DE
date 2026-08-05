---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Verknüpfen von Inhalten und Ordnern aus Experience Manager Assets mit dem Adobe Cloud-Speicher
description: Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, können Sie Inhalte und Ordner aus Experience Manager Assets mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt.
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 7%

---

# Verknüpfen von Inhalten und Ordnern aus Experience Manager Assets mit dem Adobe Cloud-Speicher

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, können Sie Inhalte und Ordner von Experience Manager Assets mit Workfront verknüpfen. Nach der Verknüpfung können Sie den Inhalt in Workfront anzeigen und verwalten. Alle Änderungen am Inhalt in Experience Manager Assets werden in Workfront übernommen.

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
   <td>Sie müssen über Experience Manager as a Cloud Service verfügen und dem Produkt müssen Sie als Benutzer in der Admin Console hinzugefügt werden.</td> 
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

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Verwenden von Adobe Experience Manager mit der Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Um die Funktion „Smart Suggestions“ oder „Campaign Briefs“ verwenden zu können, müssen Sie einen GenAI Rider signieren. Weitere Informationen finden Sie unter [Verwenden von Content Advisor für den Zugriff auf AEM-Inhalte in Adobe-Programmen](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).

## Verknüpfen von Inhalten aus Experience Manager Assets

So verknüpfen Sie Inhalte:

1. Wechseln Sie zum Workfront-Objekt, mit dem Sie Inhalte verknüpfen möchten.
1. Klicken Sie auf **Abschnitt** Dokumente“ im linken Bedienfeld.
1. Klicken Sie **rechts auf** Seite auf „Neu“ und dann auf **AEM-Dateien**, um ein einzelnes Asset zu verknüpfen.
   ![Fügen Sie AEM-Dateien zum Bereich „Dokumente“ hinzu](assets/aem-files.png)

1. Mit Content Advisor können Sie:

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Suchen nach Assets mithilfe von KI-Suchen.</strong> Verwenden Sie eine KI-gestützte Suche, die Bedeutung und Absicht hinter Abfragen versteht und mehrere Sprachen, Rechtschreibfehler und Synonyme unterstützt.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">KI-Suchen für die intelligentere Asset-Erkennung</a>.</td>
      </tr>
      <tr>
         <td><strong>Anzeigen von Smart-Vorschlägen basierend auf Kontext und Absicht.</strong> Entdecken Sie Assets, die Ihren Inhaltsanforderungen entsprechen, indem Sie kontextabhängige Empfehlungen aus der Adobe-Hostanwendung verwenden.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Intelligente Vorschläge basierend auf Kontext und Absicht</a>.</td>
      </tr>
      <tr>
         <td><strong>Laden Sie eine Kampagnenbeschreibung hoch, um relevante Assets zu finden.</strong> Laden Sie ein Kurzdokument für PDF-, DOCX- oder TXT-Kampagnen hoch, damit Content Advisor es analysieren und relevante Assets empfehlen kann.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Kampagnenbeschreibungen zur Ermittlung relevanter Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Anzeigen und Auswählen von Dynamic Media-Asset-Ausgabedarstellungen.</strong> Durchsuchen Sie kanaloptimierte Ausgabedarstellungen, einschließlich Bildvorgaben, smartem Zuschneiden und Formattypen, und wenden Sie Dynamic Media-Modifikatoren an, um Anpassungen in Echtzeit in der Vorschau anzuzeigen.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Für Dynamic Media-Assets verfügbare Ausgabedarstellungen</a>.</td>
      </tr>
      <tr>
         <td><strong>Anwenden von Dynamic Media-Modifikatoren auf Ausgabedarstellungen.</strong> Fügen Sie Modifikatoren hinzu, um Asset-Ausgabedarstellungen in Echtzeit umzuwandeln und eine Vorschau der Ergebnisse anzuzeigen, bevor Sie eine Ausgabedarstellung für Ihre Hostanwendung auswählen.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Für Dynamic Media-Assets verfügbare Ausgabedarstellungen</a>.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>Zugriff auf Asset-Metadaten.</strong> Überprüfen Sie Asset-Eigenschaften wie Titel, Beschreibung, Format, Größe und andere Metadaten-Registerkarten (Produkt, Kampagne, Tags) entsprechend der Assets-Ansicht.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Zugriff auf Asset-Metadaten, die der Assets-Ansicht entsprechen</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtern von Assets mithilfe vordefinierter Filter.</strong> Verfeinern Sie die Asset-Ergebnisse mithilfe von Filtern wie Dateityp, Dateiformat, Asset-Status, Dateigröße, Bildbreite, Bildhöhe, Änderungsdatum und Erstellungsdatum.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Zugriff auf Filter, die der Assets-Ansicht entsprechen</a>.</td>
      </tr>
      <tr>
         <td><strong>Speichern und Wiederverwenden von Suchvorgängen.</strong> Erstellen Sie gespeicherte Suchen, indem Sie einen Suchbegriff und Filteroptionen angeben und diese dann in Experience Manager Assets und anderen Adobe-Programmen wiederverwenden.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Zugreifen auf und Wiederverwenden von kürzlich durchgeführten und gespeicherten Suchen</a>.</td>
      </tr>
      <tr>
         <td><strong>Suchen nach Assets in und innerhalb von Sammlungen.</strong> Alle Sammlungen nach Assets oder Sammlungen durchsuchen oder die Suche auf eine bestimmte Sammlung beschränken.</td>
         <td>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Suchen nach Assets in und innerhalb von Sammlungen</a>.</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >Empfohlene Inhalte in Content Advisor verwendet Daten aus den folgenden Elementen, um vorgeschlagene Inhalte in Workfront zu ermitteln:
   >
   >* Felder für Workfront-Objektnamen und -Beschreibungen
   >* Benutzerdefinierte Formularfelder, die als erforderlich markiert sind
   >* Daten aus angehängten Dokumenten

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## Zu beachten

* Überprüfungs- und Genehmigungs-Workflows werden für verknüpfte AEM-Assets nicht unterstützt.
* Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets senden. Wenn Ihr Workfront-Administrator die Synchronisierung von Objektmetadaten aktiviert hat, bleiben die Felder auf dem neuesten Stand, wenn sie in einer der Anwendungen geändert werden.
