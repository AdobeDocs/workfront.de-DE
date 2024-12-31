---
product-area: projects
navigation-topic: financials
title: Festlegen der Performance-Index-Methode (PIM)
description: Die Leistungsindexmethode (PIM) für das Projekt steuert die Methode, die Adobe Workfront verwendet, um Projektleistungsmetriken wie Kostenentwicklungsindex (Cost Performance Index, CPI), Kostenplanleistungsindex (Cost Schedule Performance Index, CSI), Zeitplan-Leistungsindex (SPI) und Schätzung bei Abschluss (EAC) zu berechnen.
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 1%

---

# Festlegen der Performance-Index-Methode (PIM)

Die Leistungsindexmethode (PIM) für das Projekt steuert die Methode, die Adobe Workfront verwendet, um Projektleistungsmetriken wie Kostenentwicklungsindex (Cost Performance Index, CPI), Kostenplanleistungsindex (Cost Schedule Performance Index, CSI), Zeitplan-Leistungsindex (SPI) und Schätzung bei Abschluss (EAC) zu berechnen.

Workfront berechnet diese Werte wie folgt:

* Stunden
* Kosten

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten von Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum PIM in Workfront

* Ihr Workfront-Administrator oder ein Gruppenadministrator richtet den Standard ein, um festzulegen, ob die Leistungsindexmethode (PIM) stundenbasiert oder kostenbasiert sein soll. Die Berechnungen für die Leistungsmetriken ändern sich je nach Einstellung dieses Standardwerts. Weitere Informationen zum Ändern der Standardeinstellung für die Berechnung des PIM finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Projektmanager können auf Projektebene auch die Einstellung für das PIM für einzelne Projekte auf der Unterregisterkarte Finanzen des Projekts ändern. Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Unterregisterkarte Finanzen des Projekts bearbeiten zu können.

## Festlegen der Leistungsindexmethode (PIM) für ein Projekt

1. Wechseln Sie zu einem Projekt, dessen Besitzer Sie sind.

   >[!IMPORTANT]
   >
   >Sie müssen Berechtigungen verwalten für das Projekt, um die folgenden Schritte ausführen zu können. Wir empfehlen auch, dass nur der Projektinhaber Änderungen am Finanzierungsbereich des Projekts vornehmen sollte.

1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Bereich **Finanzen**.
1. Doppelklicken Sie auf den Wert im Feld **Leistungsindexmethode**, um ihn zu bearbeiten.
1. Wählen Sie im Feld **Leistungsindexmethode“ eine der folgenden** aus:

   | Stundenbasiert | Workfront berechnet den CPI und die EAC des Projekts anhand der geplanten Stunden. Die EAC des Projekts wird als eine Zahl in Stunden angezeigt. |
   |---|---|
   | Kostenbasiert | Workfront verwendet die geplanten Lohnkosten bei der Berechnung des CPI und der EAC des Projekts, und die EAC wird als Währungswert angezeigt. Wenn Sie diese Option auswählen, stellen Sie sicher, dass Ihre Aufgabenzugewiesenen (Aufgabengebiete oder Benutzer) mit Kostensätzen verknüpft sind. |

   {style="table-layout:auto"}

1. Klicken Sie **Speichern** **Änderungen**.
