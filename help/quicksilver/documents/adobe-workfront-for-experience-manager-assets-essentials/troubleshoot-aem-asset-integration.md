---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Fehlerbehebung bei der Adobe Experience Manager-Integration
description: "Problem: Assets werden nicht in Adobe Experience Manager gespeichert"
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: tm+mt
source-wordcount: '241'
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


