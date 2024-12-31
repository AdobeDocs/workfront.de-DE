---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Projektverbesserungen in 2020.1
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die mit der Version 2020.1 an Projekten vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau -Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Projektverbesserungen in 2020.1

Auf dieser Seite werden alle Verbesserungen beschrieben, die mit der Version 2020.1 an Projekten vorgenommen wurden. Diese Verbesserungen sind derzeit in der Vorschau -Umgebung verfügbar und werden Ende März oder Anfang April 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 2020.1 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Einfacher festzustellen, wer in einem Update getaggt ist

Es ist jetzt einfacher zu sehen, welche Benutzer in einem Update getaggt sind. Die Anzeige des Benutzernamens mit Tags in Blau und der Link zum Benutzerprofil.

Getaggte Benutzende werden auch unter dem Kommentarfeld aufgeführt.

Vor dieser Verbesserung wurden die Benutzenden, die zuvor mit Tags versehen waren, nicht im Benachrichtigungsfeld angezeigt.

Weitere Informationen finden Sie unter [Andere bei Updates taggen](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Einschließen und Identifizieren von zitiertem Text in einem Aktualisierungskommentar oder einer Antwort

Wenn Sie einen Kommentar eingeben, können Sie einen Teil des Kommentars als zitierten Text markieren, um ihn von Ihrem eigenen Kommentar zu unterscheiden. Verwenden Sie die Schaltfläche Blockzitat im HTML-Editor.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## Einen vorherigen Kommentar in einen Aktualisierungskommentar oder eine Antwort zitieren

Wenn Sie einen Kommentar in einem Aktualisierungs-Thread einfügen, können Sie schnell Text aus einem vorherigen Kommentar in den Thread einbeziehen. Suchen Sie im Menü Mehr neben dem Kommentar, den Sie zitieren möchten, nach der Option Antwort auf das Angebot.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Zusätzliche Informationen zu Risiken

Damit Sie die Risiken Ihrer Projekte besser verstehen können, können Sie jetzt sehen, wer und wann ein Risiko eingegeben und wann es bei einem Projekt aktualisiert wurde. Sie können auf diese Informationen in einer Risikoansicht und über die öffentliche Workfront-API zugreifen. Diese Felder sind ab API-Version 11 verfügbar, die mit der Produktion 2020.1 veröffentlicht wird.

Informationen zu Risiken in Workfront finden Sie unter [Erstellen und Bearbeiten von Risiken in Projekten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## Zusätzliche Felder zu Baselines und Baseline-Aufgaben hinzugefügt

Damit Sie den finanziellen Fortschritt Ihrer Projekte besser verstehen können, können Sie jetzt zusätzliche Kosten- und Umsatzinformationen in einen Baseline- oder einen Baseline-Aufgabenbericht aufnehmen. Die zusätzlichen Finanzinformationen werden nicht zu den Baselines hinzugefügt, die Sie derzeit gespeichert haben, sondern zu neuen Baselines.

Informationen zu Projekt- und Aufgabenfinanzfeldern, auf die über die Basisobjekte und Basisobjekte für Aufgaben zugegriffen werden kann, finden Sie unter [Projektfinanzen in Projektbasislinien enthalten](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Probleme mit dem Status „Geschlossene bis ausstehende Genehmigung“ werden als unvollständig betrachtet

Die Art und Weise, wie Workfront Probleme mit dem Status „Ausstehende Genehmigung abschließen“ behandelt, wurde geändert. Diese Probleme werden nun als offen wahrgenommen und das Projekt kann erst als abgeschlossen markiert werden, wenn die Genehmigung erledigt ist.

Vor dieser Änderung wurden Probleme mit dem Status „Ausstehende Genehmigung geschlossen“ als geschlossen betrachtet.

Alle Probleme, die vor dieser Änderung in den Status Geschlossen - Ausstehende Genehmigung versetzt wurden, verhalten sich genauso wie zuvor. Sie werden als abgeschlossen betrachtet, sodass das Projekt ebenfalls abgeschlossen werden kann. Alle Probleme, die nach dieser Änderung in diesen Status aufgenommen werden, werden als unvollständig betrachtet.

Informationen zum Projektstatus finden Sie unter [Zugriff auf die Liste der Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

