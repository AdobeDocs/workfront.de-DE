---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrieren vom alten Connector zum erweiterten Connector
description: Im folgenden Prozess werden die Best Practices für den Wechsel vom alten Adobe Experience Manager-Connector zum erweiterten Connector für die Integration von Adobe Workfront mit AEM Assets beschrieben.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

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
