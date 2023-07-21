---
title: Übersicht über den Formularentwickler
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular entwerfen, das Benutzer an ein Workfront-Objekt anhängen können. Benutzer, die an dem Objekt arbeiten, können das benutzerdefinierte Formular ausfüllen, um Informationen über das Objekt bereitzustellen.
author: Courtney / Lisa
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: a7b4de06965b7b5e09424fbe6f3aa2fa6c195611
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Übersicht über den Formularentwickler

Sie können den neuen Formularentwickler verwenden, um ein benutzerdefiniertes Formular zu entwerfen, das Benutzer an ein Workfront-Objekt anhängen können. Benutzer, die an dem Objekt arbeiten, können das benutzerdefinierte Formular ausfüllen, um Informationen über das Objekt bereitzustellen.

Der neue Formularentwickler verfügt über einen neuen Arbeitsbereich im Arbeitsbereich, mit dem Sie die Felder, Arbeitsfläche und Feldeinstellungen gleichzeitig anzeigen können. Außerdem können Sie bei der Erstellung Ihres Formulars Felder durch Drag &amp; Drop in die Abschnitte ziehen.

<!-- add screenshot when field settings empty state is ready -->

## Zugriff auf den neuen Formularentwickler

Oben im neuen Formularentwickler und im alten Formularersteller befindet sich eine neue Schaltfläche. Sie können diese Schaltfläche verwenden, um zwischen dem alten Builder und dem neuen Designer zu wechseln.

![Wechsel zum neuen Formularentwickler](assets/switch-views.png)

## Neue Funktionen im Formularentwickler verfügbar

Mit dem neuen Formularentwickler haben wir die Möglichkeit hinzugefügt,

* **Feld kopieren**: Sie können jetzt vorhandene Felder kopieren, indem Sie in den Feldern direkt auf der Arbeitsfläche auf das Symbol Kopieren klicken.

* **Ändern der Größe für beschreibenden Text**: Sie können jetzt beschreibende Textfelder kleine, mittlere oder große Größen zuweisen. Sie können sie auch für dieselbe Zeile mit anderen Feldern verwenden.

* **Standardabschnitt verwenden**: Wenn der Formularersteller oben im Formular keinen Abschnitt hinzugefügt hat, wird jetzt auf der Arbeitsfläche der Abschnitt &quot;Standard&quot;angezeigt, sodass Benutzer die Berechtigungen für Felder anpassen können, denen kein benutzerdefinierter Abschnitt zugewiesen wurde.

  >[!NOTE]
  >
  >Der Standardabschnitt ist in Objekten nicht sichtbar, nachdem das Formular an das Objekt angehängt wurde.

## Funktion in Kürze verfügbar

Folgendes ist derzeit nicht im Formularentwickler verfügbar, wird aber bald hinzugefügt:

* Logik anzeigen/überspringen

* Filter für Typeahead-Felder

>[!IMPORTANT]
>
>Die vorhandenen Konfigurationen für Logik- und Typeahead-Filter sind bei der Arbeit mit dem neuen Formularentwickler nicht betroffen.

### Logik anzeigen/überspringen

Sie können zwar beim Entwerfen eines neuen benutzerdefinierten Formulars noch keine Anzeige-/Übersprunglogik hinzufügen, Sie können jedoch die vorhandene Anzeige-/Übersprunglogik für Formulare anzeigen, die im alten Formular-Builder erstellt wurden.

Die Symbole in einem Feld im Formularentwickler weisen darauf hin, dass auf das Feld Logik angewendet wird.

Die **D** -Symbol unten links bedeutet, dass das Feld das Zielfeld für die Anzeigelogik ist (wenn im Formular eine bestimmte Auswahl getroffen wurde, wird dieses Feld angezeigt). Die **D** -Symbol unten rechts bedeutet, dass das Feld verwendet wird, um die Anzeigelogik zu definieren (eine bestimmte Auswahl oder ein Wert in diesem Feld zeigt das Zielfeld an).

Die **S** -Symbol unten links bedeutet, dass das Feld das Zielfeld für die Logik zum Überspringen ist (wenn eine bestimmte Auswahl im Formular vorgenommen wird, wird das Formular zu diesem Feld übersprungen). Die **S** -Symbol unten rechts bedeutet, dass das Feld verwendet wird, um die Logik zum Überspringen zu definieren (eine bestimmte Auswahl oder ein bestimmter Wert in diesem Feld überspringt andere Felder und geht direkt zum Zielfeld).

Wenn Sie ein Feld mit angewendeter Logik auswählen, werden die vorhandenen Logikregeln in den Feldeinstellungen angezeigt.

![Logische Regeln](assets/form-designer-view-only-logic.png)

## Aus dem Formularentwickler entfernte Funktion

Die folgende Funktion wurde aus dem Formular-Designer entfernt:


* Formulareinstellungen, Formularfreigabe, Registerkarten für Feldfreigabe

   * Die Formulareinstellungen sind jetzt oben auf der Arbeitsfläche verfügbar

   * Hauptregisterkarte &quot;Formularfreigabe&quot;und Unterregisterkarte &quot;Feldfreigabe&quot;

  >[!NOTE]
  >
  >Sie können die Formular- und Feldfreigabe über die Registerkarte Einrichtung > Benutzerdefinierte Forms > Forms oder Felder steuern.

* Feldänderungen in Aktualisierungs-Feeds nachverfolgen
  >[!NOTE]
  >
  >Sie finden dies unter Einrichtung > Benutzeroberfläche > Feeds aktualisieren .
