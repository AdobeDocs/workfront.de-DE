---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 2-Release-Aktivität 2018.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2-Version 2018.3 verfügbar waren. Die Funktion ist ab dem 1. August 2018 in der Vorschau-Umgebung verfügbar. Verbesserungen der Testversand-Veröffentlichung mit Beta 2 werden am Mittwoch, 18. Juli in der Vorschau-Umgebung verfügbar sein. Sie wird im November 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Beta 2-Release-Aktivität 2018.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2-Version 2018.3 verfügbar waren. Die Funktion ist ab dem 1. August 2018 in der Vorschau-Umgebung verfügbar. Verbesserungen der Testversand-Veröffentlichung mit Beta 2 werden am Mittwoch, 18. Juli in der Vorschau-Umgebung verfügbar sein. Sie wird im November 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!NOTE]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.3 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

Die Beta 2-Version 2018.3 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [E-Mail-Adresse im Benutzerprofil als Gruppenadministrator aktualisieren](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Für alle Benutzer**

* [Anzeigen von mir im Startbereich delegierten Genehmigungen](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportieren von Daten für einen bestimmten Zeitraum im Ressourcen-Planer](#export-data-for-a-given-period-in-the-resource-planner)
* [Tägliche Gesamtwerte werden jetzt rot angezeigt, wenn der Benutzer übergeordnet ist](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Aufgaben und Probleme werden in der Zeitleiste der Planung ausgeblendet, wenn minimiert](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtern von Kommentaren und Antworten nach Benutzer im Testversand-Viewer](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Kommentar zu einem Bereich von Filmmaterial in einem Videoproof](#comment-on-a-range-of-footage-in-a-video-proof)
* [Neues Polyline-Tool für Kommentarmarkierung im Testversand-Viewer](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Flash-Entfernung für Bericht, Kalender und Dokumentfreigabe](#flash-removal-for-report-calendar-and-document-sharing)

## E-Mail-Adresse im Benutzerprofil als Gruppenadministrator aktualisieren {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Sie können jetzt E-Mail-Adressen für Benutzer aktualisieren, die zu einer von Ihnen verwalteten Gruppe gehören. 

Zuvor konnten nur Workfront-Administratoren E-Mail-Adressen für andere Benutzer aktualisieren. 

Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Anzeigen von an mich delegierten Genehmigungen im Startbereich {#view-approvals-delegated-to-me-in-the-home-area}

Sie können nun im Bereich &quot;Startseite&quot;die Ihnen zugewiesenen Projekt-, Aufgaben- und Problemgenehmigungen anzeigen.

Vor dieser Änderung konnten Sie delegierte Genehmigungen nur im Bereich Meine Arbeit anzeigen.

Weitere Informationen finden Sie unter [Genehmigungsanfrage delegieren](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Daten für einen bestimmten Zeitraum im Ressourcenplaner exportieren {#export-data-for-a-given-period-in-the-resource-planner}

Beim Export der Informationen im Ressourcenplaner wird jetzt ein neues Fenster angezeigt, in dem Sie einen bestimmten Zeitrahmen für die exportierte Datei auswählen können.

Vor dieser Verbesserung konnten Sie nur die auf dem Bildschirm angezeigten Informationen exportieren.

Weitere Informationen zum Exportieren von Daten aus dem Ressourcen-Planer finden Sie unter [Navigationsübersicht für Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) im Artikel [Navigationsübersicht für Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Tägliche Gesamtwerte werden jetzt rot angezeigt, wenn der Benutzer übergeordnet ist {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Wenn ein Benutzer übergeordnet ist, werden die täglichen Summen für die Tage, an denen der Benutzer übergeordnet ist, jetzt rot angezeigt. Diese Option wird nur angezeigt, wenn die Option Gesamt für täglich geplante Stunden anzeigen in den Einstellungen der Planungszeitleiste aktiviert ist. Vor dieser Verbesserung gab es einen roten Balken-Indikator für die Tage, an denen der Benutzer übergeordnet war. Die täglichen Summen wurden jedoch ohne rote Markierung angezeigt.

Weitere Informationen zu Benutzerzuweisungen finden Sie unter &quot;Verwalten von Benutzerzuweisungen in den Planungsbereichen&quot;.

## Aufgaben und Probleme werden in der Planung ausgeblendet, wenn sie minimiert werden {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Wenn Sie Aufgaben und Probleme in Ihrer Zeitleiste der Planung minimieren, werden diese nun für Benutzer und Rollen ausgeblendet, wenn in Ihren Einstellungen die Option Gesamtwerte der geplanten täglichen Stunden anzeigen aktiviert ist. Aufgaben und Probleme im Bereich Nicht zugewiesen werden in einer komprimierten Ansicht angezeigt.

Beim Minimieren von Aufgaben und Problemen blieben die Aufgaben und Probleme bisher für Benutzer und Rollen in der Zeitleiste der Planung, wurden jedoch in einer komprimierten Ansicht angezeigt.

Weitere Informationen zum Minimieren von Aufgaben und Problemen in der Planung finden Sie unter  &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Filtern von Kommentaren und Antworten nach Benutzer im Testversand-Viewer {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Jetzt können Sie Antworten einbeziehen, wenn Sie Kommentare von von Ihnen angegebenen Benutzern filtern. Dies ist nützlich, wenn Sie sich auf das gesamte Feedback konzentrieren möchten, das von einem wichtigen Validierer wie einem Kunden oder Projektmanager abgegeben wurde.

Zuvor war die Filterung nach Benutzer auf die Kommentare beschränkt, die von den von Ihnen angegebenen Validierungsverantwortlichen erstellt (gestartet) wurden.

## Kommentar zu einem Bereich von Filmmaterial in einem Videoproof {#comment-on-a-range-of-footage-in-a-video-proof}

Sie können einen Kommentar für eine Reihe von Aufnahmen in einem Videotest erstellen. Dies ist beispielsweise dann nützlich, wenn Sie angeben müssen, dass ein Segment von Filmmaterial neu erstellt oder entfernt werden muss.

Zuvor konnten Sie einen Kommentar nur für einen einzelnen Punkt auf einer Video-Timeline erstellen.

## Neues Polyline-Tool für Kommentar-Markup im Testversand-Viewer {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Jetzt können Sie mehrzeilige Markierungen verwenden, um segmentierte Linien und Formen zu zeichnen, wenn Sie einem Testversand einen Kommentar hinzufügen. Sie können eine geöffnete segmentierte Zeile oder eine geschlossene Form erstellen. Dieses Tool ist besonders bei der Arbeit mit komplexen Bildern nützlich, z. B. technischen oder architektonischen Bildern.

Beim Markieren eines Testversands zum Hinzufügen eines Kommentars konnten Sie zuvor ein Rechteck, eine gerade Linie, eine Freihand-Linie oder Form oder einen Pfeil zeichnen.

## Flash-Entfernung für Bericht, Kalender und Dokumentfreigabe {#flash-removal-for-report-calendar-and-document-sharing}

Wir haben Flash aus den folgenden Dialogfeldern für die Freigabe in Workfront entfernt:

* Berichte
* Kalender
* Dokumente

Sie können diese Objekte weiterhin wie bisher freigeben, aber das Erlebnis verlässt sich jetzt nicht mehr auf Flash.
