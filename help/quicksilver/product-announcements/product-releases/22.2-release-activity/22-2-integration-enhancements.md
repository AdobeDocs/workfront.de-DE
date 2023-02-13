---
title: 2.2 Integrationsverbesserungen
description: 2.2 Integrationsverbesserungen
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 2.2 Integrationsverbesserungen

Auf dieser Seite werden alle Integrationsverbesserungen beschrieben, die mit Version 22.2 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022.

Eine Liste aller in Version 22.2 verfügbaren Änderungen finden Sie unter [2.2 Versionsübersicht](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront mit Anaplan-Integration jetzt verfügbar

Um Ihnen mehr Flexibilität und Einblicke in die finanziellen Aspekte Ihrer Workfront-Projekte zu geben, kann Workfront jetzt in Ihr Anaplan-Konto integriert werden. Durch die Verknüpfung von Workfront-Objekten mit Anaplan-Objekten können Sie Informationen zwischen den beiden Konten automatisch aktualisieren und sicherstellen, dass die Informationen in beiden Konten aktuell und identisch sind. Sie können in Anaplan auch automatisierte Prozesse auf der Basis von Aktionen in Workfront (oder umgekehrt) Trigger haben.

Sie können beispielsweise eine Kampagne in Anaplan erstellen und dann ein mit der Kampagne verknüpftes Workfront-Projekt oder -Programm erstellen. Alle in Workfront verfolgten Kosten können dann wieder in Anaplan hochgeladen werden, um die Kampagnenleistung zu überprüfen.

Weitere Workflows, für die Sie möglicherweise die Integration von Workfront in Anaplan verwenden, umfassen:

* Erstellen von Anaplan-Budgetanforderungen aus neuen Workfront-Projekten
* Erstellen von Workfront-Projekten aus neuen Anaplan-Listenelementen
* Initiierung von Anaplan-Lieferanfragen von Workfront-Projekten

Weitere Informationen finden Sie unter [Adobe Workfront mit Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront für Experience Manager - verbesserte Connector-Updates

Der erweiterte Connector von Workfront für Experience Manager umfasst jetzt die folgenden Updates:

* Sie können jetzt verknüpfte Ordner zwischen Adobe Workfront und Adobe Experience Manager Assets as a Cloud Service erstellen, auch wenn mehrere projektverknüpfte Ordnerkonfigurationen vorhanden sind.
* Unterstützung für die Seitennummerierung bei Ereignisabonnements hinzugefügt
* Hinzugefügte Unterstützung für AEM 6.4.x
* Unterstützung für Proxy-Umgebungen hinzugefügt
* Mehrere Fehlerbehebungen basierend auf Partner- und Kunden-Feedback

Weitere Informationen finden Sie unter [Übersicht über den Connector für Workfront für Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Für die Bereitstellung und Konfiguration dieses Connectors ist ein zertifizierter Partner erforderlich. Siehe [Workfront für Experience Manager-Connector installieren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) für weitere Informationen.

## Adobe Creative Cloud-Integrationen verwenden jetzt OAuth2

Für mehr Sicherheit und ein konsistenteres Erlebnis über Integrationen hinweg haben wir die Adobe Creative Cloud-Integrationen aktualisiert und verwenden nun die OAuth2-Authentifizierung, eine branchenübliche Methode zur Benutzerauthentifizierung. Wenn sich Ihre Benutzer jetzt anmelden, können sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben und Zugriff gewähren. Danach müssen sie sich nicht so häufig anmelden.

Weitere Informationen finden Sie unter [Verwenden der Workfront-Erweiterung für Illustrator und InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Siehe Details zum Client-Geheimnis für benutzerdefinierte OAuth2- oder JWT-Integrationen

Um Transparenz bei der Verwendung Ihrer benutzerdefinierten OAuth2- und JWT-Integrationen zu gewährleisten, haben wir es Ihnen ermöglicht, Details zu den von Ihren Integrationen verwendeten Client-Geheimnissen anzuzeigen. Jetzt können Sie sehen, wann das Client-Geheimnis erstellt und zuletzt verwendet wurde. Sie können auch eigene Notizen zum Client-Geheimnis hinzufügen und anzeigen.

Zuvor waren diese Details nicht verfügbar.

Weitere Informationen zu Client Secrets in benutzerdefinierten OAuth2- oder JWT-Integrationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Siehe Authentifizierungstyp in der Liste der benutzerdefinierten OAuth2-Anwendungen

Wenn Sie jetzt die Liste der benutzerdefinierten OAuth2-Anwendungen in Ihrem Unternehmen anzeigen, können Sie sehen, ob die einzelnen Anwendungen Benutzerauthentifizierung oder Serverauthentifizierung verwenden.

Bisher konnten Sie diese Informationen nur sehen, indem Sie die Bearbeitungsoptionen für jede Anwendung aufrufen.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Legen Sie die Gültigkeit für Aktualisierungstoken in Ihren benutzerdefinierten OAuth2-Integrationen fest.

Um den Zugriff und die Sicherheit für Ihre benutzerdefinierten OAuth2-Integrationen zu verbessern, können Sie jetzt die Lebensdauer von Aktualisierungstoken anpassen. Nachdem das Aktualisierungstoken eines Benutzers abläuft, muss er sich erneut bei der Integration anmelden.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Verwenden Sie öffentliche und private Schlüssel in Ihren benutzerdefinierten OAuth2-Integrationen für Server-zu-Server-Apps

Sie können jetzt Server-zu-Server-OAuth2-Anwendungen in Ihren benutzerdefinierten Integrationen einrichten. Durch die Einrichtung öffentlicher und privater Schlüssel können Sie Workfront die Kommunikation mit einer anderen Anwendung ermöglichen, ohne Anmeldedaten zu verwenden.

Bisher verwendete die gesamte Authentifizierung in Ihren benutzerdefinierten OAuth2-Anwendungen die Anmeldedaten des Benutzers.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Die Integration der Google G Suite verwendet jetzt OAuth2

Für mehr Sicherheit und ein konsistenteres Erlebnis über Integrationen hinweg haben wir die Google G Suite-Integration aktualisiert, um die OAuth2-Authentifizierung zu verwenden, eine branchenübliche Methode zur Authentifizierung von Benutzern. Wenn sich Ihre Benutzer jetzt anmelden, können sie die spezifischen Aktionen und Bereiche sehen, auf die die Integrationen Zugriff haben und Zugriff gewähren. Danach müssen sie sich nicht so häufig anmelden.

Weitere Informationen finden Sie unter [Anmelden bei und Abmelden von Adobe Workfront für G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
