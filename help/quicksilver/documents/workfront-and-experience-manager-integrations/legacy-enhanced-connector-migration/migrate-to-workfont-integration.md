---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migration vom alten oder erweiterten Connector zu Workfront for Adobe Experience Manager as a Cloud Service-Integration
description: Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von erweiterten oder veralteten Connectoren von Workfront für Experience Cloud zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migration vom alten oder erweiterten Connector zu Workfront for Adobe Experience Manager as a Cloud Service-Integration

Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von erweiterten oder veralteten Connectoren von Workfront für Experience Cloud zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

>[!IMPORTANT]
>
>Diese Informationen gelten nicht für Kunden, die Adobe Experience Manager Assets On-Premise- oder Managed Services-Umgebungen verwenden.

## Verschieben der Workfront-Instanz in die Admin Console

Kunden, die die neue native Integration zwischen Workfront und Adobe Experience Manager Assets as a Cloud Service verwenden möchten, müssen sicherstellen, dass ihre Workfront-Umgebung mit einer Adobe Admin Console verknüpft ist. Bei bestehenden Workfront-Umgebungen ist dies wahrscheinlich eine Migration der Umgebung auf eine verbundene Adobe Admin Console erforderlich. Weitere Informationen zu dieser Migration und der zugehörigen Checkliste finden Sie unter [Vorbereitung zur Integration Ihres Unternehmens in die Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe muss bei der Durchführung dieser Migration helfen. Führen Sie einen der folgenden Schritte aus, um Hilfe anzufordern:

* Wenn Sie Zugriff auf Workfront Hub haben, senden Sie Ihre Anfrage an die [Workfront-Migration zu Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Wenn Sie keinen Workfront Hub-Zugriff haben, können Sie Ihre Anfrage an die [Warteschlange für frühzeitige Migration von Workfront zu Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Neue as a Cloud Service Integration von Workfront für Adobe Experience Manager Assets konfigurieren

Nachdem Ihre Workfront-Umgebung in eine Adobe Admin Console migriert wurde, können Workfront-Administratoren die neue native Integration konfigurieren. Hilfe zur Konfiguration finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Vorhandene Assets in Workfront für die as a Cloud Service Integration von Adobe Experience Manager Assets verschieben

Nach der Konfiguration Ihrer Umgebung können Sie vorhandene verknüpfte Assets und Ordner nach Adobe Experience Manager verschieben. Dies ist ein optionaler Schritt, stellt jedoch sicher, dass zuvor verknüpfte Ordner und Assets über den alten oder erweiterten Connector weiterhin verfügbar sind, sobald diese Connectoren deinstalliert wurden.

Weitere Informationen zum Verschieben von Assets finden Sie unter [Verknüpfte Ordner und Dokumente migrieren](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validieren Sie alle kritischen Anwendungsfälle, die verwendet werden sollen.

Es ist wichtig, alle wichtigen Anwendungsfälle zu validieren, die für die native Integration vorgesehen sind, bevor Sie den alten oder erweiterten Connector deinstallieren.

## Deinstallieren des alten oder erweiterten Connectors

Schließlich müssen Sie den alten oder erweiterten Connector deinstallieren. Die native Integration sollte nicht parallel mit einem der beiden Connectoren ausgeführt werden.

Informationen zur Deinstallation finden Sie unter

* Anweisungen zur Deinstallation älterer Connectoren: [Deinstallieren des Legacy-Connectors von Workfront mit Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Verbesserte Anweisungen zur Connector-Deinstallation: [Deinstallieren des erweiterten Connectors Workfront mit Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
