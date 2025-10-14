---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1-Vorschau 4
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der Version R1.4 verfügbar sind. Die Funktion auf dieser Seite wurde am 15. Februar 2017 in der Vorschau-Umgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1-Vorschau 4

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der Version R1.4 verfügbar sind. Die Funktion auf dieser Seite wurde am 15. Februar 2017 in der Vorschau-Umgebung verfügbar gemacht.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [Workfront R1-Version](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Aktualisierte Projekt-, Aufgaben- und Problem-Genehmigungen

Beim Erstellen von Genehmigungsprozessen für Projekt-, Aufgaben- und Problem-Genehmigungen sind jetzt die folgenden Verbesserungen und Änderungen verfügbar: 

* Die „Genehmigungsschritte“ werden jetzt als „Genehmigungsschritte“ bezeichnet.
* Schließen Sie mehrere Arten von Genehmigern pro Schritt ein.\
  Dazu gehören Benutzer, Teams und Aufgabengebiete.\
  Vor dieser Änderung konnten Sie mehrere genehmigende Personen desselben Typs einbeziehen. Sie können beispielsweise mehrere Aufgabengebiete einbeziehen, jedoch kein Aufgabengebiet und kein Team.

* Die folgenden bereits bestehenden Einschränkungen im Zusammenhang mit der Änderung vorhandener globaler Genehmigungsprozesse wurden entfernt:

   * Der geänderte Genehmigungsprozess wird nur für Objekte im System übernommen, bei denen der Genehmigungsprozess noch nicht gestartet wurde oder der Genehmigungsprozess nicht geändert wurde. Objekte, bei denen der Genehmigungsprozess bereits gestartet oder geändert wurde, werden nicht mit den Änderungen aktualisiert.
   * Sie können den Status, der bestimmt, wann die Genehmigung beginnt, nicht ändern.

* Das Erscheinungsbild wurde aktualisiert.

Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Beim Verknüpfen eines Genehmigungsprozesses mit einem Projekt, einer Aufgabe oder einem Problem sind jetzt die folgenden Verbesserungen und Änderungen verfügbar:

* Das Erscheinungsbild wurde aktualisiert.
* Das Genehmigungsdiagramm wird auf der Registerkarte Genehmigungen angezeigt, die frühere, aktuelle und künftige Genehmigungsschritte visuell darstellt.

Weitere Informationen zum Verknüpfen von Genehmigungen mit Projekten, Aufgaben und Problemen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Ändern des Status eines Projekts direkt auf der Projektseite

Sie müssen ein Projekt nicht mehr bearbeiten, um den Projektstatus zu ändern. Sie können jetzt den Status eines Projekts direkt auf der Hauptseite des Projekts ändern.

Weitere Informationen finden Sie unter [Ändern des Status eines Projekts](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Planen von Benutzern für die Deaktivierung

Sie können jetzt festlegen, dass Benutzer zu einem späteren Zeitpunkt deaktiviert werden.

Vor dieser Verbesserung konnten Sie einen Benutzer nur sofort manuell deaktivieren.

Die Deaktivierung von Benutzenden kann in verschiedenen Szenarien nützlich sein. Wenn Sie beispielsweise in Workfront Benutzende erstellen, die vorübergehend eingestellt werden, können Sie diese so einrichten, dass sie bei Vertragsende deaktiviert werden.

Diese Funktion ist auch bei der Massenbearbeitung von Benutzern verfügbar. 

Weitere Informationen zum Planen von Benutzern für die Deaktivierung finden Sie unter [Deaktivieren oder Reaktivieren eines &#x200B;](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) und [Benutzer hinzufügen](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Neue E-Mail-Digest-Optionen für „Aktionen erforderlich“

Die Versandoption Daily Digest ist jetzt im Bereich „Aktion erforderlich“ in den Benachrichtigungseinstellungen verfügbar.

Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Verbesserung des Papierkorbs: Wird im Aktualisierungsverlauf aufgezeichnet und erhält E-Mail-Benachrichtigungen

Die folgenden Verbesserungen wurden beim Wiederherstellen gelöschter Projekte, Aufgaben und Probleme hinzugefügt:

* Sie erhalten jetzt eine E-Mail-Benachrichtigung, nachdem Sie ein Objekt wiederhergestellt haben.\
  Als Workfront-Administrator erhalten Sie jetzt eine E-Mail-Benachrichtigung, nachdem Sie ein zuvor gelöschtes Projekt, eine Aufgabe oder ein Problem wiederhergestellt haben. Die E-Mail-Benachrichtigung informiert Sie über den Status des Wiederherstellungsprozesses.\
  Weitere Informationen zum Wiederherstellen von Objekten in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Wenn das Objekt wiederhergestellt wird, wird das Löschen und Wiederherstellen des Objekts jetzt im Aktualisierungsstrom des Objekts selbst und im Aktualisierungsstrom des übergeordneten Objekts aufgezeichnet.\
  Zuvor wurde nur der Löschvorgang im Aktualisierungsverlauf des übergeordneten Objekts aufgezeichnet.\
  Wenn die Aufgabe beispielsweise wiederhergestellt wird, wird eine Meldung zum Aktualisierungsverlauf sowohl des Projekts als auch der Aufgabe selbst hinzugefügt, die angibt, dass die Aufgabe wiederhergestellt wurde. (Löschungen und Wiederherstellungen werden nicht in Teilaufgaben aufgezeichnet. Informationen zum Löschen und Wiederherstellen von Teilaufgaben sind nur für übergeordnete Aufgaben verfügbar.)\
  Weitere Informationen finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Das Dialogfeld zum Verwalten der Gruppenmitgliedschaft wurde aktualisiert

Es gibt eine neue Benutzeroberfläche für die Verwaltung von Gruppen und Untergruppen , die eine einfachere, benutzerfreundlichere Oberfläche bietet.

Das Feld Gruppeneigentümer und das Feld Gruppenmitglieder sind jetzt in einem einzigen Feld zusammengefasst, mit einer Liste der Gruppenmitglieder, die unten aufgeführt ist. Darüber hinaus können Sie die Liste der Gruppenmitglieder filtern und ändern, ob sie Inhaber oder Mitglied sind. 

Weitere Informationen zum Hinzufügen von Untergruppen zu Gruppen sowie zum Festlegen von Benutzern als Mitglieder oder Gruppenbesitzer von Gruppen finden Sie unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Kopieren von Text in die Mobile App

Sie können Text in die folgenden Felder aller Objekte kopieren, die in der Mobile App sichtbar sind:

* Name
* Beschreibung
* Referenznummer
* Kommentare

Diese Funktion sollte in der Woche vom 13. Februar sowohl für die iOS- als auch für die Android-App-Stores veröffentlicht werden.
