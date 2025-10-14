---
title: 21.4 Projektverbesserungen
description: 21.4 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# 21.4 Projektverbesserungen

Auf dieser Seite werden alle mit Version 21.4 vorgenommenen Projektverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 4. Oktober 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie in der Übersicht über die Version [21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Bilder in Aktualisierungen einschließen

Auf der Registerkarte Aktualisierungen eines Objekts können Sie nun Bilder hinzufügen, indem Sie in der Symbolleiste auf das Bildsymbol klicken. Sie können auch ein Bild per Drag-and-Drop in den Aktualisierungsbereich ziehen. Beachten Sie, dass Ihr Workfront-Administrator das Hinzufügen von Bildern aktivieren muss, bevor Sie das Bildsymbol sehen können.

Sie können sowohl in Aktualisierungen als auch in Antworten Bilder hinzufügen. Ein Miniaturbild in der Aktualisierung zeigt an, dass Empfängerinnen und Empfänger das Bild im Browser in der Vorschau anzeigen oder herunterladen können und E-Mail- und In-App-Benachrichtigungen zeigen, dass Bilder an die Aktualisierung angehängt sind.

Zuvor bestand die einzige Möglichkeit, ein Bild in Workfront freizugeben, darin, es als Dokument an ein Objekt anzuhängen. Bilder, die auf der Registerkarte Aktualisierungen hinzugefügt wurden, sind nur auf dieser Registerkarte und nicht auf der Registerkarte Dokumente verfügbar.

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Bevor Workfront-Benutzer Bilder in Aktualisierungen einbeziehen können, muss diese Funktion zunächst vom Adobe Workfront-Administrator aktiviert werden, wie unter &quot;[&#x200B; für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md) beschrieben.

## Aktualisierter Algorithmus für smarte Zuweisungen

Der Algorithmus, der bei der Erstellung intelligenter Zuweisungen verwendet wird, wurde verbessert. Im Rahmen der neuen Verbesserung untersucht Workfront die 30 letzten Zuweisungen, die der angemeldete Benutzer vorgenommen hat, um Vorschläge zu unterbreiten, wenn er Aufgaben und Probleme zuweist. Die Liste der Vorschläge kann bis zu 50 Benutzer enthalten.

Vor dieser Verbesserung hat Workfront die Arbeitsaufträge für übergeordnete Aufgaben und andere Benutzerattribute im Zusammenhang mit diesen Arbeitsaufträgen berücksichtigt, als es Benutzer vorgeschlagen hat.

Informationen zu Smart-Zuweisungen finden Sie unter [Smart-Zuweisungen - Übersicht](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Neues Erlebnis beim Erstellen eines Projekts über eine Vorlage

Damit Ihre Verwendung von Workfront mit der neuen Workfront-Version konsistent ist, haben wir die Benutzeroberfläche zum Erstellen eines Projekts aus einer Vorlage neu gestaltet. Die Funktionalität zum Erstellen eines Projekts mithilfe einer Vorlage hat sich nicht geändert. Zu den Verbesserungen dieser neu gestalteten Benutzeroberfläche gehören jedoch die folgenden:

* Vorlageninformationen vor dem Anhängen in der Vorschau anzeigen
* Hinzufügen von Vorlagen zu einer Favoritenliste während der Projekterstellung

Die Benutzeroberfläche zum Erstellen des Projekts wurde sowohl beim Erstellen über den Bereich Projekte als auch im Bereich Vorlagen aktualisiert.

Weitere Informationen finden [&#x200B; unter „Erstellen eines Projekts mithilfe einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Neues Erlebnis beim Anhängen von Vorlagen an Projekte

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um die Verwendung von Workfront mit der neuen Workfront-Version konsistent zu machen, haben wir die Benutzeroberfläche zum Anhängen einer Vorlage an ein Projekt neu gestaltet. Die Funktionalität zum Anhängen einer Vorlage hat sich nicht geändert. Es gibt jedoch einige Verbesserungen dieser neu entworfenen Benutzeroberfläche, die Folgendes umfassen:

* Vorlageninformationen vor dem Anhängen in der Vorschau anzeigen
* Hinzufügen von Vorlagen zu einer Favoritenliste während des Anfügevorgangs
* Alle Optionen zum Verwalten von Vorlagen- und Projekteinstellungen auf einer durchgehenden Seite anzeigen

Weitere Informationen finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Einheitliche Werte für Dauer und Dauer für die Einheiten der Aufgaben

Für ein saubereres und optimiertes Benutzererlebnis haben wir den Wert des Felds Dauer mit der Zeiteinheit Dauer zusammengeführt. Vor dieser Verbesserung wird die Zeiteinheit in einem separaten Dropdown-Feld nach dem Feld Dauer angezeigt.

Zusätzlich zu den Feldern „Dauer“ in den Feldern „Aufgabendetails“, „Aufgaben bearbeiten“ und „Neue Aufgabe“ werden auch die folgenden Felder aktualisiert, damit sie diesem Erlebnis entsprechen:

* Feld „Dauer“ bei erweiterten Zuweisungen
* Abgleichsverzögerungsfeld beim Erstellen oder Bearbeiten einer Aufgabe
* Feld „Häufigkeit“ bei der Erstellung einer wiederkehrenden Aufgabe (in Kürze verfügbar)
* Verzögertes Feld beim Hinzufügen eines Vorgängers (in Kürze verfügbar)

Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![Feld Dauer](assets/duration-combined-field-350x139.png)

## Deaktivieren des Hinzufügens von Problemen inline in Projekten

Um sicherzustellen, dass Benutzer beim Hinzufügen von Problemen zu Projekten durch Ausfüllen eines Anfrageformulars genaue Informationen angeben, haben wir eine neue Einstellung eingeführt, mit der Sie verwalten können, ob Probleme zu einem Projekt oder dessen Aufgaben inline hinzugefügt werden können. Diese Einstellung ist standardmäßig im Bereich „Neue Anfrageeinstellungen“ im Feld „Projekt bearbeiten“ aktiviert. Wenn Sie die Option „Weitere Probleme hinzufügen“ im Abschnitt „Probleme“ eines Projekts deaktivieren, können Benutzer keine weiteren Probleme in der Liste hinzufügen. Benutzer können den Projekten weiterhin Probleme hinzufügen, indem sie die Option „Neues Problem“ im Abschnitt „Probleme“ verwenden oder eine Anfrage-Warteschlange verwenden, wenn eine für das Projekt konfiguriert ist.

>[!NOTE]
>
>Diese Einstellung ist nur in der neuen Workfront-Version verfügbar. Benutzende, die in Workfront Classic arbeiten, können einem Projekt oder seinen Aufgaben weiterhin Probleme inline hinzufügen, selbst wenn diese Einstellung für das Projekt von einer Benutzerin oder einem Benutzer deaktiviert wurde, die bzw. der in der neuen Workfront-Version arbeitet.

Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

## Verbesserung der Anzeige benutzerdefinierter Felder für Kontrollkästchen und Optionsfelder

Das Anzeigen und Auswählen von Kontrollkästchen- und Optionsschaltflächen-Optionen in benutzerdefinierten Formularen wurde gerade einfacher. Ein benutzerdefiniertes Feld mit vielen Kontrollkästchen- oder Optionsschaltflächen-Optionen wird jetzt in mehreren Spalten auf der Seite angezeigt. Zuvor wurden sie in einer einzelnen Spalte angezeigt, was einen zusätzlichen Bildlauf für Benutzende erforderte, die das Formular ausfüllen.

Dies hängt davon ab, wie Sie die Felder im benutzerdefinierten Formular positionieren. Wenn Sie ein weiteres Feld in derselben Zeile mit dem Kontrollkästchen- oder Optionsfeld platzieren, verfügen die Optionen möglicherweise nur über genügend horizontalen Platz, um in einer einzelnen Spalte angezeigt zu werden.

Informationen zum Ausfüllen eines benutzerdefinierten Formulars finden Sie unter [Informationen in benutzerdefinierten Formularfeldern bearbeiten](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

