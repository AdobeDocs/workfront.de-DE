---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Planleistungsindex (SPI) berechnen
description: Der Zeitplan-Leistungsindex (SPI) beschreibt die Beziehung zwischen dem geplanten Zeitplan und dem tatsächlichen Zeitplan.
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# Planleistungsindex (SPI) berechnen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Der Zeitplan-Leistungsindex (SPI) beschreibt die Beziehung zwischen dem geplanten Zeitplan und dem tatsächlichen Zeitplan. Adobe Workfront berechnet den SPI auf Projekt- und Aufgabenebene. Projektmanager überprüfen diese Metrik, um festzustellen, ob Aufgaben oder Projekte derzeit geplant oder sogar vorzeitig nachverfolgt werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Licht oder höher</p>
   <p>Überprüfen oder höher</p></td>  
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Anzeigen des Zugriffs auf Projekte und Finanzdaten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Anzeigen von oder höheren Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen von Finanzdaten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über den Zeitplan-Leistungsindex (SPI)

* [Was der SPI-Wert anzeigt](#what-the-spi-value-shows)
* [So berechnet Workfront SPI](#how-workfront-calculates-spi)

### Was der SPI-Wert anzeigt {#what-the-spi-value-shows}

Projektmanager wissen, dass ein SPI-Wert von 1 bedeutet, dass das Projekt im Zeitplan oder im Plan ist.  Werte größer als 1 zeigen an, dass ein Projekt dem Zeitplan voraus ist, und Werte kleiner als 1 bedeuten, dass ein Projekt in Verzug ist.  Je weiter von 1, desto größer die Abweichung vom Plan.

| **SPI-Wert** | **Anzeige von „On Schedule“** |
|---|---|
| 1 | Nach Plan oder Zeitplan |
| > 1 (größer als 1) | Vor dem Zeitplan |
| &lt; 1 (weniger als 1) | In Verzug |

{style="table-layout:auto"}

### So berechnet Workfront SPI  {#how-workfront-calculates-spi}

Workfront berechnet den SPI anhand der folgenden Formel:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Wenn geplante Stunden bis Datum geplant sind = 0, SPI = 1*.

Die bis dato geplanten Stunden werden zu dem Zeitpunkt berechnet, zu dem Sie die Berechnungen durchführen. Zeigt die Anzahl der geplanten Stunden, die bis zum aktuellen Datum geplant sind. Sie kann automatisch neu berechnet werden, wenn Sie Ihre Finanzdaten ändern, um sie korrekt zu halten. In Workfront gibt es kein Feld, das diesen Wert angibt.

Wenn Sie beispielsweise ein Projekt mit einer Aufgabe haben und die Aufgabe 10 geplante Stunden und eine Dauer von 10 Tagen hat, lautet der Zeitplan für geplante Stunden bis zum 5. Tag 5.

## Suchen einer SPI in einem Projekt oder einer Aufgabe

1. Wechseln Sie zu dem Projekt oder der Aufgabe, in dem bzw. der Sie den SPI anzeigen möchten.
1. Führen Sie je nachdem, ob Sie die SPI für ein Projekt oder eine Aufgabe anzeigen möchten, einen der folgenden Schritte aus:

   1. Klicken Sie **linken Bedienfeld auf** Projektdetails) und dann auf den Bereich **Finanzen**.

   1. Klicken Sie **linken** auf „Aufgabendetails“ und dann auf den Bereich **Finanzen**.

      ![SPI im Projekt](assets/spi-on-project-nwe.png)

1. Suchen Sie das Feld **CPI/SPI/CSI**.
