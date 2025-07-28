---
product-area: workfront-integrations
keywords: Google,DOC,Dokument,Blatt,Folie
navigation-topic: workfront-for-g-suite
title: Datenschutz und Berechtigungen in Workfront für Google Workspace
description: Datenschutz und Berechtigungen in Workfront für Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Datenschutz und Berechtigungen in Workfront für Google Workspace

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieser Umstellung werden die folgenden Funktionen von Workfront für Google Workspace nach dem 28. **2026 nicht mehr verfügbar**:
>
>* Zugriff auf Google Workspace-Funktionen in Workfront
>
>* Anzeigen und Verwalten von Workfront-Aufgaben über Gmail oder das Site-Panel des Google-Kalenders
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Google Workspace zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Google Workspace finden Sie unter [Gmail-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) und [Google-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Da der Kundendatenschutz wichtig ist, speichert oder erfasst Adobe Workfront keine identifizierenden Kundendaten, die aus der Autorisierung einer Google Plug-in-App durch Dritte resultieren. Die Verwendung von Workfront für Google Workspace und die Übertragung von Informationen, die von Google-APIs empfangen wurden, an jede andere App erfolgen gemäß der [Benutzerdatenrichtlinie für Google-API](https://developers.google.com/terms/api-services-user-data-policy)Services, einschließlich der Anforderungen für die eingeschränkte Verwendung.

Wir benötigen die folgenden Berechtigungen, damit das Plug-in &quot;Workfront for Google Workspace&quot; seinen maximalen Nutzen erzielen kann:

* **E-Mail-Nachrichten anzeigen, wenn das Add-on ausgeführt wird**: Das Plug-in Workfront für Google Workspace kann Benutzenden unzählige Stunden an doppelter Arbeit ersparen, indem es E-Mails in Workfront in neue Aufgaben konvertiert und den Titel und die Beschreibung der Aufgabe automatisch mit Betreff und Textkörper der E-Mail füllt. Mit dem Plug-in können Sie auch Ihre E-Mails als neue Kommentare an Workfront senden. Um diesen Wert zu erzielen, muss das Plug-in Ihre E-Mail-Nachrichten anzeigen, wenn das Add-on ausgeführt wird.
* **Als Gmail-Add-on ausführen/nicht vertraulich**: Es werden Berechtigungen benötigt, damit das Add-on Workfront for Google Workspace in der Gmail-Umgebung funktioniert. Für das Plug-in ist eine Gmail-Umgebung erforderlich, daher ist eine `Run as a Gmail add-on / non-sensitive` Berechtigung erforderlich.
* **Anzeigen der Metadaten Ihrer E-Mail-Nachricht, wenn das Add-on ausgeführt wird**: Um Workflows zu verbessern, bestätigt das Plug-in &quot;Workfront für Google Workspace&quot;, ob eine E-Mail eine Workfront-Benachrichtigung ist, und identifiziert den Typ der Workfront-Benachrichtigung (neue Arbeitsanfrage, Genehmigungsanfrage, neuer Kommentar usw.). Das Plug-in erfordert die Berechtigung `View your email message metadata when the add-on is running` , um diesen Wert bereitzustellen.
* **Das Plug-in muss als Kalender-Add-on ausgeführt werden (nicht sensibel**: Das Plug-in Workfront für Google Workspace stellt eine Verbindung zu Ihrem Kalender her, damit Sie visualisieren können, wie sich Aufgaben auf Zeitpläne auswirken. Das Plug-in benötigt dazu die Berechtigung `Run as a Calendar add-on / non-sensitive` .
* **Berechtigung „Mit externem Service verbinden:** Letztendlich muss das Plug-in eine Verbindung zur Workfront-API herstellen, die das Rückgrat des Plug-in-Werts ist. Die Workfront-API ist ein Service außerhalb von Google. Daher erfordert das Plug-in die `Connect to an external service permission`, damit das Plug-in funktioniert.

Weitere Informationen zum Engagement von Adobe Workfront für den Kundendatenschutz finden Sie in der Datenschutzerklärung von [Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Weitere Informationen finden Sie unter [Benutzerdatenrichtlinie für Google-API-Services](https://developers.google.com/terms/api-services-user-data-policy).
