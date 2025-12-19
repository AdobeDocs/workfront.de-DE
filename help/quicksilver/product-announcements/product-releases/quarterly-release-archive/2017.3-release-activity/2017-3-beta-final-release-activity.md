---
content-type: release-notes
navigation-topic: product-releases-archive
title: Aktivität "Beta-Endversion 2017.3“
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde am 12. September 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 0%

---

# Aktivität &quot;Beta-Endversion 2017.3“

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2017.3 verfügbar waren. Die Funktion auf dieser Seite wurde am 12. September 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird Anfang November 2017 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2017.3 finden Sie unter  [Übersicht über die Versionsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Beta-Endversion 2017.3 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren**

* [Neue Konfiguration für Abrufanfragen im Bereich Validierungseinstellungen](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Standard-Korrekturabzug-Rollen konfigurieren](#configure-default-proof-roles)

**Für alle Benutzer**

* [Home-Bereich (Bereich „Meine Arbeit“ aktualisiert)](#home-area-updated-my-work-area)

* [Die Layoutvorlage wurde aktualisiert, um den Bereich „Startseite“ zu unterstützen](#updated-layout-template-to-support-the-home-area)

* [Kanban für Agile](#kanban-for-agile)
* [Probleme im Scrum-Rückstand für ein Agile-Team einbeziehen](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Probleme im Scrum Agile-Story-Board einschließen](#include-issues-on-the-scrum-agile-story-board)
* [Wenden Sie Gruppierungen und Filter auf den Rückstand für ein agiles Team an](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Erweiterte @Tagging kehrt in der Vorschau-Umgebung zurück](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Filtersystemaktualisierungen im Aktualisierungsstrom sind jetzt objektübergreifend persistent](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Daten im Auslastungsbericht visualisieren](#visualize-data-in-the-utilization-report)
* [Leistungsverbesserung des Auslastungsberichts](#utilization-report-performance-improvement)
* [Dokumentverbesserungen: Optimierte Benutzeroberfläche](#document-enhancements-streamlined-interface)
* [Proofing-Verbesserungen in Workfront](#proofing-enhancements-within-workfront)
* [Proofing-Verbesserungen sowohl in Workfront Proof als auch in Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Rich-Text-Formatierung für Aktualisierungen und E-Mails](#rich-text-formatting-for-updates-and-emails)
* [Neues Gantt-Diagramm - Neugestaltung](#new-gantt-chart-redesign)
* [Integrierte Berichte enthalten aktualisierte Beschreibungen](#built-in-reports-contain-updated-descriptions)
* [Branding in exportierten Berichten, Listen und Dashboards](#branding-in-exported-reports-lists-and-dashboards)
* [Verbesserungen beim Kopieren von Aufgaben und Verschieben von Aufgaben oder Problemen](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Neue Gruppierung für Ressourcenbudgetierte Stundenberichte: Zuteilungsdatum](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Verbesserungen am Ressourcenplaner](#resource-planner-improvements)
* [Verbesserungen für Mobilgeräte](#mobile-improvements)
* [Workfront-Integration mit Slack](#workfront-integration-with-slack)
* [Outlook 365 - Verbesserungen](#outlook-365-improvements)
* [API-Änderungen](#api-changes)

## Home-Bereich (Bereich „Meine Arbeit“ aktualisiert) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Diese Funktion wird mit Version 17.3 nicht in der Produktionsumgebung veröffentlicht; sie wird bis Anfang 2018 in der Vorschau bleiben.

Der neue Bereich Startseite bietet eine alternative, erweiterte Ansicht der gleichen Daten, die derzeit im Bereich Meine Arbeit verfügbar sind. Der Bereich Startseite bietet im Bereich Meine Arbeit die folgenden Vorteile:

* Eine optimierte und intuitivere Benutzeroberfläche
* Verbesserte Leistung

Die folgenden Funktionen sind im Bereich Meine Arbeit verfügbar, sind jedoch noch nicht im Bereich Startseite implementiert:

* Persönlichen Kalender anzeigen
* Aktualisieren von Aufgaben und Problemen mit Rich-Text-Formatierung
* Korrekturabzüge genehmigen
* Liste der Arbeiten anzeigen, die zur Genehmigung eingereicht wurden
* Ad-hoc-Anfrage für ein Projekt erstellen
* Nur die Genehmigungen anzeigen, die an Sie delegiert wurden

Weitere Informationen zur Verwendung des neuen Bereichs „Startseite“ finden Sie unter [Verwenden des Bereichs „Startseite](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Die Layout-Vorlage zur Unterstützung des Home-Bereichs wurde aktualisiert {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Diese Funktion wird mit Version 17.3 nicht in der Produktionsumgebung veröffentlicht; sie wird bis Anfang 2018 in der Vorschau bleiben.

Als Workfront-Administrator können Sie festlegen, ob Benutzende in Ihrem Unternehmen Zugriff auf den Bereich Startseite haben, indem Sie die Layout-Vorlage konfigurieren, der sie zugewiesen sind. Benutzende, denen keine Layout-Vorlage zugewiesen ist, können jederzeit auf den Bereich Startseite zugreifen.

Weitere Informationen finden Sie unter „Anpassen der Startseite“ in „Erstellen und Verwalten von Layout-Vorlagen“.

## Kanban für Agile  {#kanban-for-agile}

Agile-Teams können jetzt zusätzlich zur bereits unterstützten agilen Scrum-Methode eine Kanban-Methodik in Workfront verwenden.

Die agilen Methoden Scrum und Kanban in Workfront unterscheiden sich wie folgt:

**Vorteile der Verwendung von Kanban in Workfront**

* Zeigt den Rückstand auf dem Kanban-Agile-Story-Board an.

  Weitere Informationen finden Sie unter in .

* Konfigurieren Sie Elemente im Rückstand, die automatisch dem Agile-Story-Board von Kanban hinzugefügt werden sollen, wenn andere Elemente in einen Status verschoben werden, der mit „Abgeschlossen“ übereinstimmt.

  Weitere Informationen finden Sie unter [Automatische Hinzufügung von Storys aus dem Rückstand konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Konfigurieren Sie ein Work In Progress (WIP)-Limit, das im Agile-Story-Board von Kanban angezeigt werden soll.

  Weitere Informationen finden Sie unter [Konfigurieren des Work In Progress (WIP)-Limits](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Konfigurieren von Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Vorteile der Verwendung von Scrum in Workfront**

* Fügen Sie einer Agile-Iteration einen Satz von Storys hinzu und erstellen Sie ein Story Board für diese Iteration.
* Schließen Sie Probleme im Scrum-Story-Board ein.
* Schließen Sie Probleme im Rückstand eines Agile-Teams ein.

  Weitere Informationen finden Sie unter [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Teilaufgaben können im Scrum-Storyboard angezeigt werden.
* Burndown-Diagramm anzeigen, um den Fortschritt bei Storys während der Iteration anzuzeigen.

  Weitere Informationen finden Sie unter [Agile-Burndown-Diagramm - Übersicht](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Weitere Informationen zur Aktivierung und Konfiguration von Kanban für ein Agile-Team finden Sie unter [Entscheidung über eine Agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Erstellen eines Agile-Teams](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Probleme im Scrum-Rückstand für ein Agile-Team einschließen {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 mit einem verbesserten Design und erhöhter Stabilität wieder in die Vorschau-Umgebung einzuführen. Sie wird mit Version 2018.1 in der Produktionsumgebung verfügbar sein.

Sie können jetzt bei Verwendung der agilen Scrum-Methode Probleme in den Rückstand Ihres Agile-Teams einbeziehen (Probleme werden bei Verwendung der Kanban-Methode nicht im Rückstand eines Agile-Teams angezeigt). Vorhandene Agile-Scrum-Teams müssen diese Funktion aktivieren, damit Probleme einbezogen werden können. Probleme werden automatisch in den Rückstand für Scrum-Agile-Teams aufgenommen, die nach der Version 2017.3 erstellt werden.

Vor dieser Änderung konnten nur Aufgaben zum Rückstand hinzugefügt werden. Wenn Sie ein Problem hinzufügen möchten, müssen Sie das Problem zunächst in eine Aufgabe konvertieren, bevor es hinzugefügt werden kann.

Da Sie jetzt Zugriff auf mehr als nur Aufgaben im Rückstand haben, werden alle benutzerdefinierten Aufgabenansichten, die zuvor im Rückstand verfügbar waren, kopiert und dem Rückstand als benutzerdefinierte Rückstand-Arbeitsaufgabenansichten hinzugefügt.

Informationen zur Verwendung von Problemen im Auftragsbestand finden Sie unter  [Verwalten des Agile-Rückstands](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Informationen dazu, wie Probleme im Rückstand eines Agile-Scrum-Teams verfügbar sein können, finden Sie unter  [Konfigurieren Sie in „Scrum konfigurieren“, wie Datumsangaben beim Hinzufügen &#x200B;](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) Arbeitselementen [&#x200B; Iteration &#x200B;](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) werden.

## Probleme im Scrum Agile-Story-Board einschließen {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 mit einem verbesserten Design und erhöhter Stabilität wieder in die Vorschau-Umgebung einzuführen. Sie wird mit Version 2018.1 in der Produktionsumgebung verfügbar sein.

Sie können jetzt Probleme auf dem Story Board einbeziehen, wenn Sie die agile -Methode von Scrum verwenden.

Weitere Informationen finden Sie unter [Konfigurieren von Statusspalten im Agile-Story-Board](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Anwenden von Gruppierungen und Filtern auf den Rückstand eines agilen Teams {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 mit einem verbesserten Design und erhöhter Stabilität wieder in die Vorschau-Umgebung einzuführen. Sie wird mit Version 2018.1 in der Produktionsumgebung verfügbar sein.

Die Gruppierungs- und Filteroptionen sind jetzt im agilen Rückstand verfügbar, sodass Sie Ihren Rückstand nach Gruppierungen organisieren und nach bestimmten Aufgaben und Problemen filtern können.

Vor dieser Änderung konnten Sie Ansichten auf den Agile-Rückstand anwenden.

Weitere Informationen finden Sie unter  [Verwalten des Agile-](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Verwalten des Agile-Rückstands](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Rich-Text-Formatierung für Aktualisierungen und E-Mails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Formatierungsänderungen, die Sie in der Vorschau-Umgebung vornehmen, werden möglicherweise auf den unformatierten Status zurückgesetzt.

Jetzt können Sie wichtige Informationen hervorheben, indem Sie die Kommentare und Aktualisierungen formatieren, die Sie an Workfront-Objekten vornehmen. 

Mit den Rich-Text-Tools können Sie Formatierungsattribute auf Text anwenden, Aufzählungslisten und nummerierte Listen erstellen und Hyperlinks zu zusätzlichen Ressourcen hinzufügen.

Die auf Kommentare im Aktualisierungsverlauf angewendete Formatierung wird auch in den E-Mail-Benachrichtigungen zu Aktualisierungen angezeigt. Weitere Informationen zum Formatieren von Kommentaren finden Sie unter [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Die Funktion für erweiterte @Tagging gibt in der Vorschau-Umgebung zurück {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Sie können erneut das @-Symbol verwenden, um andere Benutzer im Aktualisierungsverlauf aller Objekte in der Vorschau-Umgebung zu taggen. In der Vergangenheit platzierte @tagging den Vor- und Nachnamen des getaggten Benutzers im Aktualisierungsverlauf. Jetzt zeigt die erweiterte @tagging-Funktion nur noch den Vornamen des Benutzers an. Weitere Informationen zum Tagging von Benutzern in Aktualisierungen finden Sie unter [Andere bei Aktualisierungen taggen](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filtersystemaktualisierungen im Aktualisierungsstrom sind jetzt objektübergreifend persistent {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

Die Option Systemaktualisierungen filtern ist jetzt objektübergreifend auf der gesamten Workfront-Site persistent. Auf diese Weise können Sie Systemaktualisierungen ausblenden und nur Benutzerkommentare im Aktualisierungsverlauf für ein Objekt anzeigen. Diese Einstellung bleibt erhalten, wenn Sie zu anderen Objekten navigieren.

Vor dieser Änderung mussten Sie beim Durchsuchen der Workfront-Site für jedes Objekt Systemaktualisierungen herausfiltern.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Daten im Auslastungsbericht visualisieren {#visualize-data-in-the-utilization-report}

 Sie können jetzt Informationen zur Auslastung in einer Diagrammansicht anzeigen. 

Weitere Informationen finden Sie [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) unter [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Performance-Verbesserung des Auslastungsberichts {#utilization-report-performance-improvement}

>[!NOTE]
>
>Diese Funktion wurde nach der endgültigen Veröffentlichung von Beta in einem Patch veröffentlicht.

Beim Ausführen eines Auslastungsberichts werden Sie nun aufgefordert, einen Filter anzuwenden, bevor der Bericht ausgeführt wird. Durch diese Änderung wird sichergestellt, dass die relevantesten Informationen so schnell wie möglich im Auslastungsbericht generiert werden.

Weitere Informationen zum Ausführen eines Auslastungsberichts finden Sie unter [Übersicht über den &#x200B;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) unter [Übersicht über den Bericht zur Ressourcenauslastung](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Dokumentverbesserungen: Optimierte Benutzeroberfläche {#document-enhancements-streamlined-interface}

Das Benutzererlebnis beim Hinzufügen von Dokumenten zu Workfront ist jetzt einfacher und intuitiver. Jetzt können Sie über ein einfaches Dropdown-Menü ein Dokument aus Ihrem Dateisystem hochladen, ein Dokument anfordern oder eine Datei über ein Drittanbieterprogramm (wie Google oder Dropbox) verknüpfen. 

Zuvor waren diese Optionen durch Öffnen des Dialogfelds Dokumente hinzufügen verfügbar. 

Weitere Informationen finden Sie in den folgenden Abschnitten:

* [Dokumente aus Ihrem Dateisystem zu Adobe Workfront hinzufügen](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Dokument anfordern](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Mit dieser Änderung ist die Option zum Einfügen eines Bildes oder Dokuments aus der Zwischenablage nicht mehr verfügbar.

## Proofing-Verbesserungen in Workfront {#proofing-enhancements-within-workfront}

* [Verbessertes Benutzererlebnis und zusätzliche Funktionen](#improved-user-experience-and-additional-functionality)
* [Freigeben direkt über die Proofing-Anzeige](#share-directly-from-the-proofing-viewer)
* [Standard-Korrekturabzug-Rollen konfigurieren](#configure-default-proof-roles)

### Verbessertes Benutzererlebnis und zusätzliche Funktionen {#improved-user-experience-and-additional-functionality}

Zusätzlich zu einem verbesserten Benutzererlebnis beim Erstellen von Korrekturabzügen in Workfront sind jetzt die folgenden zusätzlichen Funktionen verfügbar:

* Zusammenführen mehrerer Bilder zu einem einzigen Korrekturabzug.
* Korrekturabzugs-Websites in mehreren Auflösungen (mehrere Auflösungen können als einzelne Korrekturabzüge erstellt oder zu einem einzigen Korrekturabzug kombiniert werden).
* Bearbeiten Sie den Dateinamen während des Upload-Vorgangs.
* Fügen Sie benutzerdefinierte Felder in das Formular zur Erstellung von Korrekturabzügen ein.
* Hinzufügen einer benutzerdefinierten Nachricht zu Korrekturabzugs-E-Mail-Benachrichtigungen.
* Zusätzliche Korrekturabzugseinstellungen 
* Echtzeit-Fehlervalidierung beim Proofing einer URL (zuvor mussten Sie mehrere Minuten warten, bevor ein Fehler angezeigt wurde)

Weitere Informationen finden Sie unter .

>[!NOTE]
>
> Beim Erstellen eines neuen Korrekturabzugs mit einem automatisierten Workflow wird Drag-and-Drop nicht unterstützt, wenn Benutzer von einem Schritt in einen anderen verschoben werden. Entfernen Sie stattdessen den Benutzer aus einem Schritt und fügen Sie ihn einem anderen Schritt hinzu.

*Die Option, Benutzer per Drag-and-Drop von einem Schritt in einen anderen zu verschieben, wird mit der Version 2018.1 wieder eingeführt.*

### Freigeben direkt über die Proofing-Anzeige {#share-directly-from-the-proofing-viewer}

Jetzt können Sie Inhalte direkt über die Proofing-Anzeige für bestimmte Workfront-Benutzende freigeben.

>[!NOTE]
>
>Diese Funktion ist nur für neue Korrekturabzüge (Korrekturabzüge, die nach der Version 2017.3 erstellt werden) und nur für Workfront-Instanzen verfügbar, die in ein Workfront Proof Premium-Konto integriert sind.

Vor dieser Änderung konnten Sie einen Link nur freigeben, indem Sie ihn erstellen und dann für einen Benutzer freigeben. 

Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Standard-Korrekturabzug-Rollen konfigurieren {#configure-default-proof-roles}

Sie können jetzt die Standardrollen für Korrekturabzüge konfigurieren, die neue Benutzende und Gastbenutzende im Workfront-System für neue Korrekturabzüge verwenden können. 

Dies ist die Standardrolle, der Benutzende in einem Korrekturabzug zugewiesen werden, wenn der Korrekturabzug für sie freigegeben wird. 

## Proofing-Verbesserungen in Workfront Proof und Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Neustart und Überspringen im HTML5-Video-Proofing-Viewer (Tastaturbefehle)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5 Proofing Viewer-Aktualisierungen](#html5-proofing-viewer-updates)

### Neustart und Überspringen im HTML5-Video-Proofing-Viewer (Tastaturbefehle) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Im HTML5 Proofing Viewer stehen jetzt Tastaturbefehle für Videos zur Verfügung, mit denen Sie das Video von Anfang an neu starten und zum Ende des Videos springen können.

Weitere Informationen zu den verfügbaren Tastaturbefehlen finden Sie unter [Tastaturbefehle im Workfront Proof Proofing Viewer](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### HTML5 Proofing Viewer-Aktualisierungen {#html5-proofing-viewer-updates}

Der HTML5-Viewer unterstützt jetzt statische Korrekturabzüge.

Vor dieser Änderung unterstützte der HTML5-Viewer nur Videoabzüge. 

Der HTML-Viewer bietet beim Testen von statischen Inhalten die folgenden neuen Funktionen:

* Erstellen eines einzelnen Kommentars mit Markierungen auf mehreren Seiten in einer einzigen Ansicht

  Dies war bisher nur in der Durchlaufansicht oder Magazinansicht möglich

* Navigieren in Korrekturabzügen über die Miniaturansichten von Korrekturabzügen

   * Identifizieren Sie auf einfache Weise den Teil des Korrekturabzugs, der überprüft wird. Dies ist wichtig, insbesondere wenn Benutzende mit Korrekturabzügen im größeren Format und langen Web-Seiten arbeiten oder zu einem beliebigen Zeitpunkt  Um die Details sehen zu können, ist ein größerer Zoom erforderlich.
   * Zoom-Faktor ändern
   * Inhalt schwenken

* Angeben benutzerdefinierter Werte im Messwerkzeug
* Wenn Sie in Workfront Proof in einem Korrekturabzug im Proofing Viewer Anmerkungen zu Texten vornehmen, können Sie Optionen zum Angeben einschließen, dass der Text fett, kursiv und unterstrichen dargestellt werden soll.

Der HTML5-Viewer unterstützt noch nicht alle Funktionen, die derzeit im vorhandenen Flash-Viewer verfügbar sind. Die folgende Funktion ist derzeit nicht verfügbar, wird aber in eine zukünftige Version aufgenommen:

* Unterstützung von Rich-Media-Dateien
* Vergleichsmodus (Video und statisch)
* Kommentare filtern (Video und statisch)
* Überprüfen von Hyperlinks in Dokumenten (statisch)
* Übersetzungen (Video und statisch)
* Anwesenheitsanzeige, die die Benutzenden anzeigt, die derzeit am Korrekturabzug arbeiten
* Testsendungen freigeben

Weitere Informationen zu statischen Korrekturabzügen im HTML5-Viewer finden Sie unter .

Als Workfront-Administrator in Workfront Proof können Sie festlegen, ob Benutzende in Ihrem Unternehmen Zugriff auf den neuen HTML5 Proofing Viewer für Videoprüfungen haben.

## Neues Gantt-Diagramm neu gestalten {#new-gantt-chart-redesign}

Das neue Gantt-Diagramm enthält die folgenden Verbesserungen:

* Neue Symbole und Markierungen
* Neue Option zum Vergrößern und Verkleinern eines bestimmten Zeitrahmens
* Kleinere Aufgabenzellen im Listenteil des Diagramms
* Neu gestaltete Optionen zum Einstellen, Drucken und Wechseln zu voraussichtlichen Terminen.

Weitere Informationen zum Konfigurieren von Optionen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Integrierte Berichte enthalten aktualisierte Beschreibungen {#built-in-reports-contain-updated-descriptions}

Die Beschreibungen für unsere Systemberichte in Workfront wurden aktualisiert, um Informationen über den Berichtstyp und die eingeschlossenen Felder einzuschließen.  

Vor dieser Änderung hatten die meisten unserer integrierten Berichte keine oder nur eine sehr begrenzte Beschreibung.

Weitere Informationen zu integrierten Berichten finden Sie unter [Verwenden von integrierten Adobe Workfront-Berichten](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Branding in exportierten Berichten, Listen und Dashboards {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht auf allen Clustern in der Vorschau-Umgebung verfügbar.

Wenn Sie das Branding in Workfront nutzen, ist das Logo, das Sie in der globalen Navigationsleiste verwenden, jetzt in den PDF-Dateien enthalten, die Sie aus Workfront exportieren.

Die folgenden PDF-Dateien enthalten das Logo Ihrer Organisation im exportierten Dokument:

* Exportierte Listen
* Exportierte und bereitgestellte Berichte
* Gedruckte Dashboards

Weitere Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Exportieren von Daten](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Verbesserungen beim Kopieren von Aufgaben und Verschieben von Aufgaben oder Problemen {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Wir haben die Art und Weise verbessert, wie Sie eine Aufgabe kopieren oder eine Aufgabe oder ein Problem verschieben, um die Auswahl eines übergeordneten Elements für die kopierte oder verschobene Aufgabe oder das Problem zu erleichtern. Wenn Sie z. B. beim Kopieren einer Aufgabe eine übergeordnete Aufgabe auswählen, können Sie jetzt eine Hierarchie der Aufgaben mit ihrer hierarchischen Beziehung zwischen übergeordneter und untergeordneter Aufgabe anzeigen und in Projekten mit vielen Aufgaben nach einer übergeordneten Aufgabe suchen.

Vor dieser Änderung gab es im Schritt **Übergeordnetes Element auswählen** kein Suchfeld, und die Hierarchie der Aufgaben war in der Aufgabenliste nicht sichtbar.

Weitere Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Weitere Informationen zum Verschieben von Problemen finden Sie unter [Probleme verschieben](../../../../manage-work/issues/manage-issues/move-issues.md).

## Neue Konfiguration für Abrufanfragen im Bereich der Validierungseinstellungen {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Wir haben im Bereich der Genehmigungseinstellungen auf Systemebene eine neue Einstellung eingeführt, damit Workfront-Administratoren entscheiden können, ob sie Benutzenden erlauben sollen, ein Problem zurückzurufen oder eine Anfrage zu stellen, deren erster Status auf Genehmigung steht. Wenn der Rückruf zulässig ist, wird das Problem gelöscht. Wenn der Rückruf nicht zulässig ist, kann die Schaltfläche „Rückruf“ nicht angezeigt werden, wenn der erste Status eines Problems „Genehmigung ausstehend“ ist.

Vor dieser Änderung war ein Rückruf des Problems immer zulässig. Wenn die Genehmigung zurückgerufen wurde, wurde die Genehmigung vollständig umgangen, wodurch das Problem in den ersten Status versetzt wurde, ohne dass eine Genehmigung angehängt wurde.

Weitere Informationen zu den Genehmigungseinstellungen finden Sie unter [Konfigurieren globaler Genehmigungseinstellungen](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Diese Option wird standardmäßig deaktiviert, wenn diese Funktion veröffentlicht wird. Derzeit ist das Abrufen von Problemen standardmäßig für alle Organisationen aktiviert. Wenn diese Funktion veröffentlicht wird, muss der Workfront-Administrator diese Einstellung manuell aktivieren, damit die Funktion so bleibt, wie sie in Workfront ist.

## Neue Gruppierung für Berichte zur Ressource Budgetierte Stunde: Zuordnungsdatum {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Wir haben die Möglichkeit hinzugefügt, Ihre Ergebnisse beim Erstellen eines Berichts „Ressource - budgetierte Stunde“ nach Zuordnungsdatum zu gruppieren.

Vor dieser Änderung konnten Sie das Zuordnungsdatum in der Ansicht des Berichts anzeigen und in einem Filter verwenden, Sie konnten dieses Feld jedoch nicht in einer Gruppierung verwenden.

Weitere Informationen zum Zuordnungsdatum finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Verbesserungen am Ressourcenplaner {#resource-planner-improvements}

* [Ressourcenplaner: Daten nach FTE anzeigen](#resource-planner-show-data-by-fte)
* [Ressourcenplaner: Daten nach Woche und Quartal anzeigen](#resource-planner-show-data-by-week-and-quarter)
* [Ressourcenplaner: Nach Benutzer anzeigen](#resource-planner-view-by-user)
* [Ressourcenplaner: Projekte per Drag-and-Drop verschieben, um Priorität festzulegen](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Ressourcenplaner: Exportieren der Daten im Ressourcenplaner nach Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Ressourcenplaner: Daten nach FTE anzeigen {#resource-planner-show-data-by-fte}

Sie können jetzt die Zuordnung und Verfügbarkeit Ihrer Ressourcen nach FTE im Ressourcenplaner anzeigen. Vor dieser Änderung konnten Sie die Werte nur in Stunden anzeigen.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Daten nach Woche und Quartal anzeigen {#resource-planner-show-data-by-week-and-quarter}

Sie können jetzt das Zeitrahmenintervall für Ihren Ressourcenplaner ändern, um ihn nach Woche oder Quartal anzuzeigen. Vor dieser Änderung konnten Sie die Zuordnung und Verfügbarkeit Ihrer Ressourcen anzeigen und sie nur nach Monat budgetieren.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Nach Benutzer anzeigen {#resource-planner-view-by-user}

Sie können die Informationen jetzt im Ressourcenplaner anzeigen, zunächst nach Benutzer, dann nach Projekten, Rollen und Aufgaben. Sie können auch einen Unterschied zwischen der geplanten und der verfügbaren Stunde oder FTE für Benutzer anzeigen. Vor dieser Änderung konnten Sie die Informationen im Ressourcenplaner nach Projekten und Rollen anzeigen.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Projekte per Drag-and-Drop verschieben, um Priorität festzulegen {#resource-planner-drag-and-drop-projects-to-establish-priority}

Sie können Projekte jetzt in der gewünschten Prioritätsreihenfolge per Drag-and-Drop verschieben. Vor dieser Änderung konnten Sie die Priorität von Projekten nur festlegen, indem Sie ihnen manuell eine Zahl zuweisen.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Exportieren der Daten im Ressourcenplaner nach Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Sie können nun die Informationen im Ressourcenplaner in eine Excel-Datei exportieren.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Verbesserungen für Mobilgeräte {#mobile-improvements}

Wir haben die Möglichkeit hinzugefügt, über die Workfront Mobile App auf Ihre Projekte zuzugreifen und sie zu verwalten. Mit der Mobile App von Workfront können Sie jetzt Folgendes tun:

* Zugriff auf eine Liste Ihrer Projekte
* Zugriff auf eine Liste von Aufgaben und Teilaufgaben in einem Projekt
* Zugriff auf eine Problemliste in einem Projekt
* Ein neues Problem in einem Projekt protokollieren

Sie können diese Funktion installieren, wenn Sie Ihre Workfront Mobile App aktualisieren. Das Update wird im November 2017 sowohl in den Apple- als auch in den Android Mobile-Stores verfügbar sein.

## Integration von Workfront mit Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>Die Slack-Integration ist derzeit nicht verfügbar. Sie wird ab November 2017 in Ihrer Produktionsumgebung verfügbar sein.

Wir starten eine neue Integration zwischen Workfront und Slack. Wenn Ihr Unternehmen bereits Slack für Ihre Kommunikation verwendet hat, können Sie es jetzt in Workfront integrieren und gängige Workfront-Aktionen durchführen, ohne Ihre Kommunikationskanäle in Slack verlassen zu müssen. Sie können jetzt über Ihr Slack-Konto die folgenden Aktionen ausführen:

* Suchen nach einem Element in Workfront
* Zugriff auf Ihre Arbeits- und Genehmigungslisten
* Erstellen einer Aufgabe
* Problem erstellen
* Elemente über einen Link abonnieren, der für Sie mit diesem Element geteilt wurde
* Aufgaben und Probleme aus einem mit Ihnen geteilten Link zuweisen
* Genehmigen Ihrer Arbeit
* Zugreifen auf Favoriten und die Listen der letzten Elemente

Weitere Informationen zum Zugriff auf Workfront über Slack finden Sie unter [Verwenden von Workfront mit Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365 - Verbesserungen {#outlook-365-improvements}

Wir haben folgende Verbesserungen am Workfront-Add-in für vorgenommen  Outlook 365:

* Aufgabe oder Problem zu einem Projekt in Workfront hinzufügen: Sie können jetzt mithilfe des Outlook 365-Add-ins eine E-Mail in eine Aufgabe oder ein Problem in Workfront konvertieren. In diesem Prozess können Sie ein Projekt, dem die Aufgabe oder das Problem hinzugefügt werden soll, sowie einen Bevollmächtigten und ein Fälligkeitsdatum angeben. Vor dieser Verbesserung konnten Sie nur eine Anfrage an eine Anfrage-Warteschlange senden oder eine persönliche Aufgabe aus Outlook 365 zu Ihrer Arbeitsliste hinzufügen. 
* Beibehalten eines Links zu Workfront-Objekten in der ursprünglichen E-Mail, die in Aufgaben, Probleme oder Anfragen konvertiert wurde: Wenn Sie eine E-Mail von Outlook 365 in eine Aufgabe, ein Problem oder eine Anfrage konvertieren, behält Outlook 365 einen Link zu der Aufgabe oder dem Problem bei, die bzw. das aus dieser E-Mail in der ursprünglichen E-Mail konvertiert wurde. Vor dieser Änderung gab es in Outlook keinen Hinweis darauf, ob eine E-Mail in eine Aufgabe konvertiert oder als Anfrage gesendet wurde. 

## API-Änderungen {#api-changes}

* [API 8 jetzt verfügbar](#api-8-now-available)
* [Entfernte und veraltete Versionen der API](#removed-and-deprecated-versions-of-the-api)
* [2017.3 Beta - Endgültige Release-Aktivität](#updated-message-format-for-event-subscriptions)
* [Wiederholungen von Ereignisabonnements für nicht zustellbare Nachrichten](#event-subscription-retries-for-undeliverable-messages)

### API 8 jetzt verfügbar {#api-8-now-available}

Die Workfront-API Version 8 ist jetzt verfügbar und bietet Ihnen neue und aktualisierte Ressourcen für Ihre Workfront-Integrationen.

Eine Liste der an der Workfront-API vorgenommenen Änderungen finden Sie unter [Aktualisierungen der API Version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Entfernte und veraltete Versionen der API {#removed-and-deprecated-versions-of-the-api}

### Nachrichtenformat für Ereignisabonnements aktualisiert

Um nützlichere Informationen für Ihre Integrationen bereitzustellen, die die Workfront-Ereignisabonnement-API enthalten, haben wir das Format für ausgehende Nachrichten für unterstützte Ressourcen geändert, indem wir die alten und neuen Werte einbezogen, die mit diesen Ressourcen verknüpft sind. Um Fehler zu vermeiden, müssen alle Integrationen, die Sie mit der Workfront-Ereignisabonnement-API haben, auf das neue Format aktualisiert werden, wie in [Ereignisabonnement-API](../../../../wf-api/general/event-subs-api.md) beschrieben.

### Wiederholungen von Ereignisabonnements für nicht zustellbare Nachrichten {#event-subscription-retries-for-undeliverable-messages}

Das Workfront-Ereignisabonnement-Framework bietet jetzt einen Mechanismus für die Verarbeitung von ereignisgesteuerten ausgehenden Nachrichten, die nicht an Kundenendpunkte gesendet werden können. Um einen kontinuierlichen Nachrichtenversand sicherzustellen, sollten Kunden sicherstellen, dass alle Endpunkte, die ausgehende Nachrichten von Ereignisabonnements verwenden, ordnungsgemäß eingerichtet sind. Weitere Informationen finden Sie unter [Wiederholen von Ereignisabonnements](../../../../wf-api/api/event-sub-retries.md).
