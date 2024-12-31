---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 3 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird zwischen Ende Juli und Anfang August 2017 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Versionsaktivität von Beta 3 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird zwischen Ende Juli und Anfang August 2017 in der Produktionsumgebung verfügbar gemacht.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller in 2017.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die Beta-Version 2017.2 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren:**

* [Die Elemente werden stapelweise aus dem Papierkorb wiederhergestellt](#restoring-items-in-bulk-from-the-recycle-bin)
* [Benutzerinformationen werden von Workfront mit ProofHQ (ProofHQ und Workfront) synchronisiert](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Für alle Benutzer:** 

* [Abonnierte Benutzer anzeigen](#view-subscribed-users)
* [Konfigurieren Sie, wie Meilensteine im Gantt-Diagramm angezeigt werden](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Binden Sie beim Exportieren nach PDF die Legende des Gantt-Diagramms ein](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Korrekturabzugsgenehmigungen im Bereich „Meine Arbeit“ (Workfront) anzeigen](#view-proof-approvals-in-the-my-work-area-workfront)
* [Anzeigen von Benutzernamen beim Bearbeiten von Proofing-Genehmigungsanfragen im Bereich Meine Arbeit (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Verbesserter Proofing-Viewer für Video-Korrekturabzüge (ProofHQ und Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Rich-Media-Korrekturabzüge in alternativen Auflösungen anzeigen (ProofHQ und Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Neues Objekt &#39;Korrekturabzug-Ersteller&#39; im Bericht zur Dokumentversion (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Neue Ressourcenpool-Funktionalität vorübergehend aus der Vorschau entfernt](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Stapelweises Wiederherstellen von Elementen aus dem Papierkorb {#restoring-items-in-bulk-from-the-recycle-bin}

Sie können jetzt bis zu 10 gelöschte Projekte, Aufgaben, Probleme oder Dokumente gleichzeitig wiederherstellen.

Vor dieser Änderung konnten Sie jeweils nur ein gelöschtes Element wiederherstellen.

Weitere Informationen zum Wiederherstellen von Elementen finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Abonnierte Benutzer anzeigen {#view-subscribed-users}

Sie können jetzt sehen, wer ein Element abonniert hat, indem Sie die Anzahl der Abonnenten erweitern, die neben dem Abonnement-Link angezeigt wird.

Vor dieser Verbesserung hatten Sie keine Einsicht darüber, wer Elemente abonniert hat.

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Konfigurieren der Anzeige von Meilensteinen im Gantt-Diagramm {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Es gibt jetzt zwei Optionen zum Anzeigen von Meilensteininformationen in einem Gantt-Diagramm. Sie können einen oder beide der folgenden Meilensteinindikatoren konfigurieren:

* Meilenstein-Diamanten (Symbol)

  Dieses Symbol wird im Gantt-Diagramm nach jeder Aufgabe angezeigt, die mit einem Meilenstein verbunden ist.

* Meilenstein-Linien

  Nach jeder Aufgabe, die mit dem Meilenstein verknüpft ist, wird eine Linie angezeigt, die alle Aufgaben im Gantt-Diagramm umfasst.

Vor dieser Änderung gab es nur eine Option, um die Anzeige von Meilensteinen in einem Gantt-Diagramm zu ermöglichen, die als „Meilensteine“ bezeichnet wird. Diese Option aktiviert sowohl das Meilenstein-Diamantsymbol als auch die Meilensteinlinie. Diese Indikatoren konnten nicht getrennt werden.

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Beim Exportieren nach PDF die Gantt-Diagramm-Legende einschließen {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Wenn Sie das Gantt-Diagramm auf eine PDF exportieren, können Sie jetzt auswählen, ob Sie auch die Legende des Diagramms zusammen mit dem Diagramm selbst exportieren möchten. Die Legende enthält nur die Elemente, die Sie für die Anzeige im Gantt-Diagramm in der Benutzeroberfläche aktiviert haben. Diese Optionen sind in der Legende enthalten, wenn sie für die Aufgaben im Projekt vorhanden sind. Wenn Sie beispielsweise die Anzeige von Meilensteinen im Gantt-Diagramm aktivieren, werden diese ebenfalls in der Legende angezeigt, allerdings nur, wenn mit einem Meilenstein mindestens eine Aufgabe verknüpft ist.

Vor dieser Änderung konnten Sie die Legende nicht von der exportierten PDF ausschließen. Die Legende enthielt alle möglichen Optionen und Markierungen des Gantt-Elements, unabhängig davon, ob sie in der Benutzeroberfläche aktiviert waren oder vorhanden waren.

Weitere Informationen zum Exportieren des Gantt-Diagramms finden Sie unter [Exportieren des Gantt-Diagramms nach PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Benutzerinformationen werden von Workfront mit ProofHQ (ProofHQ und Workfront) synchronisiert {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Benutzerinformationen (Name und E-Mail) werden jetzt von Workfront mit ProofHQ synchronisiert, wenn Benutzende in Workfront erstellt oder aktualisiert werden. 

Weitere Informationen zur Benutzersynchronisierung von Workfront mit ProofHQ finden Sie unter .

## Neues Objekt „Korrekturabzug-Ersteller“ im Bericht zur Dokumentversion (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Beim Erstellen eines Dokumentversionsberichts gibt es jetzt ein neues Objekt zur Erstellung von Korrekturabzügen. Mit diesem Objekt können Sie Berichte zu Informationen über den Benutzer erstellen, der den Korrekturabzug erstellt hat. 

Das neue Objekt des Korrekturabzugs-Erstellers im Bericht Dokumentversion enthält alle Felder, die in anderen Objektberichten mit dem vorhandenen Benutzerobjekt verfügbar sind.

>[!NOTE]
>
> Diese Informationen sind im Bericht erst ab dem Zeitpunkt verfügbar, zu dem diese Funktion in die jeweilige Vorschau- oder Produktionsumgebung eingeführt wurde. Informationen in Berichten zum Objekt des Anforderers vor dem Zeitpunkt, zu dem diese Funktion eingeführt wurde, sind nicht verfügbar.

Sie greifen auf das Objekt des Korrekturabzugs-Erstellers zu, wenn Sie einen Bericht zur Dokumentversion erstellen, wie in [Erstellen eines benutzerdefinierten Berichts](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht zur Dokumentversion finden Sie im Abschnitt [Grundlegendes zu Objekten in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Grundlegendes zu Objekten in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Genehmigungen von Korrekturabzügen im Bereich Meine Arbeit anzeigen (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Alle Korrekturabzugsgenehmigungen, die Sie zur Genehmigung weitergeleitet haben, werden jetzt im Bereich Meine Arbeit auf der Registerkarte **Arbeit, die ich zur Genehmigung weitergeleitet habe** angezeigt.

Vor dieser Änderung enthielt die **Arbeit, die ich zur Genehmigung eingereicht habe** keine Korrekturabzugsgenehmigungen.

Genehmigungen von Korrekturabzügen werden nur angezeigt, wenn die folgenden Kriterien erfüllt sind:

* Die Genehmigung steht derzeit noch aus
* Der Genehmigungsprozess wird einem Benutzer zugewiesen, der ein lizenzierter Workfront-Benutzer ist (Genehmigungsprozesse, die Benutzern zugewiesen sind, die keine lizenzierten Workfront-Benutzer sind, werden nicht angezeigt)
* Die Genehmigungsprozesse wurden eingeleitet, nachdem diese Funktion freigegeben wurde (Genehmigungsprozesse, die vor der Freigabe dieser Funktion initiiert wurden, werden nicht angezeigt)

Weitere Informationen finden Sie unter [Genehmigungen anzeigen](../../../../review-and-approve-work/manage-approvals/view-approvals.md) in [Genehmigungen anzeigen](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Anzeigen von Benutzernamen bei der Bearbeitung von Proofing-Genehmigungsanfragen im Bereich Meine Arbeit (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Bei der Genehmigung von Korrekturabzugsgenehmigungen über den Bereich Meine Arbeit wird jetzt der Name des Benutzers angezeigt, der die Genehmigung angefordert hat.

Weitere Informationen finden Sie unter [Genehmigen von ](../../../../review-and-approve-work/manage-approvals/approving-work.md)&quot; in [Genehmigen von ](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Verbesserter Proofing-Viewer für Videoprüfungen (ProofHQ und Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Die Proofing-Anzeige sowohl in Workfront als auch in ProofHQ wird mit einem neuen Look-and-Feel, einer neuen HTML5-Architektur für eine bessere Leistung und Unterstützung für neue Funktionen aktualisiert.

Der neue Proofing Viewer enthält die folgenden Verbesserungen:

* Bild-für-Bild-Proofing
* Videopufferung
* Suchfunktion in der Kommentarliste
* Alle für den Kommentar festgelegten Aktionen werden bei jedem Kommentar in der Kommentarliste angezeigt
* Vollbildmodus
* Inhalte schneller oder langsamer überprüfen
* Rechtschreibprüfung beim Hinzufügen von Kommentaren und Antworten

### Vorschau

Der neue Proofing Viewer ist zum Testen in den folgenden Vorschauumgebungen verfügbar:

* ProofHQ Preview-Umgebung

  Weitere Informationen zur ProofHQ-Vorschau-Umgebung finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Workfront-Vorschau-Umgebung, wenn das Konto für das Proofing aktiviert ist

  Weitere Informationen zur Workfront-Vorschau-Umgebung finden Sie unter  [Die Sandbox-Vorschau-Umgebung von Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

In dieser Version unterstützt der neue Proofing-Viewer nur Video-Proofing. Das bedeutet, dass alle Korrekturabzüge den neuen Proofing Viewer nutzen, während alle statischen Korrekturabzüge und Rich-Media-Korrekturabzüge weiterhin den vorhandenen Proofing Viewer nutzen.

### Produktion

Nach der Veröffentlichung in der Produktionsumgebung mit der Version 17.2 können Admins auswählen, ob die neue oder die alte Proofing-Betrachter für die Benutzenden in ihrer Organisation am besten geeignet ist. Standardmäßig wird die alte Proofing-Anzeige verwendet.

Informationen zur Verwendung des neuen Video Proofing Viewers finden Sie unter  

## Rich-Media-Korrekturabzüge in alternativen Auflösungen anzeigen (ProofHQ und Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Sie können jetzt die Auflösung von Rich-Media-Korrekturabzügen anpassen, indem Sie entweder eine benutzerdefinierte Auflösung angeben oder das Bild auf die gewünschte Auflösung ziehen.

Vor dieser Änderung konnten Sie Korrekturabzüge nur mit der Auflösung überprüfen, die für den Bildschirm oder das Gerät, auf dem Sie die Inhalte überprüft haben, typisch ist.

Sie können den Vergleichsmodus verwenden, um verschiedene Auflösungen von Korrekturabzügen zu vergleichen.

Weitere Informationen finden Sie unter [Testsendungen im Desktop Proofing Viewer öffnen](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Neue Ressourcenpool-Funktionalität vorübergehend aus der Vorschau entfernt {#new-resource-pool-functionality-temporarily-removed-from-preview}

Aufgrund von Entwicklungsproblemen haben wir beschlossen, die neue Registerkarte Ressourcenplanung zu entfernen und die alte Registerkarte Ressourcenplanung wieder in ihren ursprünglichen Namen „Ressourcenplanung“ umzubenennen.

Mit dieser Änderung wurde auch die neue Funktion „Ressourcenpools“ entfernt. Die neue Registerkarte „Ressourcenplanung“ und die Funktionalität der Ressourcenpools werden Ende Juni 2017 zur Sandbox-Vorschau-Umgebung zurückkehren.
