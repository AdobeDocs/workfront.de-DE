---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 1 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 1 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 10. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Versionsaktivität von Beta 1 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 1 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 10. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Die Beta-Version 2017.2 1 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren:**

* [Dokumente wiederherstellen](#restore-documents)
* [Neues Vorschau-Banner mit Versionsinformationen](#new-preview-banner-with-release-information) 
* [API 7-Verfügbarkeit](#api-7-availability)

**Für alle Benutzer:**

* [Abonnieren von Aufgaben und Problemen](#subscribe-to-tasks-and-issues)
* [Verbesserungen bei der Ressourcenplanung](#resource-scheduling-improvements)
* [Korrekturabzüge vergleichen](#compare-proofs)
* [Neues Feld für Ressourcenpools für Benutzer und Projekte](#new-field-for-resource-pools-for-users-and-projects)
* [Aktualisiertes Erscheinungsbild in der Dashboard-Liste](#updated-look-and-feel-in-the-dashboard-list)
* [Entfernen der Funktion „Empfehlungen“ in Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Spalten in beliebigen Listen per Drag-and-Drop neu anordnen (Funktion wird entfernt)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Dokumente wiederherstellen {#restore-documents}

Workfront-Admins können jetzt einzelne Dokumente wiederherstellen, die in den letzten 30 Tagen gelöscht wurden. 

Vor dieser Änderung konnten Workfront-Administratoren nur Projekte, Aufgaben und Probleme wiederherstellen (einschließlich Dokumente, die im Zusammenhang mit dem gelöschten Projekt, der gelöschten Aufgabe oder dem gelöschten Problem gelöscht wurden).

Weitere Informationen finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Neues Vorschau-Banner mit Versionsinformationen {#new-preview-banner-with-release-information}

Das blaue Banner oben in der Sandbox-Vorschau-Umgebung zeigt jetzt den Versionsnamen und die Versionsnummer der Vorschau-Umgebung an. Wenn Sie auf den Namen der Version klicken, gelangen Sie zu einem Hilfeartikel, in dem Sie weitere Informationen zur aktuellen Vorschau-Version finden. Weitere Informationen zur Sandbox-Vorschau-Umgebung finden Sie unter [Die Sandbox-Vorschau-Umgebung von Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## API 7-Verfügbarkeit {#api-7-availability}

API 7 ist jetzt verfügbar und enthält neue und aktualisierte Objekte.

Weitere Informationen finden Sie unter [Neue Funktionen in der API-Version 7](../../../../wf-api/api/new-api-version-7.md).

## Aufgaben und Probleme abonnieren {#subscribe-to-tasks-and-issues}

Workfront sendet Benachrichtigungen zu Elementen, die Ihnen zugewiesen sind oder deren Inhaber Sie sind.

Ab der aktuellen Version können Sie Elemente abonnieren, die Ihnen nicht zugewiesen sind, sich aber auf Ihre Arbeit auswirken können.

Sie können Probleme und Aufgaben abonnieren, für die Sie zumindest über die Berechtigung „Anzeigen“ verfügen. Wenn dem Problem oder der Aufgabe, das bzw. die Sie abonniert haben, ein neuer Kommentar hinzugefügt wird, werden Sie per E-Mail über diesen Kommentar informiert.

Weitere Informationen zum Abonnieren von Problemen und Aufgaben finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Verbesserungen bei der Ressourcenplanung {#resource-scheduling-improvements}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Die folgenden Verbesserungen sind bei der Planung von Ressourcen verfügbar:

* [Zeigen Sie weitere Elemente in der Zeitleiste für die Ressourcenplanung in einer einzigen Ansicht an](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Konfigurieren Sie den Projektnamen, der in der Zeitplanleiste bei Aufgaben und Problemen angezeigt werden soll](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Konfigurieren, ob übergeordnete Aufgaben in der Zeitleiste angezeigt werden](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Alle Aufgaben und Probleme in der Zeitplanung können einfacher ein- oder ausgeblendet werden](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Rollen- und Benutzerinformationen verbleiben beim Scrollen oben in der Zeitplanleiste](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Weitere Elemente in der Zeitleiste für die Ressourcenplanung in einer einzigen Ansicht anzeigen {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Bei der Planung von Ressourcen für ein Team oder für Projekte, für die Sie der Ressourcen-Manager sind, verbrauchen Aufgaben und Probleme jetzt weniger vertikalen Platz auf der Zeitplanleiste. Auf diese Weise können Sie weitere Aufgaben und Probleme in einer einzigen Ansicht anzeigen.

Wenn Sie sich entscheiden, Projektnamen für jede Aufgabe und jedes Problem auf der Zeitleiste für die Planung anzuzeigen, wird der vertikale Raum für jede Aufgabe und jedes Problem erweitert, sodass weniger Aufgaben und Probleme in einer einzigen Ansicht angezeigt werden.

Weitere Informationen zur Ressourcenplanung finden Sie unter  „Erste Schritte mit der Ressourcenplanung“.

### Projektname konfigurieren, der bei Aufgaben und Problemen in der Zeitplanleiste angezeigt werden soll {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Bei der Planung von Ressourcen für ein Team oder für Projekte, für die Sie der Ressourcen-Manager sind, können Sie jetzt den Projektnamen konfigurieren, der bei jeder Aufgabe und jedem Problem in der Zeitplanung angezeigt werden soll. Dadurch können Benutzer die Zeitleiste der Planung anzeigen, um den Namen des Projekts, in dem sich die Aufgabe oder das Problem befindet, schnell anzuzeigen.

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

### Konfigurieren, ob übergeordnete Aufgaben in der Zeitplanleiste angezeigt werden {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Beim Planen von Ressourcen für Projekte, für die Sie der Ressourcen-Manager sind, können Sie jetzt konfigurieren, ob übergeordnete Vorgänge in der Zeitleiste angezeigt werden, wenn die Option „Zusammenfassung - Fertigstellungsmodus“ im Projekt auf „Manuell“ gesetzt ist.

Vor dieser Änderung werden übergeordnete Aufgaben immer auf der Zeitleiste für die Planung angezeigt, wenn der Fertigstellungsmodus Zusammenfassung für das Projekt auf Manuell festgelegt wurde. 

Wenn der Zusammenfassungs-Fertigstellungsmodus für das Projekt auf „Automatisch“ festgelegt ist, können übergeordnete Aufgaben nicht in der Zeitplanleiste angezeigt werden. Dieses Erlebnis hat sich nicht geändert.

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

### Einfacheres Ein- oder Ausblenden aller Aufgaben und Probleme in der Zeitplanleiste {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Es ist ein neuer Link verfügbar, mit dem Sie alle Aufgaben und Probleme in der Zeitplanleiste leichter reduzieren können.

Weitere Informationen finden Sie unter Erste Schritte mit der Ressourcenplanung .

### Rollen- und Benutzerinformationen verbleiben beim Scrollen oben in der Zeitplanleiste {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Wenn Sie nun in der Zeitplanleiste nach unten scrollen, um zusätzliche Informationen anzuzeigen, bleiben der Rollenname und der Benutzername in der Zeitplanleiste im Bereich „Benutzer und Rollen“ oben. So können Sie leichter erkennen, mit welchem Benutzer und welcher Rolle die Aufgaben und Probleme verbunden sind.

Vor dieser Änderung wurden der Rollen- und der Benutzername aus der aktuellen Ansicht gescrollt.

Weitere Informationen zur Ressourcenplanung finden Sie unter  „Erste Schritte mit der Ressourcenplanung“.

## Korrekturabzüge vergleichen {#compare-proofs}

Sie können jetzt zwei Korrekturabzüge innerhalb einer einzigen Dokumentliste vergleichen, z. B. auf der Registerkarte Dokumente in einem Projekt, einer Aufgabe, einem Problem, einem Portfolio oder im Hauptbereich Dokumente in der globalen Navigationsleiste. 

Die beiden Korrekturabzüge werden im Prüfungs- und Genehmigungs-Tool angezeigt, und Sie können jedes Dokument prüfen und gleichzeitig in einer Ansicht vergleichen.

Weitere Informationen finden Sie unter [Testsendungen vergleichen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Neues Feld für Ressourcenpools für Benutzer und Projekte {#new-field-for-resource-pools-for-users-and-projects}

Mit der Version R1.5 wurden neue Funktionen rund um die Ressourcenplanung in die Vorschau-Umgebung eingeführt. Mit dieser Funktion können Sie neue Ressourcenpools erstellen, bei denen es sich um Sammlungen von Benutzern handelt.

Jetzt können Sie diese Ressourcenpools mit Projekten sowie mit Benutzern verknüpfen. Im Projekt sowie im Benutzerobjekt wird jetzt ein neues Feld mit dem Namen „Ressourcenpools“ angezeigt.

Weitere Informationen zu den neuen Ressourcenpools und dazu, wie sie mit Projekten und Benutzern verknüpft werden können, finden Sie unter [Ressourcenpools - Übersicht](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Aktualisiertes Erscheinungsbild in der Dashboard-Liste {#updated-look-and-feel-in-the-dashboard-list}

Beim Anzeigen einer Dashboard-Liste ist das Erscheinungsbild jetzt moderner und skalierbarer.

Diese Funktion war bisher nur für Benutzer verfügbar, die für Early Access registriert waren. Dies ist jetzt für alle Benutzer in der Vorschau-Umgebung verfügbar. Sie wird mit Version 2017.2 für alle Benutzer in der Produktionsumgebung verfügbar gemacht. 

Weitere Informationen zu Dashboards finden Sie unter [Erstellen eines Dashboards](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Entfernen der Funktion „Empfehlungen“ in Workfront {#removing-the-endorsements-functionality-in-workfront}

Bei der Bewertung der im Aktualisierungsverlauf enthaltenen Funktionen haben wir festgestellt, dass Empfehlungen eine geringe Akzeptanz und eine wenig genutzte Funktion darstellen. Ab Version 2017.2 werden die folgenden Funktionen rund um Empfehlungen aus Workfront entfernt (diese Funktion ist in der Vorschau nicht mehr verfügbar):

* die Registerkarte „Empfehlungen“ im Bereich „Benutzerprofil“;
* Das Objekt der Empfehlung wird aus dem API-Explorer entfernt. Wenn Sie derzeit API-Berichte für die Objekte „Empfehlung“ oder „Empfehlung-Freigabe“ abrufen, sind die Aufrufe nach dem Entfernen dieses Objekts ungültig.

Die folgenden Funktionen bleiben weiterhin in der Web-Anwendung verfügbar:

* Die Empfehlung eines Benutzers durch einen anderen Benutzer, die vor der Entfernung dieser Funktion vorgenommen wurde, verbleibt im Aktualisierungsverlauf des Indossanten. 

Empfehlungen waren kein berichtspflichtiges Objekt, daher gibt es keine Änderungen rund um das Reporting für dieses Objekt.

## Spalten in beliebigen Listen per Drag-and-Drop neu anordnen (Funktion wird entfernt) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

Die Funktion zum Ändern der Spaltenreihenfolge in einer Liste durch Ziehen einer Spalte von einer Position und Ablegen an einer anderen Position wird mit der Version 2017.2 aus dem vorzeitigen Zugriff in der Produktionsumgebung entfernt und steht Benutzern nicht mehr zur Verfügung. 

Weitere Informationen zu dieser Funktion finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
