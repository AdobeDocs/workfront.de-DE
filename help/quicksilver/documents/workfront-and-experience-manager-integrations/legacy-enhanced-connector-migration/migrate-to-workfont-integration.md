---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrieren vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration
description: Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von den erweiterten oder veralteten Workfront for Experience Cloud-Connectoren zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 497
ht-degree: 0%

---

# Migrieren vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration

Die Informationen auf dieser Seite erläutern die Best Practices für den Wechsel von den erweiterten oder veralteten Workfront for Experience Cloud-Connectoren zur neuesten nativen Integration, die Workfront und Adobe Experience Manager Assets as a Cloud Service verbindet.

>[!IMPORTANT]
>
>Diese Informationen gelten nicht für Kunden, die Adobe Experience Manager Assets On-Premise- oder Managed Services-Umgebungen verwenden.

## Verschieben der Workfront-Instanz in die Admin Console

Kunden, die die neue native Integration zwischen Workfront und Adobe Experience Manager Assets as a Cloud Service verwenden möchten, müssen sicherstellen, dass ihre Workfront-Umgebung an eine Adobe Admin Console gebunden ist. Bei bestehenden Workfront-Umgebungen ist dazu wahrscheinlich eine Migration der Umgebung zu einem verbundenen Adobe Admin Console erforderlich. Weitere Informationen zu dieser Migration und der zugehörigen Checkliste finden Sie unter [Vorbereiten der Integration Ihres Unternehmens in die Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe muss bei dieser Migration helfen. Um Hilfe anzufordern, führen Sie einen der folgenden Schritte aus:

* Wenn Sie Zugriff auf Workfront Hub haben, senden Sie Ihre Anfrage an die [Workfront-Migration zu Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* Wenn Sie keinen Zugriff auf Workfront Hub haben, können Sie Ihre Anfrage an die Warteschlange für frühzeitige Migrationsanfragen von [Workfront an Adobe Admin Console &#x200B;](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

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
