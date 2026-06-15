---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Entscheidung der genehmigenden Person zeigt im Bericht zu Korrekturabzugsgenehmigungen einen Bindestrich an
description: Ein Bindestrich im Feld Genehmigerentscheidung des Berichts zur Korrekturabzugsgenehmigung zeigt an, dass ein Empfänger im Korrekturabzug nicht mehr in der Entscheidungsrolle ist.
author: Courtney
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 9c6e8d04c1faa2902cab870a03a68f0cb14da3aa
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# Entscheidung der genehmigenden Person zeigt im Bericht zu Korrekturabzugsgenehmigungen einen Bindestrich an

## Problem

Im Bericht zur Korrekturabzugsgenehmigung zeigt das Feld Genehmigende Entscheidung eines Empfängers einen Bindestrich (-) an, obwohl im Feld Entscheidungsdatum ein Datum und im Feld Entscheidung ausstehend „Falsch“ angezeigt wird.

![Entscheidung der genehmigenden Person zeigt im Bericht zur Korrekturabzugsgenehmigung einen Bindestrich an](assets/approver-decision-hyphen.png)

## Ursache

Ein Bindestrich im Feld Entscheidung der genehmigenden Person bedeutet, dass der Empfänger im Korrekturabzug nicht mehr in der Entscheidungsrolle ist. Dies kann passieren, wenn:

* Der Empfänger wurde zum Korrekturabzug hinzugefügt, hat eine Entscheidung getroffen und wurde später aus dem Workflow entfernt. Wenn der Empfänger den Korrekturabzug erneut besucht, zeichnet das Proofing-System den Besuch als Entscheidungsänderung auf. Da der Empfänger keine genehmigende Person mehr ist, zeichnet das System die neue Entscheidung als Bindestrich auf.
* Die Rolle des Korrekturabzugs für den Empfänger wurde in eine Rolle geändert, die keine Genehmigungsrechte enthält, wie z. B. „Prüfer“. Informationen zu den Aktionen, die jede Rolle für einen Korrekturabzug ausführen kann, finden Sie unter [Rollen für Korrekturabzüge - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* Das Berechtigungsprofil des Empfängers für Korrekturabzüge wurde nach der Entscheidung herabgestuft.

## Was dies in Ihren Berichten bedeutet

Der Bindestrich ist beabsichtigt. Sie besagt, dass das System nicht darauf wartet, dass der Empfänger den Korrekturabzug genehmigt, und dass der Empfänger für den Korrekturabzug keine Entscheidungsrolle mehr hat.

Das Feld Entscheidungsdatum zeigt weiterhin das Datum der letzten Entscheidungsaktivität des Empfängers an, aber die Entscheidung des Empfängers wird im Bericht nicht mehr gezählt.

Informationen zur Erstellung und Verwendung des Berichts zur Korrekturabzugsgenehmigung finden Sie unter [Verwenden des Berichts zur Korrekturabzugsgenehmigung](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).


