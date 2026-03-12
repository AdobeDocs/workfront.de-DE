---
content-type: release-notes
title: Veröffentlichungen für Adobe Workfront-Planung im zweiten Quartal 2026
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im zweiten Quartal 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 79d4ad4a-1dd0-431e-92cd-582b5a1b7ec8
source-git-commit: 1e05945e24770848da9d2c77b81b9475e43797ea
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 13%

---

# Veröffentlichungen für Adobe Workfront-Planung im zweiten Quartal 2026

In diesem Artikel werden die Funktionen beschrieben, die in der Version vom zweiten Quartal 2026 für Workfront Planning veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--

## New field type for Record ID  

>[!NOTE]
>
>Preview: March 12, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026

We have added a new field type for Record ID. This is a system-generated alpha-numeric indicator which uniquely identifies each record. The field displays in any record view as well as the record details area.  

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

-->

## Benutzern ohne Administratorrechte erlauben, einen Datensatztyp als verbindbar festzulegen

>[!NOTE]
>
>Vorschau: 12. März 2026
>Produktions-Schnellveröffentlichung: Donnerstag, 15. April 2026
>Produktion für alle: Freitag, 16. April 2026

Wir erlauben jetzt Nicht-Administratoren, die Workspace-Manager sind, einen Datensatztyp aus bestimmten Arbeitsbereichen verbindbar zu machen.

Vor diesem Update konnten Nicht-Admins nicht zulassen, dass Datensatztypen verbunden werden können. Jetzt können sie es ermöglichen, dass die Datensatztypen von bestimmten Arbeitsbereichen aus verbunden werden können. Sie können nicht zulassen, dass Datensatztypen von allen Arbeitsbereichen im System aus verbunden werden können.

Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Trigger-basierte Automatisierung

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt mithilfe von Planning-Automatisierungen automatisch Planungsdatensätze oder Workfront-Objekte auf der Grundlage einer Datensatzfeldänderung erstellen.

Vor dieser Verbesserung konnten Sie nur dann automatisch Planungsdatensätze oder Workfront-Objekte erstellen, wenn Sie auf eine vorkonfigurierte Schaltfläche geklickt haben.

Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

## Nur Systemadministratoren können Arbeitsbereiche systemweit freigeben

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Wir erlauben es jetzt nur noch Systemadministratoren, bei der Freigabe eines Arbeitsbereichs zwischen den folgenden Optionen zu wählen:

* Für alle im System sichtbar
* Nur eingeladene Personen haben Zugriff

Arbeitsbereiche sind standardmäßig auf die Berechtigung „Nur eingeladene Personen können darauf zugreifen“ eingestellt.

Vor dieser Änderung war es nicht möglich, diese Freigabeberechtigungen für den Arbeitsbereich auszuwählen.

Weitere Informationen finden Sie unter Freigeben von Arbeitsbereichen (help/quicksilver/planning/access/share-workspaces.md).

## Sortieren von Gruppierungen in der Zeitleisten-Ansicht

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt Gruppierungen in der Zeitleisten -Ansicht sortieren. Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Unterstützen von Benutzerverweisen für verbundene Felder

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt Workfront-Benutzerfelder mit Workfront Planning-Datensatztypen verbinden, indem Sie eine neue Verbindung zwischen einem Workfront-Objekt und einem Workfront Planning-Datensatztyp hinzufügen.

Sie können in Workfront Planning jetzt beispielsweise Projektsponsor oder Portfolio-Besitzer als Suchfeld hinzufügen, wenn Sie eine Verbindung zu Projekten oder Portfolios hinzufügen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).


## Die Echtzeit-Präsenzindikatoren zeigen jetzt Benutzende in der Tabellenansicht an

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt die Benutzer anzeigen, die Datensatzfelder gleichzeitig aktualisieren, indem Sie auf die Echtzeitpräsenz-Anzeige in der oberen rechten Ecke einer Zelle in der Tabellenansicht klicken. In der oberen rechten Ecke der Datensatztabellen-Ansicht werden Benutzer aufgeführt, die dieselbe Ansicht geöffnet haben.

Sie müssen die Einstellung „Mitarbeiter anzeigen“ in der Kopfzeile der Tabellenansicht aktivieren. Andere Benutzende können Felder entweder in der Tabellenansicht oder im Detailbereich eines Datensatzes aktualisieren.

Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).


## Aktualisiertes Freigabeerlebnis für Listenansichten

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Wenn Sie die Listenansicht auf der Seite „Mit Projekten verbundene Datensätze“ eines Datensatzes mit Ansichtsberechtigungen freigeben, kann der Benutzer, für den Sie die Ansicht freigeben, die Ansichtselemente ändern, und diese Änderungen werden gemäß den persönlichen Voreinstellungen des Benutzers gespeichert. Sie haben jetzt die Möglichkeit, eine Kopie der Ansicht zu speichern, die ihre Änderungen enthält, oder die freigegebene Ansicht auf ihre ursprünglichen Einstellungen zurückzusetzen. Sie können die kopierte Ansicht mit anderen teilen.

Diese Aktualisierung ist nur in der Listenansicht für die Seite „Verbundene Datensätze“ eines Datensatzes verfügbar, wenn Projekte angezeigt werden.

Weitere Informationen finden Sie unter [Verwalten der Listenansicht](/help/quicksilver/planning/views/manage-the-list-view.md).

## Anwenden einer bedingten Formatierung auf die Listenansicht

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt bedingte Formatierung auf Projekte in einer Listenansicht auf der Seite „Verbundene Datensätze“ eines Datensatzes anwenden. Diese Funktion war in der Listenansicht vor dieser Verbesserung nicht vorhanden.

Weitere Informationen finden Sie unter [Listenansicht verwalten](/help/quicksilver/planning/views/manage-the-list-view.md).

## Verbesserungen an globalen Datensatztypen in sekundären Arbeitsbereichen

>[!NOTE]
>
>Vorschau: 5. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Die Sichtbarkeit der globalen Datensatztypen, die von einem primären Arbeitsbereich zu einem sekundären Arbeitsbereich hinzugefügt wurden, wurde verbessert. Zu den Verbesserungen zählen:

* Ein leicht geändertes globales Symbol, das anzeigt, dass der Datensatztyp aus einem anderen Arbeitsbereich hinzugefügt wurde.

* Ein verbesserter Tooltip für das neue Symbol, der den Arbeitsbereich, in dem der Datensatztyp erstellt wurde, klar identifiziert.

Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Konfigurieren der im Vorschaufeld Details eines Datensatzes angezeigten Felder

>[!NOTE]
>
>Vorschau: 29. Januar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. Februar 2026
>Produktion für alle: Freitag, 16. April 2026

Wir haben eine Einstellung eingeführt, mit der Sie Datensatzfelder im Vorschaufeld Details eines Datensatzes basierend auf den in der Tabellenansicht angezeigten Feldern ein- oder ausblenden können. 

Mit dieser neuen Einstellung können Sie festlegen, ob in der Tabellenansicht ausgeblendete Felder in den Vorschaubereich Details des Datensatzes ein- oder ausgeschlossen werden sollen.

Weitere Informationen finden Sie unter [Seitenlayout für Einträge verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

## Neues Feld für Planning-Verbindung für ursprüngliche Anfrage

>[!NOTE]
>
>Vorschau: 29. Januar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. Februar 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt das Verbindungsfeld „Ursprüngliche Anfrage“ zu einem Datensatztyp hinzufügen. Wenn ein Datensatz durch Senden eines Planungsanfrageformulars erstellt wird, wird das Feld „Ursprüngliche Anforderung verbunden“ mit dem Namen der ursprünglichen Anforderung ausgefüllt.

Vor dieser Verbesserung konnten Sie die ursprüngliche Anfrage, mit der der Datensatz erstellt wurde, nur im Bereich Anfragen anzeigen und darauf zugreifen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Erstellen von Genehmigungsregeln für Anfragen in Workfront Planning

>[!NOTE]
>
>Vorschau: 29. Januar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. Februar 2026
>Produktion für alle: Freitag, 16. April 2026

Um Genehmigungen von Anfragen dynamischer und flexibler zu gestalten, haben wir die Möglichkeit hinzugefügt, Genehmigungsregeln zu erstellen. Diese Regeln ermöglichen die Weiterleitung von Anfragen an verschiedene genehmigende Personen auf der Grundlage der Feldwerte in der Anfrage.

Wenn beispielsweise ein Anfrageformular das Feld „Kampagnentyp“ aufweist, kann eine Regel erstellt werden, die die Anfrage an eine Person sendet, wenn das Feld den Wert „Digital“ hat, und an eine andere Person, wenn es den Wert „Drucken“ hat.

Auf dem Anfrageformular werden Validierungsregeln erstellt.

Weitere Informationen und Anweisungen finden Sie [Hinzufügen von Genehmigungsregeln zu einem Anforderungsformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md#add-approval-rules-to-a-request-form) im Artikel Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning.

## Anzeigen von E-Mails in Feldern mit automatischer Textvervollständigung in Workfront Planning

>[!NOTE]
>
>Vorschau: 22. Januar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. Februar 2026
>Produktion für alle: Freitag, 16. April 2026

Die E-Mail-Adresse eines/r Benutzenden wird jetzt angezeigt, wenn Sie den/die Benutzende(n) den folgenden Bereichen hinzufügen:

* Personenbezogene Planungsfelder
* Im Feld Freigeben bei der Freigabe von Planning-Objekten

Vor dieser Verbesserung wurde beim Hinzufügen zu diesen Bereichen neben dem Benutzernamen nur die Primäre Rolle des Benutzers angezeigt.
Weitere Informationen finden Sie in den folgenden Artikeln:

* [Erstellen von Feldern](/help/quicksilver/planning/fields/create-fields.md)
* [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md)

## Personenfelder werden als Suchfelder für Planning-Verbindungen aktiviert

>[!NOTE]
>
>Vorschau: 14. Januar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. Februar 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt beim Verbinden von zwei Planungs-Datensatztypen Felder für Personen zu Suchfeldern hinzufügen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
