---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Fehlerbehebung bei der Adobe Experience Manager-Integration
description: 'Problem: Assets werden nicht in Adobe Experience Manager gespeichert'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: 'https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%
---
# Fehlerbehebung bei der Adobe Experience Manager-Integration

## Problem: Assets werden nicht in Adobe Experience Manager gespeichert

Wenn ein(e) Benutzende(r) ein Asset oder einen Ordner auswählt, um es nach Experience Manager Assets zu exportieren, und auf Auswählen klickt, wird das Auswahlfenster geschlossen, die Assets werden jedoch nicht in Experience Manager Assets gespeichert. In Workfront gibt es keinen Hinweis darauf, dass die Assets nicht in Experience Manager Assets gespeichert wurden.

### Ursache

Dies kann aufgrund der Zulassungsliste in Adobe Cloud Manager auftreten. Wenn die Adobe Cloud Manager-Zulassungsliste für ein Unternehmen leer ist, sind IP-Adressen nicht beschränkt und Workfront kann auf die Ordner und Assets des Unternehmens in Adobe Experience Manager zugreifen. Wenn der Cloud Manager-Zulassungsliste jedoch nur eine IP-Adresse hinzugefügt wird, geht die davon aus, dass keine IP-Adresse in der Liste zulässig ist. Wenn die Cloud Manager-Zulassungsliste IP-Adressen enthält, müssen daher die Workfront-IP-Adressen auch zur -Zulassungsliste hinzugefügt werden, damit Workfront Assets an Experience Manager Assets senden kann.

### Lösung:

Fügen Sie die Workfront-IP-Adressen zur Adobe Cloud Manager-Zulassungsliste hinzu.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrer Adobe Cloud Manager finden Sie unter [Einführung in IP-Zulassungslisten &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) in der Dokumentation zu Adobe Experience Manager.
* Eine Liste der Workfront-IP-Adressen, die der Zulassungsliste hinzugefügt werden können, finden Sie unter [Konfigurieren der Firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
