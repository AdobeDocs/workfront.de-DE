---
title: 22.1 Verbesserungen bei Anfragen
description: 22.1 Verbesserungen bei Anfragen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1 Verbesserungen bei Anfragen

Auf dieser Seite werden alle mit Version 22.1 vorgenommenen Verbesserungen bei Anfragen an die Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 17. Januar 2022.

Eine Liste aller in Version 22.1 verfügbaren Änderungen finden Sie in der Übersicht über die Version [22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Verbesserung der Benutzeroberfläche für Benutzer, die keinen Zugriff zum Erstellen von Anfragen haben

Um das Benutzererlebnis bei der Arbeit mit Anfragen zu verbessern, haben wir eine Verbesserung an der Benutzeroberfläche eingeführt, die dem angemeldeten Benutzer anzeigt, dass er keinen Zugriff zum Erstellen von Anfragen hat. Mit dieser Verbesserung ist die Schaltfläche Neue Anfrage für Benutzende ohne Zugriff zum Erstellen von Problemen abgeblendet. Wenn Sie den Mauszeiger über die abgeblendete Schaltfläche bewegen, wird eine QuickInfo angezeigt, in der erläutert wird, dass der Workfront-Administrator den Zugriff des aktuellen Benutzers zum Erstellen von Anfragen eingeschränkt hat.

Vor dieser Verbesserung wurde die Schaltfläche Neue Anfrage für diese Benutzer nicht im Bereich Anfragen angezeigt. Das Kopieren und Senden einer neuen Anfrage ist ebenfalls eingeschränkt.

Weitere Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Anforderungen kopieren und senden

Um Ihren Prozess für das Senden von Anfragen zu optimieren, führen wir eine neue Funktion ein, mit der Sie eine vorhandene Anfrage kopieren und als neue Anfrage senden können. Dies ist hilfreich, wenn Sie häufig ähnliche Anfragen senden. In diesem Fall können Sie eine vorhandene Anfrage wiederverwenden, einige Änderungen vornehmen und sie dann als neue Anfrage senden.

Mit dieser Änderung können Benutzende, die von anderen gesendete Anfragen anzeigen können, diese Anfragen auch kopieren und als neu senden. Sie können dies verhindern, indem Sie im Projekt für die Anfragewarteschlange die folgende Einstellung aktualisieren: Personen aus derselben Firma erben dieselben Berechtigungen für alle Anfragen.

>[!NOTE]
>
>Probleme, die vor der Veröffentlichung dieser Funktion an eine Anfrage-Warteschlange ohne Warteschlangen-Thema gesendet wurden, können nicht kopiert und erneut gesendet werden.

Weitere Informationen finden Sie unter [Kopieren und Senden von Anfragen](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Das Bedienfeld „Zusammenfassung“ im Abschnitt „Gesendet“ im Bereich „Anfragen“ wurde aktualisiert

>[!NOTE]
>
>Diese Funktion wurde am 12. November 2021 vorübergehend aus der Vorschau-Umgebung entfernt. Sie wird zu einem späteren Zeitpunkt wieder hinzugefügt.

Um die Sichtbarkeit und Interaktion mit dem Bedienfeld Zusammenfassung zu verbessern, haben wir dem Symbol Zusammenfassung öffnen im Abschnitt Gesendet im Bereich Anfragen einen Titel hinzugefügt. Die Beschriftung ist jetzt dynamisch und wird je nachdem, ob das Bedienfeld geöffnet oder geschlossen ist, aktualisiert.

Beim Öffnen des Bedienfelds Zusammenfassung ohne vorherige Auswahl einer Anfrage wird jetzt ein benutzerfreundlicheres Bild angezeigt, um den Benutzer klar anzuweisen, ein Element auszuwählen, bevor das Bedienfeld geöffnet wird. Weitere Informationen finden Sie unter [Gesendete Anfragen suchen](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Mit dieser Änderung wurde auch das Bedienfeld Zusammenfassung für Aufgaben, Probleme und Dokumente aktualisiert. Weitere Informationen über das Bedienfeld Zusammenfassung finden Sie unter [Übersicht](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
