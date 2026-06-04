---
title: Verbesserungen für Admins im ersten Quartal 2026
description: Verbesserungen für Admins im ersten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a74d036b-e4fa-49e0-bb10-4baf379e1b1c
TQID: https://experienceleague.adobe.com/IYlqpTdS-pJNpBaCeYywassuOaTQdaSZlctxd1J0NPA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 669
ht-degree: 96%

---

# Verbesserungen für Admins im ersten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom ersten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im ersten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsüberblick für das erste Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Verwalten von Prioritäten in der Layout-Vorlage

>[!NOTE]
>
>Diese Funktion ist in der Vorschau-Umgebung vorübergehend nicht verfügbar>Vorschau: 2. Dezember 2025>Produktions-Schnellversion: 14. Januar 2026>Produktion für alle: 15. Januar 2026


Sie können jetzt in der Layout-Vorlage Prioritäten für bestimmte Benutzende aktivieren oder deaktivieren. Wenn Sie zuvor Prioritäten für Ihre Organisation deaktiviert hatten, bleiben diese mit dieser Änderung in der Layout-Vorlage deaktiviert.

Bei Lizenztypen mit Standardzugriff auf Anfragen werden automatisch Prioritäten einbezogen. Beispielsweise werden für eine Lizenz des Typs „Mitwirkender“ Anfragen, Dashboards und Prioritäten standardmäßig im Hauptmenü angezeigt, während für eine externe Lizenz nur Dokumente und Dashboards angezeigt werden, da sie keine Zugriffsrechte für das Anzeigen oder Senden von Anfragen umfasst.


Weitere Informationen finden Sie unter [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Prüfen auf Konflikte mit mehreren Formularen für berechnete benutzerdefinierte Felder

>[!NOTE]
>
>Vorschau: 18. Dezember 2025>Produktionsschnellveröffentlichung: 14. Januar 2026>Produktion für alle: 15. Januar 2026

Dasselbe berechnete Feld kann unterschiedliche Formeln aufweisen, wenn es an verschiedene benutzerdefinierte Formulare angehängt wird. Wenn zwei oder mehr Formulare, die dasselbe berechnete Feld enthalten, an ein Objekt angehängt werden, müssen die Formeln in allen Formularen identisch sein. Das Bearbeiten der Formel ist nicht zulässig, wenn die Änderung einen Konflikt verursachen könnte.

Um bei der Bearbeitung eines Ausdrucks für benutzerdefinierte Felder die möglichen Auswirkungen auf Objekte sichtbar zu machen, wurde eine Option zur Konfliktprüfung hinzugefügt. In diesem Dialogfeld werden alle Objekte gruppiert nach Objekttyp angezeigt, die von einer Änderung der Formel betroffen sein könnten. Sie können zu den Details der einzelnen Objekte navigieren und die Felder überprüfen, um zu entscheiden, ob das Feld aus einem der Formulare entfernt werden soll oder ob der Ausdruck unverändert bleiben soll.

Weitere Informationen finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Eingabedatum und ID, von der die Eingabe vorgenommen wurde, in benutzerdefinierten Objekten

>[!NOTE]
>
>Vorschau: 13. November 2025>Produktions-Schnellveröffentlichung: 13. November 2025>Produktion für alle: 13. November 2025

Das Eingabedatum und die ID, von der die Eingabe vorgenommen wurde, werden jetzt in benutzerdefinierten Formularen, Feldern und Abschnitten gespeichert. Sie können diese Datenoptionen in Berichten als Filter, Ansichten oder Gruppierungen verwenden. Um sie in der Liste der benutzerdefinierten Formulare, Felder oder Abschnitte im Setup anzuzeigen, fügen Sie „Eingabedatum“ und „Eingegeben von: Name“ als Spalten in einer neuen oder vorhandenen Ansicht ein.

>[!NOTE]
>
>Das Eingabedatum und die ID, von der die Eingabe vorgenommen wurde, sind nur für benutzerdefinierte Formulare, Felder und Abschnitte verfügbar, die am oder nach dem 13. November 2025 erstellt wurden.

## Aktualisierungen der Schaltflächennamen beim Bearbeiten einer Layout-Vorlage

>[!NOTE]
>
>Vorschau: 30. Oktober 2025>Produktions-Schnellveröffentlichung: 13. November 2025>Produktion für alle: 15. Januar 2026

Um für mehr Konsistenz mit anderen Bereichen des Setups zu sorgen, z. B. mit dem Designer für benutzerdefinierte Formulare, wurden die Schaltflächen, die Sie beim Bearbeiten einer Layout-Vorlage sehen, in **Anwenden**, **Speichern und schließen** und **Abbrechen** geändert. Mit der neuen Option **Anwenden** können Sie Ihre Änderungen an der Layout-Vorlage speichern und mit der Bearbeitung fortfahren. Zuvor waren die verfügbaren Optionen **Speichern** und **Abbrechen**.

Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Verbesserte Feldverwaltung mit Markierung „Aktiv“ für benutzerdefinierte Felder

>[!NOTE]
>
>Vorschau: 30. Oktober 2025>Produktions-Schnellveröffentlichung: 13. November 2025>Produktion für alle: 15. Januar 2026

Wenn das System eine große Anzahl benutzerdefinierter Felder enthält, kann die Verwaltung dieser Felder in benutzerdefinierten Formularen und Berichten schwierig sein. Sie können jetzt benutzerdefinierte Felder mit der neuen Markierung **Aktiv** als inaktiv kennzeichnen. Diese Markierung ist verfügbar, wenn Sie mit einem Feld in einem benutzerdefinierten Formular arbeiten oder ein Feld aus der Liste „Felder“ hinzufügen oder bearbeiten.

Wenn Sie ein Feld als inaktiv kennzeichnen:

* Ist es von Berichten, Filtern, Ansichten oder anderen Stellen in Workfront ausgeschlossen, an denen Sie ein benutzerdefiniertes Feld hinzufügen können
* Ist es nicht in der Feldbibliothek verfügbar, um es zu anderen benutzerdefinierten Formularen hinzuzufügen

>[!NOTE]
>
>Wenn Sie ein vorhandenes Feld als inaktiv kennzeichnen, ist es von diesem Zeitpunkt an nicht mehr für die Verwendung in Reporting-Elementen und benutzerdefinierten Formularen verfügbar. Wenn das inaktive Feld derzeit in einem Bericht oder Formular verwendet wird, bleiben das Feld und seine historischen Daten erhalten.

Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten eines benutzerdefinierten Feldes, eines Abschnittsumbruchs oder eines Widgets](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).
