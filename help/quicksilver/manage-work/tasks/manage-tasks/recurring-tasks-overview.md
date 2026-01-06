---
content-type: overview
product-area: projects
keywords: wiederkehrend,wiederkehrend,wiederkehrend
navigation-topic: manage-tasks
title: Übersicht über wiederkehrende Aufgaben
description: Übersicht über wiederkehrende Aufgaben
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 3%

---

# Übersicht über wiederkehrende Aufgaben

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Sie können wiederkehrende Aufgaben für Aktivitäten erstellen, die Sie im Rahmen eines einzelnen Projekts wiederholen müssen.

In diesem Artikel werden Informationen und Überlegungen zum Erstellen und Bearbeiten wiederkehrender Aufgaben beschrieben.

Informationen zum Erstellen wiederkehrender Aufgaben in Adobe Workfront finden Sie unter [Erstellen wiederkehrender Aufgaben](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Übersicht über wiederkehrende Aufgaben und Überlegungen

Sie können wiederkehrende Aufgaben erstellen, um wiederholbare Arbeiten während der Laufzeit eines Projekts anzugeben.

Während eines IT-Projekts muss beispielsweise die Software wahrscheinlich in regelmäßigen Abständen gesichert werden. Das Erstellen einer wiederkehrenden Aufgabe für diese Aktivität reduziert den Zeitaufwand für das Einrichten mehrerer einzelner Aufgaben.

Beachten Sie beim Erstellen wiederkehrender Aufgaben in Workfront Folgendes:

* Sie können einer Vorlage keine wiederkehrenden Aufgaben hinzufügen.
* Es ist nicht möglich, einer vorhandenen Aufgabe eine Wiederholungshäufigkeit hinzuzufügen.
* Wiederkehrende Aufgaben werden als Unteraufgaben oder Unteraufgaben für das Hauptereignis angezeigt, das als übergeordnete Aufgabe angezeigt wird.
* Sie können keine Genehmigung an eine übergeordnete wiederkehrende Aufgabe anhängen.
* Workfront überträgt die meisten Felder, die Sie für die übergeordnete Wiederholung beim Erstellen aktualisieren, an die untergeordneten Aufgaben. Die folgenden Felder werden beim Erstellen nicht an die untergeordneten Aufgaben übertragen:

   * Die Aufgabenbeschränkung der untergeordneten Aufgaben ändert sich automatisch in:

      * Muss beginnen am für Projekte, die ab dem Startdatum geplant sind.
      * Muss abgeschlossen sein am für Projekte, die ab Abschlussdatum geplant sind.

   * Die an das übergeordnete Element angehängten Dokumente werden nicht an die untergeordneten Elemente weitergegeben.

* Die folgenden Änderungen treten bei der übergeordneten Aufgabe auf, nachdem Sie angegeben haben, dass die Aufgabe wiederkehrend ist:

   * Das Feld Dauer wird für die übergeordnete Aufgabe in Dauer pro Vorkommen umbenannt. Es bleibt die Dauer für die untergeordneten Aufgaben.
   * Der Status wird für die übergeordnete Aufgabe deaktiviert und für die untergeordneten Aufgaben automatisch auf Neu festgelegt. Die übergeordnete Aufgabe wird automatisch abgeschlossen, und der Status wird auf Abgeschlossen aktualisiert, wenn alle untergeordneten Aufgaben abgeschlossen sind.
   * Für wiederkehrende Aufgaben stehen nur die folgenden Dauertypen zur Verfügung:

      * Einfach
      * Leistungsgesteuert
* Die Dauer und die geplanten Stunden für eine neue wiederkehrende Aufgabe entsprechen der Dauer und den geplanten Stunden für jedes Vorkommen. Die Dauer der übergeordneten Aufgabe ist die Zeit zwischen dem geplanten Startdatum der frühesten Aufgabe und dem geplanten Abschlussdatum der letzten Aufgabe. Die geplanten Stunden der übergeordneten Aufgabe sind die Gesamtstunden aller geplanten Stunden aus allen Vorfällen.

## Überlegungen zum Bearbeiten wiederkehrender Aufgaben

Einige Änderungen, die Sie an einer übergeordneten wiederkehrenden Aufgabe vornehmen, werden möglicherweise nicht bei allen vorhandenen Vorkommen aktualisiert. Untergeordnete Aufgaben, die einen Fortschritt anzeigen oder einzeln aktualisiert wurden, werden beim Aktualisieren des übergeordneten Elements nicht aktualisiert. Workfront ist der Ansicht, dass eine Aufgabe in den folgenden Situationen einen Fortschritt anzeigt:

* Status wird aktualisiert und die Aufgabe ist nicht mehr neu
* Der abgeschlossene Prozentsatz der Aufgabe ist größer als null
* Die Aufgabe hat Vorgängerbeziehungen

Die folgende Tabelle zeigt, ob Änderungen am übergeordneten Trigger bei den untergeordneten Elementen aktualisiert wurden, die nicht einzeln bearbeitet wurden, oder ob ein Fortschritt angezeigt wird:

| Felder in der übergeordneten Aufgabe aktualisiert | Aktualisierungen werden auf nicht bearbeitete untergeordnete Elemente oder untergeordnete Elemente ohne aufgezeichneten Fortschritt übertragen |
|---|---|
| Wiederholungsfrequenz* | ✔ |
| Arbeitsaufträge | ✔ |
| Name | ✔ |
| Beschreibung | ✔ |
| Priorität | ✔ |
| Dauer | ✔ |
| Geplante Stunden | ✔ |
| Kostenart | ✔ |
| Umsatztyp | ✔ |
| Ressourcenabgleich | ✔ |
| Abgleichsverzögerung | ✔ |
| Aufgabenbeschränkung | Aktualisiert die untergeordneten Elemente nicht |
| Benutzerdefinierte Forms anfügen oder entfernen | Aktualisiert die untergeordneten Elemente nicht |
| Dauertyp | Aktualisiert die untergeordneten Elemente nicht |
| Informationen zu benutzerdefinierten Formularen | Aktualisiert die untergeordneten Elemente nicht |

{style="table-layout:auto"}

&#42; Wenn Sie die Wiederholungshäufigkeit einer übergeordneten Aufgabe aktualisieren, treten folgende Szenarien auf:

* Wenn Sie die Wiederholungshäufigkeit für eine vorhandene übergeordnete Aufgabe ändern, werden die vorhandenen Teilaufgaben gelöscht und durch neue Teilaufgaben ersetzt, die der neuen Wiederholungshäufigkeit folgen, wenn sie keinen Fortschritt aufweisen und wenn Sie sie nicht manuell aktualisiert haben.
* Wenn Sie die Wiederholungshäufigkeit für eine vorhandene übergeordnete Aufgabe ändern, werden Teilaufgaben, die einen Fortschritt anzeigen, nicht gelöscht. Diese Aufgaben werden zu diesem Zeitpunkt als von der Wiederholung getrennt betrachtet.

&#42;&#42; Zuweisungen für die übergeordnete Aufgabe werden auf alle Teilaufgaben in der Wiederholung angewendet. Alle Änderungen, die an der Zuordnung für die übergeordnete Aufgabe vorgenommen werden, überschreiben einzelne Zuweisungen für die Teilaufgabe. Wenn die Aufgabe den Fortschritt anzeigt, ändert sich die Zuweisung nicht.


