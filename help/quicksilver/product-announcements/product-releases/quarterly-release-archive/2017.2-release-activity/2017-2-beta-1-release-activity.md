---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 1-Release-Aktivität 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit der Beta 1-Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 10. Mai 2017 in der Vorschau-Umgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Beta 1-Release-Aktivität 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit der Beta 1-Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 10. Mai 2017 in der Vorschau-Umgebung bereitgestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Die Version 2017.2 von Beta 1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren:**

* [Dokumente wiederherstellen](#restore-documents)
* [Neues Vorschau-Banner mit Versionsinformationen](#new-preview-banner-with-release-information) 
* [API 7-Verfügbarkeit](#api-7-availability)

**Für alle Benutzer:**

* [Abonnieren von Aufgaben und Problemen](#subscribe-to-tasks-and-issues)
* [Verbesserungen bei der Ressourcenplanung](#resource-scheduling-improvements)
* [Testsendungen vergleichen](#compare-proofs)
* [Neues Feld für Ressourcen-Pools für Benutzer und Projekte](#new-field-for-resource-pools-for-users-and-projects)
* [Aktualisiertes Erscheinungsbild in der Dashboard-Liste](#updated-look-and-feel-in-the-dashboard-list)
* [Entfernen der Funktionalität &quot;Endormente&quot;in Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Neuanordnen von Spalten in einer Liste mit Drag &amp; Drop (Funktion wird entfernt)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Dokumente wiederherstellen {#restore-documents}

Workfront-Administratoren können jetzt einzelne Dokumente wiederherstellen, die innerhalb der letzten 30 Tage gelöscht wurden. 

Vor dieser Änderung konnten Workfront-Administratoren nur Projekte, Aufgaben und Probleme wiederherstellen (einschließlich Dokumenten, die in Verbindung mit dem gelöschten Projekt, der gelöschten Aufgabe oder dem gelöschten Problem gelöscht wurden).

Weitere Informationen finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Neues Vorschau-Banner mit Versionsinformationen {#new-preview-banner-with-release-information}

Das blaue Banner oben in der Sandbox-Vorschau-Umgebung zeigt jetzt den Versionsnamen und die Versionsnummer der Vorschau-Umgebung an. Wenn Sie auf den Namen der Version klicken, gelangen Sie zu einem Artikel der Hilfe-Site, in dem Sie weitere Informationen zur aktuellen Vorschau-Version finden. Weitere Informationen zur Vorschau-Sandbox-Umgebung finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## API 7-Verfügbarkeit {#api-7-availability}

API 7 ist jetzt verfügbar und enthält neue und aktualisierte Objekte.

Weitere Informationen finden Sie unter [Neue Funktionen in API-Version 7](../../../../wf-api/api/new-api-version-7.md).

## Abonnieren von Aufgaben und Problemen {#subscribe-to-tasks-and-issues}

Workfront sendet Benachrichtigungen über Elemente, die Sie zugewiesen sind oder deren Inhaber Sie sind.

Ab der aktuellen Version können Sie diese abonnieren, wenn Sie Artikel verfolgen möchten, die Ihnen nicht zugewiesen sind, sich aber auf Ihre Arbeit auswirken können.

Sie können Probleme und Aufgaben abonnieren, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen. Wenn dem von Ihnen abonnierten Problem oder der Aufgabe ein neuer Kommentar hinzugefügt wird, werden Sie in einer E-Mail über diesen Kommentar benachrichtigt.

Weitere Informationen zum Abonnieren von Problemen und Aufgaben finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Verbesserungen bei der Ressourcenplanung {#resource-scheduling-improvements}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Die folgenden Verbesserungen sind bei der Planung von Ressourcen verfügbar:

* [Anzeigen weiterer Elemente in der Zeitleiste für die Ressourcenplanung in einer Einzelansicht](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Konfigurieren Sie den Projektnamen für die Anzeige bei Aufgaben und Problemen in der Zeitleiste für die Planung](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Konfigurieren, ob übergeordnete Aufgaben in der Zeitleiste für die Planung angezeigt werden](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [ Einfaches Erweitern oder Reduzieren aller Aufgaben und Probleme in der Planung](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [Rolle und Benutzerinformationen bleiben beim Bildlauf oben in der Zeitleiste für die Planung](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Anzeigen von mehr Elementen in der Zeitleiste für die Ressourcenplanung in einer Einzelansicht {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Beim Planen von Ressourcen für ein Team oder für Projekte, für die Sie der Ressourcen-Manager sind, verbrauchen Aufgaben und Probleme jetzt weniger vertikalen Speicherplatz in der Zeitleiste der Planung. Dadurch können Sie mehr Aufgaben und Probleme in einer einzigen Ansicht sehen.

Wenn Sie sich dazu entscheiden, Projektnamen für jede Aufgabe und jedes Problem in der Planung anzuzeigen, wird der vertikale Bereich jeder Aufgabe und jedes Problems erweitert, was zu weniger Aufgaben und Problemen in einer einzigen Ansicht führt.

Weitere Informationen zur Planung von Ressourcen finden Sie unter  &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Konfigurieren Sie den Projektnamen für die Anzeige bei Aufgaben und Problemen in der Zeitleiste für die Planung. {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Beim Planen von Ressourcen für ein Team oder für Projekte, für die Sie der Ressourcen-Manager sind, können Sie jetzt den Projektnamen so konfigurieren, dass er für jede Aufgabe und jedes Problem in der Planung angezeigt wird. Auf diese Weise können Benutzer, die sich die Planung ansehen, schnell den Namen des Projekts anzeigen, in dem sich die Aufgabe oder das Problem befindet.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Konfigurieren, ob übergeordnete Aufgaben in der Zeitleiste für die Planung angezeigt werden {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Beim Planen von Ressourcen für Projekte, für die Sie der Ressourcen-Manager sind, können Sie jetzt konfigurieren, ob die übergeordneten Aufgaben in der Planung angezeigt werden, wenn die Option Zusammenfassungsabschlussmodus im Projekt auf Manuell eingestellt ist.

Vor dieser Änderung wurden übergeordnete Aufgaben immer in der Zeitleiste der Planung angezeigt, wenn für den Modus &quot;Zusammenfassender Abschluss&quot;des Projekts &quot;Manuell&quot;ausgewählt wurde. 

Wenn der Zusammenfassungsabschlussmodus im Projekt auf Automatisch eingestellt ist, können übergeordnete Aufgaben nicht auf der Zeitleiste der Planung angezeigt werden. Dieses Erlebnis hat sich nicht geändert.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Einfaches Erweitern oder Reduzieren aller Aufgaben und Probleme in der Zeitleiste für die Planung {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Es steht ein neuer Link zur Verfügung, über den Sie mühelos alle Aufgaben und Probleme in der Planung reduzieren können.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

### Rolle und Benutzerinformationen bleiben beim Bildlauf oben in der Zeitleiste für die Planung {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Wenn Sie jetzt nach unten scrollen, um zusätzliche Informationen anzuzeigen, bleiben der Rollenname und der Benutzername oben im Bereich &quot;Benutzer und Rollen&quot;in der Zeitleiste der Planung, wodurch leichter erkennbar ist, mit welchem Benutzer und welcher Rolle die Aufgaben und Probleme verbunden sind.

Vor dieser Änderung scrollen der Rollenname und der Benutzername aus der aktuellen Ansicht hervor.

Weitere Informationen zur Planung von Ressourcen finden Sie unter  &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Testsendungen vergleichen {#compare-proofs}

Sie können jetzt zwei Dokumentenprüfungen in einer beliebigen Dokumentliste vergleichen, z. B. auf der Registerkarte &quot;Dokumente&quot;in einem Projekt, einer Aufgabe, einem Problem, einem Portfolio oder im Hauptbereich &quot;Dokumente&quot;in der globalen Navigationsleiste. 

Die beiden Testsendungen werden im Tool &quot;Überprüfen und Validieren&quot;angezeigt. Sie können jedes Dokument prüfen und dabei nebeneinander darstellen.

Weitere Informationen finden Sie unter [Testsendungen vergleichen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Neues Feld für Ressourcen-Pools für Benutzer und Projekte {#new-field-for-resource-pools-for-users-and-projects}

Mit der Version R1.5 wurden neue Funktionen rund um die Ressourcenplanung in die Vorschauumgebung eingeführt. Mit dieser Funktion können Sie neue Ressourcen-Pools erstellen, bei denen es sich um Sammlungen von Benutzern handelt.

Jetzt können Sie diese Ressourcen-Pools mit Projekten sowie mit Benutzern verknüpfen. Jetzt wird ein neues Feld namens &quot;Resource Pools&quot;im Projekt sowie im Benutzerobjekt angezeigt.

Weitere Informationen zu den neuen Ressourcenpools und dazu, wie sie mit Projekten und Benutzern verknüpft werden können, finden Sie unter [Überblick über Ressourcenpools](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md) .

## Die Anzeige in der Dashboard-Liste wurde aktualisiert. {#updated-look-and-feel-in-the-dashboard-list}

Beim Anzeigen einer Dashboard-Liste ist das Erscheinungsbild jetzt moderner und skalierbarer.

Diese Funktion war bisher nur für Benutzer verfügbar, die sich für Early Access angemeldet haben. Dieser ist jetzt für alle Benutzer in der Vorschauumgebung verfügbar. Mit Version 2017.2 wird sie allen Benutzern in der Produktionsumgebung zur Verfügung gestellt. 

Weitere Informationen zu Dashboards finden Sie unter [Dashboard erstellen](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Entfernen der Funktionalität &quot;Endormente&quot;in Workfront {#removing-the-endorsements-functionality-in-workfront}

Bei der Bewertung der im Aktualisierungsstream enthaltenen Funktionen haben wir festgestellt, dass Endorsements nur eine geringe Akzeptanz und nur eine geringe Nutzung aufweisen. In Version 2017.2 werden ab Version 2017.2 die folgenden Funktionen rund um Endorsements aus Workfront entfernt (diese Funktion ist in der Vorschau nicht mehr verfügbar):

* die Registerkarte &quot;Endorsements&quot;im Benutzerprofilbereich;
* Das Objekt &quot;Endorsements&quot;wird aus dem API-Explorer entfernt. Wenn Sie derzeit API-Berichte für die Objekte &quot;Endorsement&quot;oder &quot;Endorsement Share&quot;abrufen, sind die Aufrufe nach dem Entfernen dieses Objekts ungültig.

Die folgenden Funktionen bleiben weiterhin in der Webanwendung:

* Die Unterstützung eines Benutzers durch einen anderen Benutzer, der vor der Entfernung dieser Funktion erfolgte, verbleibt im aktualisierten Stream des Endnutzers. 

Endorsements waren kein berichtspflichtiges Objekt, daher gibt es keine Änderungen an der Berichterstellung für dieses Objekt.

## Neuanordnen von Spalten in einer Liste mit Drag &amp; Drop (Funktion wird entfernt) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

Die Funktion zum Ändern der Reihenfolge der Spalten in einer Liste durch Ziehen einer Spalte von einer Position an eine andere wird mit Version 2017.2 von der Option Early Access in der Produktionsumgebung entfernt und steht für Benutzer nicht mehr zur Verfügung. 

Weitere Informationen zu dieser Funktion finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
