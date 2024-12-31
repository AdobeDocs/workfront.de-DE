---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Update auf emailAddr aktualisiert nicht den Benutzernamen
description: Update auf emailAddr aktualisiert nicht den Benutzernamen
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Update auf emailAddr aktualisiert nicht den Benutzernamen

## Problem

Normalerweise sind `emailAddr` und `username` dasselbe Attribut. Wenn Sie daher das `emailAddr` eines Benutzers ändern, wird das `username` automatisch aktualisiert, damit es übereinstimmt.

Wenn die `username` nicht mit der `emailAddr` übereinstimmt, wird die `username` bei einer Aktualisierung der `emailAddr` nicht automatisch aktualisiert. Dies gilt sowohl für `emailAddr` Änderungen über die Benutzeroberfläche als auch für Änderungen über die API.

## Ursache

Die Diskrepanz kann auf verschiedene Weise erzeugt werden:

* Benutzer, die erstellt wurden, bevor die Synchronisierungsregel existierte. Sehr alte Benutzerkonten verfügen möglicherweise nicht über diese Attribute.

* Benutzende, die über SSO erstellt wurden, zu einer Zeit, als beim emailAddr in Workfront die Groß-/Kleinschreibung beachtet wurde. Bei der Option zur automatischen SSO-Bereitstellung wird die Groß-/Kleinschreibung der Benutzer anhand der Attribute des Benutzers vom Identitätsanbieter geprüft. Wenn keine exakte Übereinstimmung vorhanden war, erstellen die Services zur automatischen Bereitstellung einen neuen Benutzer. Wenn bereits ein Benutzer vorhanden war, bestand die Möglichkeit, dass Benutzername und `emailAddr` nicht dieselbe Groß-/Kleinschreibung aufweisen.

* Benutzende, bei denen das `username`-Attribut direkt über die API aktualisiert wurde und deren `emailAddr` nicht aktualisiert wurde. `username` und `emailAddr` stimmen möglicherweise nicht überein.

## Lösung

Verwenden Sie die -API, um das `username`-Attribut so zu ändern, dass es dem `emailAddr` entspricht. Nach der Synchronisierung der Attribute wird bei jeder Aktualisierung des `emailAddr` auch der `username` entsprechend aktualisiert (wenn das Benutzernamenfeld nicht in der Aktualisierung enthalten ist).
