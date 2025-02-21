---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Dokumentname nach dem Hochladen geändert und enthält ein ungültiges Zeichen
description: Bestimmte Dokumente können nicht in Korrekturabzüge konvertiert werden.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Dokumentname nach dem Hochladen geändert und enthält ein ungültiges Zeichen

## Problem

Bestimmte Dokumente können nicht in Korrekturabzüge konvertiert werden.

## Ursache

Dateien, die in Workfront hochgeladen werden, dürfen bestimmte Zeichen in Dateinamen nicht enthalten. Wenn eine Datei eines der folgenden Zeichen im Dateinamen enthält, werden die Zeichen beim Hochladen der Datei aus dem Dateinamen entfernt: `! # % * \ | ' " / ? < > { } [ ]`.

Wenn ein Dokumentname nach dem ersten Hochladen so aktualisiert wird, dass er ein ungültiges Zeichen enthält, schlägt die Erstellung des Korrekturabzugs fehl.

## Lösung

Entfernen Sie das ungültige Zeichen aus dem Dokumentnamen:

1. Wählen Sie das Dokument aus und klicken Sie auf **Dokumentdetails**.
1. Klicken Sie auf den Dokumentnamen, entfernen Sie das ungültige Zeichen, und drücken Sie die Eingabetaste.

   Ungültige Zeichen: `! # % * \ | ' " / ? < > { } [ ]`

   ![Dokumentname](assets/doc-name.png)

1. Aktualisieren Sie die Seite und erstellen Sie den Korrekturabzug.
