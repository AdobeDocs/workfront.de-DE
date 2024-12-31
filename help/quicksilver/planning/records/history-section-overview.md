---
title: Übersicht über den Verlaufsabschnitt
description: Änderungen am Datensatz, die vom System aufgezeichnet wurden, können in Adobe Workfront Planning im rechten Bereich eines Datensatzes eingesehen werden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 3%

---

# Übersicht über den Verlaufsabschnitt

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

Sie können an Adobe Workfront Planning-Datensätzen zusammenarbeiten, indem Sie Kommentare oder Antworten im rechten Bedienfeld eines Datensatzes hinzufügen. Sie können auch andere Änderungen am Datensatz anzeigen, die vom System in diesem Bereich aufgezeichnet wurden.

Im rechten Bereich eines Datensatzes werden die folgenden Abschnitte angezeigt:

* **Kommentare**: Zeigt Kommentare und Antworten an, die Benutzende zu Datensätzen hinzufügen. Weitere Informationen zum Verwalten von Kommentaren in Workfront-Planungsdatensätzen finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* **History**: Zeigt systemaufgezeichnete Änderungen an, die Benutzer an den Datensatzfeldern vornehmen.

## Suchen des Abschnitts „Verlauf“ eines Datensatzes

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet, und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite „Datensatztyp“ wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Die Seite des Datensatzes wird geöffnet. Der Bereich Kommentare wird standardmäßig im rechten Bedienfeld geöffnet.
1. Klicken Sie auf **Symbol** Verlauf anzeigen![](assets/show-history-icon.png). Alle Änderungen, die an den Feldern des Datensatzes vorgenommen wurden, werden im rechten Bereich angezeigt, beginnend mit dem letzten.
1. (Optional) Klicken Sie auf das ![](assets/hide-history-icon.png) **Verlauf ausblenden**, um das rechte Bedienfeld zu schließen.

## Überlegungen zum Abschnitt „Verlauf“

Die an den Datensatzfeldern vorgenommenen Änderungen können Sie im Abschnitt Verlauf des rechten Bedienfelds der Datensatzseite überprüfen.

![](assets/history-area-in-comments.png)

* Workfront Planning zeichnet die folgenden Informationen im Abschnitt History auf:

   * Alle Feldänderungen

   * Die alten und neuen Werte von Feldern, wenn sich die Werte ändern. Die alten Werte werden im durchgestrichenen Format angezeigt.

   * Der vollständige Name des Benutzers, der die Änderung vorgenommen hat

   * Ein Datums- und Zeitstempel, der angibt, wann die Änderung vorgenommen wurde.

* In Feldern der folgenden Typen werden immer der alte Wert (im Durchgestrichenformat) und der neue Wert angezeigt:

   * Text
   * Absatz
   * Währung
   * Datum
   * Zahl
   * Prozentsatz
   * Einzelauswahl

* Felder der folgenden Typen zeigen den alten Wert nur dann im durchgestrichenen Format an, wenn mindestens einer der mehreren Werte entfernt wurde:

   * Mehrfachauswahl
   * Verknüpfte Datensatzfelder
   * Personen

  Wenn durch die Änderung nur Werte zum Feld hinzugefügt werden, wird der alte Wert nicht angezeigt und nur der neue Feldwert.

* Bei Feldern vom Typ „Kontrollkästchen“ wird der alte Wert nie im Durchgestrichenformat angezeigt. Wenn das Feld bearbeitet wird, wird nur der aktuelle Status zum Zeitpunkt der Änderung angezeigt.

  Weitere Informationen zu Workfront Planning-Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

* Änderungen an Feldern der folgenden Typen werden nicht im Abschnitt Verlauf angezeigt:

   * Verknüpfte (Lookup-)Felder
   * Formel
   * Erstellt von
   * Erstellt am
   * Zuletzt geändert von
   * Zuletzt geändert am

* Wenn ein Feld aus dem System entfernt wird, bleiben die in diesem Feld vorgenommenen Aktualisierungen im Abschnitt Verlauf erhalten. Es gibt keinen Hinweis darauf, dass das Feld im Abschnitt Verlauf eines Datensatzes entfernt wurde.
