---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrieren vom alten Connector zum erweiterten Connector
description: Im folgenden Prozess werden die Best Practices für den Wechsel vom alten Adobe Experience Manager-Connector zum erweiterten Connector für die Integration von Adobe Workfront mit AEM Assets beschrieben.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
TQID: 'https://experienceleague.adobe.com/px8ysyDqpwzajmCfRPJLclKOUSuIFacl99Uf6sRCKFQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 5%
---
# Migrieren vom alten Connector zum erweiterten Connector

Im folgenden Prozess werden die Best Practices für den Wechsel vom alten Adobe Experience Manager-Connector zum erweiterten Connector für die Integration von Adobe Workfront mit AEM Assets beschrieben.

>[!IMPORTANT]
>
>Diese Dokumentation gilt nur für Kunden, die Adobe Experience Manager Assets On-Premise- oder Managed Services-Umgebungen verwenden.


Für Kunden mit Adobe Experience Manager Assets as a Cloud Service lautet der Migrationspfad vom alten Connector zur neuen nativen Integration in Workfront. Weitere Informationen zu diesem Migrationsprozess finden Sie unter [Migration vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementieren des erweiterten Connectors

>[!IMPORTANT]
>
>Für die Implementierung des erweiterten Connectors ist ein zertifizierter Partner für Adobe Consulting Services erforderlich.
>
> Partner, die für den erweiterten Connector zertifizieren möchten, lesen bitte den folgenden Artikel: [Workfront for Experience Manager Enhanced Connector Expert Series](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview).

Informationen zum Implementieren des erweiterten Connectors finden Sie unter [Konfigurieren des erweiterten Connectors für Workfront für Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/integrations/workfront-connector-configure).


## Verschieben vorhandener Assets

Nachdem Sie Ihre Umgebung konfiguriert haben, können Sie vorhandene verknüpfte Assets und Ordner nach Adobe Experience Manager verschieben. Dies ist ein optionaler Schritt, stellt jedoch sicher, dass auf zuvor verknüpfte Ordner und Assets über den Legacy-Connector weiterhin zugegriffen werden kann, sobald der Legacy-Connector deinstalliert wird.

Weitere Informationen zum Verschieben von Assets finden Sie unter [Migrieren verknüpfter Ordner und Dokumente](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validieren aller kritischen Anwendungsfälle, die verwendet werden sollen

Es ist wichtig, alle kritischen Anwendungsfälle, die über den erweiterten Connector verwendet werden sollen, vor der Deinstallation des alten Connectors zu validieren.

## Legacy-Connector deinstallieren

Schließlich müssen Sie den Legacy-Connector deinstallieren. Der alte Connector ist nicht für die parallele Ausführung mit dem erweiterten Connector vorgesehen.

Informationen zur Deinstallation finden Sie unter [Workfront mit dem Legacy-Connector von Adobe Experience Manager deinstallieren](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
