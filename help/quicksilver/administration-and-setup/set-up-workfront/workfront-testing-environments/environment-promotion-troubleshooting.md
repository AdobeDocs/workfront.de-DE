---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Fehlerbehebung bei der Umgebungsförderung
description: Beheben häufiger Probleme bei der Umgebungsförderung.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Fehlerbehebung bei der Umgebungsförderung

Dieser Artikel beschreibt, wie Sie Probleme bei der Umgebungsförderung beheben können.

## Problem: Das Umgebungs-Promotion-Paket wird angehalten oder schlägt fehl

Wenn Ihr Umgebungs-Promotion-Paket wartet oder fehlschlägt, versuchen Sie Folgendes:

* Wenn eine Paketinstallation nach 10-15 Minuten ausfällt oder eine Paketinstallation fehlschlägt, bauen Sie das vorhandene Paket neu zusammen oder erstellen Sie ein neues Paket.

* Wenn eine Paketinstallation fehlschlägt, kann ein Problem mit einem oder mehreren Objekten vorliegen. Überprüfen Sie die Fehlermeldungen, die das Objekt identifizieren und dazu beitragen können, das Problem zu identifizieren. Nachdem Sie das Problem mit dem -Objekt behoben haben, stellen Sie das Paket wieder zusammen und versuchen Sie die Installation erneut.

* Wenn Sie immer noch Probleme mit einer Installation haben, versuchen Sie, die Installation in einer anderen Zielumgebung zu replizieren. Halten Sie sich so nah wie möglich an die ursprüngliche Installation, einschließlich der ausgewählten Objekte und Installationsaktionen.

* Es wird empfohlen, den Paketinhalt immer zu überprüfen, nachdem das Paket assembliert wurde, um sicherzustellen, dass es die erwarteten Objekte enthält.


## Problem: Benutzerdefiniertes Formular kann nicht weitergeleitet werden

Dies kann vorkommen, da das benutzerdefinierte Formular ein berechnetes Feld enthält. Wenn ein berechnetes Feld auf ein Feld verweist, das in einem benutzerdefinierten Formular nicht referenziert wird, wird ein Paket, das dieses Formular enthält, nicht weitergeleitet, und der/die Benutzende sieht möglicherweise die folgende Meldung:

„Die folgenden Felder sind ungültig: Ungültiger benutzerdefinierter Ausdruck Ungültiger Ausdruck: Ungültiger benutzerdefinierter Ausdruck.“

Dieses Problem kann auftreten, wenn auf ein vorhandenes Feld verwiesen wird, das mit keinem benutzerdefinierten Formular in der Zielumgebung verknüpft ist, oder auf ein neu erstelltes Feld.

Führen Sie einen der folgenden Schritte aus, um dieses Problem zu beheben:

* Erstellen Sie ein Paket mit einem benutzerdefinierten Formular vom Typ Projekt , das das referenzierte Feld enthält. Leiten Sie nach dem Hochstufen dieses Pakets in die Zielumgebung das ursprünglich vorgesehene Paket hoch, das das berechnete Feld enthält.
* Erstellen Sie das referenzierte Feld in der Zielumgebung manuell und verknüpfen Sie es mit einem benutzerdefinierten Formular vom Typ Projekt . Danach wird das Feld erkannt, und Sie können das Paket weiterleiten, ohne den Fehler zu bemerken.
