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

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Beta-Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Webinhaltsbausteine hinzufügen oder bearbeiten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Berichterstellung**.
1. Klicks **Neuer Bericht**.

   Oder

   Gehen Sie zu einem vorhandenen Bericht und klicken Sie auf die Schaltfläche **Mehr** icon ![](assets/more-icon-27x15.png) Klicken Sie in der Berichtüberschrift auf **Bearbeiten**.

1. Auf der rechten Seite des Bildschirms unter **Baustein hinzufügen**, entweder:

   Ziehen Sie die **Webinhalt** auf der Arbeitsfläche direkt zu Ihrer gewünschten Position.

   Oder

   Doppelklicken Sie auf die **Webinhalt** -Symbol, um oben auf der Arbeitsfläche einen Block hinzuzufügen.

   >[!TIP]
   >
   >Sie können die Größe des Blocks nach seiner Platzierung durch Ziehen der Ecken-Griffe ändern.

1. Klicks **Unbenannter Webinhalt** Geben Sie in die Kopfzeile des Blocks einen Titel für den Block ein.
1. Klicken Sie auf **Bearbeiten** icon ![](assets/edit-icon.png) in der Blockkopfzeile.

   ![](assets/web-content-block-header-350x76.png)

1. Im **Einstellungen** das geöffnet wird, geben Sie die vollständige URL für die Seite ein, die Sie in der **URL** -Feld.

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

1. (Optional) Klicken Sie auf die **Parameter übergeben** Umschalten, um eine Liste der verfügbaren Übergabeparameter zu öffnen.

   >[!WARNING]
   >
   >Parameter für die Weiterleitung sind derzeit deaktiviert.

1. Klicks **Einbetten-URL** , um Ihre Auswahl zu speichern und zu Ihrem Bericht zurückzukehren.
