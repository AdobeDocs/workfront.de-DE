---
title: Integrationsverbesserungen für das erste Quartal 2024
description: Integrationsverbesserungen für das erste Quartal 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Integrationsverbesserungen für das erste Quartal 2024

Auf dieser Seite werden alle Integrationsverbesserungen beschrieben, die mit der Version vom ersten Quartal 2024 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung mit der Version vom ersten Quartal 2024 verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im Versionszyklus des ersten Quartals 2024 verfügbar sind, finden Sie unter [Versionsübersicht für das erste Quartal 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Beim Zuordnen von Metadaten in Experience Manager Assets Essentials wird jetzt `xcm:keywords` anstelle von `dc:subject` verwendet

Die Integration von Experience Manager Assets Essentials wurde aktualisiert und entspricht nun den Erlebnissen der Experience Manager Assets as a Cloud Service-Integration. Wenn nun mehrere einzeilige Textfelder in Experience Manager Assets einem einzelnen Feld zugeordnet werden, verwenden beide Dienste das Feld `xcm:keywords` .

Zuvor wurden diese Felder dem Feld `dc:subject` in Experience Manager Assets Essentials zugeordnet. Die Experience Manager Assets as a Cloud Service-Funktionalität bleibt unverändert.

Alle Experience Manager Assets Essentials-Metadaten, die derzeit `dc:subject` zugeordnet sind, müssen auf `xcm:keywords` neu zugeordnet werden.

Informationen zum Zuordnen von Metadaten zu Experience Manager Assets Essentials finden Sie unter [AEM Keyword](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Felder mit Typvorschau sind jetzt in der Adobe Experience Manager-Integration verfügbar.

Um die Verknüpfung von Feldern zwischen Workfront und Adobe Experience Manager zu vereinfachen, wurde Unterstützung für Typeahead-Felder in der Metadaten-Zuordnung hinzugefügt. Jetzt können Sie Typeahead-Felder entsprechenden Feldern in Adobe Experience Manager zuordnen.

Wenn ein Benutzer einen anderen Wert für ein Feld in Workfront auswählt, wird diese Änderung sofort in Adobe Experience Manager übernommen. Wenn sich außerdem eine Feldwertoption ändert (z. B. wenn ein Team seinen Namen in einen neuen Namen ändert), wird diese Änderung auch in Adobe Experience Manager übernommen.

Informationen und Anweisungen zur Metadatenzuordnung in der Adobe Experience Manager-Integration finden Sie unter [Einrichten von Metadaten](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Automatisches Veröffentlichen von Assets in Adobe Experience Manager

Wir haben der Adobe Experience Manager-Integration einen weiteren Workflow hinzugefügt. Jetzt können Sie festlegen, dass Ihre Assets automatisch veröffentlicht werden, wenn sie an Adobe Experience Manager gesendet werden. Die Integration kann so konfiguriert werden, dass sie im Adobe Experience Manager-Veröffentlichungsdienst oder in einem Adobe Experience Manager-Brand Portal veröffentlicht wird.

Der Workflow &quot;Automatischer Publish&quot;kann in der Adobe Experience Manager-Integration aktiviert und konfiguriert werden. Wenn diese Option aktiviert ist, kann der Workflow auf der Projektvorlage oder Projektebene bearbeitet werden.

Weitere Informationen finden Sie unter [Veröffentlichen von Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Verwenden von Workflows in der Experience Manager Assets-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
