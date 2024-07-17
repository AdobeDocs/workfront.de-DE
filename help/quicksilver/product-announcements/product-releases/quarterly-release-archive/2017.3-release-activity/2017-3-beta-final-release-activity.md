---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Abschlussversion 2017.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der endgültigen Beta-Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 12. September 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# Beta-Abschlussversion 2017.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der endgültigen Beta-Version 2017.3 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 12. September 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird Anfang November 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller 2017.3 vorgenommenen Änderungen finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die endgültige Version 2017.3 von Beta enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Neue Konfiguration für den Aufruf von Anforderungen im Bereich für Genehmigungseinstellungen](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Standardmäßige Proof-Rollen konfigurieren](#configure-default-proof-roles)

**Für alle Benutzer**

* [Startbereich (mein Arbeitsbereich wurde aktualisiert)](#home-area-updated-my-work-area)

* [Aktualisierte Layoutvorlage zur Unterstützung des Startbereichs](#updated-layout-template-to-support-the-home-area)

* [Kanban für Agile](#kanban-for-agile)
* [Probleme im Scrum-Rückholprotokoll für ein Agile-Team einschließen](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Beziehen Sie Probleme auf der Agile Story-Pinnwand des Scums ein](#include-issues-on-the-scrum-agile-story-board)
* [Anwenden von Gruppierungen und Filtern auf das Rückprotokoll für ein Agile-Team](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Verbesserte @Tagging-Funktion gibt in der Vorschauumgebung zurück](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Filtern von Systemaktualisierungen im Aktualisierungs-Stream ist jetzt über Objekte hinweg persistent](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Daten im Nutzungsbericht visualisieren](#visualize-data-in-the-utilization-report)
* [Leistungsverbesserung des Nutzungsberichts](#utilization-report-performance-improvement)
* [Verbesserungen des Dokuments: Optimierte Benutzeroberfläche](#document-enhancements-streamlined-interface)
* [Verbesserungen beim Testen in Workfront](#proofing-enhancements-within-workfront)
* [Verbesserungen beim Testen in Workfront Proof und Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Rich-Text-Formatierung für Updates und E-Mails](#rich-text-formatting-for-updates-and-emails)
* [Neuer Gantt-Diagramm-Neuentwurf](#new-gantt-chart-redesign)
* [ Integrierte Berichte enthalten aktualisierte Beschreibungen](#built-in-reports-contain-updated-descriptions)
* [Branding in exportierten Berichten, Listen und Dashboards](#branding-in-exported-reports-lists-and-dashboards)
* [Verbesserungen beim Kopieren von Aufgaben und Verschieben von Aufgaben oder Problemen](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Neue Gruppierung für ressourcenbudgetierte Stunden-Berichte: Zuordnungsdatum](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Verbesserungen beim Ressourcenplaner](#resource-planner-improvements)
* [Mobile Verbesserungen](#mobile-improvements)
* [Workfront-Integration mit Slack](#workfront-integration-with-slack)
* [Verbesserungen an Outlook 365](#outlook-365-improvements)
* [API-Änderungen](#api-changes)

## Home Area (mein Arbeitsbereich wurde aktualisiert) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Diese Funktion wird mit Version 17.3 nicht für die Produktionsumgebung freigegeben. Sie bleibt bis Anfang 2018 in der Vorschau.

Der neue Startbereich bietet eine alternative, erweiterte Ansicht zu denselben Daten, die derzeit im Arbeitsbereich &quot;Meine Arbeit&quot;verfügbar sind. Der Bereich &quot;Home&quot;bietet im Vergleich zum Bereich &quot;My Work&quot;die folgenden Vorteile:

* Eine optimierte und intuitivere Benutzeroberfläche
* Verbesserte Leistung

Die folgende Funktion ist im Bereich Meine Arbeit verfügbar, aber noch nicht im Bereich Home implementiert:

* Persönlichen Kalender anzeigen
* Aufgaben und Probleme mit der Rich-Text-Formatierung aktualisieren
* Testsendungen genehmigen
* Liste der Arbeiten anzeigen, die Sie zur Genehmigung eingereicht haben
* Erstellen eines Ad-hoc-Problems in einem Projekt
* Nur die Genehmigungen anzeigen, die Ihnen zugewiesen wurden

Weitere Informationen zur Verwendung des neuen Startbereichs finden Sie unter [Verwenden des Startbereichs](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Aktualisierte Layoutvorlage zur Unterstützung des Startbereichs {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Diese Funktion wird mit Version 17.3 nicht für die Produktionsumgebung freigegeben. Sie bleibt bis Anfang 2018 in der Vorschau.

Als Workfront-Administrator können Sie durch Konfiguration der Layout-Vorlage, der Sie zugewiesen sind, feststellen, ob Benutzer in Ihrem Unternehmen Zugriff auf den Startbereich haben. Benutzer, denen keine Layoutvorlage zugewiesen wurde, können immer auf den Startbereich zugreifen.

Weitere Informationen finden Sie unter &quot;Anpassen der Startseite&quot;in &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

## Kanban für Agile  {#kanban-for-agile}

Agile-Teams können jetzt eine Kanban-Methode innerhalb von Workfront verwenden, zusätzlich zu der bereits unterstützten Scrum-agile-Methode.

Die agilen Scrum- und Kanban-Methoden in Workfront unterscheiden sich auf folgende Weise:

**Vorteile der Verwendung von Kanban in Workfront**

* Zeigen Sie den Rückstand auf dem Landingpage von Kanban an.

  Weitere Informationen finden Sie unter .

* Konfigurieren Sie die Elemente im Backlog so, dass sie automatisch dem Landingpage der Geschichte Kanban hinzugefügt werden, wenn andere Elemente in einen Status verschoben werden, der mit Complete übereinstimmt.

  Weitere Informationen finden Sie unter [Konfigurieren von Meldungen, die automatisch aus dem Backlog hinzugefügt werden](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md) .

* Konfigurieren Sie ein Limit für laufende Arbeiten (WIP), das auf dem Landingpage von Kanban angezeigt werden soll.

  Weitere Informationen finden Sie unter [Konfigurieren des Grenzwerts für laufende Arbeiten (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Konfigurieren von Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Vorteile der Verwendung von Scrum in Workfront**

* Fügen Sie einer agilen Iteration eine Reihe von Geschichten hinzu und erstellen Sie eine Story-Pinnwand für diese Iteration.
* Fügen Sie Probleme in das Forum der Story ein.
* Schließen Sie Probleme im Rückstand eines agilen Teams ein.

  Weitere Informationen finden Sie unter [Konfigurieren, wie Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration angewendet werden](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Unteraufgaben können auf dem Forum der Story angezeigt werden.
* Sehen Sie sich eine Abbruchgrafik an, um die Fortschritte bei Meldungen während der Iteration anzuzeigen.

  Weitere Informationen finden Sie unter [Übersicht über die Agile-Burndown-Grafik](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Weitere Informationen zum Aktivieren und Konfigurieren von Kanban für ein agiles Team finden Sie unter [Entscheidung über eine agile Methode](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Erstellen eines agilen Teams](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Einbeziehen von Problemen im Scrum-Backlog für ein Agile-Team {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 wieder in die Vorschauumgebung eingeführt zu werden, mit einer verbesserten Gestaltung und erhöhter Stabilität. Es wird ab Version 2018.1 in der Produktionsumgebung verfügbar sein.

Sie können jetzt Probleme im Rückstand Ihres agile Teams bei der Verwendung der Scrum-agile-Methode einbeziehen (Probleme werden bei Verwendung der Kanban-Methode nicht im Rückstand eines agilen Teams angezeigt). Bestehende Scrum-agile-Teams müssen diese Funktion aktivieren, damit Probleme eingeschlossen werden. Probleme werden automatisch in das Backlog für Scrum-agile-Teams aufgenommen, die nach der Version 2017.3 erstellt werden.

Vor dieser Änderung konnten nur Aufgaben zum Rückstand hinzugefügt werden. Wenn Sie ein Problem hinzufügen möchten, mussten Sie das Problem zunächst in eine Aufgabe konvertieren, bevor es hinzugefügt werden konnte.

Da Sie jetzt Zugriff auf mehr als nur Aufgaben im Rückstadium haben, werden alle zuvor im Rückstau verfügbaren benutzerdefinierten Aufgabenansichten kopiert und als benutzerdefinierte Backlog Work Item-Ansichten zum Rückstau hinzugefügt.

Informationen zur Verwendung von Problemen im Rückstau finden Sie unter  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Informationen zum Aktivieren von Problemen im Rückstand eines agile Scrum-Teams finden Sie unter  [Konfigurieren Sie, wie Datumsangaben angewendet werden, wenn Sie Arbeitselemente zu einer Iteration hinzufügen](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Einbeziehen von Problemen auf dem Scrum Agile Story Board {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 wieder in die Vorschauumgebung eingeführt zu werden, mit einer verbesserten Gestaltung und erhöhter Stabilität. Es wird ab Version 2018.1 in der Produktionsumgebung verfügbar sein.

Sie können jetzt Probleme auf dem Storyboard einbeziehen, wenn Sie die Scrum-agile-Methode verwenden.

Weitere Informationen finden Sie unter [Konfigurieren von Statusspalten auf der agilen Story-Pinnwand](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Anwenden von Gruppierungen und Filtern auf das Rückprotokoll für ein Agile-Team {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Diese Funktion wurde am 14. November 2017 aus der Produktionsumgebung entfernt. Es ist geplant, Anfang 2018 wieder in die Vorschauumgebung eingeführt zu werden, mit einer verbesserten Gestaltung und erhöhter Stabilität. Es wird ab Version 2018.1 in der Produktionsumgebung verfügbar sein.

Die Optionen Gruppierung und Filter sind jetzt im agilen Backlog verfügbar, sodass Sie Ihren Rückstand nach Gruppierungen organisieren und nach bestimmten Aufgaben und Problemen filtern können.

Vor dieser Änderung können Sie Ansichten auf den agilen Rückstand anwenden.

Weitere Informationen finden Sie unter  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Verwalten Sie den agilen Backlog](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Rich-Text-Formatierung für Updates und E-Mails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>In der Vorschau-Umgebung vorgenommene Formatierungsänderungen können in den nicht formatierten Status zurückversetzt werden.

Jetzt können Sie wichtige Informationen hervorheben, indem Sie die Kommentare und Aktualisierungen an Workfront-Objekten formatieren. 

Mit den Rich-Text-Tools können Sie Formatierungsattribute auf Text anwenden, Listen mit Aufzählungszeichen und Nummerierungen erstellen und Hyperlinks zu zusätzlichen Ressourcen hinzufügen.

Die Formatierung, die auf Kommentare im Aktualisierungs-Stream angewendet wird, wird auch in den E-Mail-Benachrichtigungen Aktualisieren angezeigt. Weitere Informationen zur Formatierung Ihrer Kommentare finden Sie unter [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Verbesserte @Tagging-Funktion Gibt in der Vorschauumgebung zurück {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Sie können das @-Symbol erneut verwenden, um andere Benutzer im Update-Stream aller Objekte in der Vorschau-Umgebung mit Tags zu versehen. In der Vergangenheit hat @tagging den Vor- und Nachnamen des getaggten Benutzers im Aktualisierungs-Stream platziert. Die erweiterte Funktion @tagging zeigt jetzt nur den Vornamen des Benutzers an. Weitere Informationen zum Tagging von Benutzern in Updates finden Sie unter [Tagging anderer Benutzer bei Updates](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filtern von Systemaktualisierungen im Aktualisierungs-Stream ist jetzt über Objekte hinweg persistent {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

Die Option &quot;Systemaktualisierungen filtern&quot;ist jetzt auf der gesamten Workfront-Site über Objekte hinweg persistent. Auf diese Weise können Sie Systemaktualisierungen ausblenden und nur Benutzerkommentare im Update-Stream eines Objekts anzeigen. Diese Einstellung bleibt erhalten, wenn Sie zu anderen Objekten navigieren.

Vor dieser Änderung mussten Sie bei der Navigation auf der Workfront-Site Systemaktualisierungen für jedes Objekt herausfiltern.

Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Daten im Nutzungsbericht visualisieren {#visualize-data-in-the-utilization-report}

 Sie können jetzt die Informationen zur Verwendung in einer Diagrammansicht anzeigen. 

Weitere Informationen finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Leistungsverbesserung des Nutzungsberichts {#utilization-report-performance-improvement}

>[!NOTE]
>
>Diese Funktion wurde nach der endgültigen Beta-Version in einem Patch veröffentlicht.

Wenn Sie jetzt einen Nutzungsbericht ausführen, werden Sie aufgefordert, einen Filter anzuwenden, bevor der Bericht ausgeführt wird. Durch diese Änderung wird sichergestellt, dass die relevantesten Informationen so schnell wie möglich im Nutzungsbericht generiert werden.

Weitere Informationen zum Ausführen eines Nutzungsberichts finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Dokumentverbesserungen: optimierte Benutzeroberfläche {#document-enhancements-streamlined-interface}

Das Benutzererlebnis beim Hinzufügen von Dokumenten zu Workfront ist jetzt einfacher und intuitiver. Jetzt können Sie ein Dokument aus Ihrem Dateisystem hochladen, ein Dokument anfordern oder eine Datei aus einer Drittanbieteranwendung (z. B. Google oder Dropbox) verknüpfen - alles aus einem einfachen Dropdown-Menü. 

Zuvor waren diese Optionen durch Starten des Dialogfelds &quot;Dokumente hinzufügen&quot;verfügbar. 

Weitere Informationen finden Sie in den folgenden Informationen:

* [Dokumente aus Ihrem Dateisystem zu Adobe Workfront hinzufügen](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Dokument anfordern](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Mit dieser Änderung ist die Option zum Einfügen eines Bildes oder Dokuments aus der Zwischenablage nicht mehr verfügbar.

## Verbesserungen bei der Überprüfung in Workfront {#proofing-enhancements-within-workfront}

* [Verbessertes Benutzererlebnis und zusätzliche Funktionen](#improved-user-experience-and-additional-functionality)
* [Direkte Freigabe über den Testversand-Viewer](#share-directly-from-the-proofing-viewer)
* [Standardmäßige Proof-Rollen konfigurieren](#configure-default-proof-roles)

### Verbessertes Benutzererlebnis und zusätzliche Funktionen {#improved-user-experience-and-additional-functionality}

Zusätzlich zu einer verbesserten Benutzererfahrung beim Erstellen von Testsendungen in Workfront stehen nun die folgenden zusätzlichen Funktionen zur Verfügung:

* Zusammenführen mehrerer Bilder zu einem Testversand.
* Testversand-Websites mit mehreren Auflösungen (mehrere Auflösungen können als einzelne Testsendungen erstellt oder zu einem Testversand kombiniert werden).
* Bearbeiten Sie den Dateinamen während des Upload-Prozesses.
* Fügen Sie benutzerdefinierte Felder in das Formular zur Testversand-Erstellung ein.
* Fügen Sie eine benutzerdefinierte Nachricht zum Testversand von E-Mail-Benachrichtigungen hinzu.
* Zusätzliche Testeinstellungen 
* Validierung von Echtzeitfehlern beim Testen einer URL (zuvor mussten Sie mehrere Minuten warten, bevor ein Fehler angezeigt wurde)

Weitere Informationen finden Sie unter .

>[!NOTE]
>
> Beim Erstellen eines neuen Testversands mit einem automatisierten Workflow wird das Verschieben von Benutzern von einer Phase in eine andere durch Drag &amp; Drop nicht unterstützt. Entfernen Sie stattdessen den Benutzer aus einem Schritt und fügen Sie ihn einem anderen hinzu.

*Die Option, Benutzer mithilfe von Drag &amp; Drop von einem Schritt in einen anderen zu verschieben, wird mit Version 2018.1 neu eingeführt.*

### Direkte Freigabe über den Testversand-Viewer {#share-directly-from-the-proofing-viewer}

Jetzt können Sie bestimmte Workfront-Benutzer direkt über den Testversand-Viewer freigeben.

>[!NOTE]
>
>Diese Funktion ist nur für neue Testsendungen (Testsendungen, die nach der Version 2017.3 erstellt werden) und nur für Workfront-Instanzen verfügbar, die in ein Workfront Proof Premium-Konto integriert sind.

Vor dieser Änderung konnten Sie nur einen Link erstellen und diesen Link dann für einen Benutzer freigeben. 

Weitere Informationen finden Sie unter [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Standardmäßige Proof-Rollen konfigurieren {#configure-default-proof-roles}

Sie können jetzt die standardmäßigen Testversandrollen konfigurieren, die neue Benutzer und Gastbenutzer für neue Testsendungen im Workfront-System haben. 

Dies ist die Standardrolle, der Benutzer bei einem Testversand zugewiesen werden, wenn der Testversand für sie freigegeben wird. 

## Verbesserungen bei der Überprüfung in Workfront Proof und Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Starten und überspringen Sie im HTML5-Video-Testversand-Viewer (Tastaturbefehle)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5-Viewer-Aktualisierungen für die Überprüfung](#html5-proofing-viewer-updates)

### Starten Sie den HTML5-Video-Testversand-Viewer neu und überspringen Sie ihn (Tastaturbefehle). {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Es gibt jetzt Tastaturbefehle im HTML5-Proofing-Viewer für Videos, mit denen Sie das Video von Anfang an neu starten und bis zum Ende des Videos überspringen können.

Weitere Informationen zu den verfügbaren Tastaturbefehlen finden Sie unter [Tastaturbefehle im Workfront Proof-Testversand-Viewer](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### HTML5-Viewer-Aktualisierungen für die Überprüfung {#html5-proofing-viewer-updates}

Der HTML5-Viewer unterstützt jetzt statische Testsendungen.

Vor dieser Änderung unterstützte der HTML5-Viewer nur Videosendungen. 

Der HTML-Viewer bietet beim Testen von statischen Inhalten die folgenden neuen Funktionen:

* Einen einzelnen Kommentar mit Markups auf mehreren Seiten in der Einzelansicht erstellen

  Dies war bisher nur möglich, wenn sie sich in der Ansicht &quot;Continuous&quot;oder &quot;Magazine&quot;befanden

* Testsendungen über die Testversand-Miniaturansichten durchsuchen

   * Einfache Identifizierung des Teils des Testversands, der geprüft wird. Dies ist besonders dann wichtig, wenn Benutzer mit größeren Testsendungen und langen Webseiten arbeiten oder wenn die  Um die Details zu sehen, ist ein größerer Zoomfaktor erforderlich.
   * Zoomgrad ändern
   * Inhalt schwenken

* Festlegen benutzerdefinierter Werte im Messungstool
* Beim Kommentieren von Text in einem Testversand im Testversand-Viewer in Workfront Proof können Sie Optionen zum Angeben einschließen, dass der Text fett, kursiv und unterstrichen werden soll.

Der HTML5-Viewer unterstützt noch nicht alle Funktionen, die derzeit im bestehenden Flash-Viewer verfügbar sind. Die folgende Funktion ist derzeit nicht verfügbar, wird aber in einer zukünftigen Version enthalten sein:

* Unterstützung von Rich-Media-Dateien
* Vergleichsmodus (Video und statisch)
* Filtern von Kommentaren (Video und statisch)
* Hyperlinks in Dokumenten überprüfen (statisch)
* Übersetzungen (Video und statisch)
* Indikator der Präsenz, der Benutzer anzeigt, die derzeit am Testversand arbeiten
* Testsendungen freigeben

Weitere Informationen zum Testen von statischen Testsendungen im HTML5-Viewer finden Sie unter .

Als Workfront-Administrator in Workfront Proof können Sie festlegen, ob Benutzer in Ihrem Unternehmen Zugriff auf den neuen HTML5-Testversand-Viewer für Videosendungen haben.

## Neue Gantt-Diagramm-Neugestaltung {#new-gantt-chart-redesign}

Das neue Gantt-Diagramm enthält die folgenden Verbesserungen:

* Neue Symbole und Markierungen
* Neue Option zum Vergrößern und Verkleinern eines bestimmten Zeitrahmens
* Kleinere Aufgabenzellen im Listenbereich des Diagramms
* Neu gestaltete Optionen für Einstellungen, Drucken und Wechseln zu den geplanten Datumswerten.

Weitere Informationen zum Konfigurieren von Optionen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Integrierte Berichte enthalten aktualisierte Beschreibungen {#built-in-reports-contain-updated-descriptions}

Die Beschreibungen für unsere Systemberichte in Workfront wurden aktualisiert, um Informationen über den Berichtstyp und die darin enthaltenen Felder zu erhalten.  

Vor dieser Änderung hatten die meisten unserer integrierten Berichte keine oder sehr begrenzte Beschreibungen.

Weitere Informationen zu integrierten Berichten finden Sie unter [Verwenden der integrierten Adobe Workfront-Berichte](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Branding in exportierten Berichten, Listen und Dashboards {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Diese Funktion ist derzeit nicht für alle Cluster in der Umgebung &quot;Vorschau&quot;verfügbar.

Wenn Sie Branding in Workfront nutzen, ist das Logo, das Sie in Ihrer globalen Navigationsleiste verwenden, jetzt in den PDF-Dateien enthalten, die Sie aus Workfront exportieren.

Die folgenden .pdf-Dateien enthalten das Logo Ihrer Organisation im exportierten Dokument:

* Exportierte Listen
* Exportierte und bereitgestellte Berichte
* Gedruckte Dashboards

Weitere Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Daten exportieren](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Verbesserungen beim Kopieren von Aufgaben und Verschieben von Aufgaben oder Problemen {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Wir haben die Art und Weise, wie Sie eine Aufgabe kopieren oder eine Aufgabe oder ein Problem verschieben, verbessert, um die Auswahl eines übergeordneten Elements für die kopierte oder verschobene Aufgabe oder das Problem zu vereinfachen. Bei der Auswahl eines übergeordneten Elements beim Kopieren einer Aufgabe können Sie beispielsweise jetzt eine Hierarchie von Aufgaben mit ihrer übergeordneten - untergeordneten Beziehung sehen und in Projekten mit vielen Aufgaben nach einem übergeordneten Element suchen.

Vor dieser Änderung gab es kein Suchfeld im Schritt **Übergeordnetes Element auswählen** und die Hierarchie der Aufgaben war nicht in der Aufgabenliste sichtbar.

Weitere Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Weitere Informationen zum Verschieben von Problemen finden Sie unter [Probleme beim Verschieben](../../../../manage-work/issues/manage-issues/move-issues.md).

## Neue Konfiguration für das Aufrufen von Anforderungen im Bereich &quot;Genehmigungseinstellungen&quot; {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Im Bereich &quot;Genehmigungseinstellungen&quot;wurde auf Systemebene eine neue Einstellung eingeführt, mit der Workfront-Administratoren entscheiden können, ob sie Benutzern erlauben sollen, sich an ein Problem zu erinnern oder anzufordern, dessen erster Status auf die Genehmigung wartet. Wenn der Rückruf zulässig ist, wird das Problem gelöscht. Wenn der Rückruf nicht zulässig ist, können die Benutzer die Schaltfläche &quot;Rückruf&quot;nicht sehen, wenn der erste Status eines Problems noch nicht genehmigt wurde.

Vor dieser Änderung war immer eine Erinnerung an das Problem zulässig. Als die Genehmigung zurückgerufen wurde, wurde die Genehmigung vollständig umgangen, wodurch das Problem in den ersten Status versetzt wurde, ohne dass eine Genehmigung beigefügt war.

Weitere Informationen zu den Genehmigungseinstellungen finden Sie unter [Globale Genehmigungseinstellungen konfigurieren](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Diese Option wird standardmäßig deaktiviert, wenn diese Funktion veröffentlicht wird. Derzeit ist das Aufrufen von Problemen für alle Organisationen standardmäßig aktiviert. Wenn diese Funktion veröffentlicht wird, muss der Workfront-Administrator diese Einstellung manuell aktivieren, damit die Funktionen in Workfront unverändert bleiben.

## Neue Gruppierung für ressourcenbudgetierte Stunden-Berichte: Zuordnungsdatum {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Wir haben die Möglichkeit hinzugefügt, Ihre Ergebnisse nach dem Zuordnungsdatum zu gruppieren, wenn Sie einen Bericht &quot;Ressourcenbudgetierte Stunde&quot;erstellen.

Vor dieser Änderung konnten Sie das Zuordnungsdatum in der Berichtansicht anzeigen und in einem Filter verwenden. Dieses Feld konnte jedoch nicht in einer Gruppierung verwendet werden.

Weitere Informationen zum Zuordnungsdatum finden Sie im [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Verbesserungen beim Ressourcenplaner {#resource-planner-improvements}

* [Ressourcen-Planer: Daten nach FTE anzeigen](#resource-planner-show-data-by-fte)
* [Ressourcenplaner: Daten nach Woche und Quartal anzeigen](#resource-planner-show-data-by-week-and-quarter)
* [Ressourcenplaner: Ansicht nach Benutzer](#resource-planner-view-by-user)
* [Ressourcenplaner: Ziehen Sie Projekte per Drag-and-Drop zur Festlegung der Priorität](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Ressourcenplaner: Exportieren Sie die Daten im Ressourcenplaner nach Excel.](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Resource Planer: Daten nach FTE anzeigen {#resource-planner-show-data-by-fte}

Jetzt können Sie die Zuordnung und Verfügbarkeit Ihrer Ressourcen nach FTE im Ressourcen-Planer anzeigen. Vor dieser Änderung konnten Sie die Werte nur in Stunden anzeigen.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Daten nach Woche und Quartal anzeigen {#resource-planner-show-data-by-week-and-quarter}

Sie können jetzt das Zeitrahmenintervall für Ihren Ressourcenplaner ändern, um es nach Woche oder Quartal anzuzeigen. Vor dieser Änderung konnten Sie die Zuordnung und Verfügbarkeit Ihrer Ressourcen anzeigen und sie nur monatlich einplanen.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Ansicht nach Benutzer {#resource-planner-view-by-user}

Sie können die Informationen jetzt im Ressourcenplaner nach Benutzer, zuerst nach Projekten, Rollen und Aufgaben anzeigen. Sie können auch einen Unterschied zwischen der geplanten und der verfügbaren Stunden oder der FTE für Benutzer anzeigen. Vor dieser Änderung könnten Sie die Informationen im Ressourcenplaner nach Projekten und Rollen anzeigen.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Projekte zur Festlegung von Prioritäten ziehen und ablegen {#resource-planner-drag-and-drop-projects-to-establish-priority}

Sie können jetzt Projekte in die gewünschte Prioritätsreihenfolge ziehen und ablegen. Vor dieser Änderung können Sie die Priorität von Projekten nur durch manuelles Zuweisen einer Nummer festlegen.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Ressourcenplaner: Exportieren Sie die Daten im Ressourcenplaner nach Excel. {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Sie können die Informationen im Ressourcenplaner jetzt in eine Excel-Datei exportieren.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Mobile Verbesserungen {#mobile-improvements}

Wir haben die Möglichkeit hinzugefügt, über die Workfront Mobile App auf Ihre Projekte zuzugreifen und sie zu verwalten. Sie können jetzt mit der mobilen Workfront-App Folgendes tun:

* Projektliste aufrufen
* Zugriff auf eine Liste von Aufgaben und Unteraufgaben in einem Projekt
* Auf eine Liste von Problemen in einem Projekt zugreifen
* Neues Problem in einem Projekt protokollieren

Sie können diese Funktion installieren, wenn Sie Ihre mobile Workfront-App aktualisieren. Die Aktualisierung wird im November 2017 sowohl in den Apple- als auch in den Android-Stores verfügbar sein.

## Workfront-Integration mit Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>Die Slack-Integration ist derzeit nicht verfügbar. Es ist ab November 2017 für Ihre Produktionsumgebung verfügbar.

Wir starten eine neue Integration zwischen Workfront und Slack. Wenn Ihr Unternehmen bereits Slack für Ihre Kommunikation verwendet hat, können Sie diese nun in Workfront integrieren und gängige Workfront-Aktionen durchführen, ohne Ihre Kommunikationskanäle im Slack zu belassen. Sie können jetzt die folgenden Aktionen über Ihr Slack-Konto ausführen:

* Suchen nach einem Element in Workfront
* Zugriff auf die Listen für Arbeiten und Genehmigungen
* Aufgabe erstellen
* Problem erstellen
* Abonnieren Sie ein Element aus einem Link, der für Sie mit diesem Element freigegeben ist.
* Aufgaben und Probleme aus einem für Sie freigegebenen Link zuweisen
* Ihre Arbeit genehmigen
* Auf die Listen &quot;Favoriten&quot;und &quot;Letzte Elemente&quot;zugreifen

Weitere Informationen zum Zugriff auf Workfront über Slack finden Sie unter [Verwenden von Workfront mit Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365-Verbesserungen {#outlook-365-improvements}

Das Workfront-Add-in für wurde wie folgt verbessert:  Outlook 365:

* Aufgabe oder Problem zu einem Projekt in Workfront hinzufügen: Sie können jetzt eine E-Mail mit dem Outlook 365-Add-in in eine Aufgabe oder ein Problem in Workfront konvertieren. In diesem Prozess können Sie ein Projekt, dem die Aufgabe oder das Problem hinzugefügt werden soll, sowie einen Bevollmächtigten und ein Fälligkeitsdatum angeben. Vor dieser Verbesserung konnten Sie nur eine Anforderung an eine Anforderungswarteschlange senden oder eine persönliche Aufgabe aus Outlook 365 zu Ihrer Arbeitsaufgabenliste hinzufügen. 
* Link zu Workfront-Objekten in der ursprünglichen E-Mail beibehalten, die in Aufgaben, Probleme oder Anforderungen konvertiert wurden: Wenn Sie eine E-Mail aus Outlook 365 in eine Aufgabe, ein Problem oder eine Anfrage konvertieren, behält Outlook 365 einen Link zu der Aufgabe oder dem Problem bei, die/das aus dieser E-Mail in der ursprünglichen E-Mail konvertiert wurde. Vor dieser Änderung gab es in Outlook keinen Hinweis, ob eine E-Mail in eine Aufgabe konvertiert oder als Anfrage gesendet wurde. 

  Weitere Informationen zum Konvertieren einer E-Mail in eine Aufgabe oder ein Problem aus Outlook 365 finden Sie unter [Hinzufügen einer Outlook-E-Mail zu einem Projekt als Aufgabe oder Problem](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

## API-Änderungen {#api-changes}

* [API 8 ist jetzt verfügbar](#api-8-now-available)
* [ Entfernte und veraltete Versionen der API](#removed-and-deprecated-versions-of-the-api)
* [Aktivität &quot;Abgeschlossene Beta-Version 2017.3&quot;](#updated-message-format-for-event-subscriptions)
* [Wiederholung von Ereignisabonnements für nicht zustellbare Nachrichten](#event-subscription-retries-for-undeliverable-messages)

### API 8 ist jetzt verfügbar {#api-8-now-available}

Workfront API Version 8 ist jetzt verfügbar und bietet neue und aktualisierte Ressourcen für Ihre Workfront-Integrationen.

Eine Liste der an der Workfront-API vorgenommenen Änderungen finden Sie unter [Aktualisierungen der API-Version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Entfernte und veraltete Versionen der API {#removed-and-deprecated-versions-of-the-api}

### Aktualisiertes Nachrichtenformat für Ereignisanmeldungen

Um nützlichere Informationen für Ihre Integrationen bereitzustellen, die die Workfront Event Subscriptions API enthalten, haben wir das Format der ausgehenden Nachricht für unterstützte Ressourcen geändert, indem wir die alten und neuen Werte für diese Ressourcen aufgenommen haben. Um Fehler zu vermeiden, müssen Integrationen, die Sie mit der Workfront Event Subscriptions API haben, entsprechend der Beschreibung in der [Ereignisabonnement-API](../../../../wf-api/general/event-subs-api.md) das neue Format aktualisiert werden.

### Wiederholung von Ereignisabonnements für nicht zustellbare Nachrichten {#event-subscription-retries-for-undeliverable-messages}

Das Workfront-Framework für Ereignisabonnements bietet jetzt einen Mechanismus zur Handhabung von ereignisausgelösten ausgehenden Nachrichten, die nicht an Kundenendpunkte gesendet werden können. Um einen kontinuierlichen Nachrichtenversand sicherzustellen, sollten Kunden sicherstellen, dass alle Endpunkte, die ausgehende Nachrichten aus Ereignisabonnements verarbeiten, ordnungsgemäß eingerichtet sind. Weitere Informationen finden Sie unter [Wiederholungen von Ereignisabonnements](../../../../wf-api/api/event-sub-retries.md).
