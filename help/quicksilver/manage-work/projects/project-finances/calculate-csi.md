---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Cost Schedule Performance Index (CSI)
description: Der Cost Schedule Performance Index (CSI) ist eine automatische Berechnung, die den Cost Performance Index (CPI) und Schedule Performance Index (SPI) in einer allgemeinen Metrik kombiniert, die Kosten und Zeitplan ausgleicht.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Calculate Cost Schedule Performance Index (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Übersicht über den CSI (Cost Schedule Performance Index)

Der Cost Schedule Performance Index (CSI) ist eine automatische Berechnung, die den Cost Performance Index (CPI) und Schedule Performance Index (SPI) in einer allgemeinen Metrik kombiniert, die Kosten und Zeitplan ausgleicht. Durch Multiplikation dieser Werte kann eine einzelne Metrik einen längeren Zeitplan mit einem niedrigeren Budget berücksichtigen oder umgekehrt. Projektmanager können dies verwenden, um den allgemeinen Projekt- oder Aufgabenstatus zu bestimmen, wenn Kosten geopfert werden, um die Planung während des Projekts voranzutreiben.

>[!TIP]
>
>Adobe Workfront berechnet CSI für Aufgaben und Projekte. Workfront berechnet keinen CSI-Wert für Probleme.

Sie können von den Informationen dieser Metrik nur profitieren, wenn in Ihrer Organisation Folgendes vorhanden ist:

* Ihre Benutzer protokollieren die Zeit für die Arbeit, die sie abgeschlossen haben.\
  Dies berechnet CSI auf der Grundlage von Stunden.
* Ihren Benutzern oder Auftragseinheiten sind die Kosten pro Stunde zugeordnet. 

  Dies berechnet CSI auf der Grundlage der Kosten.

## Berechnung des CSI (Cost Schedule Performance Index) durch Workfront

Workfront berechnet den CSI (Cost Performance Index) eines Projekts oder einer Aufgabe mithilfe der folgenden Formel:

`CSI = CPI x SPI`

Weitere Informationen zu CPI finden Sie im Artikel [CPI (Cost Performance Index) berechnen](../../../manage-work/projects/project-finances/calculate-cpi.md).

Weitere Informationen zu SPI finden Sie im Artikel [Berechnung des Zeitplan-Leistungsindex (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI hat die folgenden drei möglichen Werte:

* 1 = entspricht dem Gesamtplan
* \>1 = Unter Budgetplankombination
* &lt;1) Kombination aus Budgetplankombinationen

![](assets/csi-highlighted.png)

## Suchen Sie den CSI (Cost Schedule Performance Index).

>[!CAUTION]
>
>Sie müssen Zugriff auf &quot;Finanzdaten anzeigen&quot;in Ihrer Zugriffsebene haben und berechtigt sein, das Projekt oder die Aufgabe anzuzeigen, um den CSI-Wert eines Projekts oder einer Aufgabe sehen zu können.

Sie finden CSI in den folgenden Bereichen von Workfront:

* Finanzbereich im Abschnitt Projektdetails .
* Finanzbereich im Abschnitt &quot;Aufgabendetails&quot;.
* Projekt- oder Aufgabenansicht
* Projekt- oder Aufgabenbericht
