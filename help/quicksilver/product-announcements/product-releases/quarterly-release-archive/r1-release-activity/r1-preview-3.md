---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1-Vorschau 3
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der Version R1.3 verfügbar sind. Die Funktion auf dieser Seite wurde am 1. Februar 2017 in der Vorschau-Umgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# R1-Vorschau 3

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der Version R1.3 verfügbar sind. Die Funktion auf dieser Seite wurde am 1. Februar 2017 in der Vorschau-Umgebung verfügbar gemacht.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [R1-Versionsaktivität - Übersicht](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Verbessertes Verfahren zum Verknüpfen externer Dateien

Die Option zum Verknüpfen von Dokumenten aus einer externen Quelle (z. B. Google Drive, Box, Dropbox usw.) befindet sich jetzt an einer prominenteren Stelle im Bereich Dokumente . 

Darüber hinaus ist die Aktion, einen Dokumentanbieter vor der erstmaligen Verknüpfung von Dateien von diesem Anbieter zu autorisieren, jetzt intuitiver (es ist einfach ein zusätzlicher Schritt beim Verknüpfen von Dateien von einem externen Anbieter).

Vor diesen Änderungen befand sich die Option zum Verknüpfen von Dateien aus einer externen Quelle im Dialogfeld Dokumente hinzufügen im Bereich Dokumente . Vor dem erstmaligen Verknüpfen eines Dokuments aus einer externen Quelle musste der Benutzer, der das Dokument verknüpft, diesen Dokumentanbieter im Bereich „Setup“ autorisieren.

Weitere Informationen finden Sie unter  [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Aktualisiertes Team, das am Kalender arbeitet

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Der für Teams verfügbare Arbeitskalender enthält jetzt zusätzliche Funktionen und ein aktualisiertes Erscheinungsbild. Das Team, das im Kalender arbeitet, funktioniert jetzt ähnlich wie das Tool zur Ressourcenplanung für Projekte.

Der aktualisierte Kalender des Team-Arbeitskalenders enthält die folgenden Verbesserungen:

* Benutzer alphabetisch oder nach Rolle gruppiert anzeigen.
* Filtern Sie die Zeitleiste nach Projektprioritäten, Status und einzelnen Projekten. Sie können die Zeitleiste auch nach Rollen und Benutzern filtern. (Der Filterbereich enthält weniger Optionen als bei der Planung von Ressourcen für Projekte.)
* Probleme in die Zeitplanung einbeziehen.
* Zeigen Sie Benutzerzuweisungen an und ändern Sie die Anzahl der Stunden, die Benutzenden bestimmten Aufgaben und Problemen pro Tag zugewiesen sind.
* Anzeigen von Indikatoren, die anzeigen, wenn Benutzende an einem bestimmten Tag überlastet sind.
* Konfigurieren Sie, ob abgeschlossene Arbeiten in der Zeitplanleiste angezeigt werden.

Unterschiede zum Tool Ressourcenplanung bei der Planung von Ressourcen für Projekte:

* Alle Team-Mitglieder werden im Kalender Team-Arbeit an angezeigt.\
  Bei der Planung von Ressourcen für Projekte werden nur Benutzer angezeigt, denen eine Rolle zugeordnet ist, die einer Rolle von einer oder mehreren Aufgaben im Bereich Nicht zugewiesen entspricht.
* Das Swap-Tool ist nicht verfügbar und ist nicht im Team-Arbeitskalender enthalten.
* Jedes Teammitglied kann Änderungen am Arbeitskalender des Teams vornehmen.\
  Bei der Planung von Ressourcen für Projekte können nur Ressourcenmanager Ressourcenentscheidungen für das Projekt treffen.
* Probleme werden standardmäßig im Kalender des Teams angezeigt, das an ihnen arbeitet.\
  Beim Planen von Ressourcen für Projekte werden Probleme nicht standardmäßig angezeigt.

Weitere Informationen zur Verwendung des aktualisierten Kalenders für Team-Arbeitsaufgaben finden Sie unter „Ressourcenplanung“.

## Verbesserungen der Ressourcenplanung

Die Zeitplanung umfasst die folgenden Verbesserungen:

* „Verwenden Sie den Filter, um zu steuern, welche Benutzer in der Zeitplanleiste angezeigt werden.“
* „Benutzende bleiben nach dem Zuweisen einer Aufgabe in der Zeitleiste“

### Verwenden Sie den Filter, um zu steuern, welche Benutzer in der Zeitplanleiste angezeigt werden {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Mit dem Filter können Sie jetzt steuern, welche Benutzenden in der Zeitplanleiste angezeigt werden und welche Aufgaben und Probleme im Bereich Nicht zugewiesen angezeigt werden. Wenn Benutzende im Filter ausgewählt sind, werden nur die von Ihnen ausgewählten Benutzenden angezeigt, unabhängig davon, ob sie über eine Rollenzuweisung verfügen, die der Rollenzuweisung von Aufgaben im Bereich „Nicht zugewiesen“ entspricht. Alle Aufgaben, die diesem Benutzer derzeit zugewiesen sind, werden ebenfalls angezeigt.

Vor dieser Änderung hat der Filter nur gesteuert, welche Aufgaben und Probleme im Bereich Nicht zugewiesen angezeigt wurden. Benutzende wurden nur dann in der Zeitplanleiste angezeigt, wenn der/die Benutzende mit der Rollenzuweisung einer Aufgabe im Bereich Nicht zugewiesen übereingestimmt hat.

Weitere Informationen zur Verwendung des Filters zur Steuerung dessen, was auf der Zeitplanübersicht angezeigt wird, finden Sie unter „Informationen im Zeitplanbereich filtern“ und „Nicht zugewiesene Aufgaben und Probleme in den Zeitplanbereichen manuell zuweisen“.

### Benutzer bleiben auf der Zeitleiste, nachdem sie einer Aufgabe zugewiesen wurden {#users-remain-on-the-timeline-after-being-assigned-a-task}

Benutzer bleiben auch dann in der Zeitleiste für die Planung, wenn ihnen eine Aufgabe oder ein Problem zugewiesen wurde, selbst wenn es keine verbleibenden Aufgaben oder Probleme gibt, denen eine entsprechende Rollenzuweisung zugewiesen wurde. Auf diese Weise können Sie nach der Zuweisung von Benutzern alle erforderlichen Änderungen vornehmen.

Vor dieser Änderung verschwanden Benutzer unmittelbar nach der Zuweisung einer Aufgabe oder eines Problems aus der Zeitplanleiste, wenn im Bereich Nicht zugewiesen mit einer entsprechenden Rollenzuweisung keine verbleibenden Aufgaben oder Probleme mehr vorhanden waren.

Weitere Informationen finden Sie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“.

## Anpassen der Workfront-Terminologie durch Ändern von Objektnamen

Sie können die Terminologie von Workfront jetzt anpassen, indem Sie die Namen bestimmter Objekte ändern.\
Mithilfe einer Layout-Vorlage können Sie jetzt die Namen der folgenden Arbeitsobjekte ändern, um sie an die Anforderungen in Ihrem Unternehmen anzupassen:

* Portfolio
* Programm
* Projekt
* Aufgabe
* Problem

Wenn Sie in Ihrer Organisation beispielsweise mit Kampagnen anstelle von Projekten arbeiten, können Sie den Namen des Objekts „Projekt“ durch „Kampagne“ ersetzen.

Wenn Sie diese Ersetzung vornehmen, wird in den folgenden Bereichen der Anwendung der aktualisierte Name der Objekte angezeigt:

* Globale Navigationsleiste
* Alle Registerkarten
* Alle Menüs 
* Report Builder- und Berichterstellungselemente (Ansichten, Filter und Gruppierungen)
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

Weitere Informationen zum Anpassen der Workfront-Terminologie mithilfe einer Layout-Vorlage finden Sie im Abschnitt „Anpassen der Terminologie“ in „Erstellen und Verwalten von Layout-Vorlagen“ und im Abschnitt „Auswirkungen der Anpassung von Objektnamen“ in [Grundlegendes zu Objekten in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Start- und Enddatum der Genehmigung in Berichte einschließen

Beim Erstellen oder Ändern von Berichten können Sie jetzt die folgenden Felder einbeziehen:

* Genehmigungspfad – Startdatum
* Genehmigungspfad - Abschlussdatum

In diesen Feldern können Sie sehen, wann der aktuelle oder letzte Genehmigungspfad gestartet und als abgeschlossen markiert wurde.

Weitere Informationen zu diesen Feldern finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Weitere Informationen zu Validierungspfaden, wie sie erstellt und ausgelöst werden und welche Funktion sie in Validierungsprozessen erfüllen, finden Sie unter [Erstellen eines Validierungsprozesses für Arbeitselemente](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Die folgenden Felder wurden aus Workfront entfernt und können nicht mehr in Berichte aufgenommen werden (diese Felder enthielten Informationen über das Projekt anstatt Informationen über die Genehmigungen selbst und wurden oft missbraucht):

* Validierungen geplantes Startdatum
* Voraussichtlicher Genehmigungsstarttermin
* Voraussichtlicher Genehmigungsstarttermin

## Neue E-Mail-Digest-Optionen für „Von mir eingereichte Anfragen“

Die Option Täglicher Digest-Versand wurde zum Bereich „Von mir durchgeführte Anfragen“ in Ihren Benachrichtigungseinstellungen hinzugefügt.

Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Aktualisiertes Erscheinungsbild der E-Mail-Benachrichtigungen zur Dokumentgenehmigung

Das Erscheinungsbild der Benachrichtigung für die „Dokumentgenehmigung“ wurde mit einer neuen Benutzeroberfläche aktualisiert:

Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [Adobe Workfront-](../../../../workfront-basics/using-notifications/wf-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Verbesserungen in der Meilenstein -Ansicht

Die Meilenstein -Ansicht, die beim Anzeigen einer Projektliste oder eines Projektberichts verfügbar ist, enthält jetzt die folgenden Verbesserungen:

* Geplante Termine können bearbeitet werden
* Prozent abgeschlossen für Projekte und Aufgaben wird angezeigt

Um vor dieser Änderung die Daten bearbeiten oder den abgeschlossenen Prozentsatz anzeigen zu können, mussten Sie zu der einzelnen Aufgabe gehen.

Weitere Informationen finden Sie unter [Verwenden der Meilenstein -Ansicht](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
