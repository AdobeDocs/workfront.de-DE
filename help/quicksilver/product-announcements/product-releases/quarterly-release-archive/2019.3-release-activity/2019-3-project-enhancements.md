---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Projektverbesserungen in 2019.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die mit Projektverbesserungen in der Version 2019.3 vorgenommen wurden. Es wurde in der Woche vom 19. August 2019 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Projektverbesserungen in 2019.3

Auf dieser Seite werden alle Änderungen beschrieben, die mit Projektverbesserungen in der Version 2019.3 vorgenommen wurden. Es wurde in der Woche vom 19. August 2019 in der Produktionsumgebung bereitgestellt.

Eine Liste aller in 2019.3 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Ändern des Anzeigetyps eines Felds in einem benutzerdefinierten Formular

Jetzt können Sie den Anzeigetyp eines Felds in einem benutzerdefinierten Formular ändern.

Wenn Sie beispielsweise ein Kontrollkästchen erstellt haben, können Sie es in ein Dropdown-Feld oder ein Optionsfeld ändern. Diese drei Anzeigetypen für Felder sind austauschbar.

Wenn Sie ein einzeiliges Textfeld erstellt haben, können Sie es auch in ein Absatztextfeld ändern. Diese beiden Feldanzeigetypen sind austauschbar.

Um den Anzeigetyp eines benutzerdefinierten Felds zu ändern, mussten Sie zuvor ein neues Feld erstellen und das alte löschen. Dies erforderte die Übertragung von Daten, was häufig zeitaufwendig war.

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 9. August 2019
>
>Produktionsverfügbarkeit: 30. August 2019

## Erstellen von Zeitplänen und Berichten

Sie können jetzt die Ausfallzeiten der Benutzenden für eine bessere Planung und Ausführung sehen. Sie können Ihren Dashboards auch neue Berichte und Kalender hinzufügen, um eine Echtzeitansicht der Benutzerverfügbarkeit zu erhalten.

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 9. August 2019
>
>Produktionsverfügbarkeit: 30. August 2019

## Der Filter Öffnen zeigt jetzt weitere Ergebnisse in einer Liste von Problemen an

Wenn Sie den Filter Öffnen auf eine Liste von Problemen anwenden, enthält die Liste Probleme, die:

* befinden sich im Status Geschlossen - Genehmigung steht aus
* Sind mit einem Lösungsobjekt verknüpft

Vor dieser Änderung waren diese Probleme nicht in der Liste enthalten, wenn der Filter Öffnen angewendet wurde.

## Neues Erlebnis bei der Inline-Bearbeitung von Informationen in Listen

Wenn Sie Informationen in den neuen Listen inline bearbeiten, werden die Zeilen, die bearbeitet wurden, abgeblendet, aber die Informationen bleiben sichtbar. Vor dieser Änderung waren die bearbeiteten Zeilen ausgegraut und die Informationen waren nicht sichtbar.

Die neuen Listen finden Sie in den folgenden Bereichen von Workfront:

* Projekt- und Aufgabenlisten
* Registerkarte „Stunden“ für Projekte, Aufgaben und Probleme

## Aktualisierte Listen für Projekte, Aufgaben und Probleme auf den Stunden -Registerkarten

Die verbesserten Listenansichten sind jetzt auf den Registerkarten Stunden für Projekte, Aufgaben und Probleme verfügbar.

Vor dieser Verbesserung wurden die neuen Listen nur auf Folgendes angewendet:

* Eine Liste von Aufgaben
* Eine Liste von Projekten

Informationen zum Anzeigen von Elementen in einer Liste finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Gantt bearbeiten, ohne einen speziellen Bearbeitungsmodus zu aktivieren

Sie können jetzt das Gantt-Diagramm der Aufgabenliste bearbeiten, wenn das automatische Speichern aktiviert ist oder nicht. Sie können Änderungen nicht rückgängig machen, wenn der Umschalter aktiviert ist. In diesem Fall werden die von Ihnen am Projekt vorgenommenen Änderungen automatisch gespeichert.

Weitere Informationen zum Bearbeiten des Aufgabenlisten-Gantt-Diagramms finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Entfernen der Registerkarte „Probleme“ vom Kanban-Board

Wir entfernen die Registerkarte „Probleme“ aus dem Kanban-Board in der Produktionsversion 19.3. Sie können weiterhin über den Rückstand auf dem Kanban-Board auf die Unterregisterkarte „Probleme“ zugreifen.

## Entfernen der Registerkarten Dokumente und Probleme von der Seite mit den Iterationsdetails

>[!NOTE]
>
>Diese Änderung erfolgt in der Produktionsumgebung mit der Version 2019.3. Sie wird nicht in der Vorschau-Umgebung vor der Produktionsfreigabe erstellt.

Wir entfernen die Registerkarten Dokumente und Probleme von der Seite mit den Details zur Agile-Iteration:

* **Dokumente:** Alle auf der Registerkarte Dokumente gespeicherten Dokumente müssen vor der Produktionsfreigabe verschoben werden. Wenn Sie Ihre Dokumente nicht verschieben können, haben Sie keinen Zugriff mehr darauf.
* **Probleme:** Diese Registerkarte befindet sich in der Regel unter dem Dropdown-Menü Mehr . Sie können weiterhin über die Registerkarte Arbeitselemente der Iteration auf die Unterregisterkarte Probleme zugreifen.

## Benutzer-Ausfallzeiten in Aufgabenterminen berücksichtigen oder ignorieren

Sie können jetzt entscheiden, ob der Zeitplan für die Ausfallzeit des Primären Verantwortlichen einer Aufgabe angepasst werden soll, um die geplanten Termine anzupassen.

Sie können diese Entscheidung entweder auf Systemebene, als Workfront-Administrator oder auf Projektebene als Projekt-Manager treffen.

Vor dieser Änderung wurden durch die Ausfallzeit des Primären Verantwortlichen immer die geplanten Termine der Aufgabe angepasst, wenn die Aufgabenbeschränkung die Änderung der Termine zulässt.

Weitere Informationen zur Einstellung für die Ausfallzeit von Benutzern auf Systemebene finden Sie unter [Konfigurieren von systemweiten Projektvoreinstellungen](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Weitere Informationen zur Einstellung für die Ausfallzeit von Benutzern auf Projektebene finden Sie unter [Projekte bearbeiten](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 22. Juli 2019
>
>Produktionsverfügbarkeit: 9. August 2019

## Benutzerdefinierte Bedingungen

Jetzt können Sie die folgenden Schritte ausführen, um die Bedingungen, die Sie für Projekte, Aufgaben und Probleme verwenden, anzupassen und sie besser an die Anforderungen Ihrer Organisation anzupassen:

* Erstellen Sie benutzerdefinierte Bedingungen mit eigenen Kennzeichnungen und Farben.
* Ändern Sie die Reihenfolge der Bedingungen in den Dropdown-Listen, in denen Benutzer sie auswählen.
* Verwenden Sie benutzerdefinierte Bedingungen, die Sie anstelle der integrierten Standardbedingungen erstellen, die Workfront automatisch Arbeitselementen zuweist.
* Ändern Sie die Namen und Farben der integrierten Standardbedingungen für Projekte, Aufgaben und Probleme.

Wenn Sie außerdem berechtigt sind, eine Aufgabe oder ein Problem zu bearbeiten, Ihnen aber nicht zugewiesen sind (vielleicht weil Sie diese Aufgabe oder Anfrage überwachen), können Sie jetzt mithilfe der Spalte Bedingungen in einer Listenansicht ihre Bedingung ändern.

Zuvor konnten Bedingungen nicht angepasst oder geändert werden, und nur Benutzende konnten die Bedingung einer Aufgabe oder eines Problems ändern, wenn sie ihr zugewiesen waren.

Weitere Informationen finden Sie unter [Benutzerdefinierte Bedingungen](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 4. Juli 2019
>
>Produktionsverfügbarkeit: Ende September oder Anfang Oktober

## Neue E-Mail-Benachrichtigung für Teams

Es gibt eine neue E-Mail-Ereignisbenachrichtigung für Teams. Teammitglieder erhalten eine E-Mail-Benachrichtigung, wenn ein Projekt mit Aufgaben, die ihrem Team zugewiesen sind, aktiv wird. Diese Einstellung ist standardmäßig deaktiviert.

Zuvor konnten Teammitglieder nicht benachrichtigt werden, wann Projekte aktiv wurden, an denen sie beteiligt waren.

Weitere Informationen finden Sie unter Benachrichtigungen: Informationen zu Projekten, an denen ich mitwirke.

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 4. Juli 2019
>
>Produktionsverfügbarkeit: 18. Juli 2019

## Dokumentaktualisierungen werden jetzt auf dem zugehörigen Objekt und Projekt angezeigt

Wenn Sie einen Kommentar zu einem Dokument abgeben, wird die Aktualisierung jetzt auf der Registerkarte Aktualisierungen sowohl für das Dokument als auch für das Objekt angezeigt, an das das Dokument angehängt ist.

Wenn das Objekt Teil eines Projekts ist, wird Ihr Kommentar zum Dokument auch auf der Registerkarte Aktualisierungen für das Projekt angezeigt.

Zuvor wurden Kommentare zu Aktualisierungen nur auf der Registerkarte Aktualisierungen für das Dokument angezeigt.

Weitere Informationen finden Sie im Abschnitt [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) im Artikel [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 6. Juni 2019
>
>Produktionsverfügbarkeit: 20. Juni 2019

## Einblick in den Urlaubsplan eines Benutzers bei der Zuweisung zu Aufgaben und Problemen

Wenn Sie einer Aufgabe oder einem Problem einen Benutzer zuweisen, wird jetzt eine Inline-Warnung angezeigt, wenn der Benutzer Ausfallzeiten ausgewählt hat, die zu einem beliebigen Zeitpunkt zwischen den geplanten Terminen der Aufgabe oder des Problems liegen.

Informationen zum Zuweisen von Aufgaben finden Sie unter [Aufgaben zuweisen](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Informationen zu Ausfallzeiten finden Sie unter [Konfigurieren von persönlichen Ausfallzeiten](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 30. Mai 2019
>
>Produktionsverfügbarkeit: 13. Juni 2019

## Fügen Sie Felder hinzu, die Objekte in der benutzerdefinierten Forms darstellen

Im benutzerdefinierten Formular-Builder wurde ein neuer Feldtyp mit dem Namen Typeahead erstellt. In diesem Feld können Sie den benutzerdefinierten Formularen Felder hinzufügen, die Objekte darstellen. Derzeit ist das Benutzerobjekt mit automatischer Textvervollständigung aktiviert, und weitere Objekte werden in Zukunft bereitgestellt.

Zuvor mussten Administratoren Benutzer manuell als individuelle Optionen in benutzerdefinierten Dropdown-Menüs für Formulare verwalten.

>[!NOTE]
>
>Vorschau-Verfügbarkeit: 30. Mai 2019
>
>Produktionsverfügbarkeit: 13. Juni 2019
>
>Vor dem Produktionsveröffentlichungsdatum werden die neuen benutzerdefinierten Felder in Mobile, Outlook, MS Teams und der nativen Salesforce-Integration nicht unterstützt.
>
>In der Produktion werden jetzt Outlook- und MS Teams unterstützt. Mobile wird seit Ende Juni oder Anfang Juli unterstützt; Salesforce-Integrationen werden seit Juni unterstützt.

## Das neue Feld „Betreff“ der Anfrage wurde in „Name“ umbenannt

>[!NOTE]
>
>Diese Funktion wurde entfernt und wird in der Version 2019.3 nicht enthalten sein.

Wenn Sie jetzt eine neue Anfrage an eine Anfrage-Warteschlange senden, geben Sie den Namen der Anfrage in das Feld „Name“ des neuen Anfrageformulars ein.

Vor dieser Änderung geben Sie den Namen der Anfrage im Feld „Betreff“ ein.

Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Workfront-Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

