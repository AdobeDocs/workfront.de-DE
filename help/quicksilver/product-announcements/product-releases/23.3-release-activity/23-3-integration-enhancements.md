---
title: 23.3 Integrationsverbesserungen
description: 23.3 Integrationsverbesserungen
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3 Integrationsverbesserungen

Auf dieser Seite werden alle Integrationsverbesserungen beschrieben, die mit Version 23.3 vorgenommen wurden. Diese Verbesserungen wurden mit der Version 23.3 vom 20. und 21. Juli 2023 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die derzeit im 23.3-Versionszyklus verfügbar sind, finden Sie unter [23.3 - Versionsübersicht](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Neue Google Workspace-Integration verfügbar

Eine neue Google Workspace-Integration ist jetzt im Google Marketplace verfügbar. Die neue Integration authentifiziert sich mit OAuth2 und ersetzt die vorherige Integration.

Die vorherige Google Workspace-Integration ist jetzt veraltet und wird automatisch deinstalliert.

Anweisungen zum Installieren der neuen Integration finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Weitere Informationen zu Workfront für Google Workspace finden Sie unter [Workfront für Google Workspace](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud-Integrationen unterstützen jetzt mehrere zugewiesene Benutzer

Die Adobe Creative Cloud-Integration unterstützt jetzt die Möglichkeit, zwischen &quot;Fertig mit meinem Teil&quot; und &quot;Fertig&quot;(oder &quot;gelöst&quot;) zu wählen, wenn einer Aufgabe oder einem Problem mehrere Benutzer zugewiesen sind.

Zuvor war es Benutzern durch die Integration möglich, eine Aufgabe als abgeschlossen zu markieren, ohne &quot;Fertig mit meinem Teil&quot;oder &quot;Abgeschlossen&quot;oder &quot;Aufgelöst&quot;anzugeben.

Laden Sie die neueste Workfront für Creative Cloud-Plug-ins herunter und installieren Sie sie, um diese Funktion nutzen zu können.

Weitere Informationen zur Funktion finden Sie unter [Kennzeichnen von Arbeitselementen, die mit dem Adobe Workfront-Plug-in abgeschlossen wurden](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Informationen zum Installieren von Workfront für Creative Cloud-Plug-ins finden Sie unter [Installieren des Adobe Workfront-Plug-ins für Creative Cloud-Anwendungen](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Anzeigen und Verwalten von Workfront-Benachrichtigungen über Workfront für Creative Cloud-Plug-ins

Um Ihnen den Empfang der benötigten Benachrichtigungen zu erleichtern, haben wir es ermöglicht, Workfront-Benachrichtigungen anzuzeigen und zu verwalten, ohne die Adobe Creative Cloud verlassen zu müssen. Jetzt können Sie Benachrichtigungen sowie die damit verbundenen Arbeitselemente und Kommentare direkt im Workfront-Plug-in-Fenster in der Creative Cloud-Anwendung anzeigen.

Zuvor waren Benachrichtigungen nur in Workfront und per E-Mail verfügbar.

Laden Sie die neueste Workfront für Creative Cloud-Plug-ins herunter und installieren Sie sie, um diese Funktion nutzen zu können.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten von [!DNL Adobe Workfront] Benachrichtigungen von Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Informationen zum Installieren von Workfront für Creative Cloud-Plug-ins finden Sie unter [Installieren des Adobe Workfront-Plug-ins für Creative Cloud-Anwendungen](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Automatische Erstellung verknüpfter Ordner mit Adobe Experience Manager Assets beim Erstellen eines Projekts

Mit dem neuen Workflow Verknüpften Ordner für die Adobe Experience Manager-Integration erstellen können Sie die Integration mit einem Pfad zu einem Adobe Experience Manager Assets-Ordner konfigurieren. Wenn die Integration zu einer Projektvorlage hinzugefügt wird, erstellen alle aus der Vorlage erstellten Projekte automatisch einen verknüpften Unterordner in Experience Manager Assets im angegebenen Ordner.

Bisher mussten Benutzer zum Erstellen verknüpfter Ordner Aktionen durchführen.

Diese Funktion ist nur bei einer Adobe Experience Manager as a Cloud Service-Integration in Workfront verfügbar. Dies ist im erweiterten Adobe Experience Manager-Connector nicht verfügbar.

Weitere Informationen finden Sie unter [Verwenden von Workflows in der Experience Manager Assets-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Zuordnen von Workfront-Feldwerten zu Tags in Experience Manager Assets

Jetzt können Sie Assets basierend auf Daten aus Workfront kategorisieren und schnell finden. Sie können diese Daten als Teil Ihrer Metadatenkonfiguration in der Workfront für Experience Manager Assets-Integration zuordnen.

Zuvor war die Zuordnung von Workfront-Daten zu Experience Manager Assets-Tags nicht verfügbar.

Weitere Informationen zu dieser Funktion in Experience Manager Assets as a Cloud Service finden Sie unter [Konfigurieren der Integration von [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Weitere Informationen zu dieser Funktion in Experience Manager Assets Essentials finden Sie unter [Experience Manager Assets Essentials-Integration konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Workfront-Felder benutzerdefinierten Experience Manager Assets-Metadatenfeldern zuordnen

Mit der nativen Integration können Sie jetzt sowohl native als auch integrierte Workfront-Felder benutzerdefinierten Metadatenschema-Feldern in Experience Manager Assets as a Cloud Service zuordnen.

Weitere Informationen zu dieser Funktion in Experience Manager Assets as a Cloud Service finden Sie unter [Konfigurieren der Integration von [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Weitere Informationen zu dieser Funktion in Experience Manager Assets Essentials finden Sie unter [Experience Manager Assets Essentials-Integration konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Anpassen der Workflow-Vorlageneinstellungen für automatisierte Testsendungen mit Adobe Workfront für Creative Cloud

Sie können die vorhandenen automatisierten Workflow-Vorlageneinstellungen jetzt direkt im Creative Cloud anpassen. Nachdem Sie eine vorhandene automatisierte Workflow-Vorlage ausgewählt haben, haben Sie folgende Möglichkeiten:

* Deaktivieren von Phasen
* Zusätzliche Empfänger hinzufügen
* TestRollen ändern
* Datum anpassen
* E-Mail-Benachrichtigungen aktualisieren
* Und mehr!

Weitere Informationen finden Sie unter [Hochladen von Dokumenten und Testsendungen mit dem [!DNL Adobe Workfront] Plug-in für  [!DNL Creative Cloud] Anwendungen](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Diese Verbesserungen sind für die folgenden Creative Cloud-Apps verfügbar:

* Photoshop
* XD
* InDesign
* Illustrator
