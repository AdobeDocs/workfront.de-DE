---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Projektverbesserungen
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die mit Version 2020.1 an Projekten vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau-Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 2020.1 Projektverbesserungen

Auf dieser Seite werden alle Verbesserungen beschrieben, die mit Version 2020.1 an Projekten vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau-Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller in Version 2020.1 verfügbaren Änderungen finden Sie unter [Versionsübersicht 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## In einer Aktualisierung leichter erkennbar, wer mit Tags versehen ist

Es ist jetzt einfacher zu sehen, welche Benutzer bei einer Aktualisierung mit Tags versehen sind. Die Anzeige des mit Tags versehenen Benutzernamens in Blau und der Link zum Benutzerprofil.

Tagging-Benutzer werden auch unter dem Kommentarfeld aufgeführt.

Vor dieser Verbesserung wurden die zuvor mit Tags versehenen Benutzer nicht im Feld &quot;Benachrichtigen&quot;angezeigt.

Weitere Informationen finden Sie unter [Tagging anderer Benutzer auf Updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Einschließen und Identifizieren von zitiertem Text in einen Aktualisierungskommentar oder eine Antwort

Wenn Sie einen Kommentar eingeben, können Sie einen Teil Ihres Kommentars als zitierten Text markieren, um ihn von Ihrem eigenen Kommentar zu unterscheiden. Verwenden Sie die Schaltfläche Blockangebot im HTML-Editor.

Weitere Informationen finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Vorherigen Kommentar in einem Aktualisierungskommentar oder einer Antwort zitieren

Wenn Sie Kommentare in einem Aktualisierungs-Thread erstellen, können Sie schnell Text aus einem vorherigen Kommentar in den Thread einfügen. Suchen Sie im Menü Mehr neben dem Kommentar, den Sie zitieren möchten, nach der Option Antwort zitieren .

Weitere Informationen finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Zusätzliche Informationen zu Risiken

Damit Sie die Risiken Ihrer Projekte besser verstehen können, können Sie jetzt sehen, wer und wann ein Risiko eingegangen ist und wann es über ein Projekt aktualisiert wurde. Sie können auf diese Informationen in einer Risikoansicht und über die öffentliche Workfront-API zugreifen. Diese Felder sind mit der API-Version 11 verfügbar, die für die Produktion 2020.1 veröffentlicht wird.

Informationen zu Risiken in Workfront finden Sie unter [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Zusätzliche Felder zu Grundlinien und Grundlinien-Aufgaben hinzugefügt

Um den finanziellen Fortschritt Ihrer Projekte besser zu verstehen, können Sie jetzt zusätzliche Kosten- und Umsatzinformationen in einen Baseline- oder einen Baseline-Aufgabenbericht aufnehmen. Die zusätzlichen Finanzinformationen werden nicht zu den Grundlinien hinzugefügt, die Sie derzeit gespeichert haben, sondern für neue Grundlinien hinzugefügt.

Informationen zu Projekt- und Aufgabenfinanzfeldern, auf die über die Objekte &quot;Baseline&quot;und &quot;Baseline Task&quot;zugegriffen werden kann, finden Sie unter [Projektfinanzen in Projektgrundlagen](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Probleme mit dem Status &quot;Abgeschlossene/ausstehende Genehmigung&quot;werden als unvollständig betrachtet

Die Art und Weise, wie Workfront Probleme mit dem Status &quot;Vollständige Genehmigung ausstehend&quot;behandelt, wurde geändert. Diese Probleme werden jetzt als offen wahrgenommen und das Projekt kann erst als abgeschlossen markiert werden, wenn die Genehmigung abgeschlossen ist.

Vor dieser Änderung wurden Probleme mit dem Status &quot;Geschlossene Genehmigung&quot; als geschlossen betrachtet.

Alle Probleme, die vor dieser Änderung in den Status Geschlossen - Ausstehende Genehmigung eingetragen wurden, verhalten sich genauso wie zuvor, werden als abgeschlossen betrachtet und ermöglichen auch den Abschluss des Projekts. Alle Probleme, die nach dieser Änderung in diesem Status auftreten, werden als unvollständig betrachtet.

Weitere Informationen zum Projektstatus finden Sie unter [Zugriff auf die Liste der Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

