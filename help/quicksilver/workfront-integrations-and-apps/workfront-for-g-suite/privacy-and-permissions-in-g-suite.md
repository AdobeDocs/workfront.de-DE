---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Datenschutz und -berechtigungen in Workfront für G Suite
description: Datenschutz und -berechtigungen in Workfront für G Suite
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 0862af846ca77c33132ec631cf1e3eae253d3cd8
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Datenschutz und -berechtigungen in Workfront für G Suite

Da der Kundendatenschutz wichtig ist, speichert oder erfasst Adobe Workfront keine identifizierenden Kundendaten, die aus der Autorisierung einer Google-Plug-in-App durch Dritte resultieren.

Wir benötigen die folgenden Berechtigungen, damit das Workfront for G Suite-Plug-in seinen maximalen Wert bereitstellen kann:

* **Anzeigen Ihrer E-Mail-Nachrichten bei Ausführung des Add-ons**: Mit dem Workfront for G Suite-Plug-in können Benutzer unzählige Stunden an duplizierter Arbeit sparen, indem E-Mails in Workfront in neue Aufgaben konvertiert und der Titel und die Beschreibung der Aufgabe automatisch mit dem Betreff und dem Hauptteil der E-Mail ausgefüllt werden. Mit dem -Plug-in können Sie auch Ihre E-Mails als neue Kommentare in Workfront posten. Das -Plug-in muss Ihre E-Mail-Nachrichten anzeigen, wenn das Add-on ausgeführt wird, um diesen Wert bereitzustellen.
* **Als Gmail-Add-on ausführen/nicht sensibel**: Berechtigungen sind erforderlich, damit das Workfront for G Suite-Add-on in der Gmail-Umgebung funktioniert. Für das Plug-in ist eine Gmail-Umgebung erforderlich, sodass die `Run as a Gmail add-on / non-sensitive` Berechtigung.
* **Anzeigen der Metadaten Ihrer E-Mail-Nachricht bei Ausführung des Add-ons**: Um die Workflows zu verbessern, bestätigt das Workfront for G Suite-Plug-in, dass eine E-Mail eine Workfront-Benachrichtigung ist, und identifiziert den Typ der Workfront-Benachrichtigung (neue Arbeitserforderung, Genehmigungsanfrage, neuer Kommentar usw.). Für das Plug-in ist die `View your email message metadata when the add-on is running` Berechtigung zum Bereitstellen dieses Werts.
* **Das Plug-in muss als Kalender-Add-on/nicht vertraulich ausgeführt werden**: Das Workfront for G Suite-Plug-in stellt eine Verbindung zu Ihrem Kalender her, sodass Sie visualisieren können, wie sich Aufgaben auf Zeitpläne auswirken. Das Plug-in benötigt die `Run as a Calendar add-on / non-sensitive` -Berechtigung zu verwenden.
* **Verbindung zu einer externen Dienstberechtigung herstellen:** Letztlich muss das Plug-in eine Verbindung zur Workfront-API herstellen, die das Rückgrat des Plug-in-Werts darstellt. Die Workfront-API ist ein außerhalb von Google gespeicherter Dienst. Daher erfordert das Plug-in die `Connect to an external service permission` , damit das Plug-in funktioniert.

Weitere Informationen zum Engagement von Adobe Workfront für den Kundendatenschutz finden Sie unter [Datenschutzhinweis zu Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

