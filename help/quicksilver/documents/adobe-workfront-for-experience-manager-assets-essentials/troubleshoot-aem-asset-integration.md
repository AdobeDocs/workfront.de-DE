---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Fehlerbehebung bei der Adobe Experience Manager-Integration
description: Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials - EDIT ME.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Fehlerbehebung bei der Adobe Experience Manager-Integration

## Problem: Assets werden nicht in Adobe Experience Manager gespeichert

Wenn ein Benutzer ein Asset oder einen Ordner auswählt, das bzw. der in Experience Manager Assets exportiert werden soll, und auf Auswählen klickt, wird das Auswahlfenster geschlossen, die Assets werden jedoch nicht in Experience Manager Assets gespeichert. In Workfront gibt es keinen Hinweis darauf, dass die Vermögenswerte nicht in Experience Manager Assets gespeichert wurden.

### Ursache

Dies kann aufgrund der Zulassungsliste in Adobe Cloud Manager auftreten. Wenn die Adobe Cloud Manager-Zulassungsliste für eine Organisation leer ist, sind IP-Adressen nicht beschränkt und Workfront kann auf die Ordner und Assets der Organisation in Adobe Experience Manager zugreifen. Wenn jedoch auch nur eine einzelne IP-Adresse zur Cloud Manager-Zulassungsliste hinzugefügt wird, geht die Zulassungsliste davon aus, dass alle IP-Adressen, die nicht auf der Liste stehen, nicht zulässig sind. Wenn die Zulassungsliste des Cloud Manager-Zulassungsliste IP-Adressen enthält, müssen daher auch die Workfront-IP-Adressen zur Cloud- hinzugefügt werden, damit Workfront Assets an Experience Manager Assets senden kann.

### Lösung:

Fügen Sie der Adobe Cloud Manager -IP-Adressen die Workfront-IP-Adressen hinzu.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrem Adobe Cloud Manager finden Sie unter [Einführung in IP-Zulassungslisten](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) in der Adobe Experience Manager-Dokumentation.
* Eine Liste der Workfront-IP-Adressen, die zur Zulassungsliste hinzugefügt werden sollen, finden Sie unter [Konfigurieren der Firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


