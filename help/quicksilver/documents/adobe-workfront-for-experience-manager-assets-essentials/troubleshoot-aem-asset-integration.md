---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Fehlerbehebung bei der Adobe Experience Manager-Integration
description: 'Problem: Assets wird nicht in Adobe Experience Manager gespeichert'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Fehlerbehebung bei der Adobe Experience Manager-Integration

## Problem: Assets wird nicht in Adobe Experience Manager gespeichert

Wenn ein Benutzer ein Asset oder einen Ordner auswählt, das bzw. der in Experience Manager Assets exportiert werden soll, und auf Auswählen klickt, wird das Auswahlfenster geschlossen, die Assets werden jedoch nicht in Experience Manager Assets gespeichert. In Workfront gibt es keinen Hinweis darauf, dass die Vermögenswerte nicht in Experience Manager Assets gespeichert wurden.

### Ursache

Dies kann aufgrund der Zulassungsliste in Adobe Cloud Manager auftreten. Wenn die Adobe Cloud Manager für eine Organisation leer ist, sind IP-Adressen nicht beschränkt und Workfront kann auf die Ordner und Assets der Organisation in Adobe Experience Manager zugreifen. Wenn jedoch auch nur eine IP-Adresse zur Cloud Manager-Zulassungsliste hinzugefügt wird, geht die Zulassungsliste davon aus, dass jede IP-Adresse, die nicht auf der Liste steht, nicht zulässig ist. Wenn die Cloud Manager-Zulassungsliste daher IP-Adressen enthält, müssen die IP-Adressen von Workfront zur auf die Zulassungsliste setzen-Workfronts hinzugefügt werden, damit Assets an Experience Manager Assets senden kann.

### Lösung:

Fügen Sie die Workfront-IP-Adressen zur Adobe Cloud Manager-IP-Zulassungsliste hinzu.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrer Adobe Cloud Manager finden Sie unter [Einführung in IP-Zulassungslisten](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) in der Adobe Experience Manager-Dokumentation.
* Eine Liste der Workfront-IP-Adressen, die zur Zulassungsliste hinzugefügt werden sollen, finden Sie unter [Konfigurieren der Firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
