---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: Kickstart,Kickstart,Kickstarts,Kickstarts
navigation-topic: use-kick-starts
title: Häufig gestellte Fragen zu Kickstarts
description: Hier finden Sie Antworten auf häufig gestellte Fragen zum Importieren und Exportieren von Workfront-Daten mithilfe von Kickstarts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Kickstarts

Im Folgenden finden Sie häufig gestellte Fragen zu Kickstarts:

## Warum erhalte ich diese Fehlermeldung, wenn ich versuche, eine Kickstart-Datei zu importieren: „Ihre Datei war korrekt, aber es wurde nichts importiert?“

### Antwort

Eine der folgenden drei Angaben könnte in der Kickstart-Datei fehlen:

1. Die Spalte **isNew** muss für **Elemente, die Sie importieren möchten, auf** TRUE“ gesetzt werden. **isNew** muss **TRUE** sein, da neue Daten nur mit Kickstart importiert werden können. Bestehende Daten können nicht per Kickstart geändert werden. Es können weitere Zeilen in der Tabelle mit **isNew = FALSE** enthalten sein, diese Zeilen werden jedoch nicht importiert.

1. &#x200B;Die Datei muss eine leere Zeile haben, bevor die Kopfzeilen Ihrer Daten beginnen.
1. &#x200B;Die Excel-Tabelle(n) muss/müssen den richtigen Namen haben.

Bei der Arbeit mit Kickstarts empfehlen wir, zunächst die Kickstart-Vorlage herunterzuladen, sie manuell mit den richtigen Daten zu füllen und sie dann wieder in Adobe Workfront zu importieren.

Weitere Informationen zum korrekten Importieren von Daten in Workfront mithilfe von Kickstarts finden Sie unter [Daten mithilfe einer Kickstart-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Warum erhalte ich diese Fehlermeldung, wenn ich versuche, Stunden mithilfe einer Kickstart-Datei in Workfront zu importieren: „Benutzer mit Primärschlüsselwert(en) „null“ nicht gefunden?“

### Antwort

Der Fehler bezieht sich auf die GUID des Benutzers, der mit den Stunden verknüpft ist.

Gehen Sie wie folgt vor:

1. Exportieren Sie eine leere Kickstart-Vorlage nur für das **Stunden**-Objekt.\
   Weitere Informationen zum Exportieren einer leeren Kickstart-Datei finden Sie unter „Exportieren der Kickstart-Vorlage“ in [Daten mithilfe einer Kickstart-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Kopieren Sie die Daten aus dem ursprünglichen Kickstart manuell und fügen Sie sie in die leere Datei ein.\
   Dies für jede Spalte tun.
1. Versuchen Sie erneut, die neue Datei zu importieren.\
   Der Kickstart sollte erfolgreich importiert werden.

## Warum wird das Feld „Land“ im Benutzerprofil bei einem Kickstart-Import nicht ausgefüllt?

### Problem

Beim Importieren eines Benutzer-Kickstarts mit dem Feld **setCountry** werden diese Daten nicht an das Land im Benutzerprofil übertragen.

### Antwort

Wenn die Benutzerin bzw. der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, akzeptiert das **Country**-Feld nur Ländercodewerte (z. B. US, GB, IN). Stellen Sie sicher **dass im Feld** setCountry“ in Ihrer Kickstart-Vorlage vor dem Import Ländercodewerte verwendet werden.

Weitere Informationen zum korrekten Importieren von Daten in Workfront mithilfe von Kickstarts finden Sie unter [Daten mithilfe einer Kickstart-Vorlage in Adobe Workfront importieren](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
