---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Endspiel 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Version 2017.2 verfügbar waren. Die Funktion auf dieser Seite wurde am 28. Juni 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird am 26. Juli 2017 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# Beta-Endspiel 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Version 2017.2 verfügbar waren. Die Funktion auf dieser Seite wurde am 28. Juni 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird am 26. Juli 2017 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller in 2017.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die Beta-Endversion 2017.2 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren:**

* [Ermitteln der Verfügbarkeit des HTML5-Video-Proofing-Viewers (ProofHQ und Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Unterstützung von SHA-256-Zertifikaten für SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Type-Ahead für Zuordnungsattribute](#type-ahead-for-mapping-attributes)
* [API-Verbesserung: Zugriff auf Benutzerzuweisungen](#api-enhancement-access-user-allocations)

**Für alle Benutzer:**

* [Ressourcenplaner](#resource-planner)
* [Neuer Planungsbereich in einem Projekt (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Ressourcenplanung: Standardmäßig weniger Elemente anzeigen](#resource-scheduling-show-fewer-items-by-default)
* [Ressourcenplanung: Anzeige von Ablageindikatoren und Überallokationen beim Ziehen von Aufgaben und Problemen](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Ressourcenplanung: Benutzerzuweisungen werden nicht mehr auf die nächste halbe Stunde gerundet](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exportieren des Auslastungsberichts in den Formaten TSV und PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 Beta Final](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 Beta Final](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Korrekturabzugsentscheidung wird im Bereich Meine Arbeit (Workfront) angezeigt](#proof-decision-displays-in-the-my-work-area-workfront)
* [Rich-Media-Korrekturabzüge in voreingestellten Auflösungen anzeigen (ProofHQ und Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Anzeigen von URLs zu Unterseiten in Kommentaren zu Rich-Media-Korrekturabzügen (ProofHQ und Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Erstellen benutzerdefinierter Ansichten basierend auf vorhandenen Standardansichten (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtern des Berichtsbereichs (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Anzeigen von Mindest- und Höchstwerten in Berichten (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [In-App-Benachrichtigung zur Genehmigung von Korrekturabzügen](#in-app-notification-for-proof-approval)
* [Verbesserungen für Mobilgeräte](#mobile-improvements)
* [Schrägstrich wurde zu Filteranweisungen für Feldwerte hinzugefügt, die Kommas enthalten](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Mehrere Abrechnungssätze](#multiple-billing-rates)
* [Neues Feld Ressource - budgetierte Stunde](#new-resource-budgeted-hour-field)
* [Anzeigen des Benutzeraufgabengebiets im Bereich „Zugewiesen an“ auf der Detailseite für Aufgaben und Probleme](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Neuer Planungsbereich in einem Projekt (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

Der Bereich Planung in einem Projekt (früher als Team Builder bezeichnet) wurde mit einer aktualisierten und intuitiveren Benutzeroberfläche neu gestaltet. Die neue Planungsfunktion stimmt jetzt besser mit der Ressourcenplanungs-Funktion überein, die derzeit in anderen Bereichen von Workfront verfügbar ist.

Zu den Verbesserungen gehören:

* Zeigen Sie aktuelle Ressourcenzuteilungen für Mitglieder des Projektteams an, sodass Sie fundiertere Entscheidungen bei der Zuweisung treffen können
* Visuelle Darstellung der Aufgabendauer in der Zeitleiste
* Filtern der in der Zeitplanleiste angezeigten Informationen
* Einfaches Hinzufügen und Entfernen von Benutzern zum Projekt-Team direkt über die Zeitleiste für die Planung

Die folgende Funktion ist in anderen Bereichen des Tools bei der Ressourcenplanung verfügbar, ist jedoch nicht bei der Ressourcenplanung im Bereich Teamplanung verfügbar:

* Übergeordnete Aufgaben konfigurieren, die in der Zeitleiste angezeigt werden
* Projektnamen konfigurieren, die in der Zeitplanleiste angezeigt werden sollen
* Ändern von Benutzerzuweisungen mithilfe des Auslagerungswerkzeugs
* Filtern nach Portfolio, Programmen und Projekten

Weitere Informationen zu den im Bereich „Team-Planung“ verfügbaren Funktionen finden Sie unter „Erste Schritte mit der Ressourcenplanung“.

## Ressourcenplanung: Standardmäßig weniger Elemente anzeigen {#resource-scheduling-show-fewer-items-by-default}

Standardmäßig werden jetzt maximal 10 Arbeitselemente pro Tag auf der Zeitleiste für einen bestimmten Benutzer angezeigt. Sie können die Liste erweitern, um alle Aufgaben und Probleme anzuzeigen, die diesem Benutzer derzeit zugewiesen sind.

Auf diese Weise können Sie die Zeitleiste für die Planung einfacher durchsuchen, wenn Benutzern viele Aufgaben und Probleme zugewiesen werden.

Vor dieser Änderung wurden alle Aufgaben und Probleme immer für alle Benutzer angezeigt.

Weitere Informationen zur Zuweisung von Aufgaben und Problemen zu Benutzern in der Zeitplanleiste finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## Ressourcenplanung: Anzeigen von Ablageindikatoren und Überallokationen beim Ziehen von Aufgaben und Problemen {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Beim Zuweisen einer Aufgabe oder eines Problems zu einem Benutzer über die Zeitleiste für die Planung per Drag-and-Drop werden jetzt die folgenden Informationen angezeigt, bevor die Aufgabe oder das Problem freigegeben und die Zuweisung abgeschlossen wird:

* Ein Ablageindikator wird in der Zeile des Benutzers angezeigt. Auf diese Weise können Sie sehen, wo ein Element zugewiesen wird, bevor Sie die Zuweisung vornehmen.
* Wenn Benutzerzuweisungen in der Zeitleiste für die Planung aktiviert sind, werden die roten Zuordnungsindikatoren angezeigt, wenn die Ausführung der Zuweisung dazu führt, dass der Benutzer überlastet ist.

Vor diesen Änderungen wurden keine Informationen angezeigt, bevor die Aufgabe oder das Problem freigegeben wurde.

Weitere Informationen zur Zuweisung von Aufgaben und Problemen zu Benutzern in der Zeitplanleiste finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## Ressourcenplanung: Benutzerzuweisungen werden nicht mehr auf die nächste halbe Stunde gerundet {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Wenn einer Aufgabe oder einem Problem mehrere Benutzende zugewiesen sind oder wenn eine Aufgabe oder ein Problem mehrere Tage umfasst, versucht Workfront, die geplanten Stunden gleichmäßig auf die zugewiesenen Benutzenden und Tage zu verteilen. Die Stunden werden standardmäßig auf das nächste Hundertstel gerundet (z. B. 1,33).

Wenn Sie verteilte Stunden zuvor manuell geändert haben, werden die Stunden angepasst und auf die nächste halbe Stunde gerundet (z. B. wird 1,33 auf 1,5 gerundet).

Jetzt werden die Stunden nicht mehr angepasst und auf die nächste halbe Stunde gerundet (z. B. bleibt 1,33 bei 1,33).

## API-Verbesserung: Zugriff auf Benutzerzuweisungen {#api-enhancement-access-user-allocations}

Sie können jetzt über die Workfront-API auf die Benutzerzuordnungsschattierung zugreifen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exportieren des Auslastungsberichts in den Formaten TSV und PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Sie können jetzt zusätzlich zum XLSX-Format den Auslastungsbericht für ein Projekt in den Formaten TSV und PDF exportieren.

Vor dieser Änderung konnten Sie den Auslastungsbericht nur im XLSX-Format exportieren.

Weitere Informationen zum Exportieren des Auslastungsberichts finden Sie unter [Übersicht über den ](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) unter [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Die Korrekturabzugsentscheidung wird im Bereich Meine Arbeit (Workfront) angezeigt {#proof-decision-displays-in-the-my-work-area-workfront}

Wenn Sie jetzt Korrekturabzugsgenehmigungen auf der Registerkarte Meine Genehmigungen in Ihrem Bereich Meine Arbeit anzeigen, wird die Entscheidung über den Korrekturabzug in Ihrem Bereich Meine Arbeit angezeigt und bleibt erhalten, bis Sie in Workfront auf die Schaltfläche Neu aktualisieren klicken oder bis Sie die Browser-Seite das nächste Mal aktualisieren.

Vor dieser Änderung gab es keinen Hinweis darauf, dass bereits eine Entscheidung über den Korrekturabzug getroffen wurde. Der Korrekturabzug blieb auf der Registerkarte Meine Genehmigungen , bis Sie den Browser aktualisiert haben.

Weitere Informationen finden Sie unter [Genehmigen von ](../../../../review-and-approve-work/manage-approvals/approving-work.md)&quot; in [Genehmigen von ](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Rich-Media-Korrekturabzüge in voreingestellten Auflösungen anzeigen (ProofHQ und Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

In einer früheren Version der Vorschau -Umgebung haben wir die Möglichkeit eingeführt, die Auflösung von Rich-Media-Korrekturabzügen anzupassen, indem entweder eine benutzerdefinierte Auflösung angegeben oder das Bild auf die gewünschte Auflösung gezogen wird.

Sie können jetzt aus den voreingestellten Auflösungsoptionen verschiedener Smartphones, Tablets, Notebooks und Desktops auswählen.

Weitere Informationen finden Sie unter „Anzeigen einer Vorgabenauflösung“ in [Ändern der interaktiven Korrekturabzugsauflösung im Proofing Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Anzeigen von URLs zu Unterseiten in Kommentaren zu Rich-Media-Korrekturabzügen (ProofHQ und Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Diese Funktion ist derzeit in der Produktionsumgebung verfügbar.

Wenn Sie jetzt einen Kommentar zu einer Unterseite in einem Rich-Media-Korrekturabzug abgeben, wird im Kommentar die URL zur Unterseite angezeigt.

Vor dieser Änderung war nicht klar, auf welche Unterseite sich der Kommentar bezog.

Weitere Informationen finden Sie unter

## Ermitteln der Verfügbarkeit des HTML5-Video-Proofing-Viewers (ProofHQ und Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

Als Workfront-Administrator in ProofHQ können Sie festlegen, ob Benutzende in Ihrem Unternehmen Zugriff auf den neuen HTML5-Proofing-Viewer für Videoprüfungen haben.

Weitere Informationen zum Konfigurieren dieser Option in Workfront finden Sie unter in .

## Erstellen benutzerdefinierter Ansichten basierend auf vorhandenen Standardansichten (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Jetzt können Sie eine benutzerdefinierte Ansicht erstellen, die auf einer Standardansicht basiert. Die Optionen Spalten, Sortierung und Filter aus der Standardansicht sind standardmäßig in der neuen Ansicht enthalten.

Vor dieser Änderung mussten Sie zum Erstellen einer benutzerdefinierten Ansicht die Ansicht von Grund auf neu erstellen. 

Weitere Informationen finden Sie unter [Erstellen einer benutzerdefinierten Ansicht](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [Erstellen und Verwalten von benutzerdefinierten Ansichten im Workfront Proof-Korrekturabzug](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtern des Reporting-Bereichs (ProofHQ) {#filter-the-reporting-area-proofhq}

Standardmäßig enthalten die auf der Registerkarte Berichte angezeigten Daten alle Informationen aus Ihrem ProofHQ-System. Sie können jetzt Filter verwenden, um nur Informationen anzuzeigen, die für Ihre Anforderungen relevant sind. 

Weitere Informationen finden Sie unter [Filtern von Berichten](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) in  [Berichte in Workfront Proof ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Anzeigen der Mindest- und Höchstwerte in Berichten (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Sie können jetzt konfigurieren, ob Mindest- und Höchstwerte im Diagramm angezeigt werden, wenn Berichte angezeigt werden.

Weitere Informationen finden Sie unter [ von Berichten ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in  [Berichte in Workfront Proof ](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Unterstützung von SHA-256-Zertifikaten für SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Wir unterstützen jetzt beim Konfigurieren von Workfront für SSO mit SAML 2.0 den sicheren Hash-Algorithmus 256 (SHA-256). Vor dieser Version haben wir nur den Secure Hash Algorithm 1 (SHA-1) unterstützt.

Weitere Informationen zum Konfigurieren von Workfront mit SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Type-Ahead für Zuordnungsattribute {#type-ahead-for-mapping-attributes}

Der Feldtyp Standardwert im Dialogfeld Attributzuordnung wurde in ein Feld mit automatischer Textvervollständigung geändert. Vor dieser Änderung war der Typ des Felds Standardwert ein Dropdown-Menü.

Diese Änderung gilt für die folgenden SSO-Protokolle:

* Active Directory
* LDAP
* SAML 2,0

SAML 1.1 unterstützt keine Attributzuordnung.

## Verbesserungen für Mobilgeräte {#mobile-improvements}

>[!NOTE]
>
> Die Mobile App wird unabhängig von der Workfront-Hauptanwendung veröffentlicht. Die in diesem Abschnitt beschriebenen Funktionen werden Anfang August veröffentlicht.

In den mobilen Apps werden die folgenden zusätzlichen Funktionen sowohl für die Android- als auch für die iOS-Plattform angezeigt:

* Senden von Anfragen über die Mobile App
* Arbeitszeittabellen-Neueintrag in der Mobile App
* Bearbeiten benutzerdefinierter Formulare über die Mobile App
* Anfragen zu Korrekturabzugs-Genehmigungen in der Mobile App

Für einige dieser Funktionen wird es ein öffentliches Beta-Programm für die Android-Plattform geben.

Weitere Informationen über das bevorstehende Beta-Programm für Mobile-Apps finden Sie unter  [ Seite „Betas](https://support.workfront.com/hc/en-us/sections/115000743248).

Weitere Informationen zur Verwendung der Mobile App von Workfront finden Sie unter .  

## Schrägstrich wurde zu Filteranweisungen für Feldwerte hinzugefügt, die Kommas enthalten {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Beim Erstellen eines Filters im Textmodus und Filtern nach Feldwerten, die Kommas enthalten, müssen Sie einen Schrägstrich (“/„) vor den Kommas hinzufügen, die die Werte trennen, um sicherzustellen, dass der Wert als eine Filteroption gelesen wird. Dies gilt nur für die folgenden Feldtypen:

* Dropdown-Listen
* Optionsschaltflächen
* Kontrollkästchen

Vor dieser Änderung konnten Sie nicht nach Feldern filtern, die Optionen mit Kommas enthielten.

Weitere Informationen über diese Änderung finden Sie unter [Filter - Übersicht](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Mehrere Abrechnungssätze {#multiple-billing-rates}

Sie können jetzt mehrere Abrechnungssatz-Überschreibungen für dasselbe Aufgabengebiet auf Projektebene hinzufügen. Mit dieser neuen Funktion können Sie Datumsbereiche für jede Überschreibung des Abrechnungssatzes definieren. Während des angegebenen Datumsbereichs wird ein anderer Abrechnungssatz auf das Aufgabengebiet angewendet, das Aufgaben in einem Projekt zugewiesen wurde. Abrechnungssätze werden mit den Stunden des Projekts multipliziert, um den Umsatz zu berechnen. Der innerhalb des Datumsbereichs eines Abrechnungssatzes berechnete Umsatz bleibt zu diesem Satz gesperrt und wird nicht aktualisiert, wenn die Sätze der Aufgabengebiete des Projekts aktualisiert werden. Im Fall von „Tatsächlicher Umsatz“ werden keine Stunden, die vor dem Überschreiben des Abrechnungssatzes protokolliert wurden, neu berechnet, um den aktuellen Abrechnungssatz widerzuspiegeln. Die Stunden, die protokolliert wurden, bevor die Überschreibung des Abrechnungssatzes zum Projekt hinzugefügt wurde, werden mit dem Abrechnungssatz des Aufgabengebiets zu diesem Zeitpunkt verknüpft.

Vor dieser Änderung konnten Sie den Abrechnungssatz eines Aufgabengebiets nur einmal überschreiben. Der tatsächliche Umsatz wird neu berechnet, um den aktuellen Abrechnungssatz für alle Stunden widerzuspiegeln, die protokolliert wurden, bevor der Abrechnungssatz geändert wurde.

Weitere Informationen zu Abrechnungssätzen und Umsatz finden Sie unter [Übersicht über Abrechnung und Umsatz](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Weitere Informationen zum Überschreiben der Abrechnungssätze für Aufgabengebiete auf Projektebene finden Sie unter [Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Ressourcenplaner {#resource-planner}

Mit dieser Version führen wir die erste Phase des Ressourcenplaners ein, die Teil der Neugestaltung der neuen Registerkarte Planung im Bereich Personen ist. Mithilfe des Ressourcenplaners können Sie die Stunden budgetieren, die den Benutzern in Ihren Ressourcenpools in allen aktuellen Projekten zugewiesen sind, für die Sie der Ressourcenmanager sind. Im Ressourcenplaner werden die folgenden Zuordnungsnummern nach Projekt, Aufgabengebiet und nach Benutzer angezeigt:

* Verfügbare Stunden
* Geplante Stunden
* Budgetierte Stunden
* Stundenabweichung (zwischen den budgetierten und den geplanten Stunden)
* Differenz der Nettostunden (zwischen verfügbarer und budgetierter Stunde)

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Neues Feld für budgetierte Stunde der Ressource {#new-resource-budgeted-hour-field}

Um die neue Planungsfunktion und den Ressourcenplaner zu unterstützen, wurde dem Report Builder ein neues Feld hinzugefügt, in dem Sie die budgetierten Stunden der Ressource auswerten können. Dieses Feld erfasst die Anzahl der Stunden, für die eine Ressource in einem Projekt budgetiert ist. Dieses Feld ist bei der Budgetierung von Ressourcen mit der alten Ressourcenplanungsfunktion nicht verfügbar.

Weitere Informationen zur Verwendung von budgetierten Stunden im Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## In-App-Benachrichtigung zur Genehmigung von Korrekturabzügen {#in-app-notification-for-proof-approval}

Wenn Sie als genehmigende Person für einen Korrekturabzug bestimmt werden, erhalten Sie eine In-App-Benachrichtigung über die Korrekturabzugsgenehmigung, die auf Ihre Entscheidung wartet. Die Benachrichtigung zeigt den folgenden Text an: &quot;`<User name>` bittet Sie, diesen Korrekturabzug zu genehmigen“. Wenn die Benutzerinformationen nicht verfügbar sind, ändert sich die Benachrichtigung in „Dieser Korrekturabzug erfordert Ihre Genehmigung“.

Vor dieser Verbesserung war der einzige visuelle Hinweis darauf, dass Sie als genehmigende Person für einen Korrekturabzug benannt wurden, eine neue Anforderung für einen Korrekturabzug in Ihrem Bereich Meine Arbeit .

Weitere Informationen zu In-App-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Anzeigen des Benutzeraufgabengebiets im Bereich „Zugewiesen an“ auf der Detailseite für Aufgaben und Probleme {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Wenn Sie jetzt die Detailseite einer Aufgabe oder eines Problems anzeigen, wird unter dem Namen des Verantwortlichen im Bereich Zugewiesen an ein Aufgabengebiet angezeigt. Dieses Aufgabengebiet stellt das Aufgabengebiet des Benutzers dar, das mit der Aufgabengebiet-Zuweisung der Aufgabe oder des Problems übereinstimmt. Wenn die Aufgabe oder das Problem keinem Aufgabengebiet zugewiesen ist, wird das primäre Aufgabengebiet des zugewiesenen Benutzers angezeigt.

Vor dieser Änderung wurde im Bereich Zugewiesen an nur der Titel des Benutzers unter dem Namen des Benutzers angezeigt. 
