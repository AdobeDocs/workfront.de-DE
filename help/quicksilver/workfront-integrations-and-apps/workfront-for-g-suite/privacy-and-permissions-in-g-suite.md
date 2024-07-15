---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Datenschutz und -berechtigungen in Workfront für Google Workspace
description: Datenschutz und -berechtigungen in Workfront für Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Datenschutz und -berechtigungen in Workfront für Google Workspace

Da der Kundendatenschutz wichtig ist, speichert oder erfasst Adobe Workfront keine identifizierenden Kundendaten, die aus der Autorisierung einer Google-Plug-in-App durch Dritte resultieren. Die Verwendung und Übertragung von Informationen, die von Google-APIs an andere Apps von Workfront für Google Workspace empfangen werden, erfolgt gemäß der [Benutzerdatenrichtlinie für Google-API-Dienste](https://developers.google.com/terms/api-services-user-data-policy), einschließlich der eingeschränkten Anwendungsanforderungen.

Wir benötigen die folgenden Berechtigungen, damit das Workfront für Google Workspace-Plug-in seinen maximalen Wert bereitstellen kann:

* **Anzeigen Ihrer E-Mail-Nachrichten, wenn das Add-on ausgeführt wird**: Das Workfront for Google Workspace-Plug-in kann Benutzer unzählige Stunden an duplizierter Arbeit sparen, indem E-Mails in neue Aufgaben in Workfront konvertiert und Titel und Beschreibung der Aufgabe automatisch mit dem Betreff und dem Hauptteil der E-Mail ausgefüllt werden. Mit dem -Plug-in können Sie auch Ihre E-Mails als neue Kommentare in Workfront posten. Das -Plug-in muss Ihre E-Mail-Nachrichten anzeigen, wenn das Add-on ausgeführt wird, um diesen Wert bereitzustellen.
* **Als Gmail-Add-on/nicht vertraulich ausführen**: Berechtigungen sind erforderlich, damit das Workfront für Google Workspace-Add-on in der Gmail-Umgebung funktioniert. Für das Plug-in ist eine Gmail-Umgebung erforderlich, sodass die Berechtigung `Run as a Gmail add-on / non-sensitive` erforderlich ist.
* **Metadaten Ihrer E-Mail-Nachricht anzeigen, wenn das Add-on ausgeführt wird**: Um die Workflows zu verbessern, bestätigt das Workfront for Google Workspace-Plug-in, ob es sich bei einer E-Mail um eine Workfront-Benachrichtigung handelt, und identifiziert den Typ der Workfront-Benachrichtigung (neue Arbeitserforderung, Genehmigungsanfrage, neuer Kommentar usw.). Das Plug-in benötigt die Berechtigung `View your email message metadata when the add-on is running` , um diesen Wert bereitzustellen.
* **Plug-in muss als Kalender-Add-on/nicht vertraulich ausgeführt werden**: Das Workfront für Google Workspace-Plug-in stellt eine Verbindung zu Ihrem Kalender her, sodass Sie visualisieren können, wie sich Aufgaben auf Zeitpläne auswirken. Dazu benötigt das Plug-in die `Run as a Calendar add-on / non-sensitive` -Berechtigung.
* **Verbindung zu einer externen Dienstberechtigung herstellen:** Letztlich muss das Plug-in eine Verbindung zur Workfront-API herstellen, die das Rückgrat des Plug-in-Werts darstellt. Die Workfront-API ist ein außerhalb von Google gespeicherter Dienst. Daher benötigt das Plug-in den `Connect to an external service permission` , damit das Plug-in funktioniert.

Weitere Informationen zum Engagement von Adobe Workfront für den Datenschutz von Kunden finden Sie in der [Datenschutzerklärung von Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Weitere Informationen finden Sie unter [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy).
