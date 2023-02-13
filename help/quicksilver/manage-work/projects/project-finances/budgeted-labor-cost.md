---
content-type: reference
product-area: projects
navigation-topic: financials
title: Budgetierte Arbeitskosten und budgetierte Stunden für Projekte
description: Budgetierte Arbeitskosten und budgetierte Stunden für Projekte
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Budgetierte Arbeitskosten und budgetierte Stunden für Projekte

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Sie können Ihre Ressourcen für die Arbeit mit dem Adobe Workfront Resource Planer einplanen.

Während Sie Ihre Ressourcen für die Projektarbeit einplanen, berechnet Workfront die budgetierten Arbeitskosten für die Rollen, Projekte und Benutzer anhand der Kosten pro Stunde.

Der Resource Planer Budgeted Labour Cost of a project ist eine Berechnung zwischen den Kosten, die mit den zugewiesenen Auftragsrollen verbunden sind, um die Arbeit an dem Projekt abzuschließen, und der geschätzten Anzahl der Stunden (Resource Planer Budgeted Hours), die für den Abschluss der Arbeit in jeder Rolle benötigt werden können.

>[!IMPORTANT]
>
>Die im Ressourcenplaner veranschlagten Arbeitskosten für Benutzer wirken sich nicht auf die Kosten des Projekts aus. Nur die Arbeitskosten für Stellenangebote wirken sich auf die Kosten des Projekts aus.

## Übersicht über die budgetierten Arbeitskosten für Job Roles und das Projekt

Workfront verwendet die budgetierten Arbeitskosten der Arbeitsplatzrollen im Projekt, um die budgetierten Arbeitskosten des Projekts zu berechnen.

>[!TIP]
>
>Die budgetierten Arbeitskosten eines Projekts im Geschäftsfall werden in Berichten und Listen als Ressourcenplaner mit budgetierten Arbeitskosten angezeigt.

Die **Geplante Arbeitskosten** (oder &quot;Ressourcenplaner - Budgetierte Arbeitskosten&quot;) eines Projekts wird anhand der folgenden Formel berechnet:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Die in der obigen Berechnung verwendeten Felder beziehen sich auf Folgendes:

* Die für Stellenrollen im Ressourcenbudgeting-Bereich des Projekts oder im Ressourcenplaner geplanten Stunden.

   Weitere Informationen zu Budgetierungsressourcen im Ressourcenplaner finden Sie im Abschnitt &quot;Budgetierung von Ressourcen im Ressourcenplaner&quot;im Artikel [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   Weitere Informationen über die Budgetierungsressourcen im Bereich Ressourcenbudgetierung im Geschäftsfall finden Sie unter [Haushaltsmittel im Geschäftsfall](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* Die **Kosten pro Stunde Rate der Rolle &quot;Arbeit&quot;** in der obigen Berechnung bezieht sich auf die Kosten, die mit den einzelnen Stellenangeboten des Projekts verbunden sind.\
   Weitere Informationen zum Erstellen und Verwalten von Auftrags-Rollen und deren Zuordnung zu Kostensätzen finden Sie im Artikel [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront berechnet alle Kosteninformationen unter Verwendung der Projektwährung. Wenn Sie im Ressourcenplaner Budgetzeit für Ihre Ressourcen angeben, ist die Option zum Ändern der Projektwährung deaktiviert.\
>Weitere Informationen zum Ändern der Währung eines Projekts finden Sie im Artikel [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md).

## Übersicht über die budgetierten Arbeitskosten für Benutzer

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>Die Kosten für die von den Nutzern in den Haushaltsplan eingestellte Arbeit wirken sich nicht auf die budgetierten Arbeitskosten des Projekts aus. Nur die Arbeitskosten der Arbeitsplatzrollen in einem Projekt wirken sich auf den Ressourcenplaner aus.
> 
>Die Gesamtkosten aller Benutzer für die Arbeit können mit den im Ressourcenplaner veranschlagten Arbeitskosten der den Benutzern zugeordneten Arbeitsplatzrollen übereinstimmen.
>
>Wenn Sie im Ressourcenplaner die budgetierten Stunden für Benutzer schätzen, sind die damit verbundenen Kosten die der mit den Benutzern verbundenen Stellenrollen. Es handelt sich nicht um Kosten im Zusammenhang mit den Nutzern oder deren Tarifen.

Wenn Benutzer mit den Stellenrollen des Projekts verknüpft sind und ihre Arbeitszeiten im Ressourcenplaner einberechnet werden, werden ihre budgetierten Arbeitskosten je nach Ansicht in Workfront mit den folgenden Namen angezeigt:

* [!UICONTROL **Geplante Arbeitskosten**]: Der Bereich Ressourcenbudgetierung des Geschäftsfalls unter den entsprechenden Rollen.

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: Der Ressourcenplaner beim Anzeigen von Informationen in der Projekt- und Rollenansicht nach Kosten.

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Benutzer werden im Bereich Ressourcenbudgetierung des Geschäftsfalls unter ihren jeweiligen Rollen oder im Ressourcenplaner angezeigt, wenn sie die folgenden Anforderungen erfüllen:

* Sie sind mit einer der Auftragsrollen im Projekt verknüpft.
* Sie haben im Ressourcenplaner die budgetierten Stunden angegeben.
* Ihrem Profil ist die Kosten pro Stunde zugeordnet.

   Weitere Informationen zum Hinzufügen von Kosten pro Stunde zu Benutzern finden Sie im Artikel [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Der Benutzer ist Teil eines der Ressourcen-Pools, die mit dem Projekt verknüpft sind.

Die budgetierten Arbeitskosten eines Benutzers werden anhand der folgenden Formel berechnet:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Finden Sie die budgetierten Arbeitskosten eines Projekts

Die im Ressourcenbudgeting-Bereich des Geschäftsszenarios oder des Ressourcenplaners ausgewiesenen budgetierten Arbeitskosten werden in den folgenden Bereichen von Workfront unter folgenden Namen angezeigt:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Anzeigename der budgetierten Arbeitskosten</strong></td> 
     <td><strong>Gebiet von Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Budgetierte Lohnkosten</td> 
     <td>Ressourcen-Budgeting-Bereich des Geschäftsfalles</td> 
    </tr> 
    <tr> 
     <td>Budgetierte Kosten</td> 
     <td><p>Kostenansicht des Nutzungsberichts</p><p>Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Informationen zur Nutzung anzeigen</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Projekt- oder Rollenansichten des Ressourcenplaners nach Kosten</td> 
    </tr> 
    <tr> 
     <td>Ressourcenplaner Projekt budgetierte Arbeitskosten</td> 
     <td> <p>Projektbericht</p> <p>Bericht über das Projekt (Finanzdaten)</p> <p>Aufgabenbericht</p> <p>Problembericht</p> <p>Bericht "Budgetierte Stunde"</p> <p>Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerdefinierten Bericht erstellen</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Wenn Sie den Adobe Workfront-Szenario-Planer zum Budget von Projektressourcen verwenden, entsprechen die im Bereich Ressourcenbudgetierung des Geschäftsfalls veranschlagten Arbeitskosten den Kosten der mit dem Projekt verknüpften Initiative für Personen. Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md). Weitere Informationen zu Budgeteinsätzen mithilfe des Szenario-Players finden Sie unter [Budgetressourcen im Geschäftsfall mit dem Szenario-Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Suchen Sie die budgetierten Stunden eines Projekts

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Budgetierte Stunden beeinflussen den Wert der budgetierten Arbeitskosten (oder der im Ressourcenplaner veranschlagten Kosten) des Projekts.

Die budgetierten Arbeitskosten eines Projekts sind die Kosten im Zusammenhang mit den zugewiesenen Aufgaben für die Durchführung der Arbeit am Projekt und die geschätzte Anzahl der Stunden (veranschlagte Stunden), die jede Rolle für die Fertigstellung der Arbeit in Anspruch nehmen kann.

Sie können die budgetierten Stunden in Workfront in den unten aufgelisteten Feldern anzeigen.

>[!NOTE]
>
>Jede andere Erwähnung von &quot;Budgeting Hours&quot;in Workfront bezieht sich auf die geplanten Stunden mit veralteten Funktionen, die aus Workfront entfernt wurden. Dies sind schreibgeschützte Felder und werden nicht mit aktuellen Informationen aktualisiert, wenn Sie die aktuellen Tools zur Ressourcenbudgetierung verwenden.

Die im Ressourcenbudgeting-Bereich des Business Case oder des Resource Planers im Haushaltsplan veranschlagten Stunden werden in den folgenden Bereichen von Workfront und unter folgenden Namen angezeigt:

* **Stunden**: Ressourcen-Budgeting-Bereich des Geschäftsfalles
* **BDG**:Ressourcen-Planer, der von Stunden angezeigt wird
* **Budgetierte Stunden**: Ansicht &quot;Dienstzeiten&quot;des Nutzungsberichts Weitere Informationen finden Sie unter [Informationen zur Ressourcenauslastung anzeigen](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Stunden**: Bericht &quot;Budgetierte Stunde&quot;

   Das Objekt &quot;Budgetierte Stunde&quot;im Bericht &quot;Budgetierte Stunde&quot;bezieht sich auf Informationen zu einem veralteten Tool für die Ressourcenverwaltung. Nur der &quot;Bud. Das Feld &quot;Stunden&quot;in diesem Bericht bezieht sich auf die im Ressourcenplaner oder im Bereich &quot;Ressourcenbudgetierung&quot;des Projektgeschäftes geplanten Stunden.

   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel **Benutzerdefinierten Bericht erstellen**.
* **Ressourcenplaner - Budgetierte Stunden**: in den folgenden Berichten:

   * Projektbericht
   * Bericht über das Projekt (Finanzdaten)
   * Aufgabenbericht
   * Problembericht
   * Bericht &quot;Budgetierte Stunde&quot;
