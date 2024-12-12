---
product-area: projects
navigation-topic: financials
title: Leistungsindex-Methode (PIM) festlegen
description: Die Leistungsindex-Methode (PIM) für das Projekt steuert die Methode, die Adobe Workfront zur Berechnung von Projektleistungsmetriken verwendet, z. B. den Kosten Performance Index (CPI), den Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI) und Estimate At Completion (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 1%

---

# Leistungsindex-Methode (PIM) festlegen

Die Leistungsindex-Methode (PIM) für das Projekt steuert die Methode, die Adobe Workfront zur Berechnung von Projektleistungsmetriken verwendet, z. B. den Kosten Performance Index (CPI), den Cost Schedule Performance Index (CSI), Schedule Performance Index (SPI) und Estimate At Completion (EAC).

Workfront berechnet diese Werte wie folgt:

* Stunden
* Kosten

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
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zu PIM in Workfront

* Ihr Workfront-Administrator oder ein Gruppenadministrator legt die Standardeinstellung für fest, ob die Performance Index Method (PIM) stundenbasiert oder kostenbasiert sein soll. Die Berechnungen für die Leistungsmetriken ändern sich entsprechend der Einstellung dieses Standards. Weitere Informationen zum Ändern der Standardeinstellung für die Berechnung des PIM finden Sie unter [Konfigurieren der systemweiten Projektanvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Projektmanager können auch die Einstellung für PIM auf Projektebene für einzelne Projekte auf der Unterregisterkarte Finanzen des Projekts ändern. Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Unterregisterkarte &quot;Finanzen&quot;des Projekts zu bearbeiten.

## Leistungsindex-Methode (PIM) für ein Projekt festlegen

1. Gehen Sie zu einem Projekt, dessen Eigentümer Sie sind.

   >[!IMPORTANT]
   >
   >Für die folgenden Schritte benötigen Sie die Berechtigung zum Verwalten des Projekts. Wir empfehlen auch, dass nur der Projekteigentümer Änderungen am Finanzbereich des Projekts vornehmen sollte.

1. Klicken Sie im linken Bereich auf **Projektdetails** und gehen Sie dann zum Bereich **Finanzen** .
1. Doppelklicken Sie auf den Wert im Feld **Leistungsindex-Methode** , um ihn zu bearbeiten.
1. Wählen Sie aus den folgenden Optionen im Feld **Leistungsindex-Methode** aus:

   | Stundenbasiert | Workfront verwendet die geplanten Stunden zur Berechnung des CPI und des EAC des Projekts, und der EAC des Projekts wird als Zahl in Stunden angezeigt. |
   |---|---|
   | Kostenbasiert | Workfront verwendet die geplanten Arbeitskosten zur Berechnung des CPI und des EAC des Projekts, und der EAC wird als Währungswert angezeigt. Wenn Sie diese Option auswählen, stellen Sie sicher, dass Ihre Aufgabenverantwortlichen (Auftragsrollen oder Benutzer) den Kostenstellen zugeordnet sind. |

   {style="table-layout:auto"}

1. Klicken Sie auf **Speichern** **Änderungen**.
