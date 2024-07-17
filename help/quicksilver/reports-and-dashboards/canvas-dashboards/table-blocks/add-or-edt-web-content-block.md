---
title: Webinhaltsbausteine in der Berichtsarbeitsfläche hinzufügen oder bearbeiten
description: Mit Webinhaltblöcken können Sie Informationen von externen Websites direkt in Ihrem Bericht anzeigen.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Webinhaltsbausteine in der Berichtsarbeitsfläche hinzufügen oder bearbeiten

Mit Webinhaltblöcken können Sie Informationen von externen Websites direkt in Ihrem Bericht anzeigen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Arbeitsfläche für die Berichterstellung Beta: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Webinhaltsbausteine hinzufügen oder bearbeiten

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Berichterstellung**.![](assets/main-menu-icon.png)
1. Klicken Sie auf **Neuer Bericht**.

   Oder

   Wechseln Sie zu einem vorhandenen Bericht, klicken Sie auf das Symbol **Mehr** ![](assets/more-icon-27x15.png) in der Kopfzeile des Berichts und klicken Sie dann auf **Bearbeiten**.

1. Fügen Sie rechts im Bildschirm unter **Baustein hinzufügen** einen der folgenden Schritte ein:

   Ziehen Sie das Symbol **Webinhalt** direkt an die gewünschte Position auf der Arbeitsfläche.

   Oder

   Doppelklicken Sie auf das Symbol **Webinhalt** , um oben auf der Arbeitsfläche einen Block hinzuzufügen.

   >[!TIP]
   >
   >Sie können die Größe des Blocks nach seiner Platzierung durch Ziehen der Ecken-Griffe ändern.

1. Klicken Sie im Block-Header auf **Webinhalt ohne Titel** und geben Sie dann einen Titel für den Block ein.
1. Klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) in der Kopfzeile des Blocks.

   ![](assets/web-content-block-header-350x76.png)

1. Geben Sie im sich öffnenden Bedienfeld **Einstellungen** im Feld **URL** die vollständige URL für die Seite ein, die angezeigt werden soll (einschließlich &quot;https://&quot;).

   >[!NOTE]
   >
   >Derzeit können nur Sites aus ausgewählten Domänen angezeigt werden. Folgende Domänen können derzeit verwendet werden:
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   Unter Ihrer eingegebenen URL wird ein Warnhinweis angezeigt, wenn sie nicht eingebettet werden kann. Zu diesen Warnungen gehören:

   | Warnungsname | Grund |
   |---|---|
   | Ungültige URL | Die eingegebene URL gibt keine gültige Site zurück. |
   | Einschränkungen der Website des Anbieters | Die Site, die Sie einbetten möchten, ist nicht zulässig. |

   {style="table-layout:auto"}

1. (Optional) Klicken Sie auf den Umschalter **Parameter übergeben** , um eine Liste der verfügbaren Übergabeparameter zu öffnen.

   >[!WARNING]
   >
   >Parameter für die Weiterleitung sind derzeit deaktiviert.

1. Klicken Sie auf **URL einbetten** , um Ihre Auswahl zu speichern und zu Ihrem Bericht zurückzukehren.
