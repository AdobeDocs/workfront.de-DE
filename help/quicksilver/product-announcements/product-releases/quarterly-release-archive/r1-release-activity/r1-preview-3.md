---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Vorschau 3
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der R1.3-Version verfügbar sind. Die Funktionalität auf dieser Seite wurde am 1. Februar 2017 in der Vorschau-Umgebung bereitgestellt.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# R1 Vorschau 3

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der R1.3-Version verfügbar sind. Die Funktionalität auf dieser Seite wurde am 1. Februar 2017 in der Vorschau-Umgebung bereitgestellt.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [Übersicht über die Release-Aktivität R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Verbesserte Methode zum Verknüpfen externer Dateien

Die Option zum Verknüpfen von Dokumenten aus einer externen Quelle (z. B. Google Drive, Box, Dropbox usw.) befindet sich jetzt an einer auffälligeren Stelle im Bereich &quot;Dokumente&quot;. 

Darüber hinaus ist die erstmalige Autorisierung eines Dokumentanbieters vor der Verknüpfung von Dateien von diesem Anbieter nun intuitiver (es handelt sich lediglich um einen zusätzlichen Schritt bei der Verknüpfung von Dateien von einem externen Anbieter).

Vor diesen Änderungen befand sich die Option zum Verknüpfen von Dateien aus einer externen Quelle im Dialogfeld &quot;Dokumente hinzufügen&quot;im Bereich &quot;Dokumente&quot;. Vor dem erstmaligen Verknüpfen eines Dokuments aus einer externen Quelle musste der Benutzer, der das Dokument verknüpft hat, diesen Dokumentanbieter im Bereich &quot;Einrichtung&quot;autorisieren.

Weitere Informationen finden Sie unter  [Verknüpfen von Dokumenten mit externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Aktualisiertes Team zur Kalenderarbeit

Der für Teams verfügbare Arbeitskalender enthält jetzt zusätzliche Funktionen und ein aktualisiertes Erscheinungsbild. Das Team, das mit dem Kalender arbeitet, funktioniert jetzt ähnlich wie das Tool zur Ressourcenplanung für Projekte.

Das aktualisierte Team, das am Kalender arbeitet, enthält die folgenden Verbesserungen:

* Benutzer alphabetisch anzeigen oder nach Rolle gruppieren.
* Filtern Sie die Planung nach Projektprioritäten, Status und einzelnen Projekten. Sie können die Planung auch nach Rollen und Benutzern filtern. (Der Bereich Filter enthält weniger Optionen als bei der Planung von Ressourcen für Projekte.)
* Schließen Sie Probleme in die Planung ein.
* Zeigen Sie die Benutzerzuordnungen an und ändern Sie die Anzahl der Stunden, die den Benutzern für jeden Tag bestimmte Aufgaben und Probleme zugewiesen werden.
* Anzeigen von Indikatoren, die anzeigen, wann Benutzer an einem bestimmten Tag zu viel zugeordnet sind.
* Konfigurieren Sie, ob abgeschlossene Arbeiten in der Planung angezeigt werden.

Unterschiede zum Ressourcen-Planungstool bei der Planung von Ressourcen für Projekte:

* Alle Teammitglieder werden im Team angezeigt, das am Kalender arbeitet.\
   Beim Planen von Ressourcen für Projekte werden nur Benutzer angezeigt, denen eine Rolle zugeordnet ist, die mit einer Rolle übereinstimmt, die einer oder mehreren Aufgaben im Bereich Nicht zugewiesen zugewiesen zugewiesen zugewiesen ist.
* Das Swap-Tool ist nicht im Team, das am Kalender arbeitet, enthalten.
* Jedes Teammitglied kann Änderungen am Team vornehmen, das am Kalender arbeitet.\
   Beim Planen von Ressourcen für Projekte können nur Ressourcen-Manager Ressourcenentscheidungen für das Projekt treffen.
* Probleme werden standardmäßig im Team angezeigt, das am Kalender arbeitet.\
   Beim Planen von Ressourcen für Projekte werden Probleme nicht standardmäßig angezeigt.

Weitere Informationen zur Verwendung des aktualisierten Teams, das am Kalender arbeitet, finden Sie unter [Ressourcenplanung](../../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

## Verbesserungen bei der Ressourcenplanung

Die Planung umfasst die folgenden Erweiterungen:

* [Verwenden Sie den Filter, um zu steuern, welche Benutzer in der Zeitleiste der Planung angezeigt werden.](#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline)
* [Benutzer bleiben nach der Zuweisung einer Aufgabe in der Timeline](#users-remain-on-the-timeline-after-being-assigned-a-task)

### Verwenden Sie den Filter, um zu steuern, welche Benutzer in der Zeitleiste der Planung angezeigt werden. {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

Der Filter kann jetzt verwendet werden, um zu steuern, welche Benutzer in der Planung angezeigt werden und welche Aufgaben und Probleme im Bereich Nicht zugewiesen angezeigt werden. Wenn Benutzer im Filter ausgewählt sind, werden nur die ausgewählten Benutzer angezeigt, unabhängig davon, ob sie über eine Rollenzuweisung verfügen, die der Rollenzuweisung für Aufgaben im Bereich Nicht zugewiesen entspricht. Alle Aufgaben, die diesem Benutzer derzeit zugewiesen sind, werden ebenfalls angezeigt.

Vor dieser Änderung kontrollierte der Filter nur, welche Aufgaben und Probleme im Bereich Nicht zugewiesen angezeigt wurden. Benutzer wurden nur dann in der Planung angezeigt, wenn der Benutzer der Rollenzuweisung einer Aufgabe im Bereich &quot;Nicht zugewiesen&quot;entsprach.

Weitere Informationen zur Verwendung des Filters, um zu steuern, was auf der Zeitleistensegment der Planung angezeigt wird, finden Sie unter  [Filtern von Informationen im Bereich &quot;Planung&quot;](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)und  [Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Benutzer bleiben nach der Zuweisung einer Aufgabe in der Timeline {#users-remain-on-the-timeline-after-being-assigned-a-task}

Benutzer verbleiben auf der Planung, nachdem ihnen eine Aufgabe oder ein Problem zugewiesen wurde, selbst wenn keine weiteren Aufgaben oder Probleme mit einer übereinstimmenden Rollenzuweisung vorhanden sind. Auf diese Weise können Sie alle erforderlichen Änderungen vornehmen, nachdem Benutzer zugewiesen wurden.

Vor dieser Änderung verschwanden die Benutzer unmittelbar nach der Zuweisung einer Aufgabe oder eines Problems aus der Planung, wenn keine weiteren Aufgaben oder Probleme im Bereich Nicht zugewiesen mit übereinstimmender Rollenzuweisung vorhanden waren.

Weitere Informationen finden Sie unter  [Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Anpassen der Workfront-Terminologie durch Ändern von Objektnamen

Sie können jetzt die Workfront-Terminologie anpassen, indem Sie die Namen bestimmter Objekte ändern.\
Mithilfe einer Layout-Vorlage können Sie jetzt die Namen der folgenden Arbeitsobjekte an die Anforderungen in Ihrer Organisation anpassen:

* Portfolio
* Programm
* Projekt
* Aufgabe
* Anfrage

Wenn Sie beispielsweise in Ihrer Organisation mit Kampagnen anstelle von Projekten arbeiten, können Sie den Namen des Objekts &quot;Projekt&quot;durch &quot;Kampagne&quot;ersetzen.

Wenn Sie diese Ersetzung vornehmen, wird in den folgenden Bereichen der Anwendung der aktualisierte Name der Objekte angezeigt:

* Globale Navigationsleiste
* Alle Registerkarten
* Alle Menüs 
* Berichterstellung und Berichterstellungselemente (Ansichten, Filter und Gruppierungen)
* Schaltflächen speichern
* Exportierte Dateien
* E-Mails

In den folgenden Bereichen wird der aktualisierte Name der Objekte nicht angezeigt:

* Ressourcenkalkulationen
* Ressourcen-Budgetmanager
* Kapazitätsplaner
* Ressourcenraster
* Team Builder
* Portfolio Optimizer 
* Mobile Apps
* Outlook-Add-in

Weitere Informationen zum Anpassen der Workfront-Terminologie mithilfe einer Layoutvorlage finden Sie im Abschnitt &quot;Anpassung der Terminologie&quot;unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;und im Abschnitt &quot;Auswirkungen des Anpassens von Objektnamen&quot;unter [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Aufnahme von Start- und Enddaten für die Genehmigung in Berichte

Beim Erstellen oder Ändern von Berichten können jetzt die folgenden Felder eingeschlossen werden:

* Genehmigungspfad – Startdatum
* Abschlussdatum des Genehmigungspfads

Mit diesen Feldern erhalten Sie einen Einblick in den Beginn des aktuellen oder letzten Genehmigungspfads und den Zeitpunkt, zu dem er als abgeschlossen markiert wurde.

Weitere Informationen zu diesen Feldern finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Weitere Informationen zu Validierungspfaden, ihrer Erstellung und Auslösung sowie zu den Funktionen, die sie in Genehmigungsprozessen verwenden, finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Die folgenden Felder wurden aus Workfront entfernt und können nicht mehr in Berichte aufgenommen werden (diese Felder enthielten Informationen zum Projekt und nicht Informationen über die Genehmigungen selbst, und wurden häufig falsch verwendet):

* Geplantes Anfangsdatum der Genehmigungen
* Voraussichtlicher Genehmigungsstarttermin
* Voraussichtlicher Genehmigungsstarttermin

## Neue E-Mail-Digest-Optionen für &quot;Anforderungen, die ich gestellt habe&quot;

Die Option Täglicher Digest-Versand wurde zum Bereich &quot;Anforderungen, die ich durchgeführt habe&quot;in Ihren Benachrichtigungseinstellungen hinzugefügt.

Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Aktualisierte E-Mail-Benachrichtigungen zur Dokumentgenehmigung

Das Erscheinungsbild der Benachrichtigung für &quot;Dokumentgenehmigung&quot;wurde mit einer neuen Benutzeroberfläche aktualisiert:

Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Verbesserungen in der Milestone-Ansicht

Die Meilensteinansicht, die beim Anzeigen einer Projektliste oder eines Projektberichts verfügbar ist, enthält jetzt die folgenden Verbesserungen:

* Geplante Datumswerte können bearbeitet werden
* Prozentualer Abschluss für Projekte und Aufgaben wird angezeigt

Vor dieser Änderung mussten Sie zur Änderung der Daten oder zum Anzeigen des Prozentsatzes zum Abschluss der einzelnen Aufgaben gehen.

Weitere Informationen finden Sie unter [Verwenden der Milestone-Ansicht](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
