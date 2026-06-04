---
title: Verbesserungen bei der Integration im ersten Quartal 2024
description: Verbesserungen bei der Integration im ersten Quartal 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
TQID: https://experienceleague.adobe.com/ZPt9H-R2eSNNha-gjfwkgnUOQqvU5tzAQPE5fMA-9uA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 385
ht-degree: 0%

---

# Verbesserungen bei der Integration im ersten Quartal 2024

Auf dieser Seite werden alle Integrationsverbesserungen beschrieben, die mit der Version vom ersten Quartal 2024 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden mit der Version vom ersten Quartal 2024 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im ersten Quartal 2024 verfügbar sind, finden Sie unter [Versionsübersicht 1. Quartal 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Beim Zuordnen von Metadaten in Experience Manager Assets Essentials wird jetzt `xcm:keywords` anstelle von `dc:subject` verwendet

Wir haben die Experience Manager Assets Essentials-Integration aktualisiert, damit sie dem Erlebnis der Experience Manager Assets as a Cloud Service-Integration entspricht. Wenn Sie nun in Experience Manager Assets mehrere einzeilige Textfelder einem einzigen Feld zuordnen, verwenden beide Services das `xcm:keywords`.

Zuvor wurden diese Felder dem `dc:subject` Feld in Experience Manager Assets Essentials zugeordnet. Die Funktionalität von Experience Manager Assets as a Cloud Service bleibt unverändert.

Alle Experience Manager Assets Essentials-Metadaten, die derzeit `dc:subject` zugeordnet sind, müssen `xcm:keywords` zugeordnet werden.

Informationen zum Zuordnen von Metadaten zu Experience Manager Assets Essentials finden Sie unter [AEM-Schlüsselwort](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Typeahead-Felder sind jetzt in Adobe Experience Manager Integration verfügbar

Um die Verknüpfung von Feldern zwischen Workfront und Adobe Experience Manager zu vereinfachen, haben wir Unterstützung für automatische Textvervollständigung in der Metadatenzuordnung hinzugefügt. Jetzt können Sie die Felder mit automatischer Textvervollständigung den entsprechenden Feldern in Adobe Experience Manager zuordnen.

Wenn ein(e) Benutzende(r) einen anderen Wert für ein Feld in Workfront auswählt, wird diese Änderung sofort in Adobe Experience Manager übernommen. Wenn sich der Feldwert einer Option ändert (z. B. wenn ein Team den Namen in einen neuen Namen ändert), wird diese Änderung auch in Adobe Experience Manager übernommen.

Informationen und Anweisungen zur Metadatenzuordnung in der Adobe Experience Manager-Integration finden Sie unter [Einrichten von Metadaten](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Automatisches Veröffentlichen von Assets in Adobe Experience Manager

Wir haben der Adobe Experience Manager-Integration einen weiteren Workflow hinzugefügt. Jetzt können Sie Ihre Assets so einstellen, dass sie automatisch veröffentlicht werden, wenn sie an Adobe Experience Manager gesendet werden. Die Integration kann so konfiguriert werden, dass sie im Adobe Experience Manager-Veröffentlichungs-Service oder in Adobe Experience Manager Brand Portal veröffentlicht wird.

Der Workflow für die automatische Veröffentlichung kann in der Adobe Experience Manager-Integration aktiviert und konfiguriert werden. Nach der Aktivierung kann der Workflow auf Projektvorlagen- oder Projektebene bearbeitet werden.

Weitere Informationen finden Sie unter [Veröffentlichen von &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets)&quot; in [Verwenden von Workflows in der Experience Manager Assets-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
