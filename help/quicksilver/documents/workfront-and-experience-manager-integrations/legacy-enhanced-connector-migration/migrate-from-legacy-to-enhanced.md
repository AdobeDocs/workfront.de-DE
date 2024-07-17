---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migration vom alten Connector zum erweiterten Connector
description: Im folgenden Prozess werden die Best Practices für die Umstellung des alten Adobe Experience Manager-Connectors auf den erweiterten Connector zur Integration von Adobe Workfront in AEM Assets erläutert.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Migration vom alten Connector zum erweiterten Connector

Im folgenden Prozess werden die Best Practices für die Umstellung des alten Adobe Experience Manager-Connectors auf den erweiterten Connector zur Integration von Adobe Workfront in AEM Assets erläutert.

>[!IMPORTANT]
>
>Diese Dokumentation gilt nur für Kunden, die Adobe Experience Manager Assets On-Premise- oder Managed Services-Umgebungen verwenden.


Für Kunden mit Adobe Experience Manager Assets as a Cloud Service lautet der Migrationspfad vom alten Connector zur neuen nativen Integration innerhalb von Workfront. Weitere Informationen zu diesem Migrationsprozess finden Sie unter [Migration vom alten oder erweiterten Connector zu Workfront für die Adobe Experience Manager as a Cloud Service-Integration](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Implementieren des erweiterten Connectors

>[!IMPORTANT]
>
>Für die Implementierung des erweiterten Connectors ist ein zertifizierter Partner oder Adobe Consulting Services erforderlich.
>
> Partner, die für den erweiterten Connector zertifizieren möchten, lesen den folgenden Artikel: [Workfront für Experience Manager Enhanced Connector Expert Series](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Informationen zum Implementieren des erweiterten Connectors finden Sie unter [Konfigurieren von Workfront für den Connector für Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Vorhandene Assets verschieben

Nach der Konfiguration Ihrer Umgebung können Sie vorhandene verknüpfte Assets und Ordner nach Adobe Experience Manager verschieben. Dies ist ein optionaler Schritt, stellt jedoch sicher, dass zuvor verknüpfte Ordner und Assets über den Legacy-Connector nach der Deinstallation des Legacy-Connectors weiterhin zugänglich sind.

Weitere Informationen zum Verschieben von Assets finden Sie unter [Verknüpfte Ordner und Dokumente migrieren](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validieren Sie alle kritischen Anwendungsfälle, die verwendet werden sollen

Es ist wichtig, alle wichtigen Anwendungsfälle zu validieren, die über den erweiterten Connector verwendet werden sollen, bevor der alte Connector deinstalliert wird.

## Legacy-Connector deinstallieren

Schließlich müssen Sie den Legacy-Connector deinstallieren. Der alte Connector sollte nicht parallel mit dem erweiterten Connector ausgeführt werden.

Informationen zur Deinstallation finden Sie unter [Deinstallieren des alten Workfront-Connectors mit Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
