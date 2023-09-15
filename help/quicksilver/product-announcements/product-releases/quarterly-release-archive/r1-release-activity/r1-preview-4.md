---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Vorschau 4
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der R1.4-Version verfügbar sind. Die Funktionalität auf dieser Seite wurde am 15. Februar 2017 in der Vorschau-Umgebung bereitgestellt.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# R1 Vorschau 4

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit der R1.4-Version verfügbar sind. Die Funktionalität auf dieser Seite wurde am 15. Februar 2017 in der Vorschau-Umgebung bereitgestellt.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [Workfront R1-Version](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Aktualisierte Projekt-, Aufgaben- und Problemvalidierungen

Beim Erstellen von Genehmigungsprozessen für Projekt-, Aufgaben- und Problemgenehmigungen sind jetzt die folgenden Verbesserungen und Änderungen verfügbar: 

* Die Genehmigung &quot;Schritte&quot;wird jetzt als Genehmigung &quot;Phasen&quot;bezeichnet.
* Mehrere Arten von Genehmigern pro Phase einschließen.\
  Dazu gehören Benutzer, Teams und Arbeitsplatzrollen.\
  Vor dieser Änderung könnten Sie mehrere Genehmiger desselben Typs einbeziehen. Sie können beispielsweise mehrere Jobrollen einbeziehen, jedoch keine Auftrags- und Team-Rolle.

* Die folgenden bereits bestehenden Einschränkungen bei der Änderung bestehender globaler Genehmigungsprozesse wurden entfernt:

   * Der geänderte Validierungsprozess wird nur auf Objekten im gesamten System angewendet, bei denen der Validierungsprozess noch nicht gestartet oder der Validierungsprozess nicht geändert wurde. Objekte, bei denen der Validierungsprozess bereits gestartet oder der Validierungsprozess geändert wurde, werden nicht mit Ihren Änderungen aktualisiert.
   * Sie können den Status, der den Beginn der Genehmigung bestimmt, nicht ändern.

* Das Erscheinungsbild wurde aktualisiert.

Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Beim Verknüpfen eines Genehmigungsprozesses mit einem Projekt, einer Aufgabe oder einem Problem sind jetzt die folgenden Verbesserungen und Änderungen verfügbar:

* Das Erscheinungsbild wurde aktualisiert.
* Auf der Registerkarte Genehmigungen wird ein Genehmigungsdiagramm mit einer visuellen Darstellung der vorherigen, aktuellen und künftigen Genehmigungsschritte angezeigt.

Weitere Informationen zum Verknüpfen von Genehmigungen mit Projekten, Aufgaben und Problemen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Ändern des Status eines Projekts direkt auf der Projektseite

Sie müssen ein Projekt nicht mehr bearbeiten, um den Projektstatus zu ändern. Sie können jetzt den Status eines Projekts direkt auf der Hauptseite des Projekts ändern.

Weitere Informationen finden Sie unter [Ändern des Status eines Projekts](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Planen von Benutzern für die Deaktivierung

Sie können jetzt planen, dass Benutzer zu einem späteren Zeitpunkt deaktiviert werden.

Vor dieser Verbesserung konnten Sie einen Benutzer nur manuell sofort deaktivieren.

Die Planung der Deaktivierung eines Benutzers kann in verschiedenen Szenarien nützlich sein. Wenn Sie beispielsweise Benutzer in Workfront erstellen, die vorübergehend eingestellt werden, können Sie diese so einrichten, dass sie bei Vertragsende deaktiviert werden.

Diese Funktion ist auch bei der Massenbearbeitung von Benutzern verfügbar. 

Weitere Informationen zum Planen der Deaktivierung von Benutzern finden Sie unter [Benutzer deaktivieren oder reaktivieren](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) und [Benutzer hinzufügen](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Neue E-Mail-Digest-Optionen für &quot;Erforderliche Aktionen&quot;

Die Option Täglicher Digest-Versand ist jetzt im Bereich &quot;Erforderliche Aktion&quot;Ihrer Benachrichtigungseinstellungen verfügbar.

Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können. Dies ist erforderlich, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.

## Verbesserung des Papierkorbs: Wird im Aktualisierungs-Stream aufgezeichnet und erhält E-Mail-Benachrichtigung

Die folgenden Verbesserungen wurden beim Wiederherstellen gelöschter Projekte, Aufgaben und Probleme hinzugefügt:

* Nach dem Wiederherstellen eines Objekts erhalten Sie jetzt eine E-Mail-Benachrichtigung.\
  Als Workfront-Administrator erhalten Sie jetzt eine E-Mail-Benachrichtigung, nachdem Sie ein zuvor gelöschtes Projekt, eine Aufgabe oder ein Problem wiederhergestellt haben. Die E-Mail-Benachrichtigung informiert Sie über den Status des Wiederherstellungsprozesses.\
  Weitere Informationen zum Wiederherstellen von Objekten in Workfront finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Wenn das Objekt wiederhergestellt wird, wird das Löschen und Wiederherstellen des Objekts jetzt im Aktualisierungsstream des Objekts selbst und im Aktualisierungsstream des übergeordneten Objekts aufgezeichnet.\
  Zuvor wurde nur der Löschvorgang im Aktualisierungsstream des übergeordneten Objekts aufgezeichnet.\
  Wenn die Aufgabe beispielsweise wiederhergestellt wird, wird eine Meldung zum Aktualisierungsstream des Projekts und der Aufgabe selbst hinzugefügt, die angibt, dass die Aufgabe wiederhergestellt wurde. (Löschungen und Wiederherstellungen werden nicht bei Unteraufgaben aufgezeichnet. Informationen zum Löschen und Wiederherstellen von Unteraufgaben sind nur für übergeordnete Aufgaben verfügbar.)\
  Weitere Informationen finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Aktualisiertes Dialogfeld für die Verwaltung der Gruppenmitgliedschaft

Es gibt eine neue Benutzeroberfläche für die Verwaltung von Gruppen und Untergruppen, die ein einfacheres, benutzerfreundlicheres Erlebnis bietet.

Das Feld Gruppeneigentümer und das Feld Gruppenmitglieder werden jetzt in ein einzelnes Feld mit einer Liste von Gruppenmitgliedern kombiniert, die unten aufgeführt sind. Darüber hinaus können Sie die Liste der Gruppenmitglieder filtern und ändern, ob sie Inhaber oder Mitglied sind. 

Weitere Informationen zum Hinzufügen von Untergruppen zu Gruppen sowie zum Benennen von Benutzern als Mitglieder oder Gruppeneigentümer finden Sie unter [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Text in die mobile App kopieren

Sie können Text in die folgenden Felder aller Objekte kopieren, die in der Mobile App sichtbar sind:

* Name
* Beschreibung
* Referenznummer
* Kommentare

Diese Funktion sollte sowohl für die iOS- als auch für Android-Appstores in der Woche des 13. Februar veröffentlicht werden.
