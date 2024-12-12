---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berechnung des Zeitplan-Leistungsindex (SPI)
description: Der Zeitplan-Leistungsindex (SPI) beschreibt die Beziehung zwischen dem geplanten und dem tatsächlichen Zeitplan.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Berechnung des Zeitplan-Leistungsindex (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Der Zeitplan-Leistungsindex (SPI) beschreibt die Beziehung zwischen dem geplanten und dem tatsächlichen Zeitplan. Adobe Workfront berechnet SPI auf Projekt- und Aufgabenebene. Projektmanager überprüfen diese Metrik, um festzustellen, ob Aufgaben oder Projekte derzeit vor oder hinter dem Zeitplan nachverfolgt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Licht oder höher</p>
   <p>oder</p>
   <p>Aktuell: Überprüfen oder höher</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten anzeigen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen von oder höheren Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen von Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über den Zeitplan-Leistungsindex (SPI)

* [Was der SPI-Wert anzeigt](#what-the-spi-value-shows)
* [Berechnung von SPI durch Workfront](#how-workfront-calculates-spi)

### Was der SPI-Wert anzeigt {#what-the-spi-value-shows}

Projektmanager wissen, dass ein SPI-Wert von 1 bedeutet, dass das Projekt planmäßig oder planmäßig durchgeführt wird.  Werte größer als 1 weisen darauf hin, dass ein Projekt vor dem Zeitplan liegt und Werte kleiner als 1 bedeuten, dass ein Projekt hinter dem Zeitplan liegt.  Je weiter von 1, desto größer ist die Abweichung vom Plan.

| **SPI-Wert** | **Anzeige von &quot;On Schedule&quot;** |
|---|---|
| 1 | Im Plan oder planmäßig |
| > 1 (größer als 1) | Vorfeld des Zeitplans |
| &lt; 1 (weniger als 1) | Hinter dem Zeitplan |

{style="table-layout:auto"}

### Berechnung von SPI durch Workfront  {#how-workfront-calculates-spi}

Workfront berechnet SPI anhand der folgenden Formel:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Wenn die geplanten Stunden auf Datum = 0 geplant sind, ist SPI = 1*.

Geplante Stunden Planen bis Datum werden zu dem Zeitpunkt berechnet, zu dem Sie die Berechnungen durchführen. Sie zeigt die Anzahl der geplanten Stunden bis zum aktuellen Datum an. Sie kann automatisch neu berechnet werden, wenn Sie Ihre Finanzdaten zur Genauigkeit ändern. In Workfront gibt es kein Feld, das diesen Wert angibt.

Wenn Sie beispielsweise ein Projekt mit einer Aufgabe haben und die Aufgabe 10 geplante Stunden und eine 10-tägige Dauer umfasst, beträgt der Zeitplan für geplante Stunden bis zum Datum des 5. Tages 5. 

## SPI in einem Projekt oder einer Aufgabe suchen

1. Wechseln Sie zum Projekt oder zur Aufgabe, in dem/der SPI angezeigt werden soll.
1. Je nachdem, ob Sie SPI für ein Projekt oder eine Aufgabe anzeigen möchten, führen Sie einen der folgenden Schritte aus:

   1. Klicken Sie im linken Bereich auf **Projektdetails** und zeigen Sie dann den Bereich **Finanzen** an.

   1. Klicken Sie im linken Bereich auf **Aufgabendetails** und zeigen Sie dann den Bereich **Finanzen** an.

      ![](assets/spi-on-project-nwe.png)

1. Suchen Sie das Feld **CPI/SPI/CSI**.
