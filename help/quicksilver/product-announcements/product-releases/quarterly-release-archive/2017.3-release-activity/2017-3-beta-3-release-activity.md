---
content-type: release-notes
navigation-topic: product-releases-archive
title: Aktivität "Beta-Version 3"2017.3
description: Die Version 2017.3 wird Anfang November 2017 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

---

# Aktivität &quot;Beta-Version 3&quot;2017.3

Die Version 2017.3 wird Anfang November 2017 in der Produktionsumgebung verfügbar gemacht.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller 2017.3 vorgenommenen Änderungen finden Sie unter  [Übersicht über die Release-Aktivitäten 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

Die Beta 3-Version 2017.3 enthält Verbesserungen für alle Benutzer:

* [Anpassen der Diagrammfarben](#customize-chart-colors)
* [Zusätzliche Optionen beim Kopieren von Projekten](#additional-options-when-copying-projects)
* [Verbesserung des Ressourcenplaners: Filter](#resource-planner-improvement-filters)
* [Verbesserung des Ressourcenplans: Problemzeiten im Bereich &quot;Einstellungen&quot;anzeigen](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [SSO-Informationen für benutzerdefinierte Aktualisierungs- und Vorschau-Sandboxes nicht aktualisieren](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Aktualisierte Anforderungen an die Browserunterstützung für Workfront Testversand](#updated-browser-support-requirements-for-workfront-proof)

## Anpassen der Diagrammfarben {#customize-chart-colors}

Jetzt können Sie die Farben der Elemente der Diagramme anpassen. Dies gilt für alle Diagrammtypen in Berichten. Dies gilt nicht für die Gantt-Grafik.

Vor dieser Änderung wurden die Elemente aller Grafiken standardmäßig von Workfront ausgewählt. Weitere Informationen zum Anpassen der Diagrammfarben finden Sie in den Abschnitten &quot;Anpassen der Diagrammfarben&quot;unter [Diagramm zu einem Bericht hinzufügen](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Zusätzliche Optionen beim Kopieren von Projekten {#additional-options-when-copying-projects}

Beim Kopieren eines Projekts entsprechen die Optionen jetzt denen, die beim Kopieren von Aufgaben oder Problemen verfügbar sind. Sie können auch den Status des kopierten Projekts ändern, während Sie es kopieren.

Vor dieser Aktualisierung konnten Sie den Status des kopierten Projekts beim Kopieren nicht ändern. Beim Kopieren eines Projekts waren nur zwei Optionen verfügbar:

* So behalten Sie Zuweisungen für Aufgaben und das Projekt bei
* So halten Sie den Fortschritt bei Aufgaben und Projekten aufrecht

Mit der neuen Funktion wurden die vorherigen Optionen entfernt und die folgenden Optionen wurden beim Kopieren eines Projekts hinzugefügt:

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

Weitere Informationen zu den neuen Funktionen zum Kopieren von Projekten finden Sie im Abschnitt &quot;Kopieren eines Projekts in der Vorschauumgebung&quot;unter   [Projekt kopieren](../../../../manage-work/projects/manage-projects/copy-project.md).

## Verbesserung des Ressourcenplaners: Filter {#resource-planner-improvement-filters}

Sie können die im Ressourcenplaner angezeigten Informationen nun nach den folgenden Objekten filtern:

* Portfolio
* Projektstatus
* Team
* Aufgabengebiet
* Ressourcenpool

Sie können auch einen benutzerdefinierten Filter hinzufügen, der auf diesen Objekten basiert.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Übersicht über den Ressourcenplaner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Verbesserung des Ressourcenplans: Problemzeiten im Bereich &quot;Einstellungen&quot;anzeigen {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Im Ressourcenplaner gibt es einen neuen Bereich &quot;Einstellungen&quot;, in dem mehrere Optionen zum Anpassen des Ressourcenplaners angezeigt werden. Mit dieser Version haben wir die erste Option hinzugefügt, mit der geplante Stunden aus Problemen in die Spalten &quot;Geplante Stunden&quot;des Ressourcenplaners aufgenommen werden können.

Weitere Informationen zur Verwendung des Ressourcen-Planers finden Sie unter [Übersicht über den Ressourcenplaner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## SSO-Informationen für benutzerdefinierte Aktualisierungs- und Vorschau-Sandboxes nicht aktualisieren {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

Ab dieser Version werden die SSO-Informationen beim Aktualisieren Ihrer benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes nicht aus Ihrer Produktionsumgebung kopiert und auch nicht deaktiviert. Vor dieser Änderung wurden die SSO-Informationen in den benutzerdefinierten Aktualisierungs- und Vorschau-Sandboxes deaktiviert und auf &quot;Keine&quot;gesetzt.

Weitere Informationen zur Umgebung &quot;Custom Refresh Sandbox&quot;finden Sie unter [Die benutzerdefinierte Adobe Workfront-Aktualisierungs-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Weitere Informationen zur Vorschau-Sandbox-Umgebung finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Aktualisierte Anforderungen an die Browserunterstützung für Workfront Testversand {#updated-browser-support-requirements-for-workfront-proof}

Die Anforderungen an die Browserunterstützung für Workfront Testversand wurden aktualisiert. Weitere Informationen finden Sie unter [Adobe Workfront-Browseranforderungen](../../../../workfront-basics/workfront-browser-requirements.md).
