---
content-type: release-notes
navigation-topic: product-releases-archive
title: Veröffentlichungen für Version 2017.1 Beta 3
description: Die Version 2017.3 wird Anfang November 2017 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
TQID: https://experienceleague.adobe.com/12nUGoSnwlcVACSTf-b-Fks7QRuCCl9HBujkDNG5ubU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 572
ht-degree: 7%

---

# Veröffentlichungen für Version 2017.1 Beta 3

Die Version 2017.3 wird Anfang November 2017 in der Produktionsumgebung verfügbar gemacht.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller in 2017.3 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Beta-Version 3 2017.3 enthält Verbesserungen für alle Benutzenden:

* [Anpassen der Diagrammfarben](#customize-chart-colors)
* [Zusätzliche Optionen beim Kopieren von Projekten](#additional-options-when-copying-projects)
* [Ressourcenplaner-Verbesserung: Filter](#resource-planner-improvement-filters)
* [Ressourcenplaner-Verbesserung: Problemstunden im Bereich „Einstellungen“ anzeigen](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [SSO-Informationen für die benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes werden nicht aktualisiert](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Aktualisierte Anforderungen an die Browser-Unterstützung für Workfront Proof](#updated-browser-support-requirements-for-workfront-proof)

## Anpassen der Diagrammfarben {#customize-chart-colors}

Sie können jetzt die Farben der Elemente in Diagrammen anpassen. Dies gilt für alle Diagrammtypen in Berichten. Dies gilt nicht für das Gantt-Diagramm.

Vor dieser Änderung wurden die Farben der Elemente aller Diagramme standardmäßig von Workfront ausgewählt. Weitere Informationen zum Anpassen der Diagrammfarben finden Sie in den Abschnitten zum Anpassen der Diagrammfarben in [Hinzufügen eines Diagramms zu einem Bericht](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Zusätzliche Optionen beim Kopieren von Projekten {#additional-options-when-copying-projects}

Beim Kopieren eines Projekts entsprechen die Optionen nun denen, die beim Kopieren von Aufgaben oder Problemen verfügbar sind. Sie können den Status des kopierten Projekts auch ändern, während Sie es kopieren.

Vor diesem Update konnten Sie den Status des kopierten Projekts während des Kopierens nicht ändern, und beim Kopieren eines Projekts waren nur zwei Optionen verfügbar:

* So behalten Sie Zuweisungen zu Aufgaben und zum Projekt bei
* So behalten Sie den Fortschritt bei Aufgaben und Projekten bei

Mit der neuen Funktion wurden die vorherigen Optionen entfernt und die folgenden Optionen beim Kopieren eines Projekts hinzugefügt:

* Zuweisungen löschen
* Finanzielle Informationen löschen
* Fortschritt löschen
* Genehmigungen löschen
* Benutzerdefinierte Daten löschen
* Erinnerungsnachrichten löschen
* Dokumente löschen
* Auslagen löschen
* Alle Vorgänger löschen
* Berechtigungen leeren
* Alle auswählen

Weitere Informationen zu den neuen Funktionen zum Kopieren von Projekten finden Sie im Abschnitt „Kopieren eines Projekts in die Vorschau-Umgebung“ in [Projekt kopieren](../../../../manage-work/projects/manage-projects/copy-project.md).

## Ressourcenplaner-Verbesserung: Filter {#resource-planner-improvement-filters}

Sie können jetzt die Informationen, die Sie im Ressourcenplaner sehen, nach den folgenden Objekten filtern:

* Portfolio
* Projektstatus
* Team
* Aufgabengebiet
* Ressourcen-Pool

Sie können auch einen benutzerdefinierten Filter hinzufügen, der auf diesen Objekten basiert.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Ressourcenplaner-Verbesserung: Problemstunden im Bereich „Einstellungen“ anzeigen {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Im Ressourcenplaner gibt es einen neuen Bereich Einstellungen , der mehrere Optionen zum Anpassen des Ressourcenplaners anzeigt. Mit dieser Version haben wir die erste Option hinzugefügt, um geplante Stunden aus Problemen in die Spalten „Geplante Stunden“ des Ressourcenplaners aufzunehmen.

Weitere Informationen zur Verwendung des Ressourcenplaners finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## SSO-Informationen für die benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes werden nicht aktualisiert {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

Ab dieser Version werden beim Aktualisieren der benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes die SSO-Informationen weder aus Ihrer Produktionsumgebung kopiert noch deaktiviert. Vor dieser Änderung wurden die SSO-Informationen in den benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes deaktiviert und auf „Keine“ gesetzt.

Weitere Informationen zur benutzerdefinierten Sandbox-Aktualisierungsumgebung finden Sie unter [Die benutzerdefinierte Sandbox-Aktualisierungsumgebung von Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Weitere Informationen zur Sandbox-Vorschau-Umgebung finden Sie unter [Die Sandbox-Vorschau-Umgebung von Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Aktualisierte Anforderungen an die Browser-Unterstützung für Workfront Proof {#updated-browser-support-requirements-for-workfront-proof}

Die Anforderungen an die Browser-Unterstützung für Workfront Proof wurden aktualisiert. Weitere Informationen finden Sie unter [Browser-Anforderungen für Adobe Workfront](../../../../workfront-basics/workfront-browser-requirements.md).
