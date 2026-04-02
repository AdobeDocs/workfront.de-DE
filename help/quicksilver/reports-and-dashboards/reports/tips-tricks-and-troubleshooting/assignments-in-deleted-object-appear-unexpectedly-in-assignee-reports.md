---
title: Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt
description: Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 1%

---

# Zuweisungen in einem gelöschten Objekt werden unerwartet in Empfängerberichten angezeigt

## Problem

Nachdem Sie ein Objekt gelöscht haben, das über eine Zuweisung verfügt, werden sowohl das Objekt als auch die Zuweisung gelöscht. Aber die Zuweisung kann immer noch in einigen Berichten angezeigt werden.

Wenn Sie beispielsweise eine Aufgabe löschen, die einem Benutzer zugewiesen wurde, wird auch die Zuweisung an den Benutzer gelöscht. Wenn Sie später jedoch einen Aufgabenbericht ausführen, der nach Verantwortlichem gefiltert wird, wobei dieser Benutzer angegeben ist, wird die gelöschte Aufgabe weiterhin im Bericht aufgeführt, wenn sich die Aufgabe noch im Papierkorb befindet.

## Ursache

Dies liegt an den architektonischen Einschränkungen des Papierkorbs. Es gibt derzeit keine Pläne, dieses Problem anzugehen, da eine Umgestaltung der Architektur notwendig wäre.
