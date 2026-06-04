---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Dokumentname nach dem Hochladen geändert und enthält ein ungültiges Zeichen
description: Bestimmte Dokumente können nicht in Korrekturabzüge konvertiert werden.
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 17%

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
