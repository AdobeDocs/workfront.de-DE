---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht
description: Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Aktualisierung auf emailAddr aktualisiert den Benutzernamen nicht

## Problem

Normalerweise sind `emailAddr` und `username` dasselbe Attribut. Wenn Sie daher das Attribut `emailAddr` eines Benutzers ändern, wird das Attribut `username` automatisch entsprechend aktualisiert.

Wenn die `username` nicht mit der `emailAddr` übereinstimmt, wird die `username` nicht automatisch durch eine Aktualisierung auf die `emailAddr` aktualisiert. Dies gilt sowohl für `emailAddr` -Änderungen über die Benutzeroberfläche als auch über die API.

## Ursache

Die Diskrepanz kann auf verschiedene Weise entstehen:

* Benutzer, die vor der Existenz der Synchronisierungsregel erstellt wurden. Sehr alte Benutzerkonten verfügen möglicherweise nicht über diese Attribute.

* Benutzer, die über SSO erstellt wurden, zu einem Zeitpunkt, zu dem bei der E-Mail-Adresse in Workfront zwischen Groß- und Kleinschreibung unterschieden wurde. Die Option zur automatischen SSO-Bereitstellung würde eine Prüfung der Groß-/Kleinschreibung für Benutzer ausführen, die auf den Attributen des Benutzers vom Identitäts-Provider basiert. Wenn keine exakte Übereinstimmung existierte, würden die automatischen Bereitstellungsdienste einen neuen Benutzer erstellen. Wenn bereits ein Benutzer vorhanden war, bestand die Möglichkeit, dass der Benutzername und `emailAddr` nicht dieselbe Groß-/Kleinschreibung aufweisen würden.

* Benutzer, die das Attribut `username` direkt über die API aktualisiert haben und deren `emailAddr` nicht aktualisiert wurde. Die `username` und `emailAddr` stimmen möglicherweise nicht überein.

## Lösung

Verwenden Sie die API, um das Attribut `username` so zu ändern, dass es mit dem Attribut `emailAddr` übereinstimmt. Nach der Synchronisierung der Attribute wird bei jeder Aktualisierung von `emailAddr` auch die Übereinstimmung von `username` aktualisiert (wenn das Feld für den Benutzernamen nicht in der Aktualisierung enthalten ist).
