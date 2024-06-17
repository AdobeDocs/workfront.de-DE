---
product-area: reporting
keywords: user,delegation,report,delegate,approval
navigation-topic: create-and-manage-reports
title: Erstellen eines Berichts zur Benutzerdelegation
description: Erstellen eines Berichts zur Benutzerdelegation
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# Erstellen eines Berichts zur Benutzerdelegation

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront können Benutzer Projekte-, Aufgaben- und Problemgenehmigungen an andere Benutzer delegieren, um sicherzustellen, dass ihre Genehmigungen bei Abwesenheit verwaltet werden. Benutzer mit einer Planungslizenz können einen Bericht zur Benutzerdelegierung erstellen, um folgende Informationen zu erhalten:

* Wer hat seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert
* Welche Benutzer haben Aufgaben-, Problem- und Projektgenehmigungen zugewiesen?

* Beginn und Ende der Delegationen

Weitere Informationen zum Delegieren von Genehmigungen finden Sie unter [Validierungsanfrage delegieren](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für die Elemente, deren Genehmigungen delegiert werden, und für die an der Zuweisung beteiligten Benutzer</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Bericht zur Benutzerdelegierung erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Berichte**.

1. Klicks **Neuer Bericht**, wählen Sie **Benutzerdelegierung**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Die folgenden Felder werden in diesem Bericht standardmäßig angezeigt:

   | Feld | Beschreibung |
   |---|---|
   | **Vom Benutzer** | Dies ist der Benutzer, der seine Aufgaben-, Problem- und Projektgenehmigungen an einen anderen Benutzer delegiert. |
   | **An Benutzer** | Dies ist der Benutzer, dem Aufgaben-, Problem- und Projektgenehmigungen zugewiesen wurden. |
   | **Starten** | Dies ist der Beginn der Abwesenheitszeit für den Benutzer, der die Delegationen gebildet hat. |
   | **Ende** | Dies ist das Ende der Abwesenheitszeit für den Benutzer, der die Delegationen gebildet hat. |

   {style="table-layout:auto"}

1. (Optional) Ändern Sie im ReportBuilder Folgendes:

   * Spalten
   * Gruppierungen
   * Filter
   * Diagramm

   Weitere Informationen zu diesen Funktionen finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Nachdem Sie die Berichterstellung abgeschlossen haben, klicken Sie auf **Speichern und schließen**.

1. Geben Sie im **Berichtsname** und klicken Sie auf **Bericht speichern**.

   Der Bericht wird angezeigt.
