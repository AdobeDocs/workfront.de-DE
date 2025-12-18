---
title: Verbesserungen für Administratoren im ersten Quartal 2026
description: Verbesserungen für Administratoren im ersten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: e9e7b76dc8e4b9d1cc91987d0ea63b5e2ee58224
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Verbesserungen für Administratoren im ersten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom ersten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im ersten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Übersicht über die Version im ersten Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Verwalten von Prioritäten in der Layout-Vorlage

>[!NOTE]
>
>Vorschau: 2. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

Sie können jetzt in der Layout-Vorlage Prioritäten für bestimmte Benutzer aktivieren oder deaktivieren. Wenn Sie zuvor Prioritäten für Ihre Organisation deaktiviert hatten, bleibt sie mit dieser Änderung in der Layout-Vorlage deaktiviert.

Bei Lizenztypen mit Standardzugriff auf Anfragen werden automatisch Prioritäten einbezogen. Beispielsweise werden für eine Mitwirkende-Lizenz Anfragen, Dashboards und Prioritäten standardmäßig im Hauptmenü angezeigt, während für eine externe Lizenz nur Dokumente und Dashboards angezeigt werden, da sie keinen Zugriff zum Anzeigen oder Senden von Anfragen hat.


Weitere Informationen finden Sie unter [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Prüfen auf Konflikte mit mehreren Formularen für berechnete benutzerdefinierte Felder

>[!NOTE]
>
>Vorschau: 18. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

Dasselbe berechnete Feld kann unterschiedliche Formeln aufweisen, wenn es an verschiedene benutzerdefinierte Formulare angehängt wird. Wenn zwei oder mehr Formulare, die dasselbe berechnete Feld enthalten, an ein Objekt angehängt werden, müssen die Formeln in allen Formularen identisch sein. Das Bearbeiten der Formel ist nicht zulässig, wenn die Änderung einen Konflikt verursachen könnte.

Um bei der Bearbeitung eines Ausdrucks für benutzerdefinierte Felder die möglichen Auswirkungen auf Objekte sichtbar zu machen, wurde eine Option zur Konfliktprüfung hinzugefügt. In diesem Dialogfeld werden alle Objekte gruppiert nach Objekttyp angezeigt, die von einer Änderung der Formel betroffen sein könnten. Sie können zu den Details der einzelnen Objekte navigieren und die Felder überprüfen, um zu entscheiden, ob das Feld aus einem der Formulare entfernt werden soll oder der Ausdruck unverändert bleiben soll.

Weitere Informationen finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Eingabedatum und „Eingegeben von ID“ in benutzerdefinierten Objekten

>[!NOTE]
>
>Vorschau: 13. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 13. November 2025

Das Eingabedatum und die von der ID eingegebenen Daten werden jetzt in benutzerdefinierten Formularen, Feldern und Abschnitten gespeichert. Sie können diese Datenoptionen in Berichten als Filter, Ansichten oder Gruppierungen verwenden. Um sie in der Liste der benutzerdefinierten Formulare, Felder oder Abschnitte im Setup anzuzeigen, fügen Sie „Eingabedatum“ hinzu und geben Sie „Nach Name“ als Spalten in einer neuen oder vorhandenen Ansicht ein.

>[!NOTE]
>
>Das Eingabedatum und die eingegebenen Werte nach ID sind nur für benutzerdefinierte Formulare, Felder und Abschnitte verfügbar, die am oder nach dem 13. November 2025 erstellt wurden.

## Aktualisierungen der Schaltflächennamen beim Bearbeiten einer Layout-Vorlage

>[!NOTE]
>
>Vorschau: 30. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Um für mehr Konsistenz mit anderen Bereichen von Setup zu sorgen, z. B. mit dem benutzerdefinierten Formular-Designer, wurden die Schaltflächen, die Sie beim Bearbeiten einer Layout-Vorlage sehen, in **Übernehmen**, **Speichern und schließen** und **Abbrechen** geändert. Mit der neuen Option **Übernehmen** können Sie Ihre Änderungen an der Layout-Vorlage speichern und mit der Bearbeitung fortfahren. Zuvor waren die verfügbaren Optionen **Speichern** und **Abbrechen**.

Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).



## Verbesserte Feldverwaltung mit Markierung „Aktiv“ für benutzerdefinierte Felder

>[!NOTE]
>
>Vorschau: 30. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Wenn das System eine große Anzahl benutzerdefinierter Felder enthält, kann die Verwaltung dieser Felder in benutzerdefinierten Formularen und Berichten schwierig sein. Sie können jetzt benutzerdefinierte Felder mit der neuen Markierung „Aktiv **als inaktiv**. Diese Markierung ist verfügbar, wenn Sie mit einem Feld in einem benutzerdefinierten Formular arbeiten oder ein Feld aus der Liste Felder hinzufügen oder bearbeiten.

Wenn Sie ein Feld als inaktiv markieren:

* Sie ist von Berichten, Filtern, Ansichten oder anderen Stellen in Workfront ausgeschlossen, an denen Sie ein benutzerdefiniertes Feld hinzufügen können
* Sie ist nicht in der Feldbibliothek verfügbar, um sie zu anderen benutzerdefinierten Formularen hinzuzufügen

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).




