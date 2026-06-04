---
product-area: reporting
keywords: Benutzer,Delegierung,Bericht,Delegieren,Genehmigung
navigation-topic: create-and-manage-reports
title: Erstellen eines Berichts zur Benutzerdelegierung
description: Erstellen eines Berichts zur Benutzerdelegierung
author: Courtney
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/xauKU-ASfnD7MiuqK-t9h-JGiTTlcVmzFL-pofZOPJ8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 16%

---

# Erstellen eines Berichts zur Benutzerdelegierung

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront können Benutzende Projekt-, Aufgaben- und Problem-Genehmigungen an andere Benutzende delegieren, um sicherzustellen, dass ihre Genehmigungen verwaltet werden, wenn sie abwesend sind. Benutzer mit einer Standard- oder Planlizenz können einen Bericht zur Benutzerdelegierung erstellen, um Folgendes anzuzeigen:

* Wer hat seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert?
* Welche Benutzenden haben Aufgaben-, Problem- und Projektgenehmigungen delegiert?

* Die Daten, an denen die Delegationen beginnen und enden

Weitere Informationen zum Delegieren von Genehmigungen finden Sie unter [Delegieren von Genehmigungsanfragen](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Abo</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
 <td> <p>Anzeigen von Berechtigungen für die Elemente, deren Genehmigungen delegiert wurden, und für die an der Delegierung beteiligten Benutzer</p></td>  
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Berichts zur Benutzerdelegierung

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront und dann auf **Berichte**.

1. Klicken Sie **Neuer Bericht** und wählen Sie dann **Benutzerdelegierung** aus.

   ![Benutzerdelegierung für neuen Bericht](assets/classic-new-report-user-delegation-350x644.png)

   Die folgenden Felder werden standardmäßig in diesem Bericht angezeigt:

   | Feld | Beschreibung |
   |---|---|
   | **Von Benutzer** | Dies ist der Benutzer, der seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert. |
   | **An Benutzer** | Hierbei handelt es sich um den Benutzer, dem Aufgaben-, Problem- und Projektgenehmigungen delegiert wurden. |
   | **Startdatum** | Dies ist der Beginn der Abwesenheitszeit für den Benutzer, der die Delegationen vorgenommen hat. |
   | **Enddatum** | Dies ist das Ende der Abwesenheitszeit für den Benutzer, der die Delegierungen vorgenommen hat. |

   {style="table-layout:auto"}

1. (Optional) Ändern Sie in Report Builder Folgendes:

   * Spalten (Ansicht)
   * Gruppierungen
   * Filter
   * Diagramm

   Weitere Informationen zu diesen Funktionen finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Nachdem Sie den Bericht fertig erstellt haben, klicken Sie auf **Speichern + Schließen**.

   Der Bericht wird angezeigt.
