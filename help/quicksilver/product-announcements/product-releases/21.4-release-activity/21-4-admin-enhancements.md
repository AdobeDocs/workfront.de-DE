---
title: 21.4 Administratorverbesserungen
description: 21.4 Administratorverbesserungen
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 21.4 Administratorverbesserungen

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 21.4 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden ab der Woche des 4. Oktober 2021 in der Produktionsumgebung verfügbar sein.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie unter [21.4 Versionsübersicht](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Für Administratoren: Ermitteln, welche Gruppen mit einem Genehmigungsprozess verbunden sind

Um herauszufinden, welche Gruppen mit den Genehmigungsprozessen in Ihrem System verbunden sind, haben wir der Ansicht &quot;Standard&quot;auf der Seite &quot;Genehmigungen&quot;unter Einrichtung eine Spalte &quot;Gruppenname&quot;hinzugefügt. Jetzt können Sie diese Informationen anzeigen, ohne eine benutzerdefinierte Ansicht erstellen zu müssen.

Informationen zu Validierungsprozessen finden Sie unter [Übersicht über den Genehmigungsprozess](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Informationen zum Verwalten von Gruppengenehmigungsprozessen finden Sie unter [Validierungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Neu für Administratoren: Gruppen können ihre eigenen Voreinstellungen für das Zeitblatt und die Stunde konfigurieren

>[!NOTE]
>
>In der Produktion ist diese Funktion zunächst nur für Kunden mit Cluster 4 als Teil eines schrittweisen Rollouts verfügbar. Diese Anmerkung wird aktualisiert, sobald die Funktion für andere Cluster verfügbar ist.

In einer großen Organisation müssen einige Gruppen möglicherweise die Voreinstellungen für das Zeitblatt und die Stunde unabhängig voneinander konfigurieren, um ihren individuellen Workflows anzupassen, anstatt die von einem Administrator auf Systemebene konfigurierten Voreinstellungen zu übernehmen. Jetzt können Workfront-Administratoren für alle Gruppen im System die Voreinstellungen für ein Zeitblatt und eine Stunde aufheben, damit sie es selbst konfigurieren können.

Diese Möglichkeit wurde kürzlich auch für Projektvoreinstellungen sowie für Aufgaben- und Problemeinstellungen hinzugefügt.

Informationen dazu, wie ein Workfront-Administrator die Voreinstellung für ein Zeitblatt und eine Stunde freischaltet, finden Sie im Abschnitt [Zeitblatt- und Stundenvoreinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen dazu, wie ein Gruppenadministrator entsperrte Aufgaben konfiguriert und die Voreinstellungen für eine Gruppe ausgibt, finden Sie unter [Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Neu für Workfront-Administratoren: Konfigurieren von Layoutvorlagen für automatisch bereitgestellte Benutzer im neuen Workfront-Erlebnis

Jetzt können Sie Layoutvorlagen im neuen Workfront-Erlebnis für automatisch bereitgestellte Benutzer konfigurieren. Im Dropdown-Menü Workfront-Benutzerattribut, in dem Sie Benutzerattribute zuordnen (Setup > System > Single Sign-On), ist jetzt ein neues Menüelement &quot;NWE Layout Template&quot;verfügbar, das diese Konfiguration vornehmen kann. Zuvor war es nur in Workfront Classic möglich, Layoutvorlagen für automatisch bereitgestellte Benutzer zu konfigurieren.

Anweisungen zum Zuordnen von Benutzerattributen finden Sie unter [Benutzerattribute zuordnen und neue Benutzer automatisch bereitstellen](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Das neue Feld zeigt die Gruppen an, zu denen Ihre Benutzer gehören

Jetzt ist es einfach herauszufinden, zu welchen Gruppen Ihre Benutzer gehören. In einem Bericht oder einer Ansicht, in dem Benutzer aufgelistet werden, können Sie mithilfe des neuen Felds Andere Gruppen eine Spalte erstellen. In diesem Feld werden die Gruppen aufgeführt, denen jeder Benutzer angehört.

Informationen zur Verwendung von Berichten und Ansichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) und [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Auf der Detailseite für Blueprints wird jetzt ein Bild angezeigt

Auf der Detailseite für jeden Blueprint wird jetzt ein Bild der Projektvorlage angezeigt, die mit dem Blueprint installiert ist. Das Bild bietet eine Vorschau der Blueprint-Inhalte, sodass Sie wissen, was Sie installieren werden. Sie können optional eine Vorschau des vollständigen Bildes im Browser anzeigen oder das Bild herunterladen.

Weitere Informationen finden Sie unter [Blueprints - Übersicht](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Blueprint-Voreinstellungen für neue Probleme

Für einige Blueprints sind jetzt neue Voreinstellungen für Probleme verfügbar. Sie werden standardmäßig installiert, Sie können jedoch die Installation der Voreinstellungen deaktivieren, wenn Sie Ihre Installationsdetails konfigurieren.

Zu den Voreinstellungen gehören Warteschlangen-Themengruppen, Warteschlangenthemen und Routing-Regeln, um beim Senden eines Problems oder einer Anfrage die richtigen Informationen zu erfassen und das Problem oder die Anfrage an die richtige Auftrags- oder -team zu senden. Die Verwendung der Voreinstellungen trägt dazu bei, die Konsistenz bei der Erfassung neuer Probleme oder Anforderungen in Ihren Projekten zu gewährleisten.

Beachten Sie, dass durch die Verwendung dieser Voreinstellungen die aus der Vorlage erstellten Projekte nicht in Anfragewarteschlangen umgewandelt werden.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Neu für Gruppenadministratoren: Anzeigen und Verwalten der kürzlich gelöschten und wiederhergestellten Elemente einer Gruppe

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Wir machen es weiterhin einfacher, Ihre Gruppen und die zugehörigen Objekte an einem Ort zu verwalten. Jetzt können Sie die kürzlich gelöschten und wiederhergestellten Elemente einer Gruppe aus dem Gruppenbereich anzeigen und damit arbeiten. So sparen Sie sich, diese Elemente im Bereich &quot;Kürzlich gelöscht&quot;oder &quot;Kürzlich wiederhergestellt&quot;unter &quot;Einstellungen&quot;verwalten zu müssen. Und es behält die Liste der Gruppenelemente, mit denen Sie arbeiten, getrennt von den anderen gelöschten und wiederhergestellten Elementen im System bei.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) und [Anzeigen und Verwalten der kürzlich wiederhergestellten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Neu für Gruppenadministratoren: Gruppenvoreinstellungen wirken sich jetzt auf Gruppenvorlagen aus

Es ist jetzt einfacher sicherzustellen, dass die Projektvorlagen Ihrer Gruppe den Anforderungen Ihrer Gruppe entsprechen. Wenn Sie einer Gruppe zum Zeitpunkt ihrer Erstellung eine neue Projektvorlage zuweisen, übernimmt die Vorlage die folgenden Einstellungen aus den Projekt- und Aufgabenvoreinstellungen der Gruppe:

* Performance-Index-Methode
* Bedingungstyp
* Planen aus
* Benutzerzeit
* Aktualisierungstyp
* Zugriffsparteneinstellungen

Wenn Sie eine neue Vorlagenaufgabe in einer Projektvorlage erstellen, die einer Gruppe zugeordnet ist, übernimmt die Vorlagenaufgabe die folgenden Einstellungen aus den Aufgabeneinstellungen der Gruppe:

* Dauertyp
* Umsatztyp
* Kostenart

Zuvor wurden diese Einstellungen von Projektvorlagen und Projektvorlagenaufgaben aus den auf Systemebene festgelegten Projekt- und Aufgabenvoreinstellungen übernommen.

Wenn Sie eine Vorlagen- oder Vorlagenaufgabe ohne Gruppe erstellen, z. B. auf der Hauptseite &quot;Vorlagen&quot;, werden die oben genannten Einstellungen von den Projekt- und Aufgabeneinstellungen auf Systemebene übernommen. Wenn Sie der Vorlage oder Vorlagenaufgabe später jedoch eine Gruppe zuweisen, wirken sich die Voreinstellungen der Gruppe nicht darauf aus.

Weitere Informationen finden Sie im Artikel im Abschnitt Wie Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet werden [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Neu für Administratoren: Erfahren Sie, welche benutzerdefinierten Formulare ein benutzerdefiniertes Feld verwenden

Jetzt ist es einfacher, ein benutzerdefiniertes Feld in einem benutzerdefinierten Formular zu ändern. Mit nur einem Klick im benutzerdefinierten Formular können Sie Informationen zu anderen benutzerdefinierten Formularen erhalten, die auch das Feld verwenden. Es ist wichtig zu beurteilen, ob diese Formulare angepasst werden müssen, damit sie nach der Änderung ordnungsgemäß funktionieren.

Weitere Informationen finden Sie unter [Alle benutzerdefinierten Formulare anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Neu für Gruppenadministratoren: Projekt-, Aufgaben- und Ausgabevoreinstellungen für eine Gruppe sperren und entsperren

Jetzt können Sie sicherstellen, dass alle Untergruppen unter Ihrer Gruppe dieselben Einstellungen verwenden, oder Sie können ihnen erlauben, eine Voreinstellung für ihre individuellen Workflows zu konfigurieren.

* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und für alle Untergruppen unterhalb Ihrer Gruppe sperren. Obwohl Sie die gesperrte Voreinstellung weiterhin neu konfigurieren können, können Administratoren niedrigerer Untergruppen dies nicht für ihre Gruppen tun.

   Umgekehrt können Sie eine Voreinstellung für Ihre Gruppe entsperren. Dadurch können Administratoren von Untergruppen diese für die individuellen Projekt-, Aufgaben- oder Problem-Workflow-Anforderungen ihrer Benutzer konfigurieren.

   Weitere Informationen finden Sie unter [Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Wenn Sie Workfront-Administrator sind, müssen Sie nicht zum Bereich Gruppen wechseln, um die Voreinstellungen einer Untergruppe zu konfigurieren. Im Hauptbereich Voreinstellungen für Projekte, Aufgaben und Probleme oder Voreinstellungen für Timesheets und Stunden können Sie über das Suchfeld oben auf der Seite die Untergruppe suchen und ihre Voreinstellungen konfigurieren.

   Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Neu für Gruppenadministratoren: Erstellen und Bearbeiten von Vorlagen über den Bereich &quot;Gruppen&quot;

>[!NOTE]
>
>Diese Funktion ist nur im neuen Workfront-Erlebnis verfügbar.

Wir machen es weiterhin einfacher, Ihre Gruppen und die zugehörigen Objekte an einem Ort zu verwalten. Jetzt können Sie die Vorlagen einer Gruppe im Bereich Gruppen in der Einrichtung anzeigen und damit arbeiten. Auf diese Weise vermeiden Sie, zum Bereich Vorlagen zu wechseln, um die Vorlagen einer Gruppe zu verwalten. Und es behält die Liste der Gruppenvorlagen, an denen Sie arbeiten, getrennt von den anderen im gesamten System bei.

Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Informationen in einem angehängten benutzerdefinierten Formular eingeben und speichern

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Es ist jetzt einfacher, Informationen im Abschnitt Details für ein Objekt bereitzustellen: Geben Sie Informationen in ein einzelnes benutzerdefiniertes Feld oder einen erweiterbaren Bereich (z. B. &quot;Überblick&quot;und &quot;Finanzen&quot;) ein und speichern Sie sie, selbst wenn erforderliche Felder in anderen benutzerdefinierten Formularen für das Objekt noch nicht ausgefüllt sind.

Wenn Sie zuvor Informationen in ein benutzerdefiniertes Formular oder einen erweiterbaren Bereich für ein Objekt eingegeben haben, wurden alle benutzerdefinierten Formulare, die an das Objekt angehängt waren, in den Bearbeitungsmodus versetzt und alle zugehörigen Felder mussten ausgefüllt werden, bevor Sie Ihre Änderungen speichern konnten. Dies war ein Problem, wenn Sie ein erforderliches Feld nicht ausfüllen konnten, da es für einen anderen Benutzer vorgesehen war.

Wenn Sie alle benutzerdefinierten Formulare und erweiterbaren Bereiche im Bereich Details eines Objekts bearbeiten möchten, können Sie im neuen Menü Bearbeiten , das wir dem Symbol Bearbeiten hinzugefügt haben, auf Alle bearbeiten klicken. Alternativ können Sie im selben Menü auf einen Namen klicken, um zum benutzerdefinierten Formular oder Abschnitt zu blättern, in dem Sie Änderungen vornehmen möchten

>[!NOTE]
>
>Diese Funktion wurde ursprünglich für die Vorschau mit Version 21.3 veröffentlicht.

Um es allen Ebenen einer Organisation zu erleichtern, ihre Workflows unabhängig zu verwalten und zu steuern, haben wir die Möglichkeit eingeführt, Status für Untergruppen zu erstellen und zu verwalten. Nun können Sie im Abschnitt Gruppen unter Einrichtung Folgendes für Gruppen durchführen, die Sie auf jeder Ebene verwalten:

* Erstellen, Bearbeiten, Löschen und Ausblenden eines Status für eine Gruppe
* Sperren Sie den Status für jede Gruppe, damit alle Untergruppen darunter auf die gleiche Weise verwendet werden können.
* Entsperren Sie einen Status für eine beliebige Gruppe, damit Administratoren untergeordneter Untergruppen ihn an ihre individuellen Anforderungen anpassen können.
* Festlegen des Gruppenstatus als Standardstatus
* Neuanordnen und Ausblenden der Anzeige von Gruppenstatus auf Objekten

Workfront-Administratoren können diese Aufgaben auch ausführen (für alle Gruppen).

Zuvor war diese Funktion nur für Gruppen der obersten Ebene verfügbar.

Weitere Informationen finden Sie unter [Verwalten von Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Neu für Workfront-Administratoren: Migrieren von Layoutvorlagen aus Workfront Classic zum neuen Workfront-Erlebnis

>[!NOTE]
>
>Diese Funktion wurde am 1. Juli 2021 in der Vorschau-Umgebung veröffentlicht. Es wird am 15. Juli 2021 in der Produktionsumgebung veröffentlicht.

Um Sie bei der Verwaltung von Layoutvorlagen zu unterstützen, während Ihre Benutzer zum neuen Workfront-Erlebnis wechseln, haben wir eine Schaltfläche erstellt, mit der Sie Layoutvorlagen von Workfront Classic zum neuen Erlebnis migrieren können, ohne sich auf den Workfront-Support zu verlassen.

Zuvor konnte nur der Workfront-Support Ihre Layoutvorlagen von Workfront Classic in das neue Workfront-Erlebnis migrieren.

## Wenn Sie eine Vorlage mit einer Gruppe verknüpfen, wählen Sie unter Warteschlangendetails und Warteschlangenthemen einen Gruppengenehmigungsprozess aus.

Wir haben eine neue Option zum Verknüpfen einer Vorlage mit einer Gruppe hinzugefügt. Jetzt können Sie gruppenspezifische Genehmigungsprozesse für Probleme in den Warteschlangendetails der Vorlage oder in einem ihrer Warteschlangenthemen auswählen.

Wenn wir in Version 21.3 die Möglichkeit hinzugefügt haben, eine Gruppenvorlage mit einer Gruppe zu verknüpfen, können Sie einen gruppenspezifischen Validierungsprozess in der Vorlage auswählen, dies ist jedoch in den Warteschlangendetails oder Warteschlangenthemen der Vorlage nicht möglich.

Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
