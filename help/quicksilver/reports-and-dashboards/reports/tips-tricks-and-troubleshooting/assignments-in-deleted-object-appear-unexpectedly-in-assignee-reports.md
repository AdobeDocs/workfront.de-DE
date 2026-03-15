---
title: Zuweisungen in einem gelöschten Objekt werden in Zuweisungsberichten unerwartet angezeigt
description: Zuweisungen in einem gelöschten Objekt werden in Zuweisungsberichten unerwartet angezeigt
author: Courtney
draft: Probably
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 1%

---

# Zuweisungen in einem gelöschten Objekt werden in Zuweisungsberichten unerwartet angezeigt

## Problem

Nachdem Sie ein Objekt gelöscht haben, dem eine Aufgabe zugewiesen ist, werden sowohl das Objekt als auch die Aufgabe gelöscht. Die Aufgabe wird jedoch möglicherweise immer noch in einigen Berichten angezeigt.

Wenn Sie beispielsweise eine Aufgabe löschen, die einem Benutzer zugewiesen wurde, wird die Zuweisung an den Benutzer ebenfalls gelöscht. Wenn Sie jedoch später einen Aufgabenbericht ausführen, der nach Bevollmächtigten gefiltert wird, wobei dieser Benutzer angegeben ist, wird der gelöschte Task weiterhin im Bericht aufgelistet, wenn sich der Task noch im Papierkorb befindet.

## Ursache

Dies ist auf architektonische Einschränkungen des Papierkorbs zurückzuführen. Derzeit gibt es aufgrund des notwendigen Umfangs der Architekturumgestaltung keine Pläne für eine Lösung dieses Problems.
