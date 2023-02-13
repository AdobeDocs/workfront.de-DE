---
title: 21.4 Projektverbesserungen
description: 21.4 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4 Projektverbesserungen

Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 21.4 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden ab der Woche des 4. Oktober 2021 in der Produktionsumgebung verfügbar sein.

Eine Liste aller in Version 21.4 verfügbaren Änderungen finden Sie unter [21.4 Versionsübersicht](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Bilder in Aktualisierungen einschließen

Auf der Registerkarte Updates eines Objekts können Sie jetzt Bilder hinzufügen, indem Sie in der Symbolleiste auf das Symbol Bild klicken. Sie können ein Bild auch per Drag-and-Drop in den Aktualisierungsbereich ziehen. Beachten Sie, dass Ihr Workfront-Administrator das Hinzufügen von Bildern aktivieren muss, bevor das Bildsymbol angezeigt werden kann.

Sie können Bilder sowohl in Updates als auch in Antworten hinzufügen. Eine Miniaturansicht in der Aktualisierung zeigt an, dass Empfänger eine Vorschau des Bildes im Browser anzeigen oder es herunterladen können. E-Mail- und In-App-Benachrichtigungen zeigen an, dass Bilder an die Aktualisierung angehängt sind.

Zuvor bestand die einzige Möglichkeit, ein Bild in Workfront freizugeben, darin, es als Dokument an ein Objekt anzuhängen. Auf der Registerkarte Aktualisierungen hinzugefügte Bilder sind nur auf dieser Registerkarte und nicht auf der Registerkarte Dokumente verfügbar.

Weitere Informationen finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Bevor Workfront-Benutzer Bilder in Aktualisierungen einbeziehen können, muss diese Funktion zunächst vom Adobe Workfront-Administrator aktiviert werden, wie hier beschrieben: [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Aktualisierter Algorithmus für Smart-Zuweisungen

Wir haben den Algorithmus für die Durchführung von intelligenten Zuweisungen verbessert. Mit der neuen Verbesserung untersucht Workfront die 30 neuesten Zuweisungen des angemeldeten Benutzers, um beim Zuweisen von Aufgaben und Problemen Vorschläge zu machen. Die Liste der Vorschläge kann bis zu 50 Benutzer enthalten.

Vor dieser Verbesserung berücksichtigte Workfront beim Vorschlag von Benutzern die Zuweisungen für die übergeordneten Aufgaben und andere Benutzerattribute im Zusammenhang mit diesen Zuweisungen.

Informationen zu Smart-Zuweisungen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Neues Erlebnis beim Erstellen eines Projekts aus einer Vorlage

Damit Ihre Verwendung von Workfront mit dem neuen Workfront-Erlebnis konsistent ist, haben wir die Benutzeroberfläche zum Erstellen eines Projekts aus einer Vorlage neu gestaltet. Die Funktionalität zum Erstellen eines Projekts mit einer Vorlage wurde nicht geändert. Einige der Verbesserungen dieser neu gestalteten Benutzeroberfläche umfassen jedoch Folgendes:

* Vorschau von Vorlageninformationen vor dem Anhängen
* Hinzufügen von Vorlagen zu einer Favoritenliste während des Projekterstellungsprozesses

Wir haben die Benutzeroberfläche für die Erstellung des Projekts aktualisiert, sowohl wenn Sie es aus den Projekten als auch aus dem Bereich Vorlagen erstellen.

Für Informationen: [Erstellen eines Projekts mit einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Neues Erlebnis beim Anhängen von Vorlagen an Projekte

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Damit Ihre Verwendung von Workfront mit dem neuen Workfront-Erlebnis konsistent ist, haben wir die Benutzeroberfläche für das Anhängen einer Vorlage an ein Projekt neu gestaltet. Die Funktionalität zum Anhängen einer Vorlage wurde nicht geändert. Es gibt jedoch einige Verbesserungen dieser neu gestalteten Oberfläche, die Folgendes umfassen:

* Vorschau von Vorlageninformationen vor dem Anhängen
* Hinzufügen von Vorlagen zu einer Favoritenliste während des Anlagenprozesses
* Alle Optionen zum Verwalten von Vorlagen- und Projekteinstellungen auf einer durchgehenden Seite anzeigen

Weitere Informationen finden Sie unter [Eine Vorlage an ein Projekt anhängen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Einheitliche Werte für Dauer und Dauer je Einheit für Aufgaben

Für ein saubereres und optimiertes Benutzererlebnis haben wir den Wert des Felds Dauer mit der Zeiteinheit Dauer zusammengeführt. Vor dieser Verbesserung wird die Zeiteinheit in einem separaten Dropdown-Feld nach dem Feld Dauer angezeigt.

Zusätzlich zu den Feldern &quot;Dauer&quot;in den Feldern &quot;Aufgabendetails&quot;, &quot;Aufgaben bearbeiten&quot;und &quot;Neue Aufgabe&quot;aktualisieren wir auch die folgenden Felder, um diesem Erlebnis zu entsprechen:

* Feld für die Dauer bei erweiterten Zuweisungen
* Levelverzögerungsfeld beim Erstellen oder Bearbeiten einer Aufgabe
* Frequenzfeld bei Erstellung einer wiederkehrenden Aufgabe (in Kürze verfügbar)
* Lag-Feld beim Hinzufügen eines Vorgängers (bald verfügbar)

Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Inline-Hinzufügen von Problemen in Projekten deaktivieren

Um sicherzustellen, dass Benutzer beim Hinzufügen von Problemen zu Projekten durch Ausfüllen eines Problemformulars genaue Informationen bereitstellen, haben wir eine neue Einstellung eingeführt, mit der Sie verwalten können, ob sie Probleme zu einem Projekt oder seinen Aufgaben inline hinzufügen können. Diese Einstellung ist standardmäßig im neuen Bereich &quot;Problemeinstellungen&quot;im Feld &quot;Projekt bearbeiten&quot;aktiviert. Durch Deaktivieren wird die Option Weitere Probleme hinzufügen im Abschnitt Probleme eines Projekts deaktiviert, sodass Benutzer keine weiteren Probleme in die Liste aufnehmen können. Benutzer können den Projekten weiterhin Probleme hinzufügen, indem sie im Abschnitt Probleme die Option Neues Problem verwenden oder eine Anforderungswarteschlange verwenden, wenn eine für das Projekt konfiguriert ist.

>[!NOTE]
>
>Diese Einstellung ist nur im neuen Workfront-Erlebnis verfügbar. Benutzer, die in Workfront Classic arbeiten, können einem Projekt oder seinen Aufgaben weiterhin Probleme inline hinzufügen, selbst wenn diese Einstellung von einem Benutzer, der mit dem neuen Workfront-Erlebnis arbeitet, für das Projekt deaktiviert wurde.

Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

## Verbesserte Anzeige von benutzerdefinierten Feldern für Kontrollkästchen und Optionsfelder

Die Anzeige und Auswahl von Kontrollkästchen- und Optionsschaltflächen-Optionen in benutzerdefinierten Formularen wurde einfach gestaltet - ein benutzerdefiniertes Feld mit vielen Kontrollkästchen- oder Optionsschaltflächen-Optionen wird nun in mehreren Spalten auf der Seite angezeigt. Zuvor wurden sie in einer einzigen Spalte angezeigt, sodass Benutzer, die das Formular ausfüllten, einen zusätzlichen Bildlauf durchführen mussten.

Dies hängt davon ab, wie Sie die Felder im benutzerdefinierten Formular positionieren. Wenn Sie ein anderes Feld mit dem Kontrollkästchen oder dem Optionsfeld in derselben Zeile platzieren, verfügen die Optionen möglicherweise nur über genügend horizontalen Platz, um in einer Spalte angezeigt zu werden.

Informationen zum Ausfüllen eines benutzerdefinierten Formulars finden Sie unter [Informationen in benutzerdefinierten Formularfeldern bearbeiten](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Informationen zum Erstellen eines Kontrollkästchen- oder Optionsfeld-Felds in einem benutzerdefinierten Formular finden Sie in den Abschnitten . [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) und [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

