---
product-area: documents
navigation-topic: approvals
title: Objektberechtigungen und Übersicht auf Zugriffsebene für das Adobe Enterprise-Speichermodell
description: Überblick über Berechtigungen und Zugriffsrechte für Adobe-Unternehmensspeicher
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

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

## Objektberechtigungen

Objektberechtigungen bestimmen, was Sie in Workfront mit Projekten, Aufgaben, Problemen und Dokumenten anzeigen und tun können. Berechtigungen werden zugewiesen, wenn jemand ein Objekt für Sie freigibt.

>[!IMPORTANT]
>
>Im Adobe Enterprise-Speicher funktionieren Dokumentberechtigungen anders als im alten Workfront-Speicher. Dokumente übernehmen Berechtigungen aus dem Projekt, der Aufgabe oder dem Problem, mit dem bzw. dem sie verknüpft sind.


### Funktionsweise von Dokumentberechtigungen

Dokumentberechtigungen werden von dem Objekt gesteuert, mit dem das Dokument verknüpft ist. Sie können keine Berechtigungen für einzelne Dokumente festlegen.

Wenn Sie ein Dokument in eine Aufgabe oder ein Problem hochladen, wird mithilfe des Aufgaben- oder Problemnamens ein systemgenerierter Ordner erstellt. Dieser Ordner ist mit der Aufgabe oder dem Problem verknüpft und übernimmt die Berechtigungen.

Sie können im systemgenerierten Ordner Unterordner erstellen, um Dokumente weiter zu organisieren. Alle Unterordner erben Berechtigungen vom übergeordneten Ordner. Auf Projektebene können Sie Dokumente außerhalb eines Ordners hochladen, aber nur Benutzer mit Zugriff auf Projektebene können sie sehen.

Auf Projektebene zeigen systemgenerierte Ordner ein verknüpftes Objekt an. Dies ist normalerweise der Name der Aufgabe oder des Problems und der Grund, warum das System weiß, für welche Aufgabe oder welches Problem der Ordner angezeigt werden soll.

### Projektberechtigungen

Wenn Sie über Berechtigungen auf Projektebene verfügen, können Sie Dokumente für dieses Projekt in Workfront und anderen Adobe-Produkten wie Frame.io und Adobe Creative Cloud anzeigen und verwalten. Der Projektname ist auch in diesen Tools sichtbar. Andere Projektdaten sind außerhalb von Workfront nicht sichtbar.

### Aufgaben- und Problemberechtigungen

Aufgaben und Probleme übernehmen Berechtigungen aus dem Projekt. Wenn Sie über Berechtigungen auf Aufgaben- oder Problemebene verfügen, können Sie Dokumente anzeigen und verwalten, die mit dieser Aufgabe oder diesem Problem in Workfront und anderen Adobe-Produkten wie Frame.io und Adobe Creative Cloud verknüpft sind.

**Systemgenerierte Ordner**

* Wenn Benutzer aus einer Aufgabe oder einem Problem entfernt werden, wird ihr Ordnerzugriff nicht automatisch entfernt. Sie haben möglicherweise weiterhin Zugriff über Berechtigungen auf Projektebene.
* Unteraufgaben erben keine systemgenerierten Ordnerberechtigungen von übergeordneten Aufgaben. Sie müssen einer Unteraufgabe direkt hinzugefügt werden, um auf ihren systemgenerierten Ordner zuzugreifen.
* Durch das Hinzufügen von Benutzern zu einer Aufgabe oder einem Problem wird der systemgenerierte Ordner dieses Objekts für sie freigegeben.

**Verschieben und Umbenennen systemgenerierter Ordner:**

* Systemgenerierte Ordner können umbenannt und verschoben werden.
* Wenn ein systemgenerierter Ordner an einen anderen Speicherort verschoben wird, wird sein verknüpftes -Objekt zum neuen -Objekt aktualisiert. Berechtigungen werden dann vom neuen übergeordneten Objekt vererbt.

Anfragen verhalten sich genauso wie Aufgaben und Probleme.

### Genehmigungen

Wenn Sie einem Workflow für die Dokumentgenehmigung hinzugefügt werden, sehen Sie Folgendes, unabhängig von den Projektberechtigungen:

* Projektname
* Dokumentname
* Dokument-Miniaturansicht










