---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Übersicht über Stunden-, FTE- und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners
description: Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: c9e77e11fafbf224639289977783e95ccb45a9e2
workflow-type: tm+mt
source-wordcount: '3086'
ht-degree: 0%

---

# Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Die Budgetierung Ihrer Ressourcen für die Arbeit, die sie an einem Projekt ausführen müssen, ist die Hauptfunktion des Ressourcenplaners. Sie können die verfügbare Zeit Ihrer Ressourcen anzeigen und ihre Zeit den Projekten zuweisen, denen sie zugewiesen sind.

Weitere Informationen zur Budgetierung von Ressourcen im Ressourcenplaner finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Aufgabenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

In diesem Artikel werden einige der wichtigsten Konzepte beschrieben, die Sie kennen sollten, bevor Sie mit der Budgetierung Ihrer Ressourcen im Ressourcenplaner beginnen.

## Übersicht über Budgetierungsressourcen

Beachten Sie bei der Budgetierung von Ressourcen mit dem Ressourcenplaner Folgendes:

* Sie können die Zuordnung Ihrer Ressourcen budgetieren, indem Sie einen Betrag an Stunden, FTE oder Kosten angeben, den Ihre Ressourcen für die Bearbeitung von Projekten verwenden können. Wenn Sie Zeit oder Kosten für eine Ressource budgetieren, verringern sich die verfügbaren Stunden, FTE oder Kosten für die Ressource um den budgetierten Betrag. Infolgedessen verringern sich die verfügbaren Stunden, FTE oder Kostenbeträge für die Projekte, die dem Projekt folgen, für das Sie eine Budgetierung erstellen, für diese Benutzer und Funktionen in diesen Projekten.

  >[!IMPORTANT]
  >
  >Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren budgetieren. Wenn Sie Ressourcen für ein Projekt mit einer Laufzeit von mehr als 15 Jahren budgetieren, sind die Budgetierungsinformationen möglicherweise nicht korrekt.

* Sie können Stunden, FTE oder Kosten für Ihre Ressourcen für jeden Zeitrahmen budgetieren, der im Ressourcenplaner angezeigt wird, unabhängig von der Zeitleiste des Projekts. Wenn Sie beispielsweise angeben möchten, dass Ihre Ressourcen möglicherweise nicht während der Zeitleiste des Projekts verfügbar sind (wo sie mit den geplanten Stunden verknüpft sind), aber möglicherweise während einer anderen Zeit verfügbar sind, können Sie dies tun, indem Sie sie für Zeitrahmen budgetieren, in denen die geplanten Stunden null sind, wenn diese für die Arbeit verfügbar werden. Anschließend können Sie die Zeitleiste des Projekts manuell ändern, um sie an die Verfügbarkeit Ihrer Ressourcen anzupassen.

  >[!NOTE]
  >
  >Es wird empfohlen, zuerst die Stunden, VZÄ oder Kosten für Aufgabengebiete oder für Benutzer manuell zu budgetieren. Sie können die automatischen Optionen verwenden, um die Zeit für Ihre Projekte und Ressourcen nur dann zu budgetieren, wenn Sie sicher sind, dass der Betrag der geplanten Stunden, VZÄ oder Kosten immer mit Ihren budgetierten Stunden, VZÄ oder Kosten übereinstimmen sollte.\
  >Informationen zur Verwendung der automatischen Optionen für die Budgetierung im Ressourcenplaner finden Sie im Abschnitt „Projekt und Aufgabengebiete automatisch budgetieren“ im Artikel [Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner ](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* Die Budgetierung von FTE oder Kosten ist identisch mit der Budgetierung von Stunden, bei der Adobe Workfront die FTE- und Kostenwerte anstelle von Stunden für die Ressourcen verwendet, die Sie budgetieren.

  Weitere Informationen zur Kostenberechnung im Ressourcenplaner finden Sie unter [Kosten im Ressourcenplaner berechnen](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Die Budgetierung von Zuweisungen für Ihre Ressourcen im Ressourcenplaner erfolgt wie folgt:

   * Manuell

     Oder

   * Automatisch durch Verwendung der Projekt- und Rollenoptionen in den Ansichten **Nach Projekt anzeigen** und **Nach Rolle anzeigen**.

  Weitere Informationen finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Wenn ein(e) Benutzende(r) Aufgabengebiete wechselt, gelöscht, deaktiviert oder aus einem Ressourcenpool entfernt wird, ändern sich die für die Rolle budgetierten Stunden nicht und werden an die verbleibenden Benutzenden in der Rolle verteilt. Wenn dem Aufgabengebiet kein Benutzer mehr zugeordnet ist, werden die budgetierten Stunden für das Aufgabengebiet null.

Weitere Informationen zu den Projekt- und Rollenoptionen finden Sie im Abschnitt [Werte für Stunden, FTE und Kosten im Ressourcenplaner](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) in diesem Artikel.

## Werte von Stunden, FTE und Kosten im Ressourcenplaner verstehen {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Bevor Sie Ressourcen budgetieren und die Informationen zu budgetierten Stunden im Ressourcenplaner aktualisieren, müssen Sie mit den folgenden Konzepten vertraut sein

* **Geplante Stunden, FTE oder Kosten**: Die Arbeit, die gemäß der Definition für Aufgaben und Probleme ausgeführt werden muss.
* **Verfügbare Stunden, FTE oder Kosten**: Der Zeitraum, über den Benutzer oder Aufgabengebiete für die Arbeit verfügbar sind, gemäß den Zeitplänen, die mit den Benutzern verknüpft sind.

Diese Informationen werden im Ressourcenplaner für jede Ressource (Benutzer oder Rolle) und für jedes Projekt angezeigt.

Informationen dazu, was in der Projekt- und Rollenansicht des Projekts angezeigt wird, finden Sie im Artikel [Ressourcenplaner - Navigationsübersicht](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Informationen zum Verständnis der Kostenberechnung im Ressourcenplaner finden Sie im Artikel [Kosten im Ressourcenplaner berechnen](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Die Budgetierung nach Kosten entspricht der Budgetierung nach Stunden oder FTE, aber Sie müssen verstehen, wie Workfront die Kosten für den Ressourcenplaner berechnet.
>
>Informationen zur Kostenberechnung im Ressourcenplaner finden Sie im Artikel [Kosten im Ressourcenplaner berechnen](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

In den folgenden Tabellen werden die Informationen zur Zuordnung und Verfügbarkeit angezeigt, die im Ressourcenplaner angezeigt werden, wenn entweder die Projekt- oder die Rollenansicht angewendet wird. Sie können diese Informationen nach Stunden, FTE oder Kosten anzeigen:

* [Die Spalte AVL (verfügbar)](#the-avl-available-column)
* [Die Spalte „GPL (Geplant)](#the-pln-planned-column)
* [Die Spalte BDG (Budgetiert)](#the-bdg-budgeted-column)
* [Die Spalte VAR (Varianz)](#the-var-variance-column)
* [Die Spalte NET](#the-net-column)

### Die Spalte AVL (verfügbar) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt </td> 
   <td> <p>Die Gesamtzahl der Stunden, FTEs oder Kosten, für die alle Benutzenden des Projekts gemäß ihrem Zeitplan für den ausgewählten Zeitrahmen arbeiten können. </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Gesamtzahl der Stunden, FTEs oder Kosten, für die alle mit dieser Funktion verknüpften Benutzer gemäß ihrem Zeitplan arbeiten können, und ihr <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für diese spezifische Funktion, für den ausgewählten Zeitrahmen. </p> <p>Beachten Sie Folgendes: </p> 
    <ul> 
     <li>Wenn kein Benutzer einem Aufgabengebiet zugeordnet ist, dann ist der Wert für Verfügbare Stunden für das Aufgabengebiet Null. </li> 
     <li>Wenn ein(e) Benutzende(r) einem Primären Aufgabengebiet zugeordnet ist, der <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für das Aufgabengebiet jedoch 0 % beträgt, ist der Wert für Verfügbare Stunden für das Aufgabengebiet null.</li> 
     <li>Wenn der/die Benutzende mit „Andere Funktionen“ verknüpft ist und der <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für die Rollen 0 % beträgt, werden die „Andere Funktionen“ nicht im Ressourcenplaner aufgeführt und der/die Benutzende wird nur unter der Primären Rolle angezeigt.</li> 
    </ul> <p>Weitere Informationen zum <strong>Prozentsatz der FTE-Verfügbarkeit</strong> für ein Aufgabengebiet finden Sie im Artikel <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</p> <p>Weitere Informationen zur Berechnung der Verfügbarkeit des Aufgabengebiets im Ressourcenplaner finden Sie im Abschnitt „Berechnen der verfügbaren Stunden und VZÄ für ein Aufgabengebiet im Ressourcenplaner“ im Artikel <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Stunden, FTEs oder Kosten, die der/die Benutzende gemäß seinem/ihrem Zeitplan für den ausgewählten Zeitrahmen arbeiten kann. Diese Zahl subtrahiert die Stunden, die mit Folgendem verbunden sind:</p> 
    <ul> 
     <li>Zeitplanausnahmen</li> 
     <li>Ausfallzeit des Benutzers</li> 
     <li>Für andere Projekte budgetierte Stunden. </li> 
    </ul> <p>Die verfügbaren Stunden, FTEs oder Kosten für einen Benutzer ändern sich wie folgt: </p> 
    <ul> 
     <li>wie ihr Zeitplan und VZÄ basierend auf den Voreinstellungen für das Ressourcenmanagement auf Systemebene berechnet werden.<br><p>Weitere Informationen zur Berechnung der Verfügbarkeit von Benutzern und Aufgabengebieten finden Sie im Artikel <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner</a>.</p>
     Weitere Informationen zum Konfigurieren der Voreinstellungen für das Ressourcenmanagement in Workfront finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für das Ressourcenmanagement konfigurieren</a></li> 
    </ul> 
    <ul> 
     <li>die <strong>Projektplanungspriorität</strong>, wenn der Benutzer für Arbeit budgetiert ist.<br>Weitere Informationen darüber, wie sich die Projektplanungspriorität auf die verfügbaren Stunden eines Benutzers auswirkt, finden Sie unter <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Übersicht über die Ressourcenplaner-Navigation </a>. </li> 
    </ul> <p>Wenn für die Benutzerin oder den Benutzer die Deaktivierung geplant ist, sind die verfügbaren Stunden, FTEs oder Kosten für die Tage nach dem Deaktivierungsdatum null. <br>Weitere Informationen zur Deaktivierung von Benutzern finden Sie im Artikel <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren von Benutzern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Die Spalte „GEPLANT“ {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Die Summe der geplanten Stunden, FTEs oder Kosten aus allen Aufgabengebieten oder Benutzern, die unter dem Projekt aufgelistet sind, einschließlich der Abschnitte <strong>Keine Funktion</strong> oder <strong>Kein Benutzer</strong> für den ausgewählten Zeitrahmen, und wie auf der Registerkarte Projektdetails angezeigt. </p> <p><b>NOTIZ</b>

Durch manuelle Anpassungen der täglichen Benutzerzuteilungen kann sich der Wert für die geplante wöchentliche, monatliche oder vierteljährliche Stunde im Ressourcenplaner ändern. Mit dem Workload-Balancer können Sie die tägliche Benutzerzuweisung für Aufgaben und Probleme manuell anpassen. Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload-Balancer</a>.</p> </td>
</tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Summe der geplanten Stunden aus allen Aufgaben, die der Funktion zugewiesen wurden, im ausgewählten Zeitrahmen. </p> <p>Im Abschnitt <strong>Keine </strong>" werden die geplanten Stunden angezeigt, die mit Aufgaben verknüpft sind, die entweder nicht zugewiesen oder Teams zugewiesen sind (deren Stunden im Abschnitt <strong>Kein Benutzer</strong> aufgelistet sind) oder Benutzern zugewiesen wurden, die keinem Aufgabengebiet zugeordnet sind. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Die geplanten Stunden aus allen Aufgaben, die dem Benutzer in einer bestimmten Rolle während des ausgewählten Zeitraums zugewiesen wurden. </p> <p>Im Abschnitt <strong>Kein Benutzer</strong> werden die geplanten Stunden angezeigt, die mit Aufgaben verknüpft sind, die entweder nicht zugewiesen oder Teams zugewiesen sind. </p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie beim Anzeigen der geplanten Stunden Folgendes:

* Obwohl Sie im Ressourcenplaner in den Projekt- und Rollenansichten keine Informationen zur Aufgabenzuordnung sehen können, stammt die Anzahl der geplanten Stunden aus den geplanten Stunden für die Vorgänge in den Projekten.
* Geplante Stunden werden innerhalb der Aufgabendauer für jede ihnen zugewiesene Ressource zu gleichen Teilen auf jeden Tag verteilt. Die Aufgabendauer basiert auf den geplanten Start- und Abschlussdaten der Aufgabe und umfasst jeden Kalendertag innerhalb dieses Zeitraums.\
  Workfront berücksichtigt den Zeitplan des Benutzers oder Projekts beim Verteilen der geplanten Stunden an Benutzer oder Projekte. In diesem Fall werden die geplanten Stunden innerhalb der Aufgabendauer gleichmäßig auf jeden Tag verteilt, mit Ausnahme von Wochenenden, Urlaubstagen und Zeitplanausnahmen.\
  Wenn Sie beispielsweise den Ressourcenplaner nach Woche anzeigen und Vorgänge haben, die sich über mehrere Wochen in Projekten erstrecken, hängt die Anzahl der geplanten Stunden pro Woche davon ab, wie viele Tage innerhalb dieser Woche Teil der Vorgangsdauer sind. Dies funktioniert ähnlich, wenn der Ressourcenplaner nach Monat oder Quartal angezeigt wird und wenn Vorgänge mehrere Monate oder Quartale umfassen.\
  Wochenendtage, Zeitplanausnahmen und Urlaubstage sind von dieser Verteilung ausgeschlossen.
* Die folgenden Aufgabenkategorien sind in der Berechnung der geplanten Stunden für jede Ressource enthalten:

   * Aufgaben, die Benutzern in Ressourcenpools, Aufgabengebieten oder Teams im Projekt zugewiesen sind\
     Wenn Teams Aufgaben zugewiesen werden, wird ihre Zuordnung in den Abschnitten **Keine**&quot; und **Kein Benutzer** angezeigt. Sie können die geplanten Stunden sehen, die mit Teams verknüpft sind, Sie können die Stunden jedoch nicht budgetieren, da den Aufgaben weder Rollen noch Benutzer zugeordnet sind.

   * Nicht zugewiesene Aufgaben

* Geplante Stunden im Ressourcenplaner enthalten keine geplanten Stunden, die mit Folgendem verknüpft sind:

   * Übergeordnete Aufgaben
   * Aufgaben, die Benutzern ohne Ressourcenpools zugewiesen sind
   * Probleme, wenn die Einstellung **Stunden aus Problemen einbeziehen** deaktiviert ist.

* Geplante Stunden werden nicht im Ressourcenplaner angezeigt, wenn die Aufgabendauer null ist.
* Mit deaktivierten Benutzern verknüpfte geplante Stunden werden nicht angezeigt.

### Die Spalte BDG (Budgetiert) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden, VZÄ oder Kosten Sie für ein Projekt für einen ausgewählten Zeitrahmen budgetieren. </p> <p>In der Projektansicht werden die Stunden, die Sie für das Projekt budgetieren, an die unter dem Projekt aufgelisteten Aufgabengebiete verteilt. Die Anzahl der geplanten Stunden für jede Funktion bestimmt, wie die budgetierten Stunden auf die Funktionen verteilt werden. Die budgetierten Stunden werden an die Funktionen mit höheren Werten für „Geplante Stunden“ verteilt. </p> <p>In der Rollenansicht werden die Stunden, die Sie für das Projekt budgetieren, nicht auf die Rollen oder die Benutzer im Projekt verteilt. </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden Sie für eine Funktion für einen ausgewählten Zeitraum budgetieren. </p> <p>Wenn dem Aufgabengebiet kein Benutzer zugeordnet ist, können Sie die budgetierten Stunden für das Aufgabengebiet nicht schätzen. </p> <p>In der Rollenansicht werden die Stunden, die Sie für die Rolle budgetieren, an die Projekte verteilt, die unter der Rolle aufgeführt sind. Die Anzahl der geplanten Stunden für jedes Projekt bestimmt, wie die budgetierten Stunden auf die Projekte verteilt werden. Die budgetierten Stunden werden an die Projekte mit höheren Werten für „Geplante Stunden“ verteilt.</p> <p>In der Projektansicht werden die Stunden, die Sie für die Rolle budgetieren, nicht an die Projekte oder die mit der Rolle verbundenen Benutzer verteilt. </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Ein manueller Eintrag, um zu schätzen, wie viele Stunden Sie für einen Benutzer für einen ausgewählten Zeitraum budgetieren. </p> <p> <p><b>HINWEIS</b>   Sie können die budgetierten Stunden für Benutzer schätzen, die keinen Vorgängen zugeordnet sind, aber mit einem Ressourcenpool in einem Projekt verknüpft sind, da diese Benutzer auch im Ressourcenplaner angezeigt werden. Ihre geplanten Stunden sollten jedoch null sein, wenn sie keinen Aufgaben zugewiesen sind. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie beim Arbeiten mit budgetierten Stunden Folgendes:

* Ressourcen können nur budgetiert werden, wenn Sie Bearbeitungszugriff auf Ressourcen-Management- und Finanzdaten sowie Finanzverwaltungsberechtigungen für die Projekte haben.

  Informationen zum Zugriff, der für die Budgetierung von Ressourcen erforderlich ist, finden Sie im Artikel [Zugriff auf die Budgetierung von Ressourcen in Adobe Workfront erforderlich](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Standardmäßig sind die budgetierten Stunden im Ressourcenplaner für alle Ressourcen und Projekte gleich null.
* Sie können die budgetierten Stunden für Benutzer und Funktionen manuell schätzen oder einen der Links in den Menüs Projekt oder Aufgabengebiet **Mehr** verwenden, um sie entsprechend der Anzahl der geplanten Stunden zu aktualisieren.\
  Weitere Informationen zu Projekt- und Rollenoptionen finden Sie im Abschnitt [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des ](#Budget) in diesem Artikel.

* Der kleinste Zeitraum, für den Sie Stunden, FTE oder Kosten budgetieren können, ist eine Woche. Sie können keine Stunden, FTE oder Kosten für einen Tag budgetieren.
* Budgetierte Stunden werden für jede Ressource, die ihnen zugewiesen ist, innerhalb der Aufgabendauer gleichmäßig auf jeden Tag verteilt. Die Aufgabendauer basiert auf den geplanten Start- und Abschlussdaten der Aufgabe und umfasst jeden Kalendertag innerhalb dieses Zeitraums.

  Workfront berücksichtigt den Zeitplan des Benutzers oder Projekts bei der Verteilung budgetierter Stunden auf Benutzer oder Projekte. In diesem Fall werden die budgetierten Stunden innerhalb der Aufgabendauer gleichmäßig auf jeden Tag verteilt, mit Ausnahme von Wochenenden, aber einschließlich Urlaub und Zeitplanausnahmen.

  Wenn Sie beispielsweise den Ressourcenplaner nach Woche anzeigen und Vorgänge haben, die sich über mehrere Wochen erstrecken, hängt die Anzahl der budgetierten Stunden pro Woche davon ab, wie viele Tage innerhalb dieser Woche Teil der Vorgangsdauer sind. Wochenendtage sind von dieser Verteilung ausgeschlossen. Dies funktioniert ähnlich, wenn der Ressourcenplaner nach Monat oder Quartal angezeigt wird und wenn Vorgänge mehrere Monate oder Quartale umfassen.

* Sie können einen Bericht zu budgetierten Stunden erstellen, indem Sie Budgetierte Stunde als Berichtobjekt für einen neuen Bericht auswählen.

  Informationen dazu, über welche Objekte Sie in Workfront Berichte erstellen können, finden Sie im Abschnitt „Berichte zu Objekten“ im Artikel &quot;[ von Objekten in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Informationen zum Erstellen eines Berichts zur budgetierten Stunde finden Sie im Artikel [Bericht: Budgetierte Stunde](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Stunden, die zuvor für Benutzer budgetiert waren, die später deaktiviert wurden, werden nicht angezeigt.

  Beachten Sie, dass die budgetierten Lohnkosten eines Projekts weiterhin die budgetierten Stunden für Benutzer enthalten, die im Ressourcenplaner deaktiviert wurden.

  Beispiel: Wenn eine Funktion zwei Benutzern zugewiesen wird und budgetierte Stunden hinzugefügt werden (20 Stunden pro Benutzer, insgesamt 40 Stunden) und dann die Gesamtsumme manuell für die Rolle festgelegt wird, führt die Deaktivierung eines Benutzers im Ressourcenplaner dazu, dass seine Stunden nicht mehr in der Berechnung berücksichtigt werden (wodurch die Gesamtsumme auf 20 Stunden fällt). Bei der Projektbudgetierung wird jedoch der manuell festgelegte Gesamtwert für die Rolle korrekt beibehalten, sodass die Stunden der deaktivierten Person weiterhin in der Berechnung enthalten sind (verbleiben bei 40 Stunden).

### Die Spalte VAR (Varianz) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> <p>Die Stunden-, VZÄ- oder Kostenabweichung gibt an, ob Sie über genügend budgetierte Stunden für das Projekt verfügen, um alle geplanten Stunden für das Projekt auszuführen. </p> <p>Die Projektstunde, der FTE oder die Kostenabweichung wird anhand der folgenden Formel berechnet:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> <p>Die Stunden-, VZÄ- oder Kostenabweichung gibt an, ob Sie über genügend budgetierte Stunden, VZÄ oder Kosten für die Funktion verfügen, um die ihr zugewiesenen geplanten Stunden auszuführen. </p> <p>Die Funktionsstunde, VZÄ oder Kostenabweichung wird anhand der folgenden Formel berechnet:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Die Stunden-, VZÄ- oder Kostenabweichung gibt an, ob Sie über genügend budgetierte Stunden verfügen, damit der Benutzer die ihm zugewiesenen geplanten Stunden ausführen kann. </p> <p>Die Benutzerstunden, VZÄ oder Kostenabweichungen werden anhand der folgenden Formel berechnet:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn die Stunden-, FTE- oder Kostenabweichung rot angezeigt wird, haben Sie weniger budgetierte Stunden als die geplanten Stunden der tatsächlichen Arbeit, die abgeschlossen werden muss, geschätzt. In diesem Fall reichen die budgetierten Stunden möglicherweise nicht aus, um die Arbeit abzuschließen.

### Die Spalte NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Angezeigt von</strong> </td> 
   <td><strong>Beschreibung</strong> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td> 
    <div> 
     <p>Das Projekt kann Nettostunden, FTE oder Kosten aufweisen, die eines der folgenden Merkmale aufweisen: </p> 
     <ul> 
      <li> <p>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der budgetierten Zeit oder den Kosten für das Projekt:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der geplanten Zeit oder den geplanten Kosten für das Projekt, wenn die Einstellung Geplante Werte (PLN) in NET-Berechnungen verwenden aktiviert ist: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>TIPP</b></p>        
  <p>Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</p>
  <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner überprüfen</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Funktion</td> 
   <td> 
    <div> 
     <p>Die Funktion Nettostunden, FTE oder Kosten kann eine der folgenden Eigenschaften aufweisen: </p> 
     <ul> 
      <li> <p>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der budgetierten Zeit oder den Kosten für die Funktion:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der geplanten Zeit oder den geplanten Kosten für die Funktion, wenn die Einstellung Geplante Werte (PLN) in NET-Berechnungen verwenden aktiviert ist:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPP</b> <span>

Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</span> </p> <p><span>Weitere Informationen finden Sie unter </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner überprüfen</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td> 
    <div> 
     <p>Der Benutzer „Nettostunden“, „FTE“ oder „Kosten“ kann einen der folgenden Punkte anzeigen: </p> 
     <ul> 
      <li> <p>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der budgetierten Zeit oder den Kosten für den Benutzer:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Die Differenz zwischen der verfügbaren Zeit oder den Kosten und der geplanten Zeit oder den Kosten für den Benutzer, wenn die Einstellung Geplante Werte (PLN) in NET-Berechnungen verwenden aktiviert ist:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>TIPP</b> <span>

Diese Option wird nur angewendet, wenn Sie die Ansicht im Abschnitt Ausgewählte Elemente anzeigen anpassen.</span> </p> <p><span>Weitere Informationen finden Sie unter </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Ressourcenverfügbarkeit und -zuordnung mit dem Adobe Workfront-Ressourcenplaner überprüfen</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn die Nettostunden, VZÄ oder Kosten rot angezeigt werden, gibt es nicht genügend verfügbare Zeit oder Budget, um entweder die budgetierte oder die geplante Zeit oder die mit der Arbeit verbundenen Kosten abzudecken. In diesem Fall sind die Ressourcen überlastet.

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
