---
product-area: reporting
keywords: Benutzer, Delegierung, Bericht, Delegieren, Genehmigung
navigation-topic: create-and-manage-reports
title: Erstellen eines Benutzerdelegierungsberichts
description: Erstellen eines Berichts zur Benutzerdelegierung
author: Courtney
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 17%

---

# Erstellen eines Berichts zur Benutzerdelegierung

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront können Benutzende Projekt-, Aufgaben- und Problem-Genehmigungen an andere Benutzende delegieren, um sicherzustellen, dass ihre Genehmigungen verwaltet werden, wenn sie abwesend sind. Benutzer mit einer Abo-Lizenz können einen Bericht zur Benutzerdelegierung erstellen, um Folgendes anzuzeigen:

* Wer hat seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert?
* Welche Benutzer haben Aufgaben-, Problem- und Projektgenehmigungen delegiert?

* Die Termine, zu denen die Delegationen beginnen und enden

Weitere Informationen zum Delegieren von Genehmigungen finden Sie unter [Genehmigungsanforderung delegieren](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

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
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
 <td> <p>Anzeigen von Berechtigungen für die Elemente, deren Genehmigungen delegiert werden, und für die an der Delegierung beteiligten Benutzer</p></td>  
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Benutzerdelegierungsberichts

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenü-Symbol &#x200B;](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront, und klicken Sie dann auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht**, und wählen Sie dann **Benutzerdelegation** aus.

   ![Benutzerdelegierung für neuen Bericht](assets/classic-new-report-user-delegation-350x644.png)

   Die folgenden Felder werden in diesem Bericht standardmäßig angezeigt:

   | Feld | Beschreibung |
   |---|---|
   | **Von Benutzer** | Dies ist der Benutzer, der seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert. |
   | **An Benutzer** | Dies ist der Benutzer, dem Aufgaben-, Problem- und Projektgenehmigungen delegiert wurden. |
   | **Startdatum** | Dies ist der Beginn der Abwesenheitszeit für den Benutzer, der die Delegationen gebildet hat. |
   | **Enddatum** | Dies ist das Ende der Abwesenheitszeit für den Benutzer, der die Delegierungen vorgenommen hat. |

   {style="table-layout:auto"}

1. (Optional) Ändern Sie im Report Builder Folgendes:

   * Spalten (Ansicht)
   * Gruppierungen
   * Filter
   * Diagramm

   Weitere Informationen zu diesen Features finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Nachdem Sie die Erstellung des Berichts abgeschlossen haben, klicken Sie auf **Speichern + Schließen**.

   Der Bericht wird angezeigt.
