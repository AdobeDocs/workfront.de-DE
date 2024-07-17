---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Häufig gestellte Fragen zu Kick-Starts
description: Hier finden Sie Antworten auf häufig gestellte Fragen zum Importieren und Exportieren von Workfront-Daten mithilfe von Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Kick-Starts

Im Folgenden finden Sie häufig gestellte Fragen zu Kick-Starts:

## Warum erhalte ich diesen Fehler beim Import einer Kick-Start-Datei: &quot;Ihre Datei war korrekt, aber nichts wurde importiert?&quot;

### Antwort

Eines der folgenden drei Dinge fehlt möglicherweise in der Kick-Start-Datei:

1. Die Spalte **isNew** muss für alle Elemente, die Sie importieren möchten, auf **TRUE** gesetzt sein. **isNew** muss **TRUE** sein, da Sie neue Daten nur mit Kick-Start importieren können. Sie können vorhandene Daten nicht über Kick-Start ändern. Sie können andere Zeilen im Arbeitsblatt mit **isNew = FALSE** haben, diese Zeilen werden jedoch nicht importiert.

1. &#x200B; Die Datei muss über eine leere Zeile verfügen, bevor die Header Ihrer Daten beginnen.
1. &#x200B; Die Excel-Arbeitsblätter müssen die richtigen Namen aufweisen.

Beim Arbeiten mit Kick-Starts wird empfohlen, zunächst die Kick-Start-Vorlage herunterzuladen, sie manuell mit den richtigen Daten zu füllen und sie dann wieder in Adobe Workfront zu importieren.

Weitere Informationen zum korrekten Importieren von Daten in Workfront mithilfe von Kick-Starts finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kick-Start-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Warum erhalte ich diesen Fehler, wenn ich versuche, Stunden mit einer Kick-Start-Datei in Workfront zu importieren: &quot;Benutzer mit Primärschlüsselwert(en) &quot;null&quot;wurde nicht gefunden?&quot;

### Antwort

Der Fehler bezieht sich auf die GUID des Benutzers, der den Stunden zugeordnet ist.

Um dies zu beheben:

1. Exportieren Sie eine leere Kick-Start-Vorlage nur für das Objekt **Stunden** .\
   Weitere Informationen zum Exportieren einer leeren Kick-Start-Datei finden Sie unter &quot;Exportieren der Kick-Start-Vorlage&quot;in [Importieren von Daten in Adobe Workfront mithilfe einer Kick-Start-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Kopieren Sie die Daten aus dem ursprünglichen Kick-Start manuell und fügen Sie sie in die leere Datei ein.\
   Führen Sie dies für jede Spalte aus.
1. Versuchen Sie erneut, die neue Datei zu importieren.\
   Der Kick-Start sollte erfolgreich importiert werden.

## Warum wird das Feld country im Benutzerprofil bei einem Kick-Start-Import nicht ausgefüllt?

### Problem

Beim Importieren eines User Kick-Start mit dem Feld **setCountry** werden diese Daten nicht in das Land des Benutzerprofils übertragen.

### Antwort

Wenn der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, akzeptiert das Feld **Land** nur Ländercodewerte (z. B. USA, GB, IN). Stellen Sie sicher, dass das Feld **setCountry** in Ihrer Kick-Start-Vorlage Ländercode-Werte vor dem Import verwendet.

Weitere Informationen zum korrekten Importieren von Daten in Workfront mithilfe von Kick-Starts finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kick-Start-Vorlage](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
