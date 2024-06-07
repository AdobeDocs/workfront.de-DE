---
title: Übersicht über den Verlaufsabschnitt
description: Sie können Änderungen am Datensatz überprüfen, die vom System im rechten Bereich eines Datensatzes in der Adobe Workfront-Planung vorgenommen und aufgezeichnet wurden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 3%

---

# Übersicht über den Verlaufsabschnitt

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Sie können an Adobe Workfront-Planungsdatensätzen zusammenarbeiten, indem Sie im rechten Bereich eines Datensatzes Kommentare oder Antworten hinzufügen. Sie können auch andere Änderungen anzeigen, die am Datensatz vorgenommen und vom System in diesem Bereich aufgezeichnet wurden.

Im rechten Bereich eines Datensatzes werden die folgenden Abschnitte angezeigt:

* **Kommentare**: Zeigt Kommentare und Antworten an, die Benutzer zu Datensätzen hinzufügen. Weitere Informationen zum Verwalten von Kommentaren in Workfront-Planungsprotokollen finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* **Geschichte**: Zeigt systemaufgezeichnete Änderungen an, die Benutzer an den Datensatzfeldern vornehmen.

## Suchen Sie den Abschnitt Verlauf eines Datensatzes

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite mit dem Datensatztyp wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü.
1. Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.

   Die Seite des Datensatzes wird geöffnet. Der Bereich Kommentare wird standardmäßig im rechten Bereich geöffnet.
1. Klicken Sie auf **Verlauf anzeigen** icon ![](assets/show-history-icon.png). Alle Änderungen an den Feldern des Datensatzes werden im rechten Bereich angezeigt, beginnend mit dem letzten.
1. (Optional) Klicken Sie auf die **Verlauf ausblenden** icon ![](assets/hide-history-icon.png) , um den rechten Bereich zu schließen.

## Überlegungen zum Abschnitt Verlauf

Sie können die Änderungen, die an den Feldern vorgenommen wurden, im Abschnitt Verlauf des rechten Bereichs der Datensatzseite überprüfen.

![](assets/history-area-in-comments.png)

* Die Workfront-Planung zeichnet die folgenden Informationen im Abschnitt Verlauf auf:

   * Alle Feldänderungen

   * Die alten und neuen Werte der Felder, wenn sich die Werte ändern. Die alten Werte werden im Durchstreichen-Format angezeigt.

   * Der vollständige Name des Benutzers, der die Änderung vorgenommen hat

   * Ein Datum und ein Zeitstempel für den Zeitpunkt der Änderung.

* In den Feldern der folgenden Typen werden immer der alte Wert (im Durchstreichen-Format) und der neue Wert angezeigt:

   * Text
   * Absatz
   * Währung
   * Datum
   * Zahl
   * Prozentsatz
   * Einzelauswahl

* Felder der folgenden Typen zeigen den alten Wert nur dann im Durchstreichen-Format an, wenn mindestens einer der mehreren Werte entfernt wurde:

   * Mehrfachauswahl
   * Verknüpfte Datensatzfelder
   * Personen

  Wenn durch die Änderung nur Werte zum Feld hinzugefügt werden, wird der alte Wert nicht angezeigt und nur der neue Feldwert wird angezeigt.

* Felder vom Typ Kontrollkästchen zeigen den alten Wert nie im Durchstreichen-Format an. Wenn das Feld bearbeitet wird, wird nur der aktuelle Status zum Zeitpunkt der Änderung angezeigt.

  Weitere Informationen zu Workfront-Planungsfeldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

* Änderungen an Feldern der folgenden Typen werden nicht im Abschnitt Verlauf angezeigt:

   * Verknüpfte (Lookup) Felder
   * Formel
   * Erstellt von
   * Erstellt am Datum
   * Zuletzt geändert von
   * Zuletzt geändert am

* Wenn ein Feld aus dem System entfernt wird, bleiben die in diesem Feld vorgenommenen Aktualisierungen im Abschnitt Verlauf . Es gibt keinen Hinweis darauf, dass das Feld im Abschnitt Verlauf eines Datensatzes entfernt wurde.
