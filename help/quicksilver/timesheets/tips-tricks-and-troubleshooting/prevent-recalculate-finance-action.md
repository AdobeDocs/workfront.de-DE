---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Verhindern, dass sich die Aktion „Finanzen neu berechnen“ auf historische Stunden auswirkt, wenn sich die Sätze ändern
description: Sie müssen die Stundenkosten für einen Benutzer oder ein Aufgabengebiet aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands), aber Sie möchten nicht, dass sich diese Änderung auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder Sie möchten, dass sie nur einen Teil der historischen Stunden betrifft.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Verhindern, dass sich die Aktion „Finanzen neu berechnen“ auf historische Stunden auswirkt, wenn sich die Sätze ändern

## Problem

Sie müssen die Stundenkosten für einen Benutzer oder ein Aufgabengebiet aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands), aber Sie möchten nicht, dass sich diese Änderung auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder Sie möchten, dass sie nur einen Teil der historischen Stunden betrifft.

## Lösung

Fügen Sie die Stunden hinzu, die Sie nicht in einen Rechnungsnachweis für das Projekt ändern möchten, und legen Sie den Status des Rechnungsnachweises auf In Rechnung gestellt fest.  Dadurch wird der alte Satz gesperrt und die Aktion „Finanzen neu berechnen“ ignoriert.  Alle Stunden, die nicht zu einem Rechnungsnachweis gehören, werden mit dem neuen Satz berechnet. Weitere Informationen finden Sie unter [Projektfinanzen neu berechnen](../../manage-work/projects/project-finances/recalculate-project-finances.md).
