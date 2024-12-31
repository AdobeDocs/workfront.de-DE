---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 2 2018.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.3 verfügbar waren. Die Funktion ist ab dem 1. August 2018 in der Vorschau-Umgebung verfügbar. Die mit Beta 2 veröffentlichten Proofing-Verbesserungen sind ab Mittwoch, 18. Juli in der Vorschau-Umgebung verfügbar. Sie wird im November 2018 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Versionsaktivität von Beta 2 2018.3

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.3 verfügbar waren. Die Funktion ist ab dem 1. August 2018 in der Vorschau-Umgebung verfügbar. Die mit Beta 2 veröffentlichten Proofing-Verbesserungen sind ab Mittwoch, 18. Juli in der Vorschau-Umgebung verfügbar. Sie wird im November 2018 in der Produktionsumgebung bereitgestellt.

>[!NOTE]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.3 finden Sie unter  [Übersicht über die Versionsaktivität 2018.3](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

Die Beta-Version 2018.3 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren**

* [Aktualisieren der E-Mail-Adresse im Benutzerprofil als Gruppenadministrator](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**Für alle Benutzer**

* [An mich delegierte Genehmigungen im Bereich „Startseite“ anzeigen](#view-approvals-delegated-to-me-in-the-home-area)
* [Exportieren von Daten für einen bestimmten Zeitraum im Ressourcenplaner](#export-data-for-a-given-period-in-the-resource-planner)
* [Die Tagessummen werden jetzt rot angezeigt, wenn die Benutzerzuordnung überlastet ist](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [Aufgaben und Probleme werden auf der Zeitplanleiste ausgeblendet, wenn sie minimiert werden](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [Filtern von Kommentaren und Antworten nach Benutzer im Proofing Viewer](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [Kommentar zu einer Reihe von Aufnahmen in einem Videobeweis](#comment-on-a-range-of-footage-in-a-video-proof)
* [Neues Mehrzeilenwerkzeug für Kommentar-Markup im Proofing Viewer](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [Flash-Entfernung für die Freigabe von Berichten, Kalendern und Dokumenten](#flash-removal-for-report-calendar-and-document-sharing)

## Aktualisieren der E-Mail-Adresse im Benutzerprofil als Gruppenadministrator {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

Sie können jetzt die E-Mail-Adressen von Benutzern aktualisieren, die zu einer von Ihnen verwalteten Gruppe gehören. 

Zuvor konnten nur Workfront-Administratoren die E-Mail-Adressen für andere Benutzer aktualisieren. 

Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## An mich delegierte Genehmigungen im Bereich Startseite anzeigen {#view-approvals-delegated-to-me-in-the-home-area}

Sie können jetzt den Bereich Startseite verwenden, um an Sie delegierte Projekt-, Aufgaben- und Problem-Genehmigungen anzuzeigen.

Vor dieser Änderung konnten Sie delegierte Genehmigungen nur im Bereich Meine Arbeit anzeigen.

Weitere Informationen finden Sie unter [Delegieren einer Genehmigungsanfrage](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

## Exportieren von Daten für einen bestimmten Zeitraum im Ressourcenplaner {#export-data-for-a-given-period-in-the-resource-planner}

Beim Exportieren der Informationen im Ressourcenplaner wird jetzt ein neues Fenster angezeigt, in dem Sie einen bestimmten Zeitrahmen für Ihre exportierte Datei auswählen können.

Vor dieser Verbesserung konnten Sie nur die auf dem Bildschirm angezeigten Informationen exportieren.

Weitere Informationen zum Exportieren von Daten aus dem Ressourcenplaner finden Sie unter [Übersicht über die Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md) im Artikel [Übersicht über die Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Die täglichen Gesamtwerte werden jetzt rot angezeigt, wenn die Benutzerin oder der Benutzer eine Überallokation aufweist {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Wenn eine Benutzerin oder ein Benutzer überlastet ist, werden die täglichen Gesamtwerte für die Tage, an denen die Benutzerin oder der Benutzer überlastet ist, jetzt in rot angezeigt. Diese Option wird nur angezeigt, wenn die Option zum Anzeigen der Gesamtwerte für täglich geplante Stunden in den Zeitplaneinstellungen aktiviert ist. Vor dieser Verbesserung gab es einen roten Balken für die Tage, an denen die Benutzenden überlastet waren, aber die täglichen Gesamtwerte wurden ohne rote Markierung angezeigt.

Weitere Informationen zu Benutzerzuweisungen finden Sie unter „Verwalten von Benutzerzuweisungen in den Zeitplanbereichen“.

## Aufgaben und Probleme werden auf der Zeitleiste ausgeblendet, wenn sie minimiert sind {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

Wenn Sie Aufgaben und Probleme in Ihrer Zeitleiste minimieren, werden sie jetzt für Benutzer und Rollen ausgeblendet, wenn die Option Gesamtwerte für täglich geplante Stunden anzeigen in Ihren Einstellungen aktiviert ist. Aufgaben und Probleme im Bereich Nicht zugewiesen werden in einer komprimierten Ansicht angezeigt.

Wenn Sie bisher Aufgaben und Probleme minimiert haben, blieben die Aufgaben und Probleme auf der Zeitleiste für die Planung für Benutzer und Rollen, wurden jedoch in einer komprimierten Ansicht angezeigt.

Weitere Informationen zum Minimieren von Aufgaben und Problemen in der Zeitplanung finden Sie unter  „Erste Schritte mit der Ressourcenplanung“.

## Filtern von Kommentaren und Antworten nach Benutzer im Proofing Viewer {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

Jetzt können Sie Antworten einbeziehen, wenn Sie Kommentare von Benutzern filtern, die Sie angegeben haben. Dies ist nützlich, wenn Sie sich auf das gesamte Feedback eines wichtigen Prüfers konzentrieren möchten, z. B. eines Kunden oder eines Projekt-Managers.

Zuvor war das Filtern nach Benutzer auf die Kommentare beschränkt, die von den von Ihnen angegebenen Validierungsverantwortlichen verfasst (gestartet) wurden.

## Kommentar zu einer Reihe von Aufnahmen in einem Videobeweis {#comment-on-a-range-of-footage-in-a-video-proof}

Sie können einen Kommentar für eine Reihe von Filmmaterial in einem Videobeweis erstellen. Dies ist beispielsweise nützlich, wenn Sie angeben müssen, dass ein Segment des Filmmaterials neu aufgenommen oder entfernt werden muss.

Zuvor konnten Sie einen Kommentar nur für einen einzelnen Punkt auf einer Video-Timeline erstellen.

## Neues Mehrzeilenwerkzeug für Kommentar-Markup im Proofing Viewer {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

Jetzt können Sie mehrzeiliges Markup verwenden, um segmentierte Linien und Formen zu zeichnen, wenn Sie einen Kommentar zu einem Korrekturabzug hinzufügen. Sie können eine offene segmentierte Linie oder eine geschlossene Form erstellen. Dieses Tool ist besonders nützlich bei der Arbeit mit komplexen Bildern, wie technischen oder architektonischen Bildern.

Wenn Sie einen Korrekturabzug markieren, um einen Kommentar hinzuzufügen, konnten Sie zuvor ein Rechteck, eine gerade Linie, eine Freihandlinie oder -form oder einen Pfeil zeichnen.

## Flash-Entfernung für die Freigabe von Berichten, Kalendern und Dokumenten {#flash-removal-for-report-calendar-and-document-sharing}

Wir haben Flash aus den folgenden Freigabedialogen in Workfront entfernt:

* Berichte
* Kalender
* Dokumente

Sie können diese Objekte weiterhin freigeben, wie Sie es zuvor getan haben, aber jetzt ist das Erlebnis nicht mehr vom Flash abhängig.
