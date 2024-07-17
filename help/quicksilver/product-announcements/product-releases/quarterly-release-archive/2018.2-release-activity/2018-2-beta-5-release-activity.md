---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 5-Release-Aktivität 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 5 Version 2018.2 verfügbar waren. Die Funktion ist ab dem 1. Juni 2018 in der Vorschau-Umgebung verfügbar. Verbesserungen der Testversand-Veröffentlichung mit Beta 5 werden am Montag, den 4. Juni in der Vorschau-Umgebung verfügbar sein. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3165'
ht-degree: 1%

---

# Beta 5-Release-Aktivität 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 5 Version 2018.2 verfügbar waren. Die Funktion ist ab dem 1. Juni 2018 in der Vorschau-Umgebung verfügbar. Verbesserungen der Testversand-Veröffentlichung mit Beta 5 werden am Montag, den 4. Juni in der Vorschau-Umgebung verfügbar sein. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.2 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta 5-Version 2018.2 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Anzeigen benutzerbedingter Änderungen mit Auditprotokollen](#view-user-triggered-changes-with-audit-logs)
* [Lizenzinformationen als Gruppenadministrator anzeigen](#view-license-information-as-a-group-administrator)

**Für alle Benutzer**

* [Kalenderansicht im Startbereich](#calendar-view-in-the-home-area)
* [Zusätzliche Aktualisierungen der Arbeitsliste (linker Bereich) auf der Startseite](#additional-updates-to-the-work-list-left-panel-in-home)
* [Konfigurieren von Auftragsrollenbeschränkungen für die automatisierte Ressourcenplanung](#configure-job-role-limits-for-automated-resource-scheduling)
* [Verbesserungen an Projekt- und Rollenansicht im Ressourcenplaner](#project-and-role-view-improvements-in-the-resource-planner)
* [Spaltenbreiten für Projektlisten vergrößern](#resize-column-widths-for-project-lists)
* [Symbolunterstützung für die neuen Projektlisten](#icon-support-for-the-new-project-lists)
* [Feld &quot;Große Miniaturansicht&quot;in Dokumentansichten hinzufügen](#add-large-thumbnail-field-in-document-views)
* [Excel-Exportlimit erhöhen](#increase-excel-export-limit)
* [Schnellfilter für Projektlisten](#quick-filters-for-project-lists)
* [Referenzprobleme-Sammlungen in Projekt- und Aufgabenberichten](#reference-issue-collections-in-project-and-task-reports)
* [Neues Menü mit robusteren Versionen beim Hinzufügen neuer Dokumentversionen in Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Verbesserungen für Mobilgeräte in der mobilen Android Beta-App](#mobile-improvements-in-the-android-beta-mobile-app)
* [Viewer-Verbesserungen für die Überprüfung (Workfront und Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Verbesserungen beim Testen in Workfront](#proofing-enhancements-in-workfront)
* [Verbesserungen bei der Überprüfung in Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Kalenderansicht im Startbereich {#calendar-view-in-the-home-area}

Jetzt können Sie Ihre persönlichen Arbeitsaufgaben und Zeitpläne in der Ansicht &quot;Workfront Home Calendar&quot;verwalten. In der Ansicht &quot;Home Calendar&quot;haben Sie folgende Möglichkeiten:

* Legen Sie Ihren eigenen Zeitplan für die Erfüllung der Ihnen zugewiesenen Workfront-Aufgaben fest.
* Schnelles Anzeigen der Aufgaben, die fällig oder überfällig werden
* Anzeigen der insgesamt zugewiesenen Stunden für eine Woche
* Aktualisieren von zugewiesenen Aufgaben

Wenn Sie einen Kalender in Outlook verwenden, können Sie Ihren Kalender integrieren, um Ihre Outlook-Ereignisse in Ihrer Home-Kalender-Ansicht anzuzeigen.

Weitere Informationen finden Sie unter [Ansicht &quot;Home Calendar&quot;](../../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Zusätzliche Aktualisierungen der Arbeitsliste (linker Bereich) auf der Startseite {#additional-updates-to-the-work-list-left-panel-in-home}

Die folgenden Verbesserungen sind jetzt für die Arbeitsliste im Bereich &quot;Startseite&quot;verfügbar:

* Die Anzahl der abgeschlossenen Elemente wird jetzt in Klammern neben der Option Abgeschlossen im Dropdown-Menü Filter angezeigt.

  Zuvor wurde die Anzahl der abgeschlossenen Elemente nicht im Menü Filter angezeigt. 

* Abgeschlossene Artikel werden für die letzten 2 Wochen angezeigt.

  Zuvor wurden abgeschlossene Elemente für die letzten 3 Monate angezeigt.

  Informationen zum Anzeigen abgeschlossener Arbeiten im Startbereich finden Sie unter [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) im Artikel [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Fügen Sie die Felder Dauer und Zuweisung hinzu, die angezeigt werden sollen, wenn Elemente im Bereich Startseite ausgewählt sind.

  Zuvor war das Feld Zuweisungen standardmäßig verfügbar. Wenn es jedoch gelöscht wurde, konnte es nicht erneut hinzugefügt werden. Das Feld Dauer konnte zuvor nicht hinzugefügt werden.

  Informationen zum Hinzufügen von Feldern zum Startbereich finden Sie unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

Weitere Informationen zur Verwendung des Startbereichs finden Sie unter [Verwenden des Startbereichs](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Vom Benutzer ausgelöste Änderungen mit Prüfprotokollen anzeigen {#view-user-triggered-changes-with-audit-logs}

Wir haben die folgenden Auditprotokolle für Workfront-Administratoren erstellt, um benutzergesteuerte Änderungen zu verfolgen:

* Auditprotokoll für Benutzer
* Auditprotokoll auf Zugriffsebene
* Group Audit Logs
* Prüfprotokolle für Anmeldeversuche

Zuvor gab es keine Möglichkeit, Änderungen innerhalb des Systems zu verfolgen.

Weitere Informationen finden Sie unter [Audit-Protokolle anzeigen und exportieren](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Lizenzinformationen als Gruppenadministrator anzeigen {#view-license-information-as-a-group-administrator}

Wir haben eine schreibgeschützte Lizenzseite für Gruppenadministratoren erstellt, auf der die Lizenzanzahl für die von ihnen verwalteten Gruppen angezeigt wird.

Vor dieser Änderung konnten Gruppenadministratoren keine Lizenzinformationen anzeigen.

Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Konfigurieren von Auftragsrollenbeschränkungen für die automatisierte Ressourcenplanung {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

In den Einstellungen für die Zeitplanung automatisierter Ressourcen können Sie jetzt einer Auftragsrolle ein Limit zuweisen. Auf diese Weise können Sie die Anzahl der Ressourcen steuern, denen mit der gleichen Rolle Aufgaben zugewiesen werden.

Zuvor war es nicht möglich anzugeben, wie vielen Benutzern in einer bestimmten Aufgabenrolle Arbeitsaufgaben zugewiesen werden konnten.

Weitere Informationen finden Sie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;.

## Verbesserungen an Projekt- und Rollenansicht im Ressourcenplaner {#project-and-role-view-improvements-in-the-resource-planner}

Die Projekt- und Rollenansichten des Ressourcen-Planers enthalten jetzt die folgenden Verbesserungen:

* Verbesserte Filter, die Informationen aus der gesamten Datenbank abrufen und nicht nur Informationen auf dem Bildschirm.
* Vollbildmodus.
* Die Leistung ist jetzt schneller und effizienter.

   * Neue Einschränkungen für die Anzahl der Projekte, Rollen und Benutzer, die Sie anzeigen können.
   * Lazy Loading, für schnelleres Laden von Projekten und Rollen.

* Schnellzugriff auf Projekte und Benutzer direkt über den Ressourcen-Planer.
* Schnellere Drag &amp; Drop-Funktion in der Projektansicht, um Ihre Projekte zu priorisieren.

Vor diesen Verbesserungen haben Sie berichtet, dass der Ressourcen-Planer langsam geladen wurde und dass Sie Unstimmigkeiten in den angezeigten Daten bemerkt haben. Mit diesen Verbesserungen sollten diese nun beseitigt werden.

Informationen und Informationen zu den neuen Einschränkungen für den Ressourcen-Planer finden Sie unter [Anzeigebeschränkungen für den Ressourcen-Planer](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Spaltenbreiten für Projektlisten vergrößern {#resize-column-widths-for-project-lists}

Da wir an der Verbesserung der Funktionalität unserer Listen gearbeitet haben, hatten wir die Möglichkeit vorübergehend deaktiviert, die Größe der Spalten in den folgenden Projektlisten zu ändern:

* Projekte in meinem Besitz
* Projekte, an denen ich mitwirke
* Alle Projekte

Mit dieser Version können wir nun die Größe der Spalten aller Projektlisten erneut ändern.

Diese Funktion wurde um weitere Verbesserungen ergänzt.

Wenn Sie nun den rechten Rahmen einer Spalte ziehen, um ihre Größe zu ändern, behält die benachbarte Spalte rechts ihre Größe bei, sodass die Liste breiter wird, anstatt sie auch zu ändern. Sie können auch den Rahmen einer Spalte nach rechts über die Rahmen der benachbarten Spalten ziehen.

Vor dieser Verbesserung wurde die Größe der benachbarten Spalte rechts von der Größenanpassung proportional angepasst, sodass sie auf den Bildschirm passt. Sie konnten den Rand einer Spalte nicht über den rechten Rand der benachbarten Spalte ziehen.  

Informationen zum Ändern der Größe der Neuanordnungsspalten in Listen finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Informationen zur Teilnahme an unserem Beta-Test-Programm für die aktuellen Listenverbesserungen finden Sie unter [Neue Listen-Studie .](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=6b135c15-33dd-4fa2-8bc3-7cd7f7740c57&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520) (Anmeldung erforderlich)

## Symbolunterstützung für die neuen Projektlisten {#icon-support-for-the-new-project-lists}

Da wir an der Verbesserung der Funktionalität unserer Listen gearbeitet haben, hatten wir die Anzeige von Statussymbolen in den folgenden Projektlisten vorübergehend deaktiviert:

* Projekte in meinem Besitz
* Projekte, an denen ich mitwirke
* Alle Projekte

Mit dieser Version können in Ihren Projektlisten für Projekte oder andere Objekte in einer Projektliste wieder Statussymbole angezeigt werden.

Informationen zum Arbeiten in Listen finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Feld &quot;Große Miniaturansicht&quot;in Dokumentansichten hinzufügen {#add-large-thumbnail-field-in-document-views}

Wir fügen ein neues Feld namens Große Miniaturansicht zu einer Dokumentansicht in einer Liste oder einem Bericht hinzu. Wenn dieses Feld in einer Dokumentansicht ausgewählt ist, wird eine Miniaturansicht des Dokuments in einer Liste oder einem Bericht mit einer Breite von 400 Pixel angezeigt.

Vor dieser Änderung konnten Sie nur das Feld Miniaturansicht zu einer Dokumentansicht hinzufügen, die eine 33-66 Pixel breite Miniaturansicht des Dokuments anzeigt.

Weitere Informationen zu Feldern in Listen und Berichten finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Excel-Exportlimit erhöhen {#increase-excel-export-limit}

Die Beschränkung für die Anzahl der Zeilen, die in eine Excel-Datei exportiert werden können, wurde erhöht. Jetzt können Sie Folgendes exportieren:

* 65.000 Zeilen in einer Excel.xls-Datei
* 100.000 Zeilen in einer Excel.xlsx-Datei

Die neuen Beschränkungen gelten, wenn Sie Folgendes aus Workfront exportieren:

* Liste oder Bericht über die Web-Oberfläche
* Eine Liste oder einen Bericht mit der API
* Ein terminierter und bereitgestellter Bericht

Vor dieser Verbesserung konnten Sie nur 50.000 Zeilen in eine beliebige Excel-Datei exportieren.

Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Daten exportieren](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Schnellfilter für Projektlisten {#quick-filters-for-project-lists}

Sie können jetzt einen Schnellfilter auf Listen anwenden.

Mit einem Schnellfilter können Sie direkt zu den Elementen in Ihren großen Listen navigieren, die für Sie von Bedeutung sind, sodass Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.

Derzeit sind Schnellfilter nur für Projektlisten in den folgenden Unterregisterkarten verfügbar:

* Projekte, an denen ich mitwirke
* Projekte in meinem Besitz
* Alle Projekte

Informationen zu Schnellfiltern finden Sie im Abschnitt &quot;Anwenden von Schnellfiltern auf Listen&quot;in [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Referenzprobleme-Sammlungen in Projekt- und Aufgabenberichten {#reference-issue-collections-in-project-and-task-reports}

Sie können jetzt eine Sammlung von Problemen in einer Projekt- oder Aufgabenansicht und einem Filter referenzieren. Dies ist nur im Textmodus möglich, wenn Sie einen Bericht erstellen.

Vor dieser Verbesserung konnten Sie nur eine Sammlung von Aufgaben in einer Projektansicht oder einem -filter referenzieren.

Informationen zum Verweisen auf eine Sammlung in einem Bericht finden Sie unter [Verweisen auf Sammlungen in einem Bericht](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Informationen zur Verwendung des Textmodus finden Sie unter  [Überblick über häufige Verwendungen für den Textmodus](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>Im folgenden Video war der Beispieltextmodus für Problemkollektionen falsch. Der richtige Beispieltextmodus ist in [Referenzsammlungen in einem Bericht](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md) verfügbar.

## Neues Menü für eine zuverlässigere Version beim Hinzufügen neuer Dokumentversionen in Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Beim Hinzufügen neuer Versionen zu Dokumenten in Workfront enthält das Menü &quot;Neue Version&quot;jetzt zusätzliche Optionen und ist nun in allen Bereichen von Workfront konsistent, in denen Sie eine neue Version hinzufügen können.

Sie können eine neue Dokumentversion aus den folgenden Bereichen von Workfront hinzufügen:

* Über das Dropdown-Menü Mehr auf der Registerkarte Dokumente .
* Auf der Seite mit den Dokumentdetails im Menü Dokumentaktionen .
* Auf der Seite mit den Dokumentdetails auf der Registerkarte Alle Versionen .

Vor dieser Änderung enthielt nur das Dropdown-Menü Mehr auf der Registerkarte Dokumente alle Optionen zum Hinzufügen einer neuen Version.

Die folgenden Optionen sind jetzt im Menü Neue Version für alle Bereiche verfügbar, in denen Sie eine neue Version hinzufügen können:

* Korrekturabzug
* Nur Dokument
* Verknüpfte Optionen (vom Dropbox, vom Google-Laufwerk usw.)
* Aus Zwischenablage einfügen (dies ist eine neue Option beim Hinzufügen von Versionen)

Weitere Informationen finden Sie unter [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) im Artikel [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Mobile Verbesserungen in der Android Beta Mobile App {#mobile-improvements-in-the-android-beta-mobile-app}

Die folgenden Verbesserungen sind in der Android Beta-Version der App kurz nach diesem Release verfügbar:

* Aktionen wischen

  Sie können Aktivitäten wie Freiwilligenarbeit durchführen, um eine Aufgabe zu bearbeiten, eine Aufgabe abzuschließen, eine Benachrichtigung als angezeigt oder neu zu markieren, Text schreiben oder einen Kontakt aufrufen, indem Sie in der mobilen Workfront-App verschiedene Objekte wischen.

  Die folgenden Bereiche wurden mit dieser Funktion verbessert:

   * Meine Arbeit und mein Zuhause
   * Benachrichtigungen
   * Kontakte
   * Genehmigungen

* Neues Erscheinungsbild beim Anzeigen der Registerkarte &quot;Details&quot;eines Elements

  Die Benutzeroberfläche wurde beim Anzeigen eines Elements in der Android Beta-Version der App geändert, um die Bearbeitung, Fertigstellung oder Anfügung eines Dokuments zu vereinfachen.

* Neues Erlebnis bei Protokollierungszeit

  Die Protokollierungszeit ist schneller und einfacher als zuvor, mit einer einfacheren Zugriffsmöglichkeit auf die Protokollzeit-Schaltfläche und einer optimierten Oberfläche für die Protokollierungszeiten.

Mit dieser Version sind diese Verbesserungen nur für die Android Beta-Version der mobilen Workfront-App verfügbar. Sie sind derzeit nicht für iOS verfügbar.

Weitere Informationen dazu, wie Sie sich als Beta-Tester anmelden und die Android Beta-Version der mobilen Workfront-App herunterladen, finden Sie unter .

## Viewer-Verbesserungen für die Überprüfung (Workfront und Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Aktualisierte Seite mit der Druckzusammenfassung ](#updated-print-summary-page)
* [Benutzer direkt vom Testversand-Viewer zu einem Testversand hinzufügen](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Alle Markup-Tools im Testversand-Viewer anzeigen](#display-all-markup-tools-in-the-proofing-viewer)
* [Konfigurieren der standardmäßigen Sortieroptionen im Testversand-Viewer](#configure-default-sorting-options-in-the-proofing-viewer)
* [Anzeigen von Workfront-Dokumentgenehmigungen im Desktop-Proofing-Viewer](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Konfigurieren von Links, die neue Registerkarten und Windows öffnen, um sie im Desktop Proofing Viewer zu öffnen](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Präsenzindikator im Testversand-Viewer](#presence-indicator-in-the-proofing-viewer)
* [Filtern von Kommentaren zum Anzeigen einer einzelnen Seite für interaktive URL-Testsendungen im Desktop-Testversand-Viewer](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Desktop-Proofing-Viewer für statische und Videoinhalte](#desktop-proofing-viewer-for-static-and-video-content)
* [Hinzufügen benutzerdefinierter Geräte zu Ihrem System](#add-custom-devices-to-your-system)

### Aktualisierte Seite &quot;Druckzusammenfassung&quot; {#updated-print-summary-page}

Die Seite &quot;Druckzusammenfassung&quot;wurde mit einem neuen Erscheinungsbild und verbesserter Funktionalität aktualisiert.

Weitere Informationen finden Sie unter [Drucken einer Testversand-Zusammenfassung in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Hinzufügen von Benutzern zu einem Testversand direkt über den Testversand-Viewer {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Jetzt können Sie Benutzer direkt über den Web Proofing Viewer und den Desktop Proofing Viewer zu einem Testversand hinzufügen. 

Zuvor war es nicht möglich, einzelne Benutzer zu einem Testversand hinzuzufügen. Stattdessen können Sie nur die öffentliche URL oder den Einbettungscode kopieren.

Weitere Informationen finden Sie unter [Freigeben eines Testversands durch Hinzufügen von Benutzern dazu](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) im Artikel  [Geben Sie einen Testversand aus dem Testversand-Viewer frei](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Alle Markup-Tools im Testversand-Viewer anzeigen {#display-all-markup-tools-in-the-proofing-viewer}

Sie können das Markup-Tool jetzt so konfigurieren, dass es immer wieder angezeigt wird und nicht in einem Menü, das Sie öffnen müssen. Dadurch wird der Wechsel zwischen Tools beschleunigt. Wenn Markup-Tools auf diese Weise konfiguriert werden, werden sie horizontal oben im Web Proofing Viewer und im Desktop Proofing Viewer angezeigt.

Zuvor waren Markup-Tools nur in einem Dropdown-Menü verfügbar.

Weitere Informationen zum Konfigurieren dieser Markup-Einstellung finden Sie unter [Konfigurieren der Testversand-Viewer-Einstellungen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Weitere Informationen zur Verwendung von Markup-Optionen bei der Überprüfung eines Testversands finden Sie im Artikel .

### Konfigurieren von Standardsortierungsoptionen im Testversand-Viewer {#configure-default-sorting-options-in-the-proofing-viewer}

Wenn Sie jetzt die Sortieroption innerhalb der Kommentarliste in einem Testversand ändern, wird diese Option zur standardmäßigen Sortieroption, wenn Sie das nächste Mal einen Testversand im Web Proofing Viewer oder Desktop Proofing Viewer öffnen. 

Weitere Informationen finden Sie im Artikel .

### Anzeigen von Workfront-Dokumentgenehmigungen im Desktop-Proofing-Viewer {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Jetzt können Sie im Desktop Proofing Viewer eine Workfront-Dokument-Genehmigungsentscheidung treffen.

Bisher konnten Sie nur mit dem Web Proofing-Viewer eine Workfront-Dokumentvalidierungsentscheidung treffen. 

Weitere Informationen finden Sie unter  [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) im Artikel  [Entscheiden Sie sich für einen Testversand im Testversand-Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Konfigurieren von Links, die neue Registerkarten und Windows öffnen, um sie im Desktop Proofing Viewer zu öffnen {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Beim Testen von interaktiven Inhalten im Desktop Proofing Viewer können Sie jetzt Links konfigurieren, die auf einer neuen Registerkarte oder in einem neuen Fenster geöffnet werden, um sie im Desktop Proofing Viewer zu öffnen, damit Sie mit dem Testen fortfahren können.

Im Viewer für die alte Prüfung konnten Links, die auf einer neuen Registerkarte oder in einem neuen Fenster geöffnet wurden, im Testversand-Viewer nicht überprüft werden.

Weitere Informationen finden Sie unter [Konfigurieren der Testversand-Viewer-Einstellungen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Präsenzindikator im Testversand-Viewer {#presence-indicator-in-the-proofing-viewer}

Wenn Sie nun einen Testversand im Web Proofing Viewer oder Desktop Proofing Viewer überprüfen, können Sie den Avatar jedes Benutzers anzeigen, der den Testversand gerade anzeigt, wird in der rechten oberen Ecke des Testversand-Viewers angezeigt.

Weitere Informationen finden Sie unter [Testversand gleichzeitig mit mehreren Prüfern überprüfen](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtern von Kommentaren zum Anzeigen einer einzelnen Seite für interaktive URL-Testsendungen im Desktop-Testversand-Viewer {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Beim Überprüfen einer URL in einem interaktiven Testversand im Desktop Proofing Viewer können Sie nun Kommentare filtern, um Kommentare anzuzeigen, die nur auf der aktuellen Seite erstellt wurden. 

Vor dieser Änderung war diese Option nur für statische Testsendungen verfügbar.

Weitere Informationen finden Sie im Artikel .

### Desktop Proofing Viewer für statische und Videoinhalte {#desktop-proofing-viewer-for-static-and-video-content}

Der Desktop Proofing Viewer unterstützt jetzt statische und Videoinhalte.

Zuvor wurden nur interaktive Inhalte unterstützt.

Informationen zum Konfigurieren von statischen und Video-Testsendungen, die im Desktop Proofing Viewer geöffnet werden sollen, finden Sie unter [Konfigurieren von Testversand-Viewer-Einstellungen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Weitere Informationen zum Desktop-Proofing-Viewer finden Sie unter [Überprüfen von Testsendungen im Desktop-Proofing-Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Hinzufügen benutzerdefinierter Geräte zu Ihrem System {#add-custom-devices-to-your-system}

Sie können Ihrem System jetzt alle benutzerdefinierten Geräte hinzufügen, sodass Benutzer interaktive Inhalte überprüfen und simulieren können, wie sie auf einem bestimmten Gerät angezeigt werden, wenn sie einen Testversand im Desktop Proofing Viewer überprüfen.

Vor dieser Änderung konnten Benutzer nur aus einer Liste von standardmäßigen, vorkonfigurierten Geräten auswählen.

Informationen zum Hinzufügen benutzerdefinierter Geräte finden Sie unter

Informationen dazu, wie Benutzer beim Überprüfen interaktiver Inhalte Geräte auswählen können, finden Sie unter [Ändern der interaktiven Testversandauflösung im Testversand-Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Verbesserungen bei der Überprüfung in Workfront {#proofing-enhancements-in-workfront}

* [Freigeben des Testversand-Links direkt über Workfront](#share-the-proof-link-directly-from-workfront)
* [Bericht über zusätzliche Testdaten in Workfront](#report-on-additional-proofing-data-in-workfront)
* [Historische Daten für Testversandgenehmigungen in Workfront anzeigen](#view-historical-data-for-proof-approvals-in-workfront)

### Direktes Freigeben des Testlinks über Workfront {#share-the-proof-link-directly-from-workfront}

Jetzt können Sie einen Link für einen Testversand in Workfront generieren und ihn direkt über Workfront freigeben. Alternativ können Sie die URL kopieren und mithilfe einer alternativen Methode verteilen.

Vor dieser Änderung konnten Sie den Testversand-Link nur in Workfront kopieren und mithilfe einer alternativen Methode verteilen.

Weitere Informationen finden Sie unter [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) im Artikel [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) .

>[!NOTE]
>
>Der aktuell verfügbare Einbettungslink wird in einer zukünftigen Version entfernt. Der Einbettungslink kann weiterhin über die Workfront-API aufgerufen werden.

### Bericht zu zusätzlichen Testdaten in Workfront {#report-on-additional-proofing-data-in-workfront}

In Berichten, die das Objekt &quot;Dokumentversion&quot;enthalten (z. B. den Bericht &quot;Dokumentversion&quot;und den Bericht &quot;Testversandvalidierung&quot;), stehen nun mehrere Felder zur Verfügung, mit denen Sie zusätzliche Prüfinformationen anzeigen können.

* Korrekturabzugfrist

  Zeigt den Wochentag, das Datum, die Uhrzeit und das Jahr des Testversands an.

* Korrekturabzug-Entscheidung

  Zeigt den Entscheidungsstatus des Testversands an (ausstehend, erforderliche oder genehmigte Änderungen).

* Name des Korrekturabzugs

  Zeigt den Namen des Testversands an.

* Korrekturabzugseiten

  Zeigt die Anzahl der Seiten an, die im Testversand enthalten sind.

* Korrekturabzugverlauf

  Zeigt den Fortschrittsstatus des Testversands an (Gesendet, Geöffnet, Kommentar, Entscheidungsfindung).

Weitere Informationen zu den einzelnen Feldern finden Sie unter  [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Historische Daten für Testversandgenehmigungen in Workfront anzeigen {#view-historical-data-for-proof-approvals-in-workfront}

Im Validierungsbericht können Sie ein Feld hinzufügen, in dem Sie Validierungsentscheidungen für nicht mehr aktive Testsendungen anzeigen können. Fügen Sie dazu das Feld Entscheidung des Genehmigers zu Ihrem Bericht hinzu.

Vor dieser Änderung konnte die Entscheidung nach einer Entscheidung über einen Testversand nicht mehr in einem Workfront-Bericht angezeigt werden.

Weitere Informationen finden Sie unter  [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Verbesserungen bei der Überprüfung in Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Erstellen einer neuen Version eines Testversands direkt über den Testversand-Viewer (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Neuer Link &quot;Testdetails&quot;im Testversand-Viewer und im Desktop Proofing Viewer (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Erstellen einer neuen Version eines Testversands direkt über den Testversand-Viewer (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Beim Testen in Workfront Proof können Sie jetzt direkt aus dem neuen Testversand-Viewer und dem Desktop Proofing-Viewer eine neue Testversion erstellen.

Zuvor war diese Option nur im alten Flash-Viewer verfügbar.

Weitere Informationen finden Sie unter [Kopieren von Testsendungen in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) im Artikel  [Kopieren von Testsendungen in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Neuer Link &quot;Testdetails&quot;im Testversand-Viewer und im Desktop Proofing Viewer (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Beim Anzeigen eines Testversands im Testversand-Viewer können Workfront Proof-Benutzer jetzt schnell zur Seite mit den Testversanddetails in Workfront Proof wechseln.

Weitere Informationen finden Sie unter &quot;Anzeigen von Testversanddetails&quot;.
