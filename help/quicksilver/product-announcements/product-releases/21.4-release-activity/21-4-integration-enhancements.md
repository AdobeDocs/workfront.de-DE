---
title: 21.4 Verbesserungen bei der Integration
description: 21.4 Verbesserungen bei der Integration
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 21.4 Verbesserungen bei der Integration

Auf dieser Seite werden alle mit Version 21.4 vorgenommenen Integrationsverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 4. Oktober 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie in der Übersicht über die Version [21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Dokumente aus Dropbox Business verknüpfen

Wir haben Dropbox Business als verfügbare Dokumentenintegration hinzugefügt. Jetzt können Sie direkt von Workfront aus auf Dokumente zugreifen, die Sie in Dropbox Business gespeichert haben.

Mit Dropbox Business können Sie freigegebene Dokumente verknüpfen und Dokumente in freigegebene Ordner hochladen. Beim Dropbox (nicht beim Dropbox-Business) kann nur der Eigentümer der Dokumente das Dokument in Workfront anzeigen.

Ihr Workfront-Administrator kann diese Integration für Ihr Unternehmen aktivieren.

Weitere Informationen finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Informationen dazu, wie Workfront-Admins diese Option aktivieren können, finden Sie unter [Konfigurieren von Dokumentintegrationen](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Updates für Workfront zum Slack

Die folgenden Aktualisierungen sind jetzt in der Workfront für Slack-Integration sichtbar:

* Workfront für Slack hat ein neues Look-and-Feel.
* Jetzt erhalten Sie Ihre Workfront für Slack-Benachrichtigungen in Echtzeit.

  Wenn Sie beispielsweise einer Aufgabe zugewiesen sind, erhalten Sie diese Benachrichtigung, sobald Sie zugewiesen sind. Zuvor konnte es zu einer Verzögerung kommen, bevor die Benachrichtigung auf Slack erschien.

Dieses Update erfordert, dass Sie Ihre Workfront für die Slack-Integration erneut autorisieren. Informationen zum Autorisieren der Integration finden Sie unter [Konfigurieren von Adobe Workfront für Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Weitere Informationen zu Workfront für Slack-Benachrichtigungen finden Sie unter [Empfangen von Adobe Workfront-Benachrichtigungen auf Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Genauere Anzeige der Details zum Kontozugriff bei der Erteilung der Zustimmung zu Adobe Workfront-Integrationen

Die Einverständnisbildschirme für Adobe Workfront-Integrationen werden jetzt aktualisiert. Jetzt können Sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben, damit Sie besser verstehen können, auf was Sie der Integration oder Anwendung Zugriff gewähren.

Dieser neue Einverständnisbildschirm gilt für alle Adobe Workfront-Integrationen, die OAuth 2.0 verwenden.

Einzelheiten zu bestimmten Integrationen finden Sie in der Dokumentation dieser Integration.

## API-Schlüsselauthentifizierung für Integrationen nicht mehr erforderlich

Workfront-Integrationen verwenden seit kurzem OAuth2, um die Sicherheit und Benutzerfreundlichkeit zu erhöhen. Als Teil dieser Umstellung erfordert Workfront keine API-Schlüssel mehr für die Authentifizierung von Integrationen.
