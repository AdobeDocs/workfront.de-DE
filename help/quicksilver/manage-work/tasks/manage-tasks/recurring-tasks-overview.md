---
content-type: overview
product-area: projects
keywords: recurre,reoccur,reoccur
navigation-topic: manage-tasks
title: Übersicht über wiederkehrende Aufgaben
description: Übersicht über wiederkehrende Aufgaben
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '679'
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

Sie können wiederkehrende Aufgaben für Aktivitäten erstellen, die Sie im Rahmen eines Projekts wiederholen müssen.

In diesem Artikel werden Informationen und Überlegungen zum Erstellen und Bearbeiten wiederkehrender Aufgaben beschrieben.

Informationen zum Erstellen wiederkehrender Aufgaben in Adobe Workfront finden Sie unter [Wiederkehrende Aufgaben erstellen](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Übersicht über wiederkehrende Aufgaben und Überlegungen

Sie können wiederkehrende Aufgaben erstellen, um wiederholbare Arbeiten während der Lebensdauer eines Projekts anzuzeigen.

Beispielsweise muss während eines IT-Projekts Software wahrscheinlich in regelmäßigen Abständen gesichert werden. Durch das Erstellen einer wiederkehrenden Aufgabe für diese Aktivität wird der Zeitaufwand für die Einrichtung mehrerer einzelner Aufgaben verringert.

Beachten Sie beim Erstellen wiederkehrender Aufgaben in Workfront Folgendes:

* Sie können wiederkehrende Aufgaben nicht zu einer Vorlage hinzufügen.
* Sie können einer vorhandenen Aufgabe keine Wiederholungshäufigkeit hinzufügen.
* Wiederkehrende Aufgaben werden als Unteraufgaben oder untergeordnete Aufgaben für das Hauptvorkommen angezeigt, das als übergeordnete Aufgabe angezeigt wird.
* Eine Genehmigung kann nicht an eine übergeordnete wiederkehrende Aufgabe angehängt werden.
* Workfront überträgt die meisten Felder, die Sie beim Erstellen für die übergeordnete Wiederholung aktualisieren, an die untergeordneten Aufgaben. Die folgenden Felder werden bei ihrer Erstellung nicht an die untergeordneten Aufgaben übertragen:

   * Die Aufgabenbegrenzung der untergeordneten Aufgaben ändert sich automatisch in:

      * Muss bei Projekten beginnen, die ab dem Startdatum geplant sind.
      * Muss für Projekte, die ab dem Abschlussdatum geplant sind, abgeschlossen sein.

   * Die mit dem Elternteil verknüpften Dokumente werden nicht an die untergeordneten Elemente übertragen.

* Die folgenden Änderungen betreffen die übergeordnete Aufgabe, nachdem Sie angegeben haben, dass die Aufgabe wiederkehrend ist:

   * Das Feld Dauer wird für die übergeordnete Aufgabe in Dauer pro Auftreten umbenannt. Die Dauer für die untergeordneten Aufgaben bleibt erhalten.
   * Der Status ist in der übergeordneten Aufgabe deaktiviert und für die untergeordneten Elemente automatisch auf Neu eingestellt. Die übergeordnete Aufgabe wird automatisch abgeschlossen und der Status wird in Abgeschlossen aktualisiert, wenn alle untergeordneten Elemente abgeschlossen sind.
   * Die einzigen für wiederkehrende Aufgaben verfügbaren Arten von Dauer sind:

      * Einfach
      * Leistungsgesteuert
* Die Dauer und die für eine neue wiederkehrende Aufgabe angegebenen geplanten Stunden sind die Dauer und die geplanten Stunden eines jeden Vorkommens. Die Dauer der übergeordneten Aufgabe ist die Zeit zwischen dem geplanten Startdatum der frühesten Aufgabe und dem geplanten Abschlussdatum der letzten Aufgabe. Die &quot;Geplante Stunden&quot;der übergeordneten Aufgabe ist die Gesamtanzahl aller geplanten Stunden von allen Vorkommen.

## Überlegungen zum Bearbeiten wiederkehrender Aufgaben

Einige Änderungen, die Sie an einer übergeordneten Aufgabe für wiederkehrende Aufgaben vornehmen, werden möglicherweise nicht bei allen vorhandenen Vorkommen aktualisiert. Untergeordnete Aufgaben, die Fortschritt anzeigen oder einzeln aktualisiert wurden, werden beim Aktualisieren der übergeordneten Aufgabe nicht aktualisiert. Nach Auffassung von Workfront zeigt eine Aufgabe Fortschritte in folgenden Situationen an:

* Der Status wird aktualisiert und die Aufgabe ist nicht mehr neu
* Der Prozentsatz für den Abschluss der Aufgabe ist größer als null
* Die Aufgabe hat Vorgängerbeziehungen

Die folgende Tabelle zeigt, ob Änderungen am übergeordneten Trigger an den untergeordneten Elementen, die nicht einzeln bearbeitet wurden, aktualisiert wurden oder den Fortschritt anzeigen:

| Bei der übergeordneten Aufgabe aktualisierte Felder | Updates werden an unbearbeitete Kinder oder untergeordnete Elemente übertragen, ohne dass ein Fortschritt aufgezeichnet wurde |
|---|---|
| Wiederholungsfrequenz* | ms |
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
| Aufgabenbeschränkung | Aktualisieren der untergeordneten Elemente nicht |
| Benutzerdefinierte Forms anhängen oder entfernen | Aktualisieren der untergeordneten Elemente nicht |
| Dauertyp | Aktualisieren der untergeordneten Elemente nicht |
| Benutzerdefinierte Formulare - Informationen | Aktualisieren der untergeordneten Elemente nicht |

{style="table-layout:auto"}

&#42; Die folgenden Szenarien bestehen, wenn Sie die Häufigkeit der Wiederholungen einer übergeordneten Aufgabe aktualisieren:

* Wenn Sie die Häufigkeit der Wiederholungen für eine bestehende übergeordnete Aufgabe ändern, werden die vorhandenen Unteraufgaben gelöscht und durch neue Unteraufgaben ersetzt, die auf die neue Wiederholungshäufigkeit folgen, wenn keine Fortschritte angezeigt werden und Sie sie nicht manuell aktualisiert haben.
* Wenn Sie die Häufigkeit der Wiederholungen für eine bestehende übergeordnete Aufgabe ändern, werden Unteraufgaben, die Fortschritt anzeigen, nicht gelöscht. Diese Aufgaben werden zu diesem Zeitpunkt als von der Wiederholung getrennt betrachtet.

&#42;&#42; Zuweisungen, die an der übergeordneten Aufgabe vorgenommen werden, werden auf alle Unteraufgaben in der Wiederholung angewendet. Alle Änderungen, die an der Zuweisung der übergeordneten Aufgabe vorgenommen werden, überschreiben alle einzelnen Zuweisungen für die Unteraufgabe. Wenn die Aufgabe den Fortschritt anzeigt, ändert sich die Zuweisung nicht.

 
