---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Fehlerbehebung bei der Adobe Experience Manager-Integration
description: 'Problem: Assets werden nicht in Adobe Experience Manager gespeichert'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Fehlerbehebung bei der Adobe Experience Manager-Integration

## Problem: Assets werden nicht in Adobe Experience Manager gespeichert

Wenn ein(e) Benutzende(r) ein Asset oder einen Ordner auswählt, um es nach Experience Manager Assets zu exportieren, und auf Auswählen klickt, wird das Auswahlfenster geschlossen, die Assets werden jedoch nicht in Experience Manager Assets gespeichert. In Workfront gibt es keinen Hinweis darauf, dass die Assets nicht in Experience Manager Assets gespeichert wurden.

### Ursache

Dies kann aufgrund der Zulassungsliste in Adobe Cloud Manager auftreten. Wenn die Adobe Cloud Manager-Zulassungsliste für ein Unternehmen leer ist, sind IP-Adressen nicht beschränkt und Workfront kann auf die Ordner und Assets des Unternehmens in Adobe Experience Manager zugreifen. Wenn der Cloud Manager-Zulassungsliste auf die Zulassungsliste setzte jedoch nur eine IP-Adresse hinzugefügt wird, geht die davon aus, dass keine IP-Adresse in der Liste zulässig ist. Wenn die Cloud Manager-Zulassungsliste IP-Adressen enthält, müssen daher die Workfront-IP-Adressen auch zur -Zulassungsliste hinzugefügt werden, damit Workfront Assets an Experience Manager Assets senden kann.

### Lösung:

Fügen Sie die Workfront-IP-Adressen zur Adobe Cloud Manager-Zulassungsliste hinzu.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrer Adobe Cloud Manager finden Sie unter [Einführung in IP-Zulassungslisten ](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) in der Dokumentation zu Adobe Experience Manager.
* Eine Liste der Workfront-IP-Adressen, die der Zulassungsliste hinzugefügt werden können, finden Sie unter [Konfigurieren der Firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
