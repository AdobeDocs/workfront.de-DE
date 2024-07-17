---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Verhindern Sie, dass die Aktion "Finanzen neu berechnen"historische Stunden beeinflusst, wenn sich die Beträge ändern
description: Sie müssen die stündlichen Kosten für einen Benutzer oder eine Rolle im Arbeitsbereich aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands). Sie möchten jedoch nicht, dass diese Änderung sich auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder dass sie sich nur auf einen Teil historischer Stunden auswirkt.
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Verhindern Sie, dass die Aktion &quot;Finanzen neu berechnen&quot;historische Stunden beeinflusst, wenn sich die Beträge ändern

## Problem

Sie müssen die stündlichen Kosten für einen Benutzer oder eine Rolle im Arbeitsbereich aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands). Sie möchten jedoch nicht, dass diese Änderung sich auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder dass sie sich nur auf einen Teil historischer Stunden auswirkt.

## Lösung

Fügen Sie die Stunden, die Sie nicht ändern möchten, zu einem Rechnungsdatensatz im Projekt hinzu und setzen Sie den Status des Abrechnungsdatensatzes auf &quot;Abgerechnet&quot;.  Dies hängt von der alten Rate ab und wird von der Aktion Finanzen neu berechnen ignoriert.  Alle Stunden, die nicht zu einem abrechnungsfähigen Datensatz gehören, werden zum neuen Tarif berechnet. Weitere Informationen finden Sie unter [Neuberechnen der Projektfinanzen](../../manage-work/projects/project-finances/recalculate-project-finances.md).
