---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Dokumentname nach dem Hochladen geändert und enthält ungültiges Zeichen
description: Bestimmte Dokumente können nicht in Testsendungen umgewandelt werden.
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Dokumentname nach dem Hochladen geändert und enthält ungültiges Zeichen

## Problem

Bestimmte Dokumente können nicht in Testsendungen umgewandelt werden.

## Ursache

Dateien, die in Workfront hochgeladen werden, dürfen bestimmte Zeichen in Dateinamen nicht enthalten. Wenn eine Datei eines der folgenden Zeichen im Dateinamen enthält, werden die Zeichen beim Hochladen der Datei aus dem Dateinamen entfernt: `! # % * \ | ' " / ? < > { } [ ]`.

Wenn ein Dokumentname aktualisiert wird, um nach dem ersten Upload ein ungültiges Zeichen einzuschließen, schlägt die Erstellung des Testversands fehl.

## Lösung

Entfernen Sie das ungültige Zeichen aus dem Dokumentnamen:

1. Wählen Sie das Dokument aus und klicken Sie auf **Dokumentdetails**.
1. Klicken Sie auf den Dokumentnamen, entfernen Sie das ungültige Zeichen und drücken Sie die Eingabetaste.

   Ungültige Zeichen: `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. Aktualisieren Sie die Seite und generieren Sie den Testversand.