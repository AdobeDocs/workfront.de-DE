---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht
description: Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht

## Problem

Normalerweise `emailAddr` und `username` sind dasselbe Attribut. Wenn Sie daher die `emailAddr` -Attribut `username` -Attribut automatisch entsprechend aktualisiert.

Wenn die `username` entspricht nicht dem `emailAddr`, ein Update der `emailAddr` aktualisiert die `username` automatisch. Dies gilt für beide `emailAddr` Änderungen über die Benutzeroberfläche und die API.

## Ursache

Die Diskrepanz kann auf verschiedene Weise entstehen:

* Benutzer, die vor der Existenz der Synchronisierungsregel erstellt wurden. Sehr alte Benutzerkonten verfügen möglicherweise nicht über diese Attribute.

* Benutzer, die über SSO erstellt wurden, zu einem Zeitpunkt, zu dem bei der E-Mail-Adresse in Workfront zwischen Groß- und Kleinschreibung unterschieden wurde. Die Option zur automatischen SSO-Bereitstellung würde eine Prüfung der Groß-/Kleinschreibung für Benutzer ausführen, die auf den Attributen des Benutzers vom Identitäts-Provider basiert. Wenn keine exakte Übereinstimmung existierte, würden die automatischen Bereitstellungsdienste einen neuen Benutzer erstellen. Wenn bereits ein Benutzer vorhanden war, bestand die Möglichkeit, dass der Benutzername und `emailAddr` nicht die gleiche Groß-/Kleinschreibung aufweisen.

* Benutzer mit der `username` -Attribut direkt über die API aktualisiert wird, und deren `emailAddr` wurde nicht aktualisiert. Die `username` und `emailAddr` möglicherweise nicht übereinstimmen.

## Lösung

Verwenden Sie die API, um die `username` -Attribut identisch mit dem `emailAddr`. Nach der Synchronisierung der Attribute wird jede Aktualisierung der `emailAddr` wird auch die `username` übereinstimmen (wenn das Benutzernamenfeld nicht in der Aktualisierung enthalten ist).
