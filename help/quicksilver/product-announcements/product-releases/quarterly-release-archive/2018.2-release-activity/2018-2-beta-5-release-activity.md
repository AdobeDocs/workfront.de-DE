---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 5 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 5 Version 2018.2 verfügbar waren. Die Funktion ist ab dem 1. Juni 2018 in der Vorschau-Umgebung verfügbar. Die mit Beta 5 veröffentlichten Proofing-Verbesserungen sind ab Montag, dem 4. Juni, in der Vorschau-Umgebung verfügbar. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

# Versionsaktivität von Beta 5 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 5 Version 2018.2 verfügbar waren. Die Funktion ist ab dem 1. Juni 2018 in der Vorschau-Umgebung verfügbar. Die mit Beta 5 veröffentlichten Proofing-Verbesserungen sind ab Montag, dem 4. Juni, in der Vorschau-Umgebung verfügbar. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.2 finden Sie unter  Übersicht über die Versionsaktivität [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta-Version 5 von 2018.2 enthält die Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Anzeigen von benutzerausgelösten Änderungen mit Auditprotokollen](#view-user-triggered-changes-with-audit-logs)
* [Anzeigen von Lizenzinformationen als Gruppenadministrator](#view-license-information-as-a-group-administrator)

**Für alle Benutzer**

* [Kalenderansicht im Bereich „Startseite“](#calendar-view-in-the-home-area)
* [Zusätzliche Aktualisierungen der Arbeitsliste (linker Bereich) auf der Startseite](#additional-updates-to-the-work-list-left-panel-in-home)
* [Konfigurieren von Aufgabenrollenbeschränkungen für die automatisierte Ressourcenplanung](#configure-job-role-limits-for-automated-resource-scheduling)
* [Verbesserungen der Projekt- und Rollenansicht im Ressourcenplaner](#project-and-role-view-improvements-in-the-resource-planner)
* [Spaltenbreiten für Projektlisten ändern](#resize-column-widths-for-project-lists)
* [Symbolunterstützung für die neuen Projektlisten](#icon-support-for-the-new-project-lists)
* [&#x200B; Feld „Große Miniaturansicht“ in Dokumentansichten hinzufügen](#add-large-thumbnail-field-in-document-views)
* [Excel-Exportbeschränkung erhöhen](#increase-excel-export-limit)
* [Schnellfilter für Projektlisten](#quick-filters-for-project-lists)
* [Referenzieren von Problemsammlungen in Projekt- und Aufgabenberichten](#reference-issue-collections-in-project-and-task-reports)
* [Neues, robusteres Versionsmenü beim Hinzufügen neuer Dokumentversionen in Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Verbesserungen bei Mobilgeräten in der Android Beta Mobile App](#mobile-improvements-in-the-android-beta-mobile-app)
* [Verbesserungen bei der Korrekturabzugsanzeige (Workfront und Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Proofing-Verbesserungen in Workfront](#proofing-enhancements-in-workfront)
* [Proofing-Verbesserungen in Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Kalenderansicht im Home-Bereich {#calendar-view-in-the-home-area}

Jetzt können Sie Ihre persönlichen Arbeitsaufgaben und -pläne mithilfe der Workfront-Startseiten-Kalenderansicht verwalten. Die Startseiten -Kalenderansicht bietet Ihnen folgende Möglichkeiten:

* Legen Sie einen eigenen Zeitplan für die Ausführung der Ihnen zugewiesenen Workfront-Aufgaben fest
* Schnelle Anzeige der Aufgaben, die fällig oder überfällig sind
* Anzeigen der insgesamt zugewiesenen Stunden einer Woche
* Aktualisierungen an den Ihnen zugewiesenen Aufgaben vornehmen

Wenn Sie einen Kalender in Outlook verwenden, können Sie Ihren Kalender integrieren, um Ihre Outlook-Ereignisse in Ihrer Startseiten-Kalenderansicht anzuzeigen.

## Zusätzliche Aktualisierungen der Arbeitsliste (linker Bereich) auf der Startseite {#additional-updates-to-the-work-list-left-panel-in-home}

Die folgenden Verbesserungen sind jetzt für die Arbeitsliste im Bereich Startseite verfügbar:

* Die Anzahl der abgeschlossenen Elemente wird jetzt im Dropdown-Menü Filter neben der Option Abgeschlossen in Klammern angezeigt.

  Zuvor wurde die Anzahl der abgeschlossenen Elemente nicht im Menü Filter angezeigt. 

* Abgeschlossene Elemente werden für die vorherigen 2 Wochen angezeigt.

  Zuvor wurden abgeschlossene Elemente für die letzten 3 Monate angezeigt.

  Weitere Informationen zum Anzeigen abgeschlossener Arbeiten im Bereich der Startseite finden Sie unter [Elemente in der Arbeitsliste im Bereich der Startseite anzeigen](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) im Artikel [Elemente in der Arbeitsliste im Bereich der Startseite anzeigen](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Fügen Sie die Felder Dauer und Zuweisungen hinzu, die angezeigt werden sollen, wenn Elemente im Bereich Startseite ausgewählt werden.

  Zuvor war das Feld „Arbeitsaufträge“ standardmäßig verfügbar; wenn es jedoch gelöscht wurde, konnte es nicht erneut hinzugefügt werden. Das Feld Dauer konnte zuvor nicht hinzugefügt werden.

  Informationen zum Hinzufügen von Feldern zum Bereich der Startseite finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

Weitere Informationen zur Verwendung des Bereichs „Startseite“ finden Sie unter [Verwenden des Bereichs „Startseite](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Anzeigen von benutzerausgelösten Änderungen mit Auditprotokollen {#view-user-triggered-changes-with-audit-logs}

Wir haben die folgenden Auditprotokolle für Workfront-Administratoren erstellt, um benutzerausgelöste Änderungen zu verfolgen:

* User Audit Log
* Zugriffsebene - Auditprotokoll
* Gruppen-Auditprotokolle
* Login-Prüfprotokolle

Zuvor gab es keine Möglichkeit, Änderungen innerhalb des Systems zu verfolgen.

Weitere Informationen finden Sie unter [Anzeigen und Exportieren von Auditprotokollen](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Anzeigen von Lizenzinformationen als Gruppenadministrator {#view-license-information-as-a-group-administrator}

Wir haben eine schreibgeschützte Lizenzseite für Gruppenadministratoren erstellt, um die Lizenzanzahl für die von ihnen verwalteten Gruppen anzuzeigen.

Vor dieser Änderung konnten Gruppenadministratoren keine Lizenzinformationen anzeigen.

Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Konfigurieren von Aufgabenrollenbeschränkungen für die automatisierte Ressourcenplanung {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

In den Einstellungen für die automatisierte Ressourcenplanung können Sie jetzt einem Aufgabengebiet ein Limit zuweisen. Auf diese Weise können Sie die Anzahl der Ressourcen steuern, denen dieselbe Rolle zugewiesen wird.

Zuvor konnten Sie nicht angeben, wie vielen Benutzern in einem bestimmten Aufgabengebiet Arbeit zugewiesen werden konnte.

Weitere Informationen finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## Verbesserungen der Projekt- und Rollenansicht im Ressourcenplaner {#project-and-role-view-improvements-in-the-resource-planner}

Die Projekt- und Rollenansichten des Ressourcenplaners enthalten jetzt die folgenden Verbesserungen:

* Verbesserte Filter, die Informationen aus der gesamten Datenbank abrufen, anstatt nur die Informationen auf dem Bildschirm.
* Vollbildmodus.
* Die Leistung ist jetzt schneller und effizienter.

   * Neue Beschränkungen für die Anzahl der Projekte, Rollen und Benutzenden, die Sie anzeigen können.
   * Verzögertes Laden, für ein schnelleres Laden von Projekten und Rollen.

* Schnellzugriff auf Projekte und Benutzer direkt über den Ressourcenplaner.
* Schnellere Drag &amp; Drop-Funktion in der Projektansicht, um Ihre Projekte zu priorisieren.

Im Vorfeld dieser Verbesserungen haben Sie berichtet, dass der Ressourcenplaner nur langsam geladen wurde und dass bei den angezeigten Daten Abweichungen festgestellt wurden. Mit diesen Verbesserungen sollten diese nun beseitigt werden.

Weitere Informationen und Informationen zu den neuen Beschränkungen für den Ressourcenplaner finden Sie unter [Anzeigebeschränkungen für den Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Spaltenbreiten für Projektlisten ändern {#resize-column-widths-for-project-lists}

Während wir an der Verbesserung der Funktionalität unserer Listen arbeiten, hatten wir die Möglichkeit vorübergehend deaktiviert, die Breite der Spalten in den folgenden Projektlisten zu ändern:

* Projekte in meinem Besitz
* Projekte, an denen ich mitwirke
* Alle Projekte

Mit dieser Version können wir nun die Größe der Spalten aller Projektlisten erneut ändern.

Wir haben zusätzliche Verbesserungen zu dieser Funktion hinzugefügt.

Wenn Sie jetzt den rechten Rahmen einer Spalte ziehen, um ihre Größe zu ändern, behält die benachbarte Spalte rechts ihre Größe bei, wodurch die Liste breiter wird, anstatt auch geändert zu werden. Außerdem können Sie den Rahmen einer Spalte nach rechts über die Rahmen der benachbarten Spalten hinaus ziehen.

Vor dieser Verbesserung würde die Größe der benachbarten Spalte rechts neben der angepassten Spalte proportional so geändert, dass sie auf den Bildschirm passt, und Sie könnten den Rahmen einer Spalte nicht über den rechten Rahmen der benachbarten Spalte ziehen.  

Informationen zur Größenanpassung der Spalten in Listen finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Um an unserem Beta-Testprogramm für die aktuellen Listennutzungsverbesserungen teilzunehmen, siehe [Neue Listenstudie.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=de) (Anmeldung erforderlich)

## Symbolunterstützung für die neuen Projektlisten {#icon-support-for-the-new-project-lists}

Während wir an der Verbesserung der Funktionalität unserer Listen arbeiten, hatten wir die Anzeige von Statussymbolen in den folgenden Projektlisten vorübergehend deaktiviert:

* Projekte in meinem Besitz
* Projekte, an denen ich mitwirke
* Alle Projekte

Mit dieser Version können Statussymbole wieder in Ihren Projektlisten für Projekte oder für andere Objekte in einer Projektliste angezeigt werden.

Informationen zum Arbeiten in Listen finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Feld „Große Miniaturansicht“ in Dokumentansichten hinzufügen {#add-large-thumbnail-field-in-document-views}

Wir fügen ein neues Feld namens Große Miniaturansicht zu einer Dokumentansicht in einer Liste oder einem Bericht hinzu. Bei Auswahl in einer Dokumentansicht zeigt dieses Feld eine 400 Pixel breite Miniaturansicht des Dokuments in einer Liste oder einem Bericht an.

Vor dieser Änderung konnten Sie das Feld Miniaturansicht nur einer Dokumentansicht hinzufügen, in der eine 33-66 Pixel breite Miniaturansicht des Dokuments angezeigt wird.

Informationen zu Feldern in Listen und Berichten finden Sie im [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Excel-Exportlimit erhöhen {#increase-excel-export-limit}

Wir haben das Limit für die Anzahl der Zeilen erhöht, die Sie in eine Excel-Datei exportieren können. Sie können jetzt Folgendes exportieren:

* 65.000 Zeilen in einer Excel-XLS-Datei
* 100.000 Zeilen in einer Excel-XLSX-Datei

Die neuen Beschränkungen gelten, wenn Sie Folgendes aus Workfront exportieren:

* Eine Liste oder ein Bericht über die Web-Oberfläche
* Liste oder Bericht mit der -API
* Geplanter und bereitgestellter Bericht

Vor dieser Verbesserung konnten Sie nur 50.000 Zeilen in eine Excel-Datei exportieren.

Informationen zum Exportieren von Daten aus Workfront finden Sie unter [Exportieren von Daten](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Schnellfilter für Projektlisten {#quick-filters-for-project-lists}

Sie können jetzt einen Schnellfilter auf Listen anwenden.

Mit einem Schnellfilter können Sie direkt zu den Elementen in Ihren großen Listen navigieren, die für Sie wichtig sind, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.

Derzeit sind Schnellfilter nur für die Projektlisten in den folgenden Unterregisterkarten verfügbar:

* Projekte, an denen ich mitwirke
* Projekte in meinem Besitz
* Alle Projekte

Informationen zu Schnellfiltern finden Sie im Abschnitt „Anwenden von Schnellfiltern auf Listen“ in [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Referenzieren von Anfragesammlungen in Projekt- und Aufgabenberichten {#reference-issue-collections-in-project-and-task-reports}

Sie können jetzt in einer Projekt- oder Aufgabenansicht und einem Filter auf eine Problemsammlung verweisen. Dies ist nur mit dem Textmodus beim Erstellen eines Berichts möglich.

Vor dieser Verbesserung konnten Sie nur auf eine Sammlung von Aufgaben in einer Projektansicht oder einem Filter verweisen.

Informationen zum Referenzieren einer Sammlung in einem Bericht finden Sie unter [Referenzieren von Sammlungen in einem Bericht](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Informationen zur Verwendung des Textmodus finden Sie unter  [Übersicht über häufige Verwendungen für den Textmodus](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>Im folgenden Video war der Beispiel-Textmodus für Problemsammlungen falsch. Der richtige Beispieltextmodus ist in &quot;[&#x200B; in einem Bericht“ &#x200B;](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Neues, robusteres Versionsmenü beim Hinzufügen neuer Dokumentversionen in Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Beim Hinzufügen neuer Versionen zu Dokumenten in Workfront enthält das Menü Neue Version nun zusätzliche Optionen und ist nun in allen Bereichen von Workfront konsistent, in denen Sie eine neue Version hinzufügen können.

Sie können eine neue Dokumentversion aus den folgenden Bereichen von Workfront hinzufügen:

* Aus dem Dropdown-Menü Mehr auf der Registerkarte Dokumente .
* Über das Menü Dokumentaktionen auf der Seite Dokumentdetails .
* Auf der Registerkarte Alle Versionen auf der Seite Dokumentdetails .

Vor dieser Änderung enthielt nur das Dropdown-Menü Mehr auf der Registerkarte Dokumente alle Optionen zum Hinzufügen einer neuen Version.

Die folgenden Optionen sind jetzt im Menü Neue Version für alle Bereiche verfügbar, in denen Sie eine neue Version hinzufügen können:

* Korrekturabzug
* Nur Dokument
* Verknüpfte Optionen (von Dropbox, von Google Drive usw.)
* Aus Zwischenablage einfügen (dies ist eine neue Option beim Hinzufügen von Versionen)

Weitere Informationen finden Sie unter [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem &#x200B;](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)) im Artikel [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Verbesserungen bei Mobilgeräten in der Android Beta Mobile App {#mobile-improvements-in-the-android-beta-mobile-app}

Kurz nach dem Tag dieser Version werden in der Android Beta-Version der Mobile App die folgenden Verbesserungen verfügbar sein:

* Wischen von Aktionen

  Sie können Aktivitäten wie Freiwillige ausführen, um eine Aufgabe zu bearbeiten, eine Aufgabe abzuschließen, eine Benachrichtigung als gesehen oder neu zu markieren, einen Kontakt anrufen oder einen Kontakt anrufen, indem Sie verschiedene Objekte in der Workfront-Mobile-App durchwischen.

  Die folgenden Bereiche wurden mit dieser Funktion verbessert:

   * Meine Arbeit und Startseite
   * Benachrichtigungen
   * Kontakte
   * Genehmigungen

* Neues Erscheinungsbild bei Anzeige der Registerkarte „Details“ eines Elements

  Die Benutzeroberfläche wurde beim Anzeigen eines Elements in der Android Beta-Version der Mobile App geändert, um die Bearbeitung, das Fertigstellen oder das Anhängen eines Dokuments zu vereinfachen.

* Neues Erlebnis bei der Zeitprotokollierung

  Die Protokollierung geht schneller und einfacher vonstatten als zuvor. Sie erhalten eine Schaltfläche für den Zugriff auf die Protokollierungszeit und eine optimierte Benutzeroberfläche für die Protokollierung von Stunden.

Mit dieser Version sind diese Verbesserungen nur für die Android Beta-Version der Workfront-Mobile-App verfügbar. Sie sind derzeit nicht für iOS verfügbar.

Weitere Informationen dazu, wie Sie sich als Betatester anmelden und die Android Beta-Version der Workfront-Mobile-App herunterladen, finden Sie unter .

## Verbesserungen bei der Proofing-Anzeige (Workfront und Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Seite Druckzusammenfassung wurde aktualisiert](#updated-print-summary-page)
* [Benutzer direkt über die Proofing-Anzeige zu einem Korrekturabzug hinzufügen](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Alle Markup-Tools im Proofing Viewer anzeigen](#display-all-markup-tools-in-the-proofing-viewer)
* [Konfigurieren von Standardsortierungsoptionen in der Proofing-Ansicht](#configure-default-sorting-options-in-the-proofing-viewer)
* [Anzeigen von Workfront-Dokumentgenehmigungen im Desktop Proofing Viewer](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Konfigurieren Sie Links, die neue Registerkarten und Fenster öffnen, um sie im Desktop Proofing Viewer zu öffnen](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Anzeige im Proofing Viewer](#presence-indicator-in-the-proofing-viewer)
* [Kommentare filtern, um eine einzelne Seite für interaktive URL-Korrekturabzüge im Desktop Proofing Viewer anzuzeigen](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Desktop Proofing Viewer für statische und Videoinhalte](#desktop-proofing-viewer-for-static-and-video-content)
* [Hinzufügen benutzerdefinierter Geräte zu Ihrem System](#add-custom-devices-to-your-system)

### Aktualisierte Seite Druckzusammenfassung {#updated-print-summary-page}

Die Seite Druckzusammenfassung wurde mit einem neuen Look-and-Feel und verbesserten Funktionen aktualisiert.

Weitere Informationen finden Sie unter [Drucken einer Zusammenfassung eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Hinzufügen von Benutzern zu einem Korrekturabzug direkt über die Proofing-Anzeige {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Jetzt können Sie Benutzer direkt über die Web Proofing Viewer und die Desktop Proofing Viewer zu einem Korrekturabzug hinzufügen. 

Zuvor konnten Sie keine einzelnen Benutzer zu einem Korrekturabzug hinzufügen. Stattdessen konnten Sie nur die öffentliche URL oder den Einbettungs-Code kopieren.

Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs durch Hinzufügen von Benutzern](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) im Artikel  [Freigeben eines Korrekturabzugs über die Korrekturabzugsanzeige](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Alle Markup-Tools im Proofing Viewer anzeigen {#display-all-markup-tools-in-the-proofing-viewer}

Sie können jetzt das Markup-Tool so konfigurieren, dass es immer angezeigt wird, anstatt in einem Menü, das Sie öffnen müssen. Dadurch kann schneller zwischen Tools gewechselt werden. Wenn die Markup-Tools auf diese Weise konfiguriert sind, werden sie horizontal oben im Web Proofing Viewer und Desktop Proofing Viewer angezeigt.

Zuvor waren Markup-Tools nur innerhalb eines Dropdown-Menüs verfügbar.

Weitere Informationen zum Konfigurieren dieser Markup-Einstellung finden Sie unter [Konfigurieren der Einstellungen für die Proofing-Anzeige](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Weitere Informationen zur Verwendung von Markup-Optionen bei der Überprüfung eines Korrekturabzugs finden Sie im Artikel .

### Konfigurieren von Standardsortierungsoptionen in der Proofing-Anzeige {#configure-default-sorting-options-in-the-proofing-viewer}

Wenn Sie jetzt die Sortieroption in der Kommentarliste in einem Korrekturabzug ändern, wird diese Option zur standardmäßigen Sortieroption, wenn Sie einen Korrekturabzug das nächste Mal in der Web-Korrekturabzugsansicht oder der Desktop-Korrekturabzugsansicht öffnen. 

Weitere Informationen finden Sie im Artikel .

### Anzeigen von Workfront-Dokumentgenehmigungen im Desktop Proofing Viewer {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Jetzt können Sie im Desktop Proofing Viewer eine Workfront-Dokumentgenehmigungsentscheidung treffen.

Zuvor war es Ihnen nur mit der Web Proofing Viewer möglich, eine Workfront-Dokumentgenehmigungsentscheidung zu treffen. 

Weitere Informationen finden Sie unter  [Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) im Artikel  [Treffen einer Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Konfigurieren Sie Links, die neue Registerkarten und Fenster öffnen, um sie im Desktop Proofing Viewer zu öffnen {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Beim Proofing interaktiver Inhalte im Desktop Proofing Viewer können Sie jetzt Links konfigurieren, die in einer neuen Registerkarte oder einem neuen Fenster geöffnet werden, um sie im Desktop Proofing Viewer zu öffnen, damit Sie mit dem Proofing fortfahren können.

Im alten Proofing Viewer konnten Links, die in einer neuen Registerkarte oder einem neuen Fenster geöffnet wurden, nicht in der Proofing Viewer überprüft werden.

Weitere Informationen finden Sie unter [Konfigurieren der Einstellungen für Proofing Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Anzeige des Vorhandenseins im Proofing Viewer {#presence-indicator-in-the-proofing-viewer}

Beim Überprüfen eines Korrekturabzugs im Web Proofing Viewer oder Desktop Proofing Viewer können Sie nun den Avatar jedes Benutzers anzeigen, der den Korrekturabzug derzeit betrachtet, der in der oberen rechten Ecke der Proofing Viewer angezeigt wird.

Weitere Informationen finden Sie unter [Testversand gleichzeitig mit mehreren Validierungsverantwortlichen &#x200B;](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filterkommentare, um im Desktop Proofing Viewer eine einzelne Seite für interaktive URL-Korrekturabzüge anzuzeigen {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Beim Überprüfen einer URL in einem interaktiven Korrekturabzug im Desktop Proofing Viewer können Sie jetzt Kommentare filtern, um Kommentare anzuzeigen, die nur auf der aktuellen Seite erstellt wurden. 

Vor dieser Änderung war diese Option nur für statische Korrekturabzüge verfügbar.

Weitere Informationen finden Sie im Artikel .

### Desktop Proofing Viewer für statische und Videoinhalte {#desktop-proofing-viewer-for-static-and-video-content}

Der Desktop Proofing Viewer unterstützt jetzt statische und Videoinhalte.

Zuvor wurden nur interaktive Inhalte unterstützt.

Informationen zum Konfigurieren von statischen Korrekturabzügen und von Korrekturabzügen zum Öffnen im Desktop Proofing Viewer finden Sie [Konfigurieren der Einstellungen für die Korrekturabzugsansicht](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Weitere Informationen zum Desktop Proofing Viewer finden Sie unter [Überprüfen von Korrekturabzügen im Desktop Proofing Viewer.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Hinzufügen benutzerdefinierter Geräte zu Ihrem System {#add-custom-devices-to-your-system}

Sie können Ihrem System jetzt beliebige benutzerdefinierte Geräte hinzufügen, damit Benutzer interaktive Inhalte überprüfen und simulieren können, wie sie auf einem bestimmten Gerät angezeigt werden, wenn sie einen Korrekturabzug im Desktop Proofing Viewer prüfen.

Vor dieser Änderung konnten Benutzer nur aus einer Liste von vorkonfigurierten Standardgeräten auswählen.

Informationen zum Hinzufügen benutzerdefinierter Geräte finden Sie unter in

Informationen dazu, wie Benutzer bei der Überprüfung interaktiver Inhalte Geräte auswählen können, finden Sie unter [Ändern der interaktiven Korrekturabzugsauflösung im Proofing Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Proofing-Verbesserungen in Workfront {#proofing-enhancements-in-workfront}

* [Proof-Link direkt in Workfront freigeben](#share-the-proof-link-directly-from-workfront)
* [Bericht zu zusätzlichen Proofing-Daten in Workfront](#report-on-additional-proofing-data-in-workfront)
* [Anzeigen historischer Daten für Korrekturabzugsgenehmigungen in Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Freigeben des Korrekturabzugs-Links direkt in Workfront {#share-the-proof-link-directly-from-workfront}

Jetzt können Sie in Workfront einen Link für einen Korrekturabzug generieren und ihn direkt in Workfront freigeben. Alternativ können Sie die URL kopieren und mithilfe einer alternativen Methode verteilen.

Vor dieser Änderung konnten Sie den Link für den Korrekturabzug nur in Workfront kopieren und mithilfe einer alternativen Methode verteilen.

Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) im Artikel [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>Der derzeit verfügbare Einbettungs-Link wird in einer zukünftigen Version entfernt. Auf den Einbettungs-Link kann weiterhin über die Workfront-API zugegriffen werden.

### Bericht zu zusätzlichen Proofing-Daten in Workfront {#report-on-additional-proofing-data-in-workfront}

In Berichten, die das Objekt Dokumentversion enthalten (z. B. Berichte zur Dokumentversion und zur Korrekturabzugsgenehmigung), sind jetzt mehrere Felder verfügbar, mit denen Sie zusätzliche Korrekturabzugsinformationen anzeigen können.

* Korrekturabzugfrist

  Zeigt den Wochentag, das Datum, die Tageszeit und das Jahr der Testversandfrist an.

* Korrekturabzug-Entscheidung

  Zeigt den Entscheidungsstatus des Korrekturabzugs an (ausstehend, Änderungen erforderlich oder genehmigt).

* Name des Korrekturabzugs

  Zeigt den Namen des Korrekturabzugs an.

* Korrekturabzugseiten

  Zeigt die Anzahl der im Korrekturabzug enthaltenen Seiten an.

* Korrekturabzugverlauf

  Zeigt den Fortschrittsstatus des Testversands an (gesendet, geöffnet, kommentiert, Entscheidung getroffen).

Weitere Informationen zu den einzelnen Feldern finden Sie unter  [Glossar der Terminologie von Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Anzeigen historischer Daten für Korrekturabzugsgenehmigungen in Workfront {#view-historical-data-for-proof-approvals-in-workfront}

Dem Bericht zu Korrekturabzugsgenehmigungen können Sie ein Feld hinzufügen, in dem Sie Korrekturabzugsgenehmigungsentscheidungen für Korrekturabzüge anzeigen können, die nicht mehr aktiv sind. Sie können dies tun, indem Sie das Feld Genehmigende Entscheidung zu Ihrem Bericht hinzufügen.

Vor dieser Änderung konnte die Entscheidung, nachdem eine Entscheidung über einen Korrekturabzug getroffen wurde, nicht mehr in einem Workfront-Bericht angezeigt werden.

Weitere Informationen finden Sie unter  [Glossar der Terminologie von Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Proofing-Verbesserungen in Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Erstellen einer neuen Version eines Korrekturabzugs direkt über die Proofing-Anzeige (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Neuer Link „Korrekturabzugsdetails“ im Proofing Viewer und Desktop Proofing Viewer (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Erstellen einer neuen Version eines Korrekturabzugs direkt über die Proofing-Anzeige (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Sie können jetzt beim Proofing in Workfront Proof direkt über die neue Proofing-Anzeige und die Desktop-Proofing-Anzeige eine neue Version eines Korrekturabzugs erstellen.

Zuvor war diese Option nur in Legacy Flash Viewer verfügbar.

Weitere Informationen finden Sie unter [&#x200B; von Testsendungen in Workfront Proof &#x200B;](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) Artikel  [Testsendungen in Workfront Proof kopieren](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Neuer Link „Korrekturabzugsdetails“ im Proofing Viewer und Desktop Proofing Viewer (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Wenn Sie einen Korrekturabzug im Proofing Viewer anzeigen, können Workfront Proof-Benutzende jetzt schnell zur Detailseite des Korrekturabzugs in Workfront Proof gehen.

Weitere Informationen finden Sie unter „Anzeigen von Korrekturabzugsdetails“.
