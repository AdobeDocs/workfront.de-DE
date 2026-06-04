---
title: Verbesserungen bei Integrationen in Version 22.2
description: Verbesserungen bei Integrationen in Version 22.2
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
TQID: https://experienceleague.adobe.com/qTSusDr5AYmDf-RE0-w1bl0OR1vKEER6BwuxKFhCRYI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: bbf3fe51-0066-4980-9062-f8005585ee10
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 777
ht-degree: 2%

---

# Verbesserungen bei Integrationen in Version 22.2

Auf dieser Seite werden alle mit Version 22.2 vorgenommenen Integrationsverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022.

Eine Liste aller Änderungen, die mit Version 22.2 verfügbar sind, finden Sie unter Übersicht über Version [22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront mit Anaplan-Integration jetzt verfügbar

Um Ihnen mehr Flexibilität und insight bei den finanziellen Aspekten Ihrer Workfront-Projekte zu bieten, kann Workfront jetzt in Ihr Anaplan-Konto integriert werden. Durch die Verknüpfung von Workfront-Objekten mit Anaplan-Objekten können Sie die Informationen zwischen den beiden Konten automatisch aktualisieren, um sicherzustellen, dass die Informationen in beiden auf dem neuesten Stand und identisch sind. Sie können auch automatisierte Prozesse in Anaplan basierend auf Aktionen in Workfront (oder umgekehrt) in Trigger nehmen.

Sie können beispielsweise eine Kampagne in Anaplan erstellen und dann ein Workfront-Projekt oder -Programm erstellen, das mit der Kampagne verknüpft ist. Alle in Workfront nachverfolgten Kosten können dann wieder in Anaplan hochgeladen werden, um die Kampagnenleistung zu überprüfen.

Andere Workflows, für die Sie die Integration von Workfront in Anaplan in Betracht ziehen können, sind:

* Erstellen von Anaplan-Budgetanfragen aus neuen Workfront-Projekten
* Erstellen von Workfront-Projekten aus neuen Anaplan-Listenelementen
* Anaplan-Lieferantenanfragen aus Workfront-Projekten initiieren

Weitere Informationen finden Sie unter [Adobe Workfront mit Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Updates für den erweiterten Connector von Workfront für Experience Manager

Der erweiterte Connector von Workfront für Experience Manager enthält jetzt die folgenden Aktualisierungen:

* Sie können jetzt zwischen Adobe Workfront und Adobe Experience Manager Assets as a Cloud Service verknüpfte Ordner erstellen, auch wenn es mehrere Konfigurationen für verknüpfte Projektordner gibt.
* Unterstützung für die Paginierung von Ereignisabonnements hinzugefügt
* Unterstützung für AEM 6.4.x hinzugefügt
* Unterstützung für Proxy-Umgebungen hinzugefügt
* Mehrere Fehlerbehebungen auf der Grundlage von Partner- und Kunden-Feedback

Weitere Informationen finden Sie unter Übersicht über den erweiterten Connector von [Workfront für Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Für die Bereitstellung und Konfiguration dieses Connectors ist ein zertifizierter Partner erforderlich. Weitere Informationen finden [ unter „Installieren des erweiterten Connectors ](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install) Workfront für Experience Manager&quot;.

## Adobe Creative Cloud-Integrationen verwenden jetzt OAuth2

Um die Sicherheit zu erhöhen und ein konsistenteres Erlebnis über alle Integrationen hinweg zu ermöglichen, haben wir die Adobe Creative Cloud-Integrationen aktualisiert, um die OAuth2-Authentifizierung zu verwenden, eine branchenübliche Methode zur Authentifizierung von Benutzern. Wenn sich Ihre Benutzer jetzt anmelden, können sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben und auf die sie zugreifen können. Danach müssen sie sich nicht mehr so häufig anmelden.

Weitere Informationen finden Sie unter [Verwenden der Workfront-Erweiterung für Illustrator und InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Siehe Details zum Client-Geheimnis für benutzerdefinierte OAuth2- oder JWT-Integrationen

Um Transparenz bei der Verwendung Ihrer benutzerdefinierten OAuth2- und JWT-Integrationen zu gewährleisten, haben wir es Ihnen ermöglicht, Details zu den von Ihren Integrationen verwendeten Client-Geheimnissen anzuzeigen. Jetzt können Sie die Daten sehen, an denen das Client-Geheimnis erstellt und zuletzt verwendet wurde. Sie können auch eigene Notizen zum Client-Geheimnis hinzufügen und anzeigen.

Zuvor waren diese Details nicht verfügbar.

Weitere Informationen zu Client-Geheimnissen in benutzerdefinierten OAuth2- oder JWT-Integrationen finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Siehe Authentifizierungstyp in der Liste der benutzerdefinierten OAuth2-Anwendungen

Wenn Sie nun die Liste der benutzerdefinierten OAuth2-Anwendungen in Ihrer Organisation anzeigen, können Sie sehen, ob jede Anwendung die Benutzerauthentifizierung oder die Serverauthentifizierung verwendet.

Zuvor konnten Sie diese Informationen nur sehen, indem Sie in die Bearbeitungsoptionen der einzelnen Programme navigierten.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Festlegen des Ablaufs für Aktualisierungs-Token in Ihren benutzerdefinierten OAuth2-Integrationen

Um den Zugriff und die Sicherheit für Ihre benutzerdefinierten OAuth2-Integrationen besser zu steuern, können Sie jetzt die Lebensdauer von Aktualisierungs-Token anpassen. Nachdem das Aktualisierungs-Token einer Benutzerin oder eines Benutzers abgelaufen ist, muss sie bzw. er sich erneut bei der Integration anmelden.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Verwenden Sie öffentliche und private Schlüssel in Ihren benutzerdefinierten OAuth2-Integrationen für Server-zu-Server-Apps

Sie können jetzt OAuth2-Server-zu-Server-Anwendungen in Ihren benutzerdefinierten Integrationen einrichten. Durch das Einrichten von öffentlichen und privaten Schlüsseln können Sie Workfront erlauben, mit einer anderen Anwendung zu kommunizieren, ohne Anmeldeinformationen zu verwenden.

Zuvor verwendete die gesamte Authentifizierung in Ihren benutzerdefinierten OAuth2-Anwendungen die Anmeldedaten des Benutzers.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Die Google Google Workspace-Integration verwendet jetzt OAuth2

Um die Sicherheit zu erhöhen und ein konsistenteres Erlebnis über Integrationen hinweg zu ermöglichen, haben wir die Google Google Workspace-Integration aktualisiert, um die OAuth2-Authentifizierung zu verwenden, eine branchenübliche Methode zur Authentifizierung von Benutzern. Wenn sich Ihre Benutzer jetzt anmelden, können sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben und auf die sie zugreifen können. Danach müssen sie sich nicht mehr so häufig anmelden.

Weitere Informationen finden Sie unter [An- und Abmelden von Adobe Workfront für Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
