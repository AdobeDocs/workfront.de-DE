---
product-area: documents
navigation-topic: approvals
title: Objektberechtigungen und Übersicht auf Zugriffsebene für das Adobe Enterprise-Speichermodell
description: Adobe Enterprise-Speicherberechtigungen und Zugriffsübersicht
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Objektberechtigungen und Übersicht auf Zugriffsebene für das Adobe Enterprise-Speichermodell

<!--linked in UI -->

Adobe Enterprise Storage ist eine Cloud-basierte Speicherlösung, die als zentrales Speicher-Repository für Assets in allen Adobe Enterprise-Produkten dient. Workfront-Umgebungen, die Adobe Enterprise Storage verwenden, weisen etwas andere Objektberechtigungen und Zugriffsverhaltensweisen auf als Umgebungen, die Legacy-Dokumentspeicher von Workfront verwenden.

## Zugriffsebenen

Die Zugriffsebenen von Workfront gelten nur innerhalb von Workfront. Projekt- und Dokumenteinschränkungen in Workfront gelten nicht immer für andere Adobe-Programme.

### Umgebungen, die sowohl Adobe Enterprise-Speicher als auch Legacy-Workfront-Speicher verwenden

Der Dokumentzugriff verhält sich unterschiedlich, je nachdem, ob sich das Projekt im Adobe Enterprise-Speicher oder im Legacy-Workfront-Speicher befindet:

* **Legacy-Workfront-**: Projekte, Programme, Portfolios und Vorlagen, die Legacy-Workfront-Speicher verwenden, folgen beim Dokumentzugriff der standardmäßigen Workfront-Zugriffsebenen-Logik. Wenn für eine Zugriffsebene **Kein Zugriff** für Dokumente ausgewählt ist, können die Dokumente in Workfront oder anderen Adobe-Produkten wie Frame.io oder Creative Cloud nicht angezeigt werden.
* **Adobe Enterprise-Speicher**: Projekte, Programme, Portfolios und Vorlagen, die Adobe Enterprise-Speicher verwenden, folgen für andere Adobe-Produkte der Zugriffslogik auf Adobe Enterprise-Speicher.


   * **Objektberechtigungen für Projekte, Programme, Portfolios und Vorlagen**: Wenn eine Zugriffsebene **Kein Zugriff** für Projekte, Programme, Portfolios und Vorlagen ausgewählt hat, das Objekt jedoch für sie freigegeben ist, können Benutzende das Objekt nicht in Workfront sehen, aber sie können weiterhin den Objektnamen und alle zugehörigen Dokumente in anderen Adobe-Tools wie Frame.io und Adobe Creative Cloud anzeigen.
   * **Dokumentberechtigungen**: Wenn für eine Zugriffsebene **Kein Zugriff** für Dokumente ausgewählt ist, können Benutzende keine Dokumente zu Projekten in Workfront anzeigen. Sie können jedoch weiterhin Dokumente für Projekte anzeigen und verwalten, die in anderen Adobe-Tools wie Frame.io und Adobe Creative Cloud für sie freigegeben sind. Dies liegt daran, dass der Dokumentzugriff durch Berechtigungen auf Projektebene im Adobe Enterprise-Speicher und nicht allein durch die Workfront-Zugriffsebenen bestimmt wird.

Wenn Adobe Enterprise Storage in Ihrer Workfront-Umgebung aktiviert ist, können Sie sowohl Adobe Enterprise Storage-Projekte als auch Legacy-Workfront-Speicherprojekte erstellen. Ältere Workfront-Speicherprojekte zeigen ein Symbol neben dem Projektnamen an, wo immer er in Workfront angezeigt wird. In Adobe Enterprise-Speicherprojekten wird kein Symbol angezeigt.

![Legacy Workfront Storage-Symbol neben dem Projektnamen](assets/legacy-project-icon.png)


### Umgebungen, die nur Adobe Enterprise-Speicher verwenden

Sie können Dokumentberechtigungen auf der Zugriffsebene für Projekte, Programme und Portfolios, die Adobe Enterprise-Speicher verwenden, nicht ändern.

Alle Zugriffsebenen haben Bearbeitungszugriff auf Dokumente. Berechtigungen auf Projektebene bestimmen den Dokumentzugriff in anderen Adobe-Tools.

Sie können den Dokumentvererbungszugriff nicht einschränken.


### Umgebungen, die nur Legacy-Workfront-Speicher verwenden

Keine Änderungen an Zugriffsebenen oder Verhalten von Dokumenten.


## Projekte

Benutzende mit Berechtigungen auf Projektebene können Dokumente für Projekte in anderen Adobe-Produkten wie Frame.io und Adobe Creative Cloud anzeigen und verwalten.

Projektnamen sind auch außerhalb von Workfront für ESM-Projekte sichtbar.

Finanzdaten für ESM-Projekte sind außerhalb von Workfront nicht sichtbar.

## Aufgaben und Probleme

Dokumente werden auf Projektebene gespeichert, können jedoch bei Bedarf für einzelne Aufgaben und Probleme freigegeben werden. Benutzende mit Aufgaben- und Problemzugriff erben automatisch den Dokumentzugriff aus dem Projekt. Die Zugriffsebene kann nicht geändert werden. Sie haben verwalteten Zugriff oder keinen Zugriff.