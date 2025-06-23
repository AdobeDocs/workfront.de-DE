---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kostenplan-Leistungsindex (CSI) berechnen
description: Der Cost Schedule Performance Index (CSI) ist eine automatische Berechnung, die den Cost Performance Index (CPI) und den Schedule Performance Index (SPI) zu einer allgemeinen Kennzahl kombiniert, die Kosten und Zeitplan ausgleicht.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Kostenplan-Leistungsindex (CSI) berechnen

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Übersicht über den Kostenplan-Leistungsindex (CSI)

Der Cost Schedule Performance Index (CSI) ist eine automatische Berechnung, die den Cost Performance Index (CPI) und den Schedule Performance Index (SPI) zu einer allgemeinen Kennzahl kombiniert, die Kosten und Zeitplan ausgleicht. Indem Sie diese Werte miteinander multiplizieren, kann eine einzelne Metrik einen längeren Zeitplan mit einem niedrigeren Budget berücksichtigen oder umgekehrt. Projektmanager können dies verwenden, um den allgemeinen Projekt- oder Aufgabenzustand zu bestimmen, wenn Kosten geopfert werden, um den Zeitplan während des Projekts zu erstellen.

>[!TIP]
>
>Adobe Workfront berechnet CSI sowohl für Aufgaben als auch für Projekte, aber nicht für Probleme.

Sie können von den von dieser Metrik bereitgestellten Informationen nur profitieren, wenn die folgenden Szenarien in Ihrer Organisation vorhanden sind:

* Ihre Benutzer protokollieren Zeit für die Arbeit, die sie abschließen. CSI wird anhand der Stunden berechnet.
* Ihren Benutzern oder Aufgabengebieten sind Kosten pro Stunde zugeordnet. Diese berechnet CSI auf der Grundlage der Kosten.

## So berechnet Workfront den Kostenplan-Leistungsindex (CSI)

Workfront berechnet den Kostenentwicklungsindex (Cost Performance Index, CSI) eines Projekts oder einer Aufgabe anhand der folgenden Formel:

`CSI = CPI x SPI`

Informationen zum CPI finden Sie im Artikel [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Informationen zu SPI finden Sie im Artikel [Calculate Schedule Performance Index (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI hat die folgenden drei möglichen Werte:

* 1= Folgt dem Gesamtplan
* \>1 = Kombination aus Unterbudgetplan
* &lt;1 = Kombination aus überbudgetiertem Zeitplan

![CSI](assets/csi-highlighted.png)

## Suchen Sie den Kostenplan-Leistungsindex (CSI)

>[!CAUTION]
>
>Sie müssen Zugriff auf „Finanzdaten anzeigen“ in Ihrer Zugriffsebene und auf die Berechtigungen zum Anzeigen des Projekts oder der Aufgabe haben, um den CSI-Wert eines Projekts oder einer Aufgabe sehen zu können.

Sie können CSI in den folgenden Bereichen von Workfront finden:

* Finanzbereich im Abschnitt Projektdetails.
* Finanzbereich im Abschnitt „Aufgabendetails“
* Eine Projekt- oder Aufgabenansicht.
* Ein Projekt- oder Aufgabenbericht.
