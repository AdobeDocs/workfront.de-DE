---
title: Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt
description: Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt

## Problem

Nachdem Sie ein Objekt gelöscht haben, das über eine Zuweisung verfügt, werden sowohl das Objekt als auch die Zuweisung gelöscht. Aber die Zuweisung kann immer noch in einigen Berichten angezeigt werden.

Wenn Sie beispielsweise eine Aufgabe löschen, die einem Benutzer zugewiesen wurde, wird auch die Zuweisung an den Benutzer gelöscht. Wenn Sie später jedoch einen Aufgabenbericht ausführen, der nach Verantwortlichem gefiltert wird, wobei dieser Benutzer angegeben ist, wird die gelöschte Aufgabe weiterhin im Bericht aufgeführt, wenn sich die Aufgabe noch im Papierkorb befindet.

## Ursache

Dies liegt an den architektonischen Einschränkungen des Papierkorbs. Es gibt derzeit keine Pläne, dieses Problem anzugehen, da eine Umgestaltung der Architektur notwendig wäre.
