---
title: 21.4 Administrator-Verbesserungen
description: 21.4 Administrator-Verbesserungen
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4 Administrator-Verbesserungen

Auf dieser Seite werden alle mit Version 21.4 vorgenommenen Administrationsverbesserungen für die Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 4. Oktober 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie in der Übersicht über die Version [21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Für Admins: Hier können Sie sehen, welche Gruppen mit einem Genehmigungsprozess verknüpft sind

Um herauszufinden, welche Gruppen mit den Genehmigungsprozessen in Ihrem System verknüpft sind, haben wir auf der Seite Genehmigungen im Setup eine Spalte Gruppenname zur Standardansicht hinzugefügt. Jetzt können Sie diese Informationen anzeigen, ohne eine benutzerdefinierte Ansicht erstellen zu müssen.

Informationen zu Genehmigungsprozessen finden Sie unter [Übersicht über Genehmigungsprozesse](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Informationen zum Verwalten von Gruppengenehmigungsprozessen finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Neu für Administratoren: Gruppen können ihre eigenen Arbeitszeittabellen- und Stundeneinstellungen konfigurieren

>[!NOTE]
>
>Zunächst in der Produktionsumgebung ist diese Funktion als Teil eines schrittweisen Rollouts nur für Kunden auf Cluster 4 verfügbar. Diese Anmerkung wird aktualisiert, sobald die Funktion für andere Cluster verfügbar wird.

In einem großen Unternehmen müssen einige Gruppen möglicherweise die Arbeitszeittabellen- und Stundeneinstellungen unabhängig voneinander konfigurieren, um sie an ihre spezifischen Workflows anzupassen, anstatt die von einem Administrator auf Systemebene konfigurierten Einstellungen zu übernehmen. Jetzt können Workfront-Administratoren eine Arbeitszeittabelle und Stundenvoreinstellungen für alle Gruppen im System entsperren, sodass sie sie selbst konfigurieren können.

Diese Funktion wurde kürzlich für Projektvoreinstellungen sowie für Aufgaben- und Problemvoreinstellungen hinzugefügt.

Informationen dazu, wie Workfront-Admins eine Arbeitszeittabelle und Stundeneinstellungen entsperren, finden Sie im Abschnitt [Arbeitszeittabelle und Stundeneinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Arbeitszeittabelle und Stundeneinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen dazu, wie Gruppenadmins die Einstellungen für entsperrte Aufgaben und Probleme für eine Gruppe konfigurieren, finden [ unter „Arbeitszeittabelle und Stundeneinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Neu für Workfront-Admins: Konfigurieren von Layout-Vorlagen für automatisch bereitgestellte Benutzende in der neuen Workfront-Version

Jetzt können Sie Layout-Vorlagen in der neuen Workfront-Version für automatisch bereitgestellte Benutzerinnen und Benutzer konfigurieren. Im Dropdown-Menü Workfront-Benutzerattribut, in dem Sie Benutzerattribute zuordnen (Einrichtung > System > Single Sign-On), ist jetzt ein neues Menüelement „NEUE Layout-Vorlage“ verfügbar, um diese Konfiguration vorzunehmen. Zuvor konnten Sie Layout-Vorlagen nur für automatisch bereitgestellte Benutzende in Workfront Classic konfigurieren.

Anweisungen zum Zuordnen von Benutzerattributen finden Sie [Zuordnen von Benutzerattributen und automatische Bereitstellung neuer Benutzer](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Das neue Feld zeigt die Gruppen an, denen Ihre Benutzer angehören

Jetzt ist es einfach herauszufinden, zu welchen Gruppen Ihre Benutzerinnen und Benutzer gehören. In einem Bericht oder einer Ansicht, in dem bzw. der Benutzende aufgelistet sind, können Sie eine Spalte mithilfe des neuen Felds Sonstige Gruppen erstellen. In diesem Feld werden die Gruppen aufgelistet, in denen jeder Benutzer Mitglied ist.

Informationen zur Verwendung von Berichten und Ansichten finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) und [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Die Blueprint-Detailseite zeigt jetzt ein Bild an

Auf der Detailseite für jeden Blueprint wird jetzt ein Bild der Projektvorlage angezeigt, die mit dem Blueprint installiert wird. Die Abbildung bietet eine Vorschau der Blueprint-Inhalte, damit Sie wissen, was Sie installieren werden. Sie können optional eine Vorschau des vollständigen Bildes im Browser anzeigen oder das Bild herunterladen.

Weitere Informationen finden Sie unter [Blueprints - Übersicht](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Blueprint-Voreinstellungen für neue Probleme

Für einige Blueprints sind jetzt Einstellungen für neue Probleme verfügbar. Sie werden standardmäßig installiert, Sie können die Installation der Voreinstellungen jedoch deaktivieren, wenn Sie Ihre Installationsdetails konfigurieren.

Zu den Voreinstellungen gehören Warteschlangen-Themengruppen, Warteschlangen-Themen und Routing-Regeln, um die richtigen Informationen zu erfassen, wenn ein Problem oder eine Anfrage gesendet wird, und das Problem oder die Anfrage an das richtige Aufgabengebiet oder Team zu senden. Die Verwendung der Voreinstellungen hilft dabei, die Art und Weise, wie neue Probleme oder Anfragen in Ihren Projekten erfasst werden, konsistent zu gestalten.

Beachten Sie, dass durch die Verwendung dieser Voreinstellungen die aus der Vorlage erstellten Projekte nicht in Anfrage-Warteschlangen umgewandelt werden.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Neu für Gruppenadministratoren: Anzeigen und Verwalten der kürzlich gelöschten und wiederhergestellten Elemente einer Gruppe

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Wir erleichtern Ihnen weiterhin, Ihre Gruppen und die mit ihnen verbundenen Objekte an einem Ort zu verwalten. Jetzt können Sie die kürzlich gelöschten und wiederhergestellten Elemente einer Gruppe aus dem Bereich Gruppen anzeigen und damit arbeiten. Dadurch müssen Sie nicht mehr in den Bereich „Kürzlich gelöscht“ oder „Kürzlich wiederhergestellt“ in „Setup“ gehen, um diese Elemente zu verwalten. Außerdem wird die Liste der Gruppenelemente, mit denen Sie arbeiten, getrennt von den anderen gelöschten und wiederhergestellten Elementen im System aufbewahrt.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) und [Anzeigen und Verwalten der kürzlich wiederhergestellten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Neu für Gruppenadministratoren: Gruppeneinstellungen wirken sich jetzt auf Gruppenvorlagen aus

Es ist jetzt einfacher, sicherzustellen, dass die Projektvorlagen Ihrer Gruppe den Anforderungen Ihrer Gruppe entsprechen. Wenn Sie einer Gruppe zum Zeitpunkt der Erstellung eine neue Projektvorlage zuweisen, übernimmt die Vorlage die folgenden Einstellungen aus den Projekt- und Aufgabenvoreinstellungen der Gruppe:

* Performance-Index-Methode
* Bedingungstyp
* Zeitplan ab
* Benutzer-Ausfallzeit
* Update-Typ
* Zugriff auf Abschnittseinstellungen

Wenn Sie eine neue Vorlagenaufgabe in einer Projektvorlage erstellen, die einer Gruppe zugeordnet ist, übernimmt die Vorlagenaufgabe die folgenden Einstellungen aus den Aufgabenvoreinstellungen der Gruppe:

* Dauertyp
* Umsatztyp
* Kostenart

Zuvor haben Projektvorlagen und Projektvorlagenaufgaben diese Einstellungen von den Projekt- und Aufgabenvoreinstellungen übernommen, die auf Systemebene festgelegt wurden.

Wenn Sie eine Vorlage oder Vorlagenaufgabe ohne Gruppe erstellen, z. B. auf der Hauptseite Vorlagen , werden die oben genannten Einstellungen von den Voreinstellungen für Projekte und Aufgaben auf Systemebene übernommen. Wenn Sie der Vorlage oder Vorlagenaufgabe später jedoch eine Gruppe zuweisen, wirken sich die Einstellungen der Gruppe nicht auf sie aus.

Weitere Informationen finden Sie im Abschnitt Wie Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet werden im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Neu für Admins: Finden Sie heraus, welche benutzerdefinierten Formulare ein benutzerdefiniertes Feld verwenden

Jetzt ist es einfacher, ein benutzerdefiniertes Feld in einem benutzerdefinierten Formular zu ändern. Mit einem Klick in das benutzerdefinierte Formular können Sie sich über alle anderen benutzerdefinierten Formulare informieren, die ebenfalls das Feld verwenden. Es ist wichtig zu beurteilen, ob diese Formulare angepasst werden müssen, damit sie nach der Änderung weiterhin ordnungsgemäß funktionieren.

Weitere Informationen finden Sie unter [Alle benutzerdefinierten Formulare anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Neu für Gruppenadministratoren: Voreinstellungen für Projekte, Aufgaben und Probleme einer Gruppe sperren und entsperren

Jetzt können Sie sicherstellen, dass alle in den Untergruppen unter Ihrer Gruppe dieselben Voreinstellungen verwenden. Alternativ können Sie zulassen, dass sie eine Voreinstellung für ihre eindeutigen Workflows konfigurieren.

* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und dann für alle Untergruppen unter Ihrer Gruppe sperren. Sie können die gesperrte Voreinstellung zwar noch neu konfigurieren, Administratoren niedrigerer Untergruppen können dies jedoch nicht für ihre Gruppen tun.

  Umgekehrt können Sie eine Voreinstellung für Ihre Gruppe entsperren. Auf diese Weise können Untergruppenadministratoren sie für die individuellen Projekt-, Aufgaben- oder Problem-Workflow-Anforderungen ihrer Benutzer konfigurieren.

  Weitere Informationen finden Sie unter [Projekt, Aufgabe oder Problem für Untergruppen sperren oder entsperren](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Wenn Sie Workfront-Administrator sind, müssen Sie nicht zum Bereich Gruppen gehen, um die Einstellungen einer Untergruppe zu konfigurieren. Im Hauptbereich Projektvoreinstellungen, Voreinstellungen für Aufgaben und Probleme oder Arbeitszeittabellen- und Stunden-Voreinstellungen können Sie das Suchfeld oben auf der Seite verwenden, um die Untergruppe zu finden und ihre Voreinstellungen zu konfigurieren.

  Weitere Informationen finden Sie unter [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Aufgaben- und Problemeinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Neu für Gruppenadministratoren: Erstellen und Bearbeiten von Vorlagen über den Bereich Gruppen

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Workfront-Version verfügbar.

Wir erleichtern Ihnen weiterhin, Ihre Gruppen und die mit ihnen verbundenen Objekte an einem Ort zu verwalten. Jetzt können Sie die Vorlagen einer Gruppe im Bereich Gruppen unter „Setup“ anzeigen und damit arbeiten. Dadurch müssen Sie nicht mehr zum Bereich Vorlagen gehen, um die Vorlagen einer Gruppe zu verwalten. Außerdem wird die Liste der Gruppenvorlagen, an denen Sie arbeiten, von den anderen Vorlagen im System getrennt aufbewahrt.

Weitere Informationen finden Sie [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Geben Sie Informationen in jeweils einem angehängten benutzerdefinierten Formular ein und speichern Sie sie

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Es ist jetzt einfacher, Informationen im Abschnitt Details für ein Objekt anzugeben: Geben Sie Informationen in ein einzelnes benutzerdefiniertes Feld oder einen erweiterbaren Bereich ein und speichern Sie sie (z. B. Übersicht und Finanzen), auch wenn erforderliche Felder in anderen benutzerdefinierten Formularen auf dem Objekt noch nicht ausgefüllt sind.

Wenn Sie bisher Informationen in ein benutzerdefiniertes Formular oder einen erweiterbaren Bereich für ein Objekt eingegeben haben, wurden alle benutzerdefinierten Formulare, die mit dem Objekt verknüpft waren, in den Bearbeitungsmodus versetzt, und alle erforderlichen Felder mussten ausgefüllt werden, bevor Sie Ihre Änderungen speichern konnten. Dies war ein Problem, wenn Sie ein erforderliches Feld nicht ausfüllen konnten, da es für einen anderen Benutzer vorgesehen war.

Wenn Sie nicht alle benutzerdefinierten Formulare und erweiterbaren Bereiche im Detailbereich für ein Objekt bearbeiten möchten, können Sie im neuen Menü Bearbeiten , das wir zum Bearbeitungssymbol hinzugefügt haben, auf Alle bearbeiten klicken. Oder Sie können im selben Menü auf einen Namen klicken, um zum benutzerdefinierten Formular oder Abschnitt zu scrollen, in dem Sie Änderungen vornehmen möchten

>[!NOTE]
>
>Diese Funktion wurde ursprünglich mit Version 21.3 zur Vorschau veröffentlicht.

Um es allen Unternehmensebenen zu erleichtern, ihre Workflows unabhängig zu verwalten und zu steuern, haben wir die Möglichkeit eingeführt, Status für Untergruppen zu erstellen und zu verwalten. Jetzt können Sie im Abschnitt Gruppen unter Setup die folgenden Aktionen für Gruppen durchführen, die Sie auf jeder Ebene verwalten:

* Erstellen, Bearbeiten, Löschen und Ausblenden eines Status für eine Gruppe
* Sperren Sie einen Status für eine beliebige Gruppe, damit alle darunter liegenden Untergruppen ihn auf die gleiche Weise verwenden können
* Entsperren Sie einen Status für eine beliebige Gruppe, damit Administratoren niedrigerer Untergruppen ihn an ihre individuellen Anforderungen anpassen können
* Festlegen eines Gruppenstatus als Standardstatus
* Neuanordnung und Ausblenden der Anzeige von Gruppenstatus in Objekten

Workfront-Administratoren können auch diese Aufgaben ausführen (für alle Gruppen).

Zuvor war diese Funktion nur für Gruppen der obersten Ebene verfügbar.

Weitere Informationen finden Sie unter [Verwalten von Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Neu für Workfront-Admins: Migrieren Sie Layout-Vorlagen von Workfront Classic eigenständig in das neue Workfront-Erlebnis

>[!NOTE]
>
>Diese Funktion wurde am 1. Juli 2021 in der Vorschau-Umgebung veröffentlicht. Die Version wird am 15. Juli 2021 in der Produktionsumgebung veröffentlicht.

Um Sie bei der Verwaltung von Layout-Vorlagen zu unterstützen, während Ihre Benutzer zur Verwendung der neuen Workfront-Version wechseln, haben wir eine Schaltfläche erstellt, mit der Sie Layout-Vorlagen von Workfront Classic zur neuen Version migrieren können, ohne auf den Workfront-Kunden-Support angewiesen zu sein.

Zuvor konnte nur der Workfront-Kunden-Support Ihre Layout-Vorlagen von Workfront Classic zum neuen Workfront-Erlebnis migrieren.

## Wenn Sie eine Vorlage mit einer Gruppe verknüpfen, wählen Sie in Warteschlangendetails und Warteschlangenthemen einen Gruppengenehmigungsprozess aus

Es wurde eine neue Option zum Verknüpfen einer Vorlage mit einer Gruppe hinzugefügt. Jetzt können Sie gruppenspezifische Genehmigungsprozesse für Probleme in den Warteschlangendetails der Vorlage oder in einem ihrer Warteschlangenthemen auswählen.

Wenn wir in 21.3 die Möglichkeit hinzugefügt haben, eine Gruppenvorlage mit einer Gruppe zu verknüpfen, konnten Sie einen gruppenspezifischen Genehmigungsprozess in der Vorlage auswählen, aber dies war in den Warteschlangendetails oder Warteschlangenthemen der Vorlage nicht möglich.

Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeiten](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
