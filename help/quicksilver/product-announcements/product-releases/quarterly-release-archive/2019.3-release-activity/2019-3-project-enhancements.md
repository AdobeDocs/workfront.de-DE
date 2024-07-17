---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Projektverbesserungen
description: Auf dieser Seite werden alle Änderungen beschrieben, die mit Version 2019.3 vorgenommen wurden. Es wurde in der Produktionsumgebung in der Woche vom 19. August 2019 zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# 2019.3 Projektverbesserungen

Auf dieser Seite werden alle Änderungen beschrieben, die mit Version 2019.3 vorgenommen wurden. Es wurde in der Produktionsumgebung in der Woche vom 19. August 2019 zur Verfügung gestellt.

Eine Liste aller Änderungen, die in Version 2019.3 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Ändern des Anzeigetyps eines Felds in einem benutzerdefinierten Formular

Jetzt können Sie den Anzeigetyp eines Felds in einem benutzerdefinierten Formular ändern.

Wenn Sie beispielsweise ein Kontrollkästchen-Feld erstellt haben, können Sie es in ein Dropdown-Feld oder ein Optionsfeld ändern. Diese drei Feldanzeigetypen sind austauschbar.

Wenn Sie ein einzeiliges Textfeld erstellt haben, können Sie es in ein Absatztext -Feld ändern. Diese beiden Feldanzeigetypen sind austauschbar.

Bisher mussten Sie zum Ändern des Anzeigetyps eines benutzerdefinierten Felds ein neues Feld erstellen und das alte löschen. Dies erforderte die Übertragung von Daten, die häufig zeitaufwendig waren.

Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) im Artikel [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 9. August 2019
>
>Produktionsverfügbarkeit: 30. August 2019

## Erstellen von Zeitplänen und Berichten

Sie können nun die Zeitdauer des Benutzers für eine bessere Planung und Ausführung sehen. Sie können Ihren Dashboards auch neue Zeiträume für Berichte und Kalender hinzufügen, um einen Echtzeitüberblick über die Benutzerverfügbarkeit zu erhalten.

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 9. August 2019
>
>Produktionsverfügbarkeit: 30. August 2019

## Der Filter Öffnungen zeigt jetzt mehr Ergebnisse in einer Liste von Problemen an

Wenn Sie den Filter Öffnungen auf eine Liste von Problemen anwenden, enthält die Liste Probleme, die:

* Befindet sich in einem geschlossenen - Status Ausstehende Genehmigung
* sind mit einem auflösenden Objekt verknüpft

Vor dieser Änderung wurden diese Probleme beim Anwenden des Filters &quot;Öffnen&quot;nicht in die Liste aufgenommen.

## Neues Erlebnis bei der Inline-Bearbeitung von Informationen in Listen

Wenn Sie Informationen in den neuen Listen inline bearbeiten, werden die bearbeiteten Zeilen abgeblendet, die Informationen bleiben jedoch sichtbar. Vor dieser Änderung wurden die bearbeiteten Zeilen grau ausgeblendet und die Informationen waren nicht sichtbar.

Die neuen Listen finden Sie in den folgenden Bereichen von Workfront:

* Listen &quot;Projekt und Aufgaben&quot;
* Registerkarte &quot;Stunden&quot;für Projekte, Aufgaben und Probleme

## Aktualisierte Listen für die Registerkarten &quot;Projekt&quot;, &quot;Aufgabe&quot;und &quot;Problemstunden&quot;

Die verbesserten Listenansichten sind jetzt auf den Registerkarten Stunden für Projekte, Aufgaben und Probleme verfügbar.

Vor dieser Verbesserung wurden die neuen Listen nur auf Folgendes angewendet:

* Eine Liste von Aufgaben
* Liste der Projekte

Informationen zum Anzeigen von Elementen in einer Liste finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Gantt bearbeiten, ohne einen speziellen Bearbeitungsmodus zu aktivieren

Sie können jetzt das Gantt-Diagramm der Aufgabenliste bearbeiten, wenn die automatische Speicherung aktiviert ist oder nicht. Sie können Änderungen nicht rückgängig machen, wenn der Umschalter aktiviert ist. In diesem Fall werden die Änderungen, die Sie am Projekt vornehmen, automatisch gespeichert.

Informationen zum Bearbeiten des Gantt-Diagramms der Aufgabenliste finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Entfernen der Registerkarte Probleme aus dem Kanban-Forum

Wir entfernen die Registerkarte Probleme im Kanban-Board in der Produktionsversion 19.3. Der Zugriff auf die Unterregisterkarte Probleme erfolgt weiterhin über das Backlog auf der Kanban-Pinnwand.

## Entfernen der Registerkarten Dokumente und Probleme von der Seite mit den Iterationsdetails

>[!NOTE]
>
>Diese Änderung erfolgt in der Produktion mit der Version 2019.3. Sie wird nicht vor der Produktionsversion in der Vorschau-Umgebung vorgenommen.

Wir entfernen die Registerkarten Dokumente und Probleme von der Seite mit Details zur Agile-Iteration:

* **Dokumente:** Alle auf der Registerkarte &quot;Dokumente&quot;gespeicherten Dokumente müssen vor der Produktionsversion verschoben werden. Wenn Sie Ihre Dokumente nicht verschieben, haben Sie keinen Zugriff mehr auf sie.
* **Probleme:** Diese Registerkarte befindet sich im Allgemeinen im Dropdownmenü Mehr . Sie können weiterhin auf die Unterregisterkarte Probleme auf der Registerkarte Arbeitselemente der Iteration zugreifen.

## Benutzerzeitlimit in Aufgabendaten berücksichtigen oder ignorieren

Jetzt können Sie entscheiden, ob Sie die Zeitdauer des Primären Verantwortlichen einer Aufgabe so einstellen möchten, dass die geplanten Daten angepasst werden.

Sie können diese Entscheidung entweder auf Systemebene, als Workfront-Administrator oder auf Projektebene als Projektmanager treffen.

Vor dieser Änderung hat die Zeitdauer des Primären Verantwortlichen immer die geplanten Zeitpunkte der Aufgabe angepasst, wenn die Aufgabenbegrenzung eine Änderung der Daten zulässt.

Weitere Informationen zur Einstellung &quot;Zeitlimit für Benutzer&quot;auf Systemebene finden Sie unter [Systemweite Projektanvoreinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Weitere Informationen zur Einstellung &quot;Zeitlimit für Benutzer&quot;auf Projektebene finden Sie unter [Projekte bearbeiten](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 22. Juli 2019
>
>Produktionsverfügbarkeit: 9. August 2019

## Benutzerdefinierte Bedingungen

Jetzt können Sie die folgenden Schritte ausführen, um die Bedingungen, die Sie für Projekte, Aufgaben und Probleme verwenden, anzupassen und die Anforderungen Ihrer Organisation besser zu erfüllen:

* Erstellen Sie benutzerdefinierte Bedingungen mit Ihren eigenen Beschriftungen und Farben.
* Ändern Sie die Reihenfolge der Bedingungen in den Dropdown-Listen, in denen die Benutzer sie auswählen.
* Verwenden Sie benutzerdefinierte Bedingungen, die Sie anstelle der integrierten Standardbedingungen erstellen, die Workfront Arbeitselementen automatisch zuweist.
* Ändern Sie die Namen und Farben der integrierten Standardbedingungen für Projekte, Aufgaben und Probleme.

Wenn Sie darüber hinaus berechtigt sind, eine Aufgabe oder ein Problem zu bearbeiten, ihr jedoch nicht zugewiesen sind (weil Sie sie möglicherweise übersehen), können Sie jetzt ihre Bedingung mithilfe der Spalte Bedingungen in einer Listenansicht ändern.

Zuvor konnten Bedingungen nicht angepasst oder geändert werden und nur Benutzer konnten die Bedingung einer Aufgabe oder eines Problems ändern, wenn sie ihr zugewiesen waren.

Weitere Informationen finden Sie unter [Benutzerdefinierte Bedingungen](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 4. Juli 2019
>
>Produktionsverfügbarkeit: Ende September oder Anfang Oktober

## Neue E-Mail-Benachrichtigung für Teams

Es gibt eine neue E-Mail-Ereignisbenachrichtigung für Teams. Teammitglieder erhalten eine E-Mail-Benachrichtigung, wenn ein Projekt mit Aufgaben, die ihrem Team zugewiesen sind, aktiv wird. Diese Einstellung ist standardmäßig deaktiviert.

Zuvor konnten Teammitglieder nicht benachrichtigt werden, wenn Projekte aktiv wurden.

Weitere Informationen finden Sie unter Benachrichtigungen: Informationen zu Projekten, die ich verwende.

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 4. Juli 2019
>
>Produktionsverfügbarkeit: 18. Juli 2019

## Dokumentaktualisierungen werden jetzt auf dem zugehörigen Objekt und Projekt angezeigt

Wenn Sie einen Kommentar zu einem Dokument abgeben, wird Ihre Aktualisierung jetzt auf der Registerkarte &quot;Aktualisierungen&quot;sowohl für das Dokument als auch für das Objekt angezeigt, an das das Dokument angehängt ist.

Wenn das Objekt Teil eines Projekts ist, wird der Kommentar zum Dokument auch auf der Registerkarte &quot;Aktualisierungen&quot;für das Projekt angezeigt.

Zuvor wurden Aktualisierungskommentare nur auf der Registerkarte Aktualisierungen für das Dokument angezeigt.

Weitere Informationen finden Sie im Abschnitt [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) im Artikel [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 6. Juni 2019
>
>Produktionsverfügbarkeit: 20. Juni 2019

## Sichtbarkeit des Zeitplans eines Benutzers bei der Zuweisung dieser Daten zu Aufgaben und Problemen

Wenn Sie einen Benutzer einer Aufgabe oder einem Problem zuweisen, wird jetzt eine Inline-Warnung angezeigt, wenn der ausgewählte Benutzer zwischen den geplanten Daten der Aufgabe oder des Problems eine Zeitüberschreitung hat.

Weitere Informationen zum Zuweisen von Aufgaben finden Sie unter [Aufgaben zuweisen](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Weitere Informationen zur Zeitdauer finden Sie unter [Persönliche Zeit von ](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md) konfigurieren.

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 30. Mai 2019
>
>Produktionsverfügbarkeit: 13. Juni 2019

## Felder hinzufügen, die Objekte in benutzerdefiniertem Forms darstellen

Wir haben einen neuen Feldtyp im benutzerdefinierten Formular-Builder mit dem Namen &quot;TypeAhead&quot;erstellt. In diesem Feld können Sie Felder hinzufügen, die Objekte zu Ihren benutzerdefinierten Formularen darstellen. Derzeit ist das User-Objekt mit &quot;TypeAhead&quot;aktiviert, und andere Objekte werden in Zukunft verfügbar sein.

Zuvor mussten Administratoren Benutzer manuell als einzelne Optionen in Dropdown-Menüs für benutzerdefinierte Formulare verwalten.

Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>Vorschau der Verfügbarkeit: 30. Mai 2019
>
>Produktionsverfügbarkeit: 13. Juni 2019
>
>Vor dem Produktionsveröffentlichungsdatum werden die neuen benutzerdefinierten Felder in Mobile, Outlook, MS Teams und der nativen Salesforce-Integration nicht unterstützt.
>
>In der Produktion werden Outlook- und MS-Teams jetzt unterstützt. Mobile wird seit Ende Juni oder Anfang Juli unterstützt. Salesforce-Integrationen werden seit Juni unterstützt.

## Das neue Feld &quot;Betreff&quot;der Anfrage wurde in &quot;Name&quot;umbenannt.

>[!NOTE]
>
>Diese Funktion wurde entfernt und wird in der Version 2019.3 nicht enthalten sein.

Wenn Sie jetzt eine neue Anforderung an eine Anforderungswarteschlange senden, geben Sie den Namen der Anforderung in das Feld &quot;Name&quot;des neuen Anfrageformulars ein.

Vor dieser Änderung geben Sie den Namen der Anfrage in das Feld &quot;Betreff&quot;ein.

Informationen zum Erstellen von Anforderungen finden Sie unter [Erstellen und Senden von Workfront-Anforderungen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

