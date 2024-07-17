---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 3-Release-Aktivität 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung bereitgestellt. Es wird von Ende Juli bis Anfang August 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Beta 3-Release-Aktivität 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung bereitgestellt. Es wird von Ende Juli bis Anfang August 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die in Version 2017.2 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die Beta 2-Version 2017.2 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren:**

* [Massenwiederherstellung von Elementen aus dem Papierkorb](#restoring-items-in-bulk-from-the-recycle-bin)
* [Benutzerinformationen werden von Workfront mit ProofHQ synchronisiert (ProofHQ und Workfront).](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Für alle Benutzer:** 

* [Abonnierte Benutzer anzeigen](#view-subscribed-users)
* [Konfigurieren der Anzeige von Meilensteinen auf dem Gantt-Diagramm](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Schließen Sie beim Exportieren in PDF die Gantt-Diagramm-Legende ein](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Anzeigen von Testversandgenehmigungen im Arbeitsbereich (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Anzeigen von Benutzernamen bei der Bearbeitung von Proofing-Genehmigungsanfragen aus meinem Arbeitsbereich (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Verbesserter Testversand-Viewer für Videosendungen (ProofHQ und Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Anzeigen von Rich-Media-Testsendungen in alternativen Auflösungen (ProofHQ und Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Neues Objekt &quot;Testversand-Ersteller&quot;im Bericht &quot;Dokumentversion&quot;(Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Neue Ressourcenpool-Funktion vorübergehend aus der Vorschau entfernt](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Massenwiederherstellung von Elementen aus dem Papierkorb {#restoring-items-in-bulk-from-the-recycle-bin}

Sie können jetzt bis zu 10 gelöschte Projekte, Aufgaben, Probleme oder Dokumente gleichzeitig wiederherstellen.

Vor dieser Änderung konnten Sie jeweils nur ein gelöschtes Element wiederherstellen.

Weitere Informationen zum Wiederherstellen von Elementen finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Abonnierte Benutzer anzeigen {#view-subscribed-users}

Sie können jetzt sehen, wer einen Artikel abonniert, indem Sie die Anzahl der Abonnenten erweitern, die neben dem Anmelde-Link angezeigt werden.

Vor dieser Verbesserung war nicht sichtbar, wer Artikel abonniert hat.

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Konfigurieren der Anzeige von Meilensteinen im Gantt-Diagramm {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Es gibt jetzt zwei Optionen zum Anzeigen von Meilensteininformationen in einem Gantt-Diagramm. Sie können eine oder beide der folgenden Meilensteinindikatoren konfigurieren:

* Milestone Diamonds (Symbol)

  Dieses Symbol wird im Gantt-Diagramm nach jeder Aufgabe angezeigt, die mit einem Meilenstein verknüpft ist.

* Meilenstein-Linien

  Nach jeder mit dem Meilenstein verknüpften Aufgabe wird eine Zeile angezeigt, die sich über alle Aufgaben im Gantt-Diagramm erstreckt.

Vor dieser Änderung gab es nur eine Option, mit der Meilensteine in einem Gantt-Diagramm angezeigt werden konnten, die als &quot;Meilensteine&quot;bezeichnet wurde. Mit dieser Option wurden sowohl das Meilensteindiamantensymbol als auch die Meilensteinlinie aktiviert. Diese Indikatoren konnten nicht getrennt werden.

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Schließen Sie beim Exportieren in PDF die Gantt-Diagrammlegende ein. {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Wenn Sie das Gantt-Diagramm in eine PDF exportieren, können Sie jetzt auswählen, ob Sie auch die Legende des Diagramms zusammen mit der Grafik selbst exportieren möchten. Die Elemente in der Legende sind nur die Optionen, die Sie für die Anzeige in der Gantt-Grafik in der Benutzeroberfläche aktiviert haben. Diese Optionen sind in der Legende enthalten, wenn sie für die Aufgaben im Projekt vorhanden sind. Wenn Sie beispielsweise die Anzeige von Meilensteinen im Gantt-Diagramm aktivieren, werden diese ebenfalls in der Legende angezeigt, allerdings nur, wenn mindestens eine Aufgabe mit einem Meilenstein verbunden ist.

Vor dieser Änderung konnten Sie die Legende nicht aus der exportierten PDF ausschließen. Die Legende enthielt alle möglichen Optionen und Markierungen des Gantt, unabhängig davon, ob sie in der Benutzeroberfläche aktiviert waren oder vorhanden waren.

Weitere Informationen zum Exportieren des Gantt-Diagramms finden Sie unter [Exportieren des Gantt-Diagramms in PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Benutzerinformationen werden von Workfront mit ProofHQ synchronisiert (ProofHQ und Workfront). {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Benutzerinformationen (Name und E-Mail) werden jetzt von Workfront mit ProofHQ synchronisiert, wenn Benutzer in Workfront erstellt oder aktualisiert werden. 

Weitere Informationen zur Benutzersynchronisierung von Workfront mit ProofHQ finden Sie unter .

## Neues Objekt &quot;Proof Creator&quot;im Bericht &quot;Dokumentversion&quot;(Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Beim Erstellen eines Berichts &quot;Dokumentversion&quot;gibt es jetzt ein neues Proof Creator -Objekt. Mit diesem Objekt können Sie Berichte zu Informationen über den Benutzer erstellen, der den Testversand erstellt hat. 

Das neue Testversand-Erstellungsobjekt im Bericht Dokumentversion enthält alle Felder, die mit dem vorhandenen Benutzerobjekt in anderen Objektberichten verfügbar sind.

>[!NOTE]
>
> Diese Informationen sind im Bericht nur ab dem Zeitpunkt verfügbar, zu dem diese Funktion erstmals in der jeweiligen Vorschau- oder Produktionsumgebung eingeführt wurde. Informationen in Berichten zum Anforderungsobjekt, die vor der Einführung dieser Funktion erstellt wurden, sind nicht verfügbar.

Sie greifen beim Erstellen eines Berichts &quot;Dokumentversion&quot;auf das Objekt &quot;Testversand-Erstellung&quot;zu, wie unter [Benutzerdefinierten Bericht erstellen](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Dokumentversion finden Sie im Abschnitt [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Anzeigen von Testversandgenehmigungen im Arbeitsbereich (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Alle Testversandgenehmigungen, die Sie zur Genehmigung eingereicht haben, werden jetzt im Bereich Meine Arbeit auf der Registerkarte **Arbeit, die ich zur Genehmigung eingereicht habe** angezeigt.

Vor dieser Änderung enthielt der Tab **Arbeit, die ich zur Genehmigung eingereicht habe** keine Testversandgenehmigungen.

Testversandgenehmigungen werden nur angezeigt, wenn die folgenden Kriterien erfüllt sind:

* Genehmigung steht derzeit noch aus
* Der Genehmigungsprozess wird einem Benutzer zugewiesen, der lizenzierter Workfront-Benutzer ist (Genehmigungsprozesse, die Benutzern ohne Workfront-Lizenz zugewiesen sind, werden nicht angezeigt)
* Die Validierungsprozesse wurden nach Freigabe dieser Funktion initiiert (Validierungsprozesse, die vor der Freigabe dieser Funktion initiiert wurden, werden nicht angezeigt)

Weitere Informationen finden Sie unter [Genehmigungen anzeigen](../../../../review-and-approve-work/manage-approvals/view-approvals.md) in [Genehmigungen anzeigen](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Anzeigen von Benutzernamen bei der Bearbeitung von Proofing-Genehmigungsanfragen aus meinem Arbeitsbereich (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Bei der Genehmigung von Testversandgenehmigungen aus dem Bereich &quot;Meine Arbeit&quot;wird nun der Name des Benutzers angezeigt, der die Genehmigung angefordert hat.

Weitere Informationen finden Sie unter [Arbeiten genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Arbeiten genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Verbesserter Testversand-Viewer für Videosendungen (ProofHQ und Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Der Testversand-Viewer in Workfront und ProofHQ wird mit einem neuen Look-and-Feel, einer HTML5-Architektur für bessere Leistung und Unterstützung für neue Funktionen aktualisiert.

Der neue Testversand-Viewer enthält die folgenden Verbesserungen:

* Einzelbildprüfung
* Video-Pufferung
* Suchfunktion in der Kommentarliste
* Alle für den Kommentar festgelegten Aktionen werden für jeden Kommentar in der Kommentarliste angezeigt
* Vollbildmodus
* Inhalte schneller oder langsamer überprüfen
* Rechtschreibprüfung beim Hinzufügen von Kommentaren und Antworten

### Vorschau

Der neue Testversand-Viewer steht in den folgenden Vorschauumgebungen zum Testen zur Verfügung:

* ProofHQ-Vorschau-Umgebung

  Weitere Informationen zur ProofHQ-Vorschau-Umgebung finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Workfront-Vorschauumgebung, wenn Ihr Konto für die Prüfung aktiviert ist

  Weitere Informationen zur Workfront-Vorschau-Umgebung finden Sie unter  [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

In dieser Version unterstützt der neue Testversand-Viewer nur die Videoprüfung. Das bedeutet, dass alle Videoproofs den neuen Testversand-Viewer nutzen, während alle statischen und Rich-Media-Testsendungen weiterhin den vorhandenen Testversand-Viewer nutzen.

### Produktion

Wenn sie mit Version 17.2 in die Produktionsumgebung freigegeben werden, können Administratoren auswählen, ob der neue oder alte Testversand-Viewer für die Benutzer in ihrer Organisation geeignet ist. Standardmäßig wird der alte Testversand-Viewer verwendet.

Informationen zur Verwendung des neuen Video-Testversand-Viewers finden Sie unter  

## Anzeigen von Rich-Media-Testsendungen in alternativen Auflösungen (ProofHQ und Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Sie können jetzt die Auflösung von Rich-Media-Testsendungen anpassen, indem Sie entweder eine benutzerdefinierte Auflösung angeben oder das Bild auf die gewünschte Auflösung ziehen.

Vor dieser Änderung konnten Sie Testsendungen nur mit der Auflösung überprüfen, die dem Bildschirm oder dem Gerät, auf dem Sie den Inhalt überprüft haben, innewohnt.

Sie können den Vergleichsmodus verwenden, um verschiedene Testauflösungen zu vergleichen.

Weitere Informationen finden Sie unter [Öffnen von Testsendungen im Desktop Proofing Viewer](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Neue Ressourcenpool-Funktion vorübergehend aus der Vorschau entfernt {#new-resource-pool-functionality-temporarily-removed-from-preview}

Aufgrund von Entwicklungsproblemen haben wir beschlossen, die neue Registerkarte &quot;Ressourcenplanung&quot;zu entfernen und die Registerkarte &quot;Alte Ressourcenplanung&quot;wieder in den ursprünglichen Namen &quot;Ressourcenplanung&quot;umzubenennen.

Mit dieser Änderung wurde auch die neue Funktion Resource Pools entfernt. Die neue Registerkarte &quot;Ressourcenplanung&quot;und die Funktionalität der Ressourcen-Pools werden Ende Juni 2017 zur Sandbox-Vorschau-Umgebung zurückkehren.
