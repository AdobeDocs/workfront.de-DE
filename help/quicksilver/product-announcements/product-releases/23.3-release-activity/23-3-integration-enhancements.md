---
title: 23.3 Verbesserungen bei der Integration
description: 23.3 Verbesserungen bei der Integration
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3 Verbesserungen bei der Integration

Auf dieser Seite werden alle Integrationsverbesserungen beschrieben, die mit Version 23.3 vorgenommen wurden. Diese Verbesserungen wurden mit der Version 23.3 vom 20. und 21. Juli 2023 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im Versionszyklus 23.3 verfügbar sind, finden Sie unter Übersicht über Version [23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Neue Google Workspace-Integration jetzt verfügbar

Im Google Marketplace ist jetzt eine neue Google Workspace-Integration verfügbar. Die neue Integration authentifiziert sich über OAuth2 und ersetzt die vorherige Integration.

Die vorherige Google Workspace-Integration ist jetzt veraltet und wird automatisch deinstalliert.

Anweisungen zur Installation der neuen Integration finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Weitere Informationen zu Workfront für Google Workspace finden Sie unter [Workfront für Google Workspace](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud-Integrationen unterstützen jetzt mehrere zugewiesene Benutzende

Die Adobe Creative Cloud-Integration unterstützt jetzt die Möglichkeit, zwischen „Fertig mit meinem Teil“ und „Abgeschlossen“ (oder „Gelöst„) zu wählen, wenn einer Aufgabe oder einem Problem mehrere Benutzende zugewiesen sind.

Zuvor ermöglichte die Integration es Benutzenden, eine Aufgabe als erledigt zu markieren, ohne „Mit meinem Teil erledigt“ oder „Abgeschlossen“/„Aufgelöst“ anzugeben.

Um diese Funktion nutzen zu können, laden Sie die neuesten Workfront for Creative Cloud-Plug-ins herunter und installieren Sie sie.

Weitere Informationen zur Funktionalität finden Sie unter [Arbeitselemente mit dem Adobe Workfront-Plug-in als abgeschlossen markieren](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Informationen zum Installieren der Plug-ins für Workfront for Creative Cloud finden Sie unter [Installieren des Plug-ins für Adobe Workfront for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Anzeigen und Verwalten von Workfront-Benachrichtigungen über die Workfront für Creative Cloud-Plug-ins

Um den Empfang der benötigten Benachrichtigungen zu vereinfachen, haben wir die Anzeige und Verwaltung von Workfront-Benachrichtigungen ermöglicht, ohne die Adobe Creative Cloud verlassen zu müssen. Jetzt können Sie Benachrichtigungen sowie die mit diesen Benachrichtigungen verbundenen Arbeitselemente und Kommentare direkt über das Workfront-Plug-in-Fenster in der Creative Cloud-Anwendung anzeigen.

Zuvor waren Benachrichtigungen nur innerhalb von Workfront und per E-Mail verfügbar.

Um diese Funktion nutzen zu können, laden Sie die neuesten Workfront for Creative Cloud-Plug-ins herunter und installieren Sie sie.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten [!DNL Adobe Workfront]  von Benachrichtigungen aus Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Informationen zum Installieren der Plug-ins für Workfront for Creative Cloud finden Sie unter [Installieren des Plug-ins für Adobe Workfront for Creative Cloud Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Beim Erstellen eines Projekts automatisch verknüpfte Ordner mit Adobe Experience Manager Assets erstellen

Mit dem neuen Workflow Verknüpften Ordner erstellen für die Adobe Experience Manager-Integration können Sie die Integration mit einem Pfad zu einem Adobe Experience Manager Assets-Ordner konfigurieren. Wenn die Integration zu einer Projektvorlage hinzugefügt wird, wird automatisch für alle aus der Vorlage erstellten Projekte ein verknüpfter Unterordner in Experience Manager Assets im angegebenen Ordner erstellt.

Zuvor war für das Erstellen verknüpfter Ordner ein Eingreifen des Benutzers erforderlich.

Diese Funktion ist nur bei einer Adobe Experience Manager as a Cloud Service-Integration in Workfront verfügbar. Dies ist im erweiterten Adobe Experience Manager-Connector nicht verfügbar.

Weitere Informationen finden Sie unter [Verwenden von Workflows in der Experience Manager Assets-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Zuordnen von Workfront-Feldwerten zu Tags in Experience Manager Assets

Jetzt können Sie Assets anhand von Daten aus Workfront kategorisieren und schnell finden. Sie können diese Daten als Teil Ihrer Metadatenkonfiguration in der Integration von Workfront für Experience Manager Assets zuordnen.

Zuvor war das Zuordnen von Workfront-Daten zu Experience Manager Assets-Tags nicht verfügbar.

Weitere Informationen zu dieser Funktion in Experience Manager Assets as a Cloud Service finden Sie unter [Konfigurieren der [!UICONTROL Experience Manager Assets as a Cloud Service]-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Weitere Informationen zu dieser Funktion in Experience Manager Assets Essentials finden Sie unter [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Zuordnen von Workfront-Feldern zu benutzerdefinierten Experience Manager Assets-Metadatenfeldern

Mit der nativen Integration können Sie jetzt sowohl native als auch integrierte Workfront-Felder benutzerdefinierten Metadatenschemafeldern in Experience Manager Assets as a Cloud Service zuordnen.

Weitere Informationen zu dieser Funktion in Experience Manager Assets as a Cloud Service finden Sie unter [Konfigurieren der [!UICONTROL Experience Manager Assets as a Cloud Service]-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Weitere Informationen zu dieser Funktion in Experience Manager Assets Essentials finden Sie unter [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Anpassen der Einstellungen für automatisierte Korrekturabzugs-Workflows mit Adobe Workfront für Creative Cloud

Sie können jetzt bestehende automatisierte Workflow-Vorlageneinstellungen direkt auf der Creative Cloud anpassen. Nachdem Sie eine vorhandene automatisierte Workflow-Vorlage ausgewählt haben, können Sie:

* Stadien deaktivieren
* Zusätzliche Empfänger hinzufügen
* Korrekturabzug-Rollen ändern
* Fristablauf anpassen
* E-Mail-Benachrichtigungen aktualisieren
* Und vieles mehr!

Weitere Informationen finden Sie unter [Hochladen von Dokumenten und Testsendungen mit dem  [!DNL Adobe Workfront] -Plug-in für  [!DNL Creative Cloud] -Programme](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Diese Erweiterungen sind für die folgenden Creative Cloud-Apps verfügbar:

* Photoshop
* XD
* InDesign
* Illustrator
