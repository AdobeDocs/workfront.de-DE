---
product-area: projects
navigation-topic: financials
title: Festlegen der Performance Index Method (PIM)
description: Die Leistungsindexmethode (PIM) für das Projekt steuert die Methode, die Adobe Workfront verwendet, um Projektleistungsmetriken wie Kostenentwicklungsindex (Cost Performance Index, CPI), Kostenplanleistungsindex (Cost Schedule Performance Index, CSI), Zeitplan-Leistungsindex (SPI) und Schätzung bei Abschluss (EAC) zu berechnen.
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 12%

---

# Festlegen der Performance Index Method (PIM)

Die Leistungsindexmethode (PIM) für das Projekt steuert die Methode, die Adobe Workfront verwendet, um Projektleistungsmetriken wie Kostenentwicklungsindex (Cost Performance Index, CPI), Kostenplanleistungsindex (Cost Schedule Performance Index, CSI), Zeitplan-Leistungsindex (SPI) und Schätzung bei Abschluss (EAC) zu berechnen.

Workfront berechnet diese Werte wie folgt:

* Stunden
* Kosten

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten von Projektberechtigungen mit Berechtigungen zum Bearbeiten von General Finance</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
