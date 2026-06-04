---
title: Verbesserungen bei Integrationen in Version 21.4
description: Verbesserungen bei Integrationen in Version 21.4
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
TQID: https://experienceleague.adobe.com/dCRr9YQiXiX82Jw7wyeT786T8oJ74-u6kOuevYy-SWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 367
ht-degree: 2%

---

# Verbesserungen bei Integrationen in Version 21.4

Auf dieser Seite werden alle mit Version 21.4 vorgenommenen Integrationsverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 4. Oktober 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie in der Übersicht über die Version [21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Verknüpfen von Dokumenten aus Dropbox Business

Wir haben Dropbox Business als verfügbare Dokumentenintegration hinzugefügt. Jetzt können Sie direkt von Workfront aus auf Dokumente zugreifen, die Sie in Dropbox Business gespeichert haben.

Mit Dropbox Business können Sie freigegebene Dokumente verknüpfen und Dokumente in freigegebene Ordner hochladen. Dropbox (nicht Dropbox Business) ermöglicht es nur dem Eigentümer der Dokumente, das Dokument in Workfront anzuzeigen.

Ihr Workfront-Administrator kann diese Integration für Ihr Unternehmen aktivieren.

Weitere Informationen finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Informationen dazu, wie Workfront-Admins diese Option aktivieren können, finden Sie unter [Konfigurieren von Dokumentintegrationen](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Aktualisierungen für Workfront für Slack

Die folgenden Aktualisierungen sind jetzt in der Integration von Workfront für Slack sichtbar:

* Workfront für Slack hat ein neues Look-and-Feel.
* Jetzt erhalten Sie Ihre Workfront for Slack-Benachrichtigungen in Echtzeit.

  Wenn Sie beispielsweise einer Aufgabe zugewiesen sind, erhalten Sie diese Benachrichtigung, sobald Sie zugewiesen sind. Zuvor konnte es zu Verzögerungen kommen, bevor die Benachrichtigung in Slack erschien.

Dieses Update erfordert, dass Sie Ihre Workfront für die Slack-Integration erneut autorisieren. Informationen zum Autorisieren der Integration finden Sie unter [Konfigurieren von Adobe Workfront für Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Weitere Informationen zu Workfront für Slack-Benachrichtigungen finden Sie unter [Empfangen von Adobe Workfront-Benachrichtigungen in Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Genauere Anzeige der Details zum Kontozugriff bei der Erteilung der Zustimmung zu Adobe Workfront-Integrationen

Die Einverständnisbildschirme für Adobe Workfront-Integrationen werden jetzt aktualisiert. Jetzt können Sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben, damit Sie besser verstehen können, auf was Sie der Integration oder Anwendung Zugriff gewähren.

Dieser neue Einverständnisbildschirm gilt für alle Adobe Workfront-Integrationen, die OAuth 2.0 verwenden.

Einzelheiten zu bestimmten Integrationen finden Sie in der Dokumentation dieser Integration.

## API-Schlüsselauthentifizierung für Integrationen nicht mehr erforderlich

Workfront-Integrationen verwenden seit kurzem OAuth2, um die Sicherheit und Benutzerfreundlichkeit zu erhöhen. Als Teil dieser Umstellung erfordert Workfront keine API-Schlüssel mehr für die Authentifizierung von Integrationen.
