---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrieren vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration
description: Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von den erweiterten oder veralteten Connectoren von Workfront für Experience Cloud zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Migrieren vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration

Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von den erweiterten oder veralteten Connectoren von Workfront für Experience Cloud zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

>[!IMPORTANT]
>
>Diese Informationen gelten nicht für Kunden, die Adobe Experience Manager Assets On-Premise- oder Managed Services-Umgebungen verwenden.

## Verschieben der Workfront-Instanz in die Admin Console

>[!IMPORTANT]
>
>Da alle Workfront-Organisationen in die Adobe Admin Console migriert wurden, wird dieser Abschnitt in naher Zukunft entfernt.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## Konfigurieren der as a Cloud Service-Integration Ihres neuen Workfront für Adobe Experience Manager Assets

Nachdem Ihre Workfront-Umgebung in eine Adobe Admin Console migriert wurde, können Workfront-Administratoren die neue native Integration konfigurieren. Konfigurationshilfen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Verschieben vorhandener Assets in Ihre Workfront für die as a Cloud Service-Integration mit Adobe Experience Manager Assets

Nachdem Sie Ihre Umgebung konfiguriert haben, können Sie vorhandene verknüpfte Assets und Ordner nach Adobe Experience Manager verschieben. Dies ist ein optionaler Schritt, stellt jedoch sicher, dass zuvor verknüpfte Ordner und Assets über den alten oder erweiterten Connector weiterhin verfügbar sind, sobald diese Connectoren deinstalliert werden.

Weitere Informationen zum Verschieben von Assets finden Sie unter [Migrieren verknüpfter Ordner und Dokumente](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validieren aller kritischen Anwendungsfälle, die verwendet werden sollen

Es ist wichtig, alle kritischen Anwendungsfälle, die über die native Integration verwendet werden sollen, vor der Deinstallation des alten oder erweiterten Connectors zu validieren.

## Deinstallieren des alten oder erweiterten Connectors

Schließlich müssen Sie den alten oder erweiterten Connector deinstallieren. Die native Integration ist nicht für die parallele Ausführung mit einem der beiden Connectoren vorgesehen.

Zur Deinstallation siehe

* Deinstallationsanweisungen für alten Connector: [Deinstallieren Sie den Workfront mit dem Legacy-Connector von Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Deinstallationsanweisungen für den erweiterten Connector: [Deinstallieren Sie den erweiterten Connector von Workfront mit Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
