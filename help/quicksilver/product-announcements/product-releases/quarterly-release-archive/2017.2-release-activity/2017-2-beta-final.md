---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta endgültig 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2017.2 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 28. Juni 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird am 26. Juli 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# Beta endgültig 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2017.2 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 28. Juni 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird am 26. Juli 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die in Version 2017.2 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die endgültige Version 2017.2 von Beta enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren:**

* [Bestimmen der Verfügbarkeit des HTML5-Video-Testversand-Viewers (ProofHQ und Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Unterstützung von SHA-256-Zertifikaten für SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [ Type-Ahead für die Zuordnung von Attributen](#type-ahead-for-mapping-attributes)
* [API-Verbesserung: Zugriff auf Benutzerzuordnungen](#api-enhancement-access-user-allocations)

**Für alle Benutzer:**

* [Ressourcenplaner](#resource-planner)
* [Neuer Planungsbereich in einem Projekt (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Ressourcenplanung: Zeigt standardmäßig weniger Elemente an](#resource-scheduling-show-fewer-items-by-default)
* [Ressourcenplanung: Anzeigen von Dropindikatoren und Überzuordnungen beim Ziehen von Aufgaben und Problemen](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Ressourcenplanung: Benutzerzuweisungen werden nicht mehr auf die nächste halbe Stunde gerundet](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportieren des Nutzungsberichts in TSV- und PDF-Formate](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Beta Final 2017.2](#user-calendar-enhancements-in-the-my-work-area%22)
* [Beta Final 2017.2](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Testversandentscheidung wird im Arbeitsbereich (Workfront) angezeigt](#proof-decision-displays-in-the-my-work-area-workfront)
* [Anzeigen von Rich-Media-Testsendungen in Vorgabeauflösungen (ProofHQ und Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Anzeigen der URL zu Unterseiten in Kommentaren zu Rich-Media-Testsendungen (ProofHQ und Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Erstellen benutzerdefinierter Ansichten basierend auf vorhandenen Standardansichten (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtern des Berichtsbereichs (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Mindest- und Höchstwerte in Berichten anzeigen (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [In-App-Benachrichtigung für die Validierung des Testversands](#in-app-notification-for-proof-approval)
* [Mobile Verbesserungen](#mobile-improvements)
* [ Schrägstrich zum Filtern von Anweisungen für Feldwerte mit Kommas hinzugefügt](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Mehrere Abrechnungsraten](#multiple-billing-rates)
* [Neues Ressourcenbudget - Haushaltsstundenfeld ](#new-resource-budgeted-hour-field)
* [Benutzerauftragsrolle im Bereich &quot;Zugeordnet&quot;auf der Detailseite für Aufgaben und Probleme anzeigen](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Neuer Planungsbereich in einem Projekt (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

Der Bereich &quot;Planung&quot;in einem Projekt (ehemals &quot;Team Builder&quot;) wurde mit einer aktualisierten und intuitiveren Benutzeroberfläche umgestaltet. Die neue Planungsfunktion entspricht nun eher der in anderen Bereichen von Workfront derzeit verfügbaren Funktion für die Ressourcenplanung.

Zu den Verbesserungen gehören:

* Aktuelle Ressourcenzuweisungen für Mitglieder des Projektteams anzeigen, sodass Sie bei der Zuweisung fundiertere Entscheidungen treffen können
* Visuelle Darstellung der Aufgabendauer in der Zeitleiste der Planung
* Filtern der in der Planung angezeigten Informationen
* Einfaches Hinzufügen und Entfernen von Benutzern aus dem Projektteam direkt aus der Zeitleiste für die Planung

Die folgende Funktion ist in anderen Bereichen des Tools verfügbar, wenn Ressourcen geplant werden, aber nicht verfügbar, wenn Ressourcen im Bereich Teamplanung geplant werden:

* Konfigurieren von übergeordneten Aufgaben für die Anzeige in der Planung
* Konfigurieren Sie die Projektnamen, die in der Zeitplanungs-Timeline angezeigt werden sollen
* Ändern von Benutzerzuweisungen mit dem Swap-Tool
* Filtern nach Portfolio, Programmen und Projekten

Weitere Informationen zu den verfügbaren Funktionen im Bereich &quot;Teamplanung&quot;finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Ressourcenplanung: Standardmäßig weniger Elemente anzeigen {#resource-scheduling-show-fewer-items-by-default}

Standardmäßig werden für einen bestimmten Benutzer maximal 10 Arbeitselemente pro Tag in der Planung angezeigt. Sie können die Liste erweitern, um alle Aufgaben und Probleme anzuzeigen, die diesem Benutzer derzeit zugewiesen sind.

Auf diese Weise können Sie die Planung einfacher durchsuchen, wenn Benutzern viele Aufgaben und Probleme zugewiesen werden.

Vor dieser Änderung wurden alle Aufgaben und Probleme für alle Benutzer angezeigt.

Weitere Informationen zum Zuweisen von Aufgaben und Problemen zu Benutzern in der Planung finden Sie unter &quot;Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen&quot;.

## Ressourcenplanung: Anzeigen von Dropindikatoren und Überzuordnungen beim Ziehen von Aufgaben und Problemen {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Beim Zuweisen einer Aufgabe oder eines Problems zu einem Benutzer in der Planung per Drag &amp; Drop werden nun die folgenden Informationen angezeigt, bevor die Aufgabe oder das Problem freigegeben und die Zuweisung abgeschlossen wird:

* In der Zeile des Benutzers wird ein Dropindikator angezeigt. Auf diese Weise können Sie sehen, wo ein Element zugewiesen wird, bevor Sie die Zuweisung vornehmen.
* Wenn die Benutzerzuordnung in der Planung aktiviert ist, werden die roten Zuordnungsindikatoren angezeigt, wenn der Benutzer nach Abschluss der Zuweisung übergeordnet wird.

Vor diesen Änderungen wurden keine Informationen angezeigt, bevor die Aufgabe oder das Problem freigegeben wurde.

Weitere Informationen zum Zuweisen von Aufgaben und Problemen zu Benutzern in der Planung finden Sie unter &quot;Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen&quot;.

## Ressourcenplanung: Benutzerzuweisungen werden nicht mehr auf die nächste halbe Stunde gerundet {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Wenn mehrere Benutzer einer Aufgabe oder einem Problem zugewiesen sind oder wenn eine Aufgabe oder ein Problem mehrere Tage umfasst, versucht Workfront, geplante Stunden gleichmäßig auf die zugewiesenen Benutzer und Tage zu verteilen. Stunden werden standardmäßig auf das nächste Hundertstel gerundet (z. B. 1,33).

Bisher wurden bei manuellen Änderungen der verteilten Stunden Stunden Stunden angepasst und auf die nächste halbe Stunde gerundet (beispielsweise wird 1,33 auf 1,5 gerundet).

Jetzt werden die Stunden nicht mehr angepasst und auf die nächste halbe Stunde gerundet (z. B. bleibt 1,33 bei 1,33).

## API-Verbesserung: Zugriff auf Benutzerzuordnungen {#api-enhancement-access-user-allocations}

Sie können jetzt über die Workfront-API auf die Schattierung der Benutzerzuordnung zugreifen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportieren des Nutzungsberichts in die Formate TSV und PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Zusätzlich zum XLSX-Format können Sie jetzt den Utilization-Bericht für ein Projekt in die Formate TSV und PDF exportieren.

Vor dieser Änderung konnten Sie den Nutzungsbericht nur im XLSX-Format exportieren.

Weitere Informationen zum Exportieren des Nutzungsprotokolls finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Testversandentscheidung wird im Arbeitsbereich (Workfront) angezeigt {#proof-decision-displays-in-the-my-work-area-workfront}

Wenn Sie nun im Tab Meine Genehmigungen in Ihrem Arbeitsbereich Testversandgenehmigungen anzeigen, wird die Testversandentscheidung in Ihrem Arbeitsbereich angezeigt und bleibt erhalten, bis Sie in Workfront auf die neue Schaltfläche Aktualisieren klicken oder die Browserseite das nächste Mal aktualisieren.

Vor dieser Änderung gab es keinen Hinweis darauf, dass bereits eine Entscheidung über den Testversand getroffen wurde und der Testversand auf dem Tab Meine Validierungen verbleibte, bis Sie den Browser aktualisiert haben.

Weitere Informationen finden Sie unter [Arbeiten genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Arbeiten genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Anzeigen von Rich-Media-Testsendungen in Vorgabeauflösungen (ProofHQ und Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

In einer früheren Version der Vorschau-Umgebung haben wir die Möglichkeit eingeführt, die Auflösung von Rich-Media-Testsendungen anzupassen, indem entweder eine benutzerdefinierte Auflösung angegeben oder das Bild auf die gewünschte Auflösung gezogen wurde.

Sie können jetzt aus den voreingestellten Auflösungsoptionen für verschiedene Smartphones, Tablets, Notebooks und Desktops auswählen.

Weitere Informationen finden Sie unter &quot;Anzeigen einer Vorgabenauflösung&quot;in [Ändern der interaktiven Testversandauflösung im Testversand-Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Anzeigen der URL zu Unterseiten in Kommentaren zu Rich-Media-Testsendungen (ProofHQ und Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Diese Funktion ist derzeit in der Produktionsumgebung verfügbar.

Wenn Sie nun einen Kommentar zu einer Unterseite in einem Rich Media-Testversand abgeben, wird die URL zur Unterseite im Kommentar angezeigt.

Vor dieser Änderung war nicht klar, auf welche Unterseite der Kommentar Bezug nahm.

Weitere Informationen finden Sie unter

## Bestimmen der Verfügbarkeit des HTML5-Video-Testversand-Viewers (ProofHQ und Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Als Workfront-Administrator in ProofHQ können Sie festlegen, ob Benutzer in Ihrem Unternehmen Zugriff auf den neuen HTML5-Testversand-Viewer für Videosendungen haben.

Weitere Informationen zum Konfigurieren dieser Option in Workfront finden Sie unter .

## Erstellen benutzerdefinierter Ansichten basierend auf vorhandenen Standardansichten (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Jetzt können Sie eine benutzerdefinierte Ansicht basierend auf einer Standardansicht erstellen. Spalten-, Sortierungs- und Filteroptionen aus der Standardansicht sind standardmäßig in der neuen Ansicht enthalten.

Vor dieser Änderung mussten Sie die Ansicht von Grund auf neu erstellen, um eine benutzerdefinierte Ansicht zu erstellen. 

Weitere Informationen finden Sie unter [Erstellen einer benutzerdefinierten Ansicht](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [Erstellen und Verwalten benutzerdefinierter Ansichten im Workfront Proof-Testversand](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtern des Berichtsbereichs (ProofHQ) {#filter-the-reporting-area-proofhq}

Standardmäßig enthalten die auf der Registerkarte Berichte angezeigten Daten alle Informationen aus Ihrem ProofHQ-System. Sie können jetzt Filter verwenden, um nur Informationen anzuzeigen, die für Ihre Anforderungen relevant sind. 

Weitere Informationen finden Sie unter [Filtern von Berichten](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) in  [Ausführen von Berichten in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Anzeigen von Mindest- und Höchstwerten in Berichten (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Sie können jetzt konfigurieren, ob Mindest- und Höchstwerte im Diagramm angezeigt werden, wenn Sie Berichte anzeigen.

Weitere Informationen finden Sie unter [Anzeigen von Berichten](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in  [Ausführen von Berichten in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Unterstützung von SHA-256-Zertifikaten für SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Bei der Konfiguration von Workfront für SSO mit SAML 2.0 unterstützen wir jetzt den Secure Hash Algorithm 256 (SHA-256). Vor dieser Version haben wir nur Secure Hash Algorithm 1 (SHA-1) unterstützt.

Weitere Informationen zum Konfigurieren von Workfront mit SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Typübersicht für Zuordnungsattribute {#type-ahead-for-mapping-attributes}

Der Feldtyp &quot;Standardwert&quot;im Dialogfeld &quot;Attributzuordnung&quot;wurde in ein Feld &quot;type-ahead&quot;aktualisiert. Vor dieser Änderung war der Typ des Felds Standardwert eine Dropdown-Liste.

Diese Änderung gilt für die folgenden SSO-Protokolle:

* Active Directory
* LDAP
* SAML 2,0

SAML 1.1 unterstützt keine Attributzuordnung.

## Mobile Verbesserungen {#mobile-improvements}

>[!NOTE]
>
> Die Mobile App wird unabhängig von der Workfront-Hauptanwendung veröffentlicht. Die in diesem Abschnitt beschriebenen Funktionen werden Anfang August veröffentlicht.

Die folgenden Funktionen werden in den mobilen Apps für die Plattformen Android und iOS hinzugefügt:

* Anforderungen von der mobilen App übermitteln
* Datenblatt Neuer Eintrag in der Mobile App
* Benutzerdefinierte Formularbearbeitung über die Mobile App
* Validierungsanfragen für mobile Apps

Für einige dieser Funktionen wird es ein öffentliches Betaprogramm für die Android-Plattform geben.

Weitere Informationen zum kommenden Betaprogramm für Mobilgeräte finden Sie im  Seite [&quot;Betas&quot;](https://support.workfront.com/hc/en-us/sections/115000743248).

Weitere Informationen zur Verwendung der mobilen Workfront-App finden Sie unter .  

## Schrägstrich zum Filtern von Anweisungen für Feldwerte mit Kommas hinzugefügt {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Wenn Sie einen Filter im Textmodus erstellen und nach Feldwerten filtern, die Kommas enthalten, müssen Sie vor den Kommas, die die Werte trennen, einen Schrägstrich (&quot;/&quot;) hinzufügen, um sicherzustellen, dass der Wert als eine Filteroption gelesen wird. Dies gilt nur für die folgenden Feldtypen:

* Dropdowns
* Optionsschaltflächen
* Kontrollkästchen

Vor dieser Änderung konnten Sie nicht nach Feldern filtern, die Optionen mit Kommas enthielten.

Weitere Informationen zu dieser Änderung finden Sie unter [Filterübersicht](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Verschiedene Abrechnungsraten {#multiple-billing-rates}

Sie können jetzt mehrere Außerkraftsetzungen der Abrechnungsrate für dieselbe Auftragsrolle auf Projektebene hinzufügen. Mit dieser neuen Funktion können Sie Datumsbereiche für jede Außerkraftsetzung der Abrechnungsrate definieren. Während des angegebenen Datumsbereichs wird eine andere Abrechnungsrate auf die Auftragsrolle angewendet, die Aufgaben in einem Projekt zugewiesen ist. Die Abrechnungsraten werden mit den Stunden multipliziert, die dem Projekt zur Berechnung des Umsatzes berechnet werden. Der innerhalb des Datumsbereichs einer Abrechnungsrate berechnete Umsatz bleibt mit dieser Rate gesperrt und wird nicht mit den Raten der Auftragsrollen bei der Projektaktualisierung aktualisiert. Im Falle des tatsächlichen Umsatzes werden keine Stunden neu berechnet, die vor dem Außerkraftsetzen des Abrechnungskurses protokolliert werden, um den aktuellen Abrechnungskurs widerzuspiegeln. Die Stunden, die protokolliert wurden, bevor dem Projekt die Außerkraftsetzung der Abrechnungsrate hinzugefügt wurde, werden mit der Abrechnungsrate der Auftragsrolle zu diesem Zeitpunkt verknüpft.

Vor dieser Änderung konnten Sie die Abrechnungsrate einer Auftragsrolle nur einmal überschreiben und der tatsächliche Umsatz wurde neu berechnet, um die aktuelle Abrechnungsrate für alle Stunden widerzuspiegeln, die vor der Änderung des Abrechnungskurses protokolliert wurden.

Weitere Informationen zu Abrechnungsraten und Umsätzen finden Sie unter [Übersicht über Abrechnung und Umsatz](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Weitere Informationen zum Außerkraftsetzen der Abrechnungsraten für Stellenrollen auf Projektebene finden Sie unter [Übersicht über die Außerkraftsetzungsraten für Auftragsrollen und die Berechnung des Umsatzes für ein Projekt](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Ressourcenplaner {#resource-planner}

Mit dieser Version führen wir die erste Phase des Ressourcen-Planers ein, der Teil der Neugestaltung der neuen Registerkarte Planung im Bereich Personen ist. Mit dem Resource Planer können Sie die Anzahl der Stunden, die die Benutzer in Ihren Ressourcen-Pools zugewiesen sind, in allen aktuellen Projekten einplanen, für die Sie der Ressourcen-Manager sind. Die folgenden Zuordnungsnummern werden nach Projekt, Rolle und Benutzer im Ressourcenplaner angezeigt:

* Verfügbare Stunden
* Geplante Stunden
* Budgetierte Stunden
* Stündliche Abweichung (zwischen den veranschlagten und den geplanten Stunden)
* Nettostundendifferenz (zwischen den verfügbaren und den veranschlagten Stunden)

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Neue Ressourcen - Budgetierter Stundenbereich {#new-resource-budgeted-hour-field}

Um die neue Planungsfunktion und den Ressourcenplaner zu unterstützen, wurde dem ReportBuilder ein neues Feld hinzugefügt, in dem Sie Berichte zu den für Ressourcen veranschlagten Stunden erstellen können. In diesem Feld wird die Anzahl der Stunden erfasst, die eine Ressource in einem Projekt in den Haushalt aufgenommen wird. Dieses Feld ist nicht verfügbar, wenn Ressourcen mit der Funktion für die Planung älterer Ressourcen in den Haushaltsplan eingesetzt werden.

Weitere Informationen zur Verwendung von budgetierten Stunden im Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## In-App-Benachrichtigung für Validierung des Testversands {#in-app-notification-for-proof-approval}

Wenn Sie als Genehmiger für einen Testversand benannt sind, erhalten Sie eine In-App-Benachrichtigung über die Genehmigung des Testversands, die auf Ihre Entscheidung wartet. In der Benachrichtigung wird folgender Text angezeigt: `<User name>` wünscht, dass Sie diesen Testversand validieren&quot;. Wenn die Benutzerinformationen nicht verfügbar sind, ändert sich die Benachrichtigung in &quot;Dieser Testversand erfordert Ihre Zustimmung&quot;.

Vor dieser Verbesserung war der einzige visuelle Hinweis, dass Sie als Genehmiger für einen Testversand benannt wurden, eine neue Testversand-Anfrage in Ihrem Arbeitsbereich.

Weitere Informationen zu In-App-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Benutzerauftragsrolle im Bereich &quot;Zugeordnet&quot;auf der Detailseite für Aufgaben und Probleme anzeigen {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Beim Anzeigen der Detailseite einer Aufgabe oder eines Problems wird nun unter dem Namen des Verantwortlichen im Bereich Zugeordneter Benutzer eine Auftragsrolle angezeigt. Diese Vorgangsrolle stellt die Rolle des Benutzers dar, der der Aufgabenrollenzuweisung der Aufgabe oder des Problems entspricht. Wenn die Aufgabe bzw. das Problem keiner Auftragsrolle zugewiesen ist, wird die Rolle des Hauptauftrags des zugewiesenen Benutzers angezeigt.

Vor dieser Änderung wurde nur der Titel des Benutzers unter dem Namen des Benutzers im Bereich Zugeordneter Benutzer angezeigt. 
