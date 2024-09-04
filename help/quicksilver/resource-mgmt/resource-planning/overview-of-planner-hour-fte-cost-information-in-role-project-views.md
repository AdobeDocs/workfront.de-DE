---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Übersicht über Stunden, FTE und Kosteninformationen im Projekt und Rollenansichten des Ressourcenplaners
description: Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 0%

---

# Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Die Budgetierung Ihrer Ressourcen für die Arbeit, die sie an einem Projekt durchführen müssen, ist die Hauptfunktion des Ressourcenplaners. Sie können die verfügbare Zeit Ihrer Ressourcen anzeigen und die ihnen zugewiesenen Projekte mit der Zeit verknüpfen.

Weitere Informationen zu Budgeteinträgen im Ressourcenplaner finden Sie unter [Budgetressourcen im Ressourcenplaner unter Verwendung der Projekt- und Rollenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

In diesem Artikel werden einige der Schlüsselkonzepte beschrieben, die Sie kennen müssen, bevor Sie mit dem Budget Ihrer Ressourcen im Ressourcenplaner beginnen.

## Übersicht über die Budgetierungsressourcen

Beachten Sie Folgendes bei der Budgetierung von Ressourcen mithilfe des Ressourcen-Planers:

* Sie können die Zuordnung Ihrer Ressourcen mit einem Budget versehen, indem Sie einen Betrag von Stunden, FTE oder Kosten angeben, den Ihre Ressourcen zum Ausführen der Arbeit an Projekten verwenden können. Wenn Sie die Budgetzeit oder die Kosten für eine Ressource festlegen, werden die Verfügbaren Stunden, VZÄ oder Kosten für die Ressource um den veranschlagten Betrag reduziert. Die verfügbaren Stunden-, FTE- oder Kostenbeträge für die Projekte, die dem Projekt folgen, für das Sie eine Budgetierung vornehmen, verringern sich daher für diese Benutzer und Rollen bei diesen Projekten.

  >[!IMPORTANT]
  >
  >Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren einplanen. Wenn Sie Ressourcen für ein Projekt mit einer Dauer von mehr als 15 Jahren einsetzen, sind die Budgetierungsinformationen möglicherweise nicht korrekt.

* Sie können Stunden, FTE oder Kosten für Ihre Ressourcen für jeden im Ressourcenplaner angezeigten Zeitraum einplanen, unabhängig von der Zeitleiste des Projekts. Wenn Sie beispielsweise angeben möchten, dass Ihre Ressourcen während der Planung des Projekts möglicherweise nicht verfügbar sind (wo sie mit geplanten Stunden verknüpft sind), aber zu einem anderen Zeitpunkt verfügbar sein können, können Sie dies tun, indem Sie sie für Zeiträume mit null geplanten Stunden in den Haushaltsplan einbeziehen, sofern diese zur Verfügung stehen. Danach können Sie die Timeline des Projekts manuell ändern und Ihre Ressourcenverfügbarkeit anpassen.

  >[!NOTE]
  >
  >Wir empfehlen Ihnen, Ihre Stunden, FTE-Kosten oder Kosten manuell für Stellenrollen oder für Benutzer zu finanzieren. Sie können die automatischen Optionen nur dann verwenden, wenn Sie sicher sind, dass die Anzahl der geplanten Stunden, VZÄ oder Kosten immer mit Ihren geplanten Stunden, VZÄ oder Kosten übereinstimmt.\
  >Informationen zur Verwendung der automatischen Budgetierungsoptionen im Ressourcenplaner finden Sie im Abschnitt &quot;Budgetierungsprojekt und -rollen automatisch&quot;im Artikel [Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planers](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* Die Budgetierung von FTE oder Kosten ist identisch mit den Haushaltszeiten, bei denen Adobe Workfront die FTE und Kostenwerte anstelle von Stunden für die von Ihnen bereitgestellten Mittel verwendet.

  Weitere Informationen zur Berechnung der Kosten im Ressourcenplaner finden Sie unter [Berechnen der Kosten im Ressourcenplaner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Die Budgetierung von Zuweisungen für Ihre Ressourcen im Ressourcenplaner erfolgt auf folgende Weise:

   * Manuell

     Oder

   * Automatisch durch Verwendung der Projekt- und Rollenoptionen in den Ansichten **Nach Projekt anzeigen** und **Nach Rolle anzeigen** .

  Weitere Informationen finden Sie unter [Budgetressourcen im Ressourcenplaner mit der Projekt- und Rollenansicht](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Wenn ein Benutzer die Aufgabenrollen ändert, gelöscht, deaktiviert oder aus einem Ressourcen-Pool entfernt wird, ändern sich die für die Rolle vorgesehenen Stunden nicht und werden an die verbleibenden Benutzer in der Rolle verteilt. Wenn kein Benutzer mehr mit der Rolle &quot;job&quot;verknüpft ist, werden die budgetierten Stunden für die Rolle zu null.

Weitere Informationen zu den Projekt- und Rollenoptionen finden Sie im Abschnitt [Grundlegendes zu den Werten für Stunden, FTE und Kosten im Ressourcenplaner](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) in diesem Artikel.

## Grundlegendes zu den Werten für Stunden, FTE und Kosten im Ressourcenplaner {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Bevor Sie Ihre Ressourcen einplanen und die Budgetierungsinformationen im Ressourcenplaner aktualisieren, müssen Sie mit den folgenden Konzepten vertraut sein

* **Geplante Stunden, VZÄ oder Kosten**: Die Arbeit, die gemäß Definition für Aufgaben und Probleme ausgeführt werden muss.
* **Verfügbare Stunden, VZÄ oder Kosten**: Die Zeit, die Benutzer oder Stellenrollen gemäß den mit den Benutzern verknüpften Zeitplänen für die Arbeit zur Verfügung stehen.

Diese Informationen werden im Ressourcenplaner für jede Ressource (Benutzer oder Rolle) und für jedes Projekt angezeigt.

Informationen dazu, was in den Projekt- und Rollenansichten des Projekts angezeigt wird, finden Sie im Artikel [Navigationsübersicht für den Ressourcenplaner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Informationen dazu, wie Kosten im Ressourcenplaner berechnet werden, finden Sie im Artikel [Kosten im Ressourcenplaner berechnen](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Die Budgetierung nach Kosten ist mit der Budgetierung nach Stunden oder VZÄ identisch. Sie müssen jedoch verstehen, wie Workfront Kosten für den Ressourcenplaner berechnet.
>
>Informationen zur Berechnung der Kosten im Ressourcenplaner finden Sie im Artikel [Berechnen der Kosten im Ressourcenplaner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Die folgenden Tabellen zeigen die Zuordnungs- und Verfügbarkeitsinformationen, die im Ressourcenplaner angezeigt werden, wenn entweder das Projekt oder die Rollenansicht angewendet wird. Sie können diese Informationen nach Stunden, FTE oder Kosten anzeigen:

* [Die (verfügbare) AVL Spalte](#the-avl-available-column)
* [Die Spalte PLN (Geplant)](#the-pln-planned-column)
* [Die (budgetierte) BDG-Spalte](#the-bdg-budgeted-column)
* [Die VAR-Spalte (Varianz)](#the-var-variance-column)
* [Die Spalte NET](#the-net-column)

### Die Spalte AVL (verfügbar) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von </strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt </td> 
   <td> <p>Die Gesamtdauer der Stunden, FTEs oder Kosten, für die alle Benutzer des Projekts während des ausgewählten Zeitraums gemäß ihrem Zeitplan zur Verfügung stehen. </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Gesamtdauer der Stunden, VZÄ oder Kosten, für die alle mit dieser Rolle verbundenen Benutzer gemäß ihrem Zeitplan und ihrem <strong>Prozentsatz der VZÄ-Verfügbarkeit</strong> für diese spezifische Rolle für den ausgewählten Zeitraum arbeiten können. </p> <p>Beachten Sie Folgendes: </p> 
    <ul> 
     <li>Wenn kein Benutzer mit einer Auftragsrolle verknüpft ist, ist der Wert für die "Verfügbare Stunden"für die Auftragsrolle null. </li> 
     <li>Wenn ein Benutzer mit einer Primären Auftragsrolle verknüpft ist, der <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für die Rolle jedoch 0 % beträgt, ist der Wert für die Auftragsrolle Verfügbare Stunden null.</li> 
     <li>Wenn der Benutzer mit anderen Rollen verknüpft ist und der <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für die Rollen 0 % beträgt, werden die anderen Rollen nicht im Ressourcenplaner aufgeführt und der Benutzer wird nur unter seiner Primären Rolle angezeigt.</li> 
    </ul> <p>Weitere Informationen zum <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für eine Auftragsrolle finden Sie im Artikel <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a> .</p> <p>Weitere Informationen dazu, wie die Verfügbarkeit der Auftragsrollen im Ressourcenplaner berechnet wird, finden Sie im Abschnitt "Berechnen der verfügbaren Stunden und der FTE für eine Stellenrolle im Ressourcenplaner"im Artikel <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnungsstunden und die FTE für Benutzer und Rollen im Ressourcenplaner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Stunden, FTEs oder Kosten, die der Benutzer für den ausgewählten Zeitraum gemäß seinem Zeitplan zur Verfügung hat. Diese Zahl subtrahiert die Stunden, die mit den folgenden Stunden verbunden sind:</p> 
    <ul> 
     <li>Zeitplanausnahmen</li> 
     <li>Zeitlimit des Benutzers</li> 
     <li>für andere Projekte veranschlagte Stunden. </li> 
    </ul> <p>Die verfügbaren Stunden, FTEs oder Kosten für eine Benutzeränderung gemäß den folgenden Kriterien: </p> 
    <ul> 
     <li>die Berechnung des Zeitplans und der FTE anhand der Voreinstellungen für die Ressourcenverwaltung auf Systemebene.<br><p>Weitere Informationen zur Berechnung der Verfügbarkeit von Benutzer- und Stellenwerten finden Sie im Artikel <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und FTE für Benutzer und Rollen im Resource Planer</a>.</p>
     Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung in Workfront finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a></li> 
    </ul> 
    <ul> 
     <li>die <strong>Priorität für die Projektplanung</strong>, wenn der Benutzer für die Arbeit in den Haushaltsplan eingestellt ist.<br>Weitere Informationen dazu, wie sich die Priorität der Projektplanung auf die verfügbaren Stunden eines Benutzers auswirkt, finden Sie unter <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Navigationsübersicht für den Ressourcenplaner </a>. </li> 
    </ul> <p>Wenn der Benutzer für die Deaktivierung eingeplant ist, sind die verfügbaren Stunden, FTEs oder Kosten für die Tage nach dem Deaktivierungsdatum null. <br>Weitere Informationen zum Deaktivieren von Benutzern finden Sie im Artikel <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Die Spalte PLN (Geplant) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von </strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Die Gesamtsumme der geplanten Stunden, FTEs oder Kosten aus allen Auftrags- oder Benutzerrollen, die unter dem Projekt aufgeführt sind, einschließlich in den Abschnitten <strong>Keine Rolle</strong> oder <strong>Kein Benutzer</strong> , für den ausgewählten Zeitraum und wie auf der Registerkarte Projektdetails des Projekts angezeigt. </p> <p><b>NOTIZ</b>

Durch manuelle Anpassungen der täglichen Benutzerzuweisungen kann der Wert für wöchentliche, monatliche oder vierteljährliche geplante Stunden im Ressourcenplaner geändert werden. Sie können die täglichen Benutzerzuweisungen für Aufgaben und Probleme mithilfe des Workload Balancer manuell anpassen. Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Arbeitslade-Balancer</a>.</p> </td>
</tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Gesamtanzahl der geplanten Stunden aus allen Aufgaben, die der Rolle zugewiesen sind, im ausgewählten Zeitraum. </p> <p>Im Abschnitt <strong>Keine Rolle</strong> werden die geplanten Stunden angezeigt, die Aufgaben zugeordnet sind, die entweder nicht zugewiesen, Teams zugewiesen (deren Stunden im Abschnitt <strong>Kein Benutzer</strong> aufgelistet sind) oder Benutzern zugewiesen sind, die keiner Auftragsrolle zugeordnet sind. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Die geplanten Stunden aus allen Aufgaben, die dem Benutzer während des ausgewählten Zeitraums in einer bestimmten Rolle zugewiesen wurden. </p> <p>Im Abschnitt <strong>Kein Benutzer</strong> werden die geplanten Stunden angezeigt, die Aufgaben zugeordnet sind, die Teams nicht zugewiesen oder zugewiesen sind. </p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie bei der Anzeige der geplanten Stunden Folgendes:

* Obwohl Sie im Ressourcenplaner keine Informationen über Aufgabenzuweisungen in der Projekt- und Rollenansicht sehen können, stammt die geplante Zeitdauer aus den geplanten Stunden für die Aufgaben in den Projekten.
* Die geplanten Stunden werden innerhalb der Dauer der Aufgaben für jede ihnen zugewiesene Ressource gleichmäßig auf jeden Tag verteilt. Die Aufgabendauer basiert auf der Aufgabe Geplante Start- und Abschlussdaten und umfasst jeden Kalendertag innerhalb dieses Zeitraums.\
  Workfront berücksichtigt den Zeitplan des Benutzers oder des Projekts bei der Verteilung von geplanten Stunden an Benutzer oder Projekte. In diesem Fall werden geplante Stunden innerhalb der Dauer von Aufgaben (außer Wochenenden, Verweiltagen und Planausnahmen) gleichmäßig auf jeden Tag verteilt.\
  Wenn Sie beispielsweise den Ressourcenplaner nach Woche anzeigen und Aufgaben mit mehreren Wochen Projektdauer haben, hängt die Anzahl der geplanten Stunden pro Woche davon ab, wie viele Tage innerhalb dieser Woche Teil der Aufgabendauer sind. Dies funktioniert auf ähnliche Weise, wenn der Ressourcenplaner nach Monat oder Quartal angezeigt wird und Aufgaben mehrere Monate oder Quartale umfassen.\
  Wochenendtage, zeitgesteuerte Ausnahmen und Verfallstage sind von dieser Verteilung ausgeschlossen.
* Die folgenden Aufgabenkategorien werden bei der Berechnung der geplanten Stunden für jede Ressource berücksichtigt:

   * Aufgaben, die Benutzern in Ressourcenpools, Jobrollen oder Teams im Projekt zugewiesen wurden\
     Wenn Teams Aufgaben zugewiesen sind, wird ihre Zuordnung unter den Abschnitten **Keine Rolle** und **Kein Benutzer** angezeigt. Sie können die mit Teams verknüpften geplanten Stunden sehen, aber Sie können die Stunden nicht einplanen, da weder Rollen noch Benutzer mit den Aufgaben verbunden sind.

   * nicht zugewiesene Aufgaben

* Geplante Stunden im Ressourcenplaner enthalten keine geplanten Stunden, die mit den folgenden Punkten verknüpft sind:

   * Übergeordnete Aufgaben
   * Aufgaben, die Benutzern ohne Ressourcen-Pools zugewiesen wurden
   * Probleme, wenn die Einstellung **Stunden aus Problemen einschließen** deaktiviert ist.

* Geplante Stunden werden nicht im Ressourcenplaner angezeigt, wenn die Aufgabendauer null ist.
* Für deaktivierte Benutzer zugeordnete geplante Stunden werden nicht angezeigt.

### Spalte BDG (Budgetierung) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von </strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden, FTE oder Kosten Sie für ein Projekt in einem ausgewählten Zeitraum einplanen. </p> <p>In der Projektansicht werden die Stunden, die Sie für das Projekt einplanen, an die im Projekt aufgelisteten Jobrollen verteilt. Die Anzahl der geplanten Stunden für jede Rolle bestimmt, wie die geplanten Stunden auf die Rollen verteilt werden. Die budgetierten Stunden werden an die Rollen mit höheren Werten für geplante Stunden verteilt. </p> <p>In der Rollenansicht werden die Stunden, die Sie für das Projekt einplanen, nicht an die Rollen oder die Benutzer im Projekt verteilt. </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden Sie für eine Rolle in einem ausgewählten Zeitraum einplanen. </p> <p>Wenn kein Benutzer mit der Stellenrolle verknüpft ist, können Sie die budgetierten Stunden für die Stellenrolle nicht schätzen. </p> <p>In der Rollenansicht werden die Stunden, die Sie für die Rolle einplanen, an die Projekte verteilt, die unter der Rolle aufgeführt sind. Die geplante Stundenzahl für jedes Projekt bestimmt, wie die Budgetzeit auf die Projekte verteilt wird. Die budgetierten Stunden werden an Projekte mit höheren Werten für geplante Stunden verteilt.</p> <p>In der Projektansicht werden die Stunden, die Sie für die Rolle einplanen, nicht an die Projekte oder die mit der Rolle verknüpften Benutzer verteilt. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden Sie für einen Benutzer in einem ausgewählten Zeitraum einplanen. </p> <p> <p><b>NOTE</b>   Sie können die budgetierten Stunden für Benutzer schätzen, die keinen Aufgaben zugewiesen, aber mit einem Ressourcen-Pool für ein Projekt verknüpft sind, da diese Benutzer auch im Ressourcenplaner angezeigt werden. Ihre geplanten Stunden sollten jedoch null sein, wenn sie nicht Aufgaben zugewiesen sind. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie beim Arbeiten mit Budgetzeit Folgendes:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Sie können Ressourcen nur mit Berechtigungen zum Bearbeiten des Zugriffs auf Ressourcen-Management und Finanzdaten sowie zum Verwalten von Finanzberechtigungen für die Projekte budget.

  Weitere Informationen zum Zugriff für Budgetierungsressourcen finden Sie im Artikel [Für Budgetressourcen in Adobe Workfront benötigter Zugriff](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Standardmäßig sind die im Ressourcenplaner veranschlagten Stunden für alle Ressourcen und für alle Projekte null.
* Sie können die budgetierten Stunden für Benutzer und Rollen manuell schätzen oder einen der Links in den Menüs Projekt oder Auftragsrolle **Mehr** verwenden, um sie entsprechend der Anzahl der geplanten Stunden zu aktualisieren.\
  Weitere Informationen zu Projekt- und Rollenoptionen finden Sie im Abschnitt [Übersicht über Stunden, FTE und Kosten-Informationen in den Projekt- und Rollenansichten des Ressourcenplaners](#Budget) in diesem Artikel.

* Die kleinste Zeitspanne, für die Sie Stunden, FTE oder Kosten einplanen können, ist eine Woche. Sie können keine Stunden, FTE oder Kosten für einen Tag einplanen.
* Budgetierte Stunden werden für jede ihnen zugewiesene Ressource gleichmäßig auf jeden Tag innerhalb der Dauer der Aufgaben verteilt. Die Aufgabendauer basiert auf der Aufgabe Geplante Start- und Abschlussdaten und umfasst jeden Kalendertag innerhalb dieses Zeitraums.\
  Workfront berücksichtigt den Zeitplan des Benutzers oder des Projekts bei der Verteilung der Budgetzeit an Benutzer oder Projekte. In diesem Fall werden die budgetierten Stunden innerhalb der Dauer der Aufgaben (außer Wochenenden) gleichmäßig auf jeden Tag verteilt, wobei Ausnahmen und Zeitpläne ausgeschlossen sind.\
  Wenn Sie beispielsweise den Ressourcenplaner nach Woche anzeigen und Aufgaben mit mehreren Wochen ausführen, hängt die Anzahl der pro Woche geplanten Stunden davon ab, wie viele Tage in dieser Woche Teil der Aufgabendauer sind. Wochenendtage sind von dieser Verteilung ausgeschlossen. Dies funktioniert auf ähnliche Weise, wenn der Ressourcenplaner nach Monat oder Quartal angezeigt wird und Aufgaben mehrere Monate oder Quartale umfassen.

* Sie können einen Bericht über die budgetierten Stunden erstellen, indem Sie die budgetierte Stunde als Berichtsobjekt für einen neuen Bericht auswählen.\
  Informationen dazu, über welche Objekte Sie in Workfront Berichte erstellen können, finden Sie im Abschnitt &quot;Berichte zu Objekten&quot;im Artikel [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Informationen zum Erstellen eines Budgeting-Stunden-Berichts finden Sie im Artikel [Bericht: Budgetierte Stunde](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Stunden, die zuvor für Benutzer, die später deaktiviert wurden, budgetiert wurden, werden nicht angezeigt.

### Die Spalte VAR (Varianz) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von </strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Die Stunden-, FTE- oder Kostenvarianz zeigt an, ob Sie über genügend geplante Stunden verfügen, um alle geplanten Stunden für das Projekt zu erreichen. </p> <p>Die Projektstunde, die FTE oder die Kostenabweichung werden anhand der folgenden Formel berechnet:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Stunden-, FTE- oder Kostenvarianz zeigt an, ob Sie über ausreichend geplante Stunden, FTE oder Kosten verfügen, um die ihr zugewiesene geplante Stunde zu erreichen. </p> <p>Die Berechnung der Role Hour, FTE oder Cost Variation erfolgt anhand der folgenden Formel:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Die Stunden-, FTE- oder Kostenvarianz zeigt an, ob Sie über genügend geplante Stunden verfügen, damit der Benutzer die ihnen zugewiesenen geplanten Stunden ausführen kann. </p> <p>Die User Hours, FTE oder Cost Variation werden anhand der folgenden Formel berechnet:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn die Stunden-, FTE- oder Kostenvarianz in Rot angezeigt werden, haben Sie geschätzte weniger budgetierte Stunden als die geplanten Stunden der tatsächlichen Arbeit, die abgeschlossen werden muss. In diesem Fall reichen die budgetierten Stunden möglicherweise nicht aus, um die Arbeit abzuschließen.

### Die Spalte NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von </strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> 
    <div> 
     <p>Im Projekt "Nettozeiten", "VZÄ"oder "Kosten"kann Folgendes angezeigt werden: </p> 
     <ul> 
      <li> <p>Differenz zwischen der Verfügbaren Zeit oder den Kosten und der für das Projekt veranschlagten Zeit oder Kosten:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Die Differenz zwischen der Verfügbaren Zeit oder den Kosten und der geplanten Zeit oder Kosten für das Projekt, wenn die Einstellung Planete Nutzung (PLN) in NET-Berechnungen aktiviert ist: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>TIPP</b></p>        
  <p>Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</p>
  <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planers</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> 
    <div> 
     <p>Die Rolle "Net Hours", "FTE"oder "Cost"kann eine der folgenden Aussagen enthalten: </p> 
     <ul> 
      <li> <p>Differenz zwischen der verfügbaren Zeit oder den Kosten und der für die Rolle zugewiesenen budgetierten Zeit oder Kosten:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Die Differenz zwischen der Verfügbaren Zeit oder den Kosten und der geplanten Zeit oder Kosten für die Rolle, wenn die Einstellung Planete Verwendung (PLN) in NET-Berechnungen aktiviert ist:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPP</b> <span>

Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</span> </p> <p><span>Weitere Informationen finden Sie unter </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planers</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> 
    <div> 
     <p>Der Benutzer "Net Hours", "FTE"oder "Cost"kann Folgendes anzeigen: </p> 
     <ul> 
      <li> <p>Die Differenz zwischen der Verfügbaren Zeit oder den Kosten und der für den Benutzer vorgesehenen budgetierten Zeit oder Kosten:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Die Differenz zwischen der Verfügbaren Zeit oder den Kosten und der für den Benutzer geplanten Zeit oder Kosten, wenn die Einstellung Planete Nutzung (PLN) in NET-Berechnungen aktiviert ist:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPP</b> <span>

Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</span> </p> <p><span>Weitere Informationen finden Sie unter </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Überprüfen der Ressourcenverfügbarkeit und -zuordnung mithilfe des Adobe Workfront Resource Planers</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Wenn die NET Hours, FTE oder Kosten rot angezeigt werden, ist nicht genügend Zeit oder Budget verfügbar, um entweder den Budgetierten** oder die geplante Zeit oder Kosten im Zusammenhang mit der Arbeit abzudecken. In diesem Fall werden die Ressourcen überverteilt.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
