---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Verhindern, dass sich die Aktion „Finanzen neu berechnen“ auf historische Stunden auswirkt, wenn sich die Sätze ändern
description: Sie müssen die Stundenkosten für einen Benutzer oder ein Aufgabengebiet aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands), aber Sie möchten nicht, dass sich diese Änderung auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder Sie möchten, dass sie nur einen Teil der historischen Stunden betrifft.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 13%

---

# Verhindern, dass sich die Aktion „Finanzen neu berechnen“ auf historische Stunden auswirkt, wenn sich die Sätze ändern

## Problem

Sie müssen die Stundenkosten für einen Benutzer oder ein Aufgabengebiet aktualisieren (aufgrund einer Erhöhung oder eines anderen Umstands), aber Sie möchten nicht, dass sich diese Änderung auf Stunden auswirkt, die zuvor in Projekten protokolliert wurden, oder Sie möchten, dass sie nur einen Teil der historischen Stunden betrifft.

## Lösung

Fügen Sie die Stunden hinzu, die Sie nicht in einen Rechnungsnachweis für das Projekt ändern möchten, und legen Sie den Status des Rechnungsnachweises auf In Rechnung gestellt fest.  Dadurch wird der alte Satz gesperrt und die Aktion „Finanzen neu berechnen“ ignoriert.  Alle Stunden, die nicht zu einem Rechnungsnachweis gehören, werden mit dem neuen Satz berechnet. Weitere Informationen finden Sie unter [Projektfinanzen neu berechnen](../../manage-work/projects/project-finances/recalculate-project-finances.md).
