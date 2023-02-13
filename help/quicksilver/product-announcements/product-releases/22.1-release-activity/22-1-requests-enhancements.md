---
title: 2.1 Verbesserungen bei Anforderungen
description: 2.1 Verbesserungen bei Anforderungen
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 2.1 Verbesserungen bei Anforderungen

Auf dieser Seite werden alle Anforderungsverbesserungen beschrieben, die mit Version 22.1 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 17. Januar 2022.

Eine Liste aller in Version 22.1 verfügbaren Änderungen finden Sie unter [2.1 - Versionsübersicht](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Verbesserung der Benutzeroberfläche für Benutzer, die keinen Zugriff auf die Erstellung von Anforderungen haben

Um das Benutzererlebnis beim Arbeiten mit Anforderungen zu verbessern, wurde die Benutzeroberfläche verbessert, die dem angemeldeten Benutzer anzeigt, dass er keinen Zugriff auf die Erstellung von Anforderungen hat. Mit dieser Verbesserung ist die Schaltfläche Neue Anforderung für Benutzer ohne Zugriff auf die Erstellung von Problemen abgeblendet. Wenn Sie den Mauszeiger über die abgeblendete Schaltfläche bewegen, wird eine QuickInfo angezeigt, in der erklärt wird, dass der Workfront-Administrator den Zugriff des aktuellen Benutzers auf das Erstellen von Anforderungen eingeschränkt hat.

Vor dieser Verbesserung wurde die Schaltfläche Neue Anforderung nicht im Bereich Anforderungen für diese Benutzer angezeigt. Das Kopieren und Senden einer Anforderung als neuer ist ebenfalls eingeschränkt.

Weitere Informationen zum Erstellen von Anforderungen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Anforderungen kopieren und senden

Um Ihren Prozess zum Senden von Anfragen zu optimieren, führen wir eine neue Funktion ein, mit der Sie eine vorhandene Anforderung kopieren und als neue Anforderung senden können. Dies ist hilfreich, wenn Sie ähnliche Anfragen häufig senden. In diesem Fall können Sie eine vorhandene Anforderung wiederverwenden, einige Änderungen vornehmen und sie dann als neue Anforderung senden.

Mit dieser Änderung können Benutzer, die von anderen Benutzern eingereichte Anforderungen anzeigen können, diese Anforderungen auch kopieren und als neue senden. Sie können dies verhindern, indem Sie die folgende Einstellung im Anforderungswarteschlangenprojekt aktualisieren: Die Personen desselben Unternehmens erben dieselben Berechtigungen für alle Anforderungen.

>[!NOTE]
>
>Sie können Probleme, die vor der Freigabe dieser Funktion an eine Anforderungswarteschlange ohne Warteschlangenthema gesendet wurden, nicht kopieren und erneut senden.

Weitere Informationen finden Sie unter [Anforderungen kopieren und senden](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Das Zusammenfassungsfenster wurde im Abschnitt &quot;Gesendet&quot;des Bereichs Anforderungen aktualisiert.

>[!NOTE]
>
>Diese Funktion wurde am 12. November 2021 vorübergehend aus der Vorschau-Umgebung entfernt. Sie wird zu einem späteren Zeitpunkt erneut hinzugefügt.

Um die Sichtbarkeit und Interaktion mit dem Bedienfeld &quot;Zusammenfassung&quot;zu verbessern, haben wir dem Symbol &quot;Zusammenfassung öffnen&quot;im Abschnitt &quot;Gesendet&quot;des Bereichs &quot;Anforderungen&quot;eine Bezeichnung hinzugefügt. Die Bezeichnung ist jetzt dynamisch und wird je nachdem, ob das Bedienfeld geöffnet oder geschlossen ist, aktualisiert.

Wenn Sie das Bedienfeld Zusammenfassung öffnen, ohne zunächst eine Anforderung auszuwählen, wird jetzt ein benutzerfreundlicheres Bild angezeigt, das den Benutzer anweist, vor dem Öffnen des Bedienfelds ein Element auszuwählen. Weitere Informationen finden Sie unter [Gesendete Anforderungen suchen](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Mit dieser Änderung wurde auch das Bedienfeld &quot;Zusammenfassung&quot;für Aufgaben, Probleme und Dokumente aktualisiert. Weitere Informationen zum Bedienfeld &quot;Zusammenfassung&quot;finden Sie unter [Zusammenfassungsübersicht](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
