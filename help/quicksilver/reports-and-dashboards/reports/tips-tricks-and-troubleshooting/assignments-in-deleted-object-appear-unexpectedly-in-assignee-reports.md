---
title: Zuweisungen in einem gelöschten Objekt werden in den Bevollmächtigten-Berichten unerwartet angezeigt
description: Zuweisungen in einem gelöschten Objekt werden in den Bevollmächtigten-Berichten unerwartet angezeigt
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Zuweisungen in einem gelöschten Objekt werden in den Bevollmächtigten-Berichten unerwartet angezeigt

## Problem

Nachdem Sie ein Objekt gelöscht haben, das über eine Zuweisung verfügt, werden sowohl das Objekt als auch die Zuweisung gelöscht. Die Zuweisung wird jedoch möglicherweise noch in einigen Berichten angezeigt.

Wenn Sie beispielsweise eine Aufgabe löschen, die einem Benutzer zugewiesen wurde, wird auch die Zuweisung zum Benutzer gelöscht. Wenn Sie jedoch später einen Aufgabenbericht ausführen, der nach Verantwortlichen gefiltert wird und der Benutzer angegeben ist, wird die gelöschte Aufgabe im Bericht weiterhin aufgeführt, wenn sich die Aufgabe noch im Papierkorb befindet.

## Ursache

Dies ist auf architektonische Einschränkungen des Papierkorbs zurückzuführen. Es gibt derzeit keine Pläne für die Lösung dieses Problems, da die architektonische Neugestaltung notwendig wäre.
