---
product-area: projects
navigation-topic: financials
title: Übersicht über das Überschreiben der Abrechnungsraten für Auftragsrollen und Berechnung des Umsatzes in einem Projekt
description: Sie können die Abrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu berechnen, wenn Sie diese mit den im Projekt verbrachten Stunden multiplizieren. Weitere Informationen zu Abrechnungsraten und Umsätzen finden Sie im Artikel Übersicht über Abrechnung und Umsatz .
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '3860'
ht-degree: 0%

---

# Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts

{{highlighted-preview}}

Sie können die Abrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu berechnen, wenn Sie diese mit den im Projekt verbrachten Stunden multiplizieren. Weitere Informationen zu Abrechnungsraten und Umsätzen finden Sie im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Übersicht über die Abrechnungsraten für Auftragsrollen und die Rolle &quot;Stündliche Umsatztypen&quot;

Als Adobe Workfront-Administrator können Sie die Abrechnungsraten sowohl Benutzern als auch Auftragsrollen zuordnen.\
Weitere Informationen zum Erstellen von Benutzern und zum Verknüpfen dieser Benutzer mit Abrechnungsraten finden Sie im Artikel [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md) . Weitere Informationen zum Erstellen von Auftrags-Rollen und deren Zuordnung zu Abrechnungsraten finden Sie im Artikel [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Mit Benutzern verknüpfte Abrechnungsraten können nicht überschrieben werden.

Abrechnungsraten, die mit Stellenrollen verknüpft sind, können auf Unternehmens- oder Projektebene überschrieben werden.

Zur Berechnung des Umsatzes aus Projekten basierend auf den Abrechnungsraten von Auftragsrollen muss der **Umsatz Typ** der Aufgaben für die Projekte einer der folgenden sein:

* Stundensatz nach Funktion
* Stundensatz nach Funktion mit Begrenzung
* Stündliche Rolle plus fest

Weitere Informationen zu **Umsatztyp** und Abrechnungsraten finden Sie unter [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hierarchie der Abrechnungsrate überschreibt bei der Berechnung des Umsatzes

Eine Auftragsrolle kann wie folgt mit einer Abrechnungsrate verbunden sein:

* Als Workfront-Administrator können Sie die Abrechnungsrate auf Systemebene definieren, die einer Auftragsrolle zugeordnet ist, wenn Sie diese Auftragsrolle erstellen.\
  Weitere Informationen zum Erstellen von Auftragsrollen finden Sie unter [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Als Workfront-Administrator können Sie bei der Erstellung eines Unternehmens die Abrechnungsrate auf Unternehmensebene für dieselbe Rolle festlegen.\
  Wenn Workfront den Umsatz für die mit diesem Unternehmen verbundenen Projekte berechnet, wird der Abrechnungskurs des Unternehmens verwendet, wenn die Rolle Aufgaben zugewiesen wird, anstatt der Abrechnungsrate auf Systemebene für diese Auftragsrolle.\
  Die auf Unternehmensebene geänderten Job-Rollenraten wirken sich auf alle mit diesem Unternehmen verbundenen Projekte aus.

  >[!NOTE]
  >
  >Wenn Sie die Abrechnungsrate des Unternehmens aktualisieren müssen, wird die Projektrate nicht automatisch aktualisiert. Sie müssen das Unternehmen aus dem Projekt entfernen, den Unternehmenssatz für das Unternehmen aktualisieren und das Unternehmen dann erneut an das Projekt anhängen, bevor der neue Unternehmenssatz auf das Projekt wirksam wird. Anweisungen zum Anhängen eines Unternehmens an ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

  Weitere Informationen zum Erstellen von unternehmensspezifischen Abrechnungsraten für Rollen finden Sie unter [Unternehmen erstellen und bearbeiten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Als Workfront-Administrator können Sie beim Bearbeiten eines Projekts eine Option aktivieren, um Änderungen an den Abrechnungsraten auf Unternehmensebene auf das Projekt anzuwenden, wenn Benutzer die Projektfinanzierung manuell neu berechnen.\
  Weitere Informationen finden Sie unter [Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Als Workfront-Administrator können Sie Ratenkarten mit mehreren Abrechnungsraten pro Rolle definieren, die auf Standort und Datum basieren. Wenn eine Preiskarte an ein Projekt angehängt wird, werden alle Rollen (nach Ort, falls Standorte verwendet werden) und die zugehörigen Abrechnungsraten zum Abschnitt mit den Abrechnungsraten des Projekts hinzugefügt. Wenn Sie eine Preiskarte anhängen, werden die bestehenden Abrechnungsraten für das Projekt überschrieben.

  Weitere Informationen finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) und [Eine Ratenkarte an ein Projekt anhängen](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Als Projektmanager können Sie die Abrechnungsrate für dieselbe Auftragsrolle auf Projektebene definieren.\
  Die auf dem Projekt geänderten Job-Rollenraten wirken sich nur auf dieses Projekt aus.

  Weitere Informationen zum Überschreiben von Rollenraten für das Projekt finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Wenn eine Auftragsrolle mit einer Abrechnungsrate auf Systemebene, Unternehmensebene und Projektebene verknüpft ist, berechnet Workfront den Umsatz der Aufgaben anhand der Abrechnungsrate der Auftragsrolle auf Projektebene, wenn die Auftragsrollenraten verwendet werden. Der Umsatz aus allen Aufgaben rechnet mit dem Umsatz des Projekts.

## Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene

Als Projektmanager können Sie festlegen, welcher Abrechnungskurs für eine Auftragsrolle in einem bestimmten Projekt gilt. Diese Abrechnungsrate auf Projektebene überschreibt die Abrechnungsrate auf Systemebene für diese Arbeitsplatzrolle. Workfront verwendet zur Berechnung des Umsatzes die Abrechnungsrate auf Projektebene der Auftragsrolle, anstatt die Abrechnungsrate auf Systemebene zu verwenden.

<span class="preview">Sie können auch eine Ratenkarte an das Projekt anhängen, die die Abrechnungsraten für die Rolle &quot;Job&quot;von der Ratenkarte in das Projekt importiert.</span>

Informationen dazu, wie Sie die Abrechnungsraten für Auftragsrollen auf Projektebene überschreiben, finden Sie unter [Überschreiben der Abrechnungsraten für Auftragsrollen auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des Umsatzes im Projekt verwendet wird, finden Sie im Abschnitt &quot;Umsatzberechnungen für Aufgaben, die auf Benutzer- und Rollenzuweisungen basieren&quot;in [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Informationen zum Anhängen einer Ratenkarte an ein Projekt finden Sie unter [Anhängen einer Ratenkarte an ein Projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Im Falle des tatsächlichen Umsatzes sollten die Abrechnungsraten, die auf Stunden angewendet werden, die zu einem Abrechnungsdatensatz hinzugefügt werden, der als Abrechnung gekennzeichnet ist, nicht durch Überschreibungen des Abrechnungskurses beeinträchtigt werden, die nach Abrechnung des Abrechnungsdatensatzes auftreten.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Übersicht über den Abschnitt &quot;Abrechnungssätze&quot;eines Projekts

Nachdem Sie die Überschreibungsraten für die mit dem Projekt verknüpften Auftragsrollen festgelegt haben, können Sie alle Auftragsrollen und deren Überschreibungen auf der Registerkarte **Abrechnungsraten** des Projekts sehen.

Beachten Sie die folgenden Informationen in der Liste der **Abrechnungsraten**:

* [Aufgabenrollengruppierung](#job-role-grouping)
* [Wert der Projektabrechnungsrate](#project-billing-rate-value)
* [Standardwert für die Abrechnungsrate](#default-billing-rate-value)
* [Wert des Abrechnungskurses des Unternehmens](#company-billing-rate-value)
* [Verschiedene Abrechnungsratenwerte und Zeitrahmen](#multiple-billing-rate-values-and-timeframes)

### Gruppierung von Auftragsrollen {#job-role-grouping}

Die Abrechnungsraten werden im Bereich **Abrechnungsraten** nach ihren jeweiligen Stellenrollen gruppiert. <span class="preview">Wenn eine Ratenkarte an das Projekt angehängt ist, werden die Auftragsrollen auch nach Ratenkarte gruppiert. Wenn Orte auf Auftragsrollen angewendet werden, wird der Standortname als Teil des Auftrags-Rollennamens einbezogen. Sie können dieselbe Auftragsrolle für mehrere Standorte aufführen.</span>

### Wert des Projektabrechnungskurses {#project-billing-rate-value}

Beachten Sie in der Gruppierungszeile, die einer Auftragsrolle entspricht, die Abrechnungsrate für diese Auftragsrolle auf Projektebene in der Spalte **Projektabrechnungsrate** . Wenn die Auftragsrolle über mehrere Überschreibungsraten verfügt, wird die Überschreibungsrate, die dem aktuellen Datum entspricht, in der Gruppierungszeile in der Spalte **Projektabrechnungsrate** angezeigt.

### Standardwert für Abrechnungsrate {#default-billing-rate-value}

Beachten Sie in der Gruppierungszeile einer Auftragsrolle die Abrechnungsrate für diese Auftragsrolle auf Systemebene in der Spalte **Standardabrechnungsrate** .

>[!NOTE]
>
>Wenn es für eine Auftragsrolle Projektabrechnungsraten gibt, wird der **Standardabrechnungssatz** nie auf die Berechnung des Umsatzes für das Projekt angewendet. Zur Berechnung des Umsatzes werden nur die **Abrechnungsraten des Projekts** angewendet.

### Wert des Unternehmensumrechnungskurses {#company-billing-rate-value}

Beachten Sie in der Gruppierungszeile einer Auftragsrolle die Abrechnungsrate für diese Arbeitsplatzrolle auf Unternehmensebene in der Spalte **Abrechnungsrate für Unternehmen** . Das bedeutet, dass mit diesem Projekt ein Unternehmen verbunden ist und diese Rolle bei der Arbeit einen anderen Abrechnungskurs für dieses Unternehmen aufweist. Der Abrechnungskurs für das Unternehmen wird angezeigt, auch wenn er mit dem Projektpreis identisch ist.

>[!NOTE]
>
><span class="preview">Wenn eine Preiskarte an das Projekt angehängt wird, werden die **Abrechnungsraten für Unternehmen** nicht in die Abrechnungssätze importiert. Die Berechnungen basieren entweder auf Ratenkarten-Raten oder Unternehmensraten für die Jobrollen.</span>
>
>Wenn es für eine Arbeitsplatzrolle Projektabrechnungssätze gibt, wird der **Abrechnungskurs des Unternehmens** nie auf die Berechnung des Umsatzes für das Projekt angewendet. Zur Berechnung des Umsatzes werden nur die **Projektabrechnungsraten** angewendet.

### Verschiedene Abrechnungsratenwerte und Zeitrahmen {#multiple-billing-rate-values-and-timeframes}

Wenn Sie mehrere Abrechnungsraten für eine bestimmte Auftragsrolle überschreiben, werden diese unter der Gruppierung für diese Auftragsrolle aufgeführt. Mithilfe der Inline-Bearbeitung können Sie die Überschreibungsraten und die Abrechnungsraten für **Start** **Datum** und **Enddatum** auf dieser Registerkarte ändern.

>[!NOTE]
>
>Sie können kein **Startdatum** für die erste Überschreibungsrate angeben und kein **Enddatum** für die letzte Überschreibungsrate angeben. Workfront geht davon aus, dass die erste Überschreibungsrate für alle Stunden mit einem Datum angewendet wird, das älter als das **Enddatum** der ersten Außerkraftsetzung ist, und dass die letzte Überschreibungsrate für alle Stunden mit einem Datum angewendet wird, das neuer als das **Startdatum** der letzten Überschreibung ist.\
>Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird die erste Abrechnungsrate verwendet.\
>Wenn eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert wird, wird die letzte Abrechnungsrate verwendet.

## Planeten Umsatz berechnen

* [Berechnen Sie den geplanten Umsatz anhand einer einmaligen Außerkraftsetzung des Abrechnungskurses.](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Planen Sie den Umsatz anhand mehrerer Außerkraftsetzungen des Abrechnungssatzes berechnen](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Verteilung der geplanten Stunden über die Dauer einer Aufgabe](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Planen Sie den Umsatz basierend auf einer einmaligen Außerkraftsetzung der Abrechnungsrate berechnen. {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Beachten Sie Folgendes bei der Berechnung des geplanten Umsatzes basierend auf einer einmaligen Außerkraftsetzung der Abrechnungsrate:

* Wenn der **Umsatztyp** einer Aufgabe den Wert **Stündliche Rolle** hat, multipliziert Workfront die geplanten Stunden einer Aufgabe mit der Abrechnungsrate der mit der Aufgabe verbundenen Auftragrolle, um den geplanten Umsatz für die Aufgabe zu berechnen.

* Wenn die Abrechnungsrate der Auftragsrolle auf Projektebene überschrieben wurde, verwendet Workfront die Überschreibungsrate aus dem Projekt, um den geplanten Umsatz zu berechnen.
* Wenn eine Aufgabe über mehrere Zuweisungen verfügt, wird der geplante Umsatz berechnet, indem die Abrechnungsrate der Stellenrolle jeder Zuweisung und der jeweiligen geplanten Stundenzuweisung multipliziert wird.

>[!NOTE]
>
>Die geplanten Stunden pro Zuweisung sind bei mehreren Zuweisungen nicht mit den geplanten Stunden für die Aufgabe identisch.

Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des geplanten Umsatzes verwendet wird, finden Sie im Abschnitt &quot;Grundlegendes zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen&quot;im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Planeten Umsatz basierend auf mehreren Überschreibungen des Abrechnungssatzes berechnen {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Beachten Sie Folgendes bei der Berechnung des geplanten Umsatzes auf der Grundlage mehrerer Außerkraftsetzungen der Abrechnungsrate:

* Wenn der **Umsatztyp** einer Aufgabe den Wert **Stündliche Rolle** hat, multipliziert Workfront die geplanten Stunden einer Aufgabe mit der Abrechnungsrate der mit der Aufgabe verbundenen Auftragrolle, um den geplanten Umsatz für die Aufgabe zu berechnen.

  Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des geplanten Umsatzes verwendet wird, finden Sie im Abschnitt &quot;Grundlegendes zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen&quot;im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Bei Mehrfachüberschreibung der Abrechnungsrate ändert sich der Prozentsatz, mit dem die geplanten Stunden multipliziert werden, während der Dauer einer Aufgabe. Standardmäßig verteilt Workfront die geplanten Stunden gleichmäßig auf die Dauer einer Aufgabe, wobei jedem Tag der Aufgabe eine gleiche Anzahl von Stunden zugewiesen wird. Bei der Berechnung des **geplanten Umsatzes** für eine Aufgabe multipliziert Workfront die geplante Stunde pro Tag mit der Abrechnungsrate dieses Tages. Bei mehreren Abrechnungsraten kann dieser Satz täglich unterschiedlich sein.

  Beispiel: Sie haben eine Aufgabe mit der Rolle Stündlich **Umsatz Typ**. Die Aufgabe hat eine Dauer von 5 Tagen und einen Wert für &quot;Geplante Stunden&quot;von 40 Stunden. Die geplanten Stunden pro Tag sind 8 Stunden. Weisen Sie der Aufgabe eine Projektleiter-Auftragsrolle zu und überschreiben Sie die Abrechnungsrate dieser Auftragsrolle für die letzten 3 Tage der Aufgabe, sodass Sie eine Abrechnungsrate von Rate 1 für die ersten beiden Tage und eine Abrechnungsrate von Rate 2 für die verbleibenden 3 Tage der Aufgabe für diese Auftragsrolle haben.

  Die Formel zur Berechnung des **geplanten Umsatzes** dieser Aufgabe lautet:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Weitere Informationen zum Auffinden des Betrags für geplante Stunden pro Tag in Workfront finden Sie im Abschnitt [Verteilung geplanter Stunden über die Dauer einer Aufgabe](#distribution-of-planned-hours-across-the-duration-of-a-task) in diesem Artikel.

>[!NOTE]
>
>Wenn Sie mehrere Verantwortliche für die Aufgabe haben, wird die Anzahl der geplanten Stunden zunächst an jeden Verantwortlichen verteilt und dann während der Dauer der Aufgabe an jeden Tag. In diesem Fall wird der geplante Umsatz unter Berücksichtigung der Tagesstunden für jeden Bevollmächtigten und des Abrechnungskurses jeder Auftragsrolle berechnet, der sich während der Dauer der Aufgabe ändern könnte, falls mehrere Abrechnungsraten vorliegen.

### Verteilung der geplanten Stunden über die Dauer einer Aufgabe {#distribution-of-planned-hours-across-the-duration-of-a-task}

Beachten Sie Folgendes, wenn Sie die Verteilung der geplanten Stunden über die Dauer einer Aufgabe verstehen:

* Standardmäßig verteilt Workfront die geplanten Stunden gleichmäßig auf die Dauer einer Aufgabe und weist je nach Verfügbarkeit des Projektplans für jeden Tag der Aufgabe eine identische Anzahl geplanter Stunden zu.

  Weitere Informationen zur Verteilung der geplanten Stunden über die Dauer einer Aufgabe finden Sie im Abschnitt &quot;Grundlegendes zur Verteilung der geplanten Stunden über die Dauer einer Aufgabe&quot;im Artikel [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Die geplante Stunde pro Tag ist die Zuweisung geplanter Stunden für jeden Tag während der Dauer der Aufgabe. Wenn die Aufgabe eine Zuweisung hat, stellt diese Zahl auch die geplanten Stunden pro Tag pro Zuweisung dar. Wenn die Aufgabe mehrere Zuweisungen aufweist, unterscheiden sich die geplanten Stunden pro Tag pro Zuweisung von den geplanten Stunden pro Tag für die Aufgabe. Es gibt keine visuelle Darstellung in Workfront für die geplanten Stunden pro Tag pro Zuweisung für Aufgaben mit mehreren Zuweisungen.
  >
  >
  >Die geplanten Stunden pro Tag werden mit der Abrechnungsrate für die der Aufgabe für diesen Tag zugewiesene Auftragrolle multipliziert, um den geplanten Umsatz pro Tag für diese Aufgabe zu berechnen. Eine Summe aller auf diese Weise berechneten geplanten täglichen Umsätze entspricht dem für diese Aufgabe geplanten Umsatz.

## Tatsächlichen Umsatz berechnen

* [Berechnen des tatsächlichen Umsatzes basierend auf einer einmaligen Außerkraftsetzung der Abrechnungsrate](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Berechnung des tatsächlichen Umsatzes auf der Grundlage mehrerer Außerkraftsetzungen der Abrechnungsrate](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Berechnung des tatsächlichen Umsatzes basierend auf einer einmaligen Außerkraftsetzung des Abrechnungskurses {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Beachten Sie Folgendes bei der Berechnung des tatsächlichen Umsatzes basierend auf einer einmaligen Außerkraftsetzung der Abrechnungsrate:

* Wenn der **Umsatztyp** einer Aufgabe den Wert **Stündliche Rolle** hat, multipliziert Workfront die **tatsächlichen Stunden** einer Aufgabe mit der Abrechnungsrate der der Aufgabe zugeordneten Auftragsrolle, um den **tatsächlichen Umsatz** für die Aufgabe zu berechnen. Die tatsächlichen Stunden werden direkt für die Aufgabe protokolliert.

  Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt &quot;Grundlagen zu den Umsatzberechnungen für Aufgaben, die auf Benutzer- und Rollenzuweisungen basieren&quot;im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Wenn die Abrechnungsrate der Auftragsrolle auf Projektebene überschrieben wurde, verwendet Workfront die Überschreibungsrate des Projekts zur Berechnung des tatsächlichen Umsatzes. Wenn Sie die Abrechnungsrate der Auftragsrolle im Projekt überschreiben, wird der **Tatsächliche Umsatz** des Projekts automatisch unter Verwendung der neuen angepassten Rate neu berechnet.

  Weitere Informationen zum Überschreiben von Rollenraten für das Projekt finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Wenn Sie die Stunden beibehalten möchten, die Sie bereits im Projekt angemeldet haben, bevor Sie den ursprünglichen Abrechnungskurs zum ursprünglichen Preis überschrieben haben, müssen Sie sie in einen **Abrechnungsdatensatz** aufnehmen und den **Abrechnungsdatensatz** als **Abrechnung** markieren. Andernfalls wird der **tatsächliche Umsatz** aus den Stunden, die vor der Außerkraftsetzung des Abrechnungskurses für das Projekt protokolliert wurden, anhand des neuen Satzes neu berechnet, wenn die Finanzierung der Projekte neu berechnet wird.\
>Weitere Informationen zum Einbeziehen von Stunden in einen Rechnungsdatensatz und zum Kennzeichnen des Datensatzes als **Abgerechnet** finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

### Berechnung des tatsächlichen Umsatzes auf der Grundlage mehrerer Außerkraftsetzungen der Abrechnungsrate {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Beachten Sie Folgendes bei der Berechnung des tatsächlichen Umsatzes auf der Grundlage mehrerer Außerkraftsetzungen der Abrechnungsrate:

* Wenn der **Umsatztyp** einer Aufgabe den Wert **Stündliche Rolle** hat, multipliziert Workfront die **tatsächlichen Stunden** für die Aufgabe mit der Abrechnungsrate der Auftragsrollen, die der Aufgabe zugewiesen sind, um den **tatsächlichen Umsatz** für die Aufgabe zu berechnen. Die tatsächlichen Stunden werden direkt für die Aufgabe protokolliert.

* Bei Mehrfachüberschreibung der Abrechnungsrate kann sich der Prozentsatz, mit dem die **tatsächlichen Stunden** multipliziert werden, um den **tatsächlichen Umsatz** zu berechnen, während der Dauer einer Aufgabe ändern. Workfront verwendet die Abrechnungsrate der Auftragsrolle, deren Zeitrahmen mit dem **Einstiegsdatum** der Stunden übereinstimmt, die für die Aufgabe protokolliert wurden, um den **tatsächlichen Umsatz** zu berechnen.

  Beispielsweise weist eine Aufgabe den **Umsatztyp** von **Stündliche Rolle** auf und wird der Auftragsrolle des Projekt-Managers zugewiesen. Überschreiben Sie die Abrechnungsrate dieser Auftragsrolle mit Rate 1 für die Datumsangaben zwischen dem 19. Juni und dem 25. Juni. Ab dem 26. Juni müssen Sie den Abrechnungskurs mit Rate 2 überschreiben. 2 Stunden für den 20. Juni und 3 Stunden für den 28. Juni protokollieren.

  Workfront berechnet den **tatsächlichen Umsatz** für diese Aufgabe anhand der folgenden Formel:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt &quot;Grundlagen zu den Umsatzberechnungen für Aufgaben, die auf Benutzer- und Rollenzuweisungen basieren&quot;im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Auswirkungen von Zeitzonen bei der Berechnung des Umsatzes auf der Grundlage mehrerer Abrechnungsraten

Benutzer können verschiedene geplante Stunden pro Tag sehen als andere Benutzer, wenn Zeitzonenunterschiede zwischen ihnen und anderen Entitäten in Workfront auftreten. Die folgenden Szenarien könnten die Informationen zu geplanten Stunden pro Tag für einen Benutzer von den Informationen eines anderen Benutzers verfälschen:

* Die Computer der beiden Benutzer sind möglicherweise auf zwei verschiedene Zeitzonen eingestellt
* Die beiden Benutzerprofile in Workfront können auf zwei verschiedene Zeitzonen eingestellt sein.
* Die mit dem Benutzerprofil verknüpfte Zeitzone unterscheidet sich möglicherweise von der Systemzeitzone in Workfront
* Die mit dem Benutzerprofil verknüpfte Zeitzone kann sich von der Zeitzone des Zeitplans des Projekts unterscheiden.

In diesen Fällen kann die Anzahl der geplanten Stunden pro Tag von zwei Benutzern unterschiedlich sein, die nicht dieselben Einstellungen für Zeitzonen verwenden. Außerdem werden ihnen verschiedene geplante Umsatzzahlen angezeigt, wenn mehrere Außerkraftsetzungen der Abrechnungsrate für ein Projekt verwendet werden.

* [Planeten Umsatz für Benutzer in verschiedenen Zeitzonen berechnen](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Tatsächlichen Umsatz für Benutzer in verschiedenen Zeitzonen berechnen](#calculate-actual-revenue-for-users-in-different-time-zones)

### Planeten Umsatz für Benutzer in verschiedenen Zeitzonen berechnen {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Wenn Sie Benutzer in verschiedenen Zeitzonen haben, die an denselben Projekten arbeiten, empfehlen wir, die Überschreibungen der Abrechnungsrate für Ihre Projekte während der Woche nicht zu ändern. Auf diese Weise kann ein fehlerhafter Betrag des geplanten Umsatzes für Ihr Projekt angezeigt werden, da zwischen den Zeitzonen im Zeitplan der Benutzer und der Zeitzone des Workfront-Systems Stundenunterschiede bestehen. Die meisten Zeitpläne ermöglichen den Ausschluss von Wochenenden aus den Berechnungen für geplante Stunden. Wenn eine Änderung beim Außerkraftsetzen der Abrechnungsrate einer Auftragrolle eintritt, ist es besser, sie an einem Wochenende vorzunehmen als in der Mitte einer Woche, an der sie mit der Mitte der Dauer einer Aufgabe zusammenfallen könnte.

Beachten Sie bei der Berechnung des geplanten Umsatzes für Benutzer in verschiedenen Zeitzonen Folgendes:

* Für Aufgaben mit dem Umsatztyp **von** Role Hourly **und den Auftragsrollen zugewiesen wird, wird der** geplante Umsatz **berechnet, indem die** Planeten Stunden **einer Aufgabe mit der Abrechnungsrate der Auftragsrolle multipliziert wird.**

* Die **geplanten Stunden** werden gleichmäßig über die **Dauer** der Aufgabe verteilt.

* Die **Dauer** ist der Zeitraum zwischen dem **geplanten Start** **Datum** und dem **geplanten Abschlussdatum** der Aufgabe. Da das **geplante Startdatum** und das **geplante Abschlussdatum** der Aufgaben je nach Zeitzone der Benutzer, die die Aufgabe anzeigen, unterschiedlich sein können, kann die Anzahl der geplanten Stunden pro Tag für zwei Benutzer in zwei verschiedenen Zeitzonen variieren.

* Die Höhe der geplanten Stunden pro Tag ändert nicht den geplanten Umsatz eines Projekts, wenn die Abrechnungsrate der Auftrags-Rolle nicht geändert wird oder wenn nur eine Abrechnungsrate überschrieben wird. Selbst wenn zwei Benutzer aus zwei verschiedenen Zeitzonen verschiedene geplante Stunden pro Tag sehen, ist der geplante Gesamtumsatz des Projekts zwischen den beiden Benutzern identisch.

  Bei mehreren Überschreitungen der Abrechnungsrate scheint der Gesamtumsatz **Geplanter Umsatz** des Projekts jedoch für zwei Benutzer in zwei verschiedenen Zeitzonen unterschiedlich zu sein, da er sich auf die Anzahl der geplanten Stunden pro Tag (was für die beiden Benutzer unterschiedlich sein kann) und die Abrechnungsrate (die für denselben Tag unterschiedlich sein könnte, wenn sich jeder Benutzer die Aufgabe in seiner eigenen Zeitzone ansieht) stützt.

* Der genaue Betrag von **Geplanter Umsatz** ist der Betrag, den der Benutzer sieht, der dieselbe Zeitzone wie die Zeitzone Ihrer Workfront-Instanz hat. Ihr Workfront-Administrator definiert die Zeitzone von Workfront im Bereich &quot;Systemkundeninformationen&quot;.\
  Weitere Informationen zum Definieren der Zeitzone für Ihr System finden Sie im Artikel [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Tatsächlichen Umsatz für Benutzer in verschiedenen Zeitzonen berechnen {#calculate-actual-revenue-for-users-in-different-time-zones}

Beachten Sie bei der Berechnung des tatsächlichen Umsatzes für Benutzer in verschiedenen Zeitzonen Folgendes:

* Wenn der **Umsatztyp** einer Aufgabe den Wert **Stündliche Rolle** hat, multipliziert Workfront die **tatsächlichen Stunden** für die Aufgabe mit der Abrechnungsrate der Auftragsrollen, die der Aufgabe zur Berechnung des **tatsächlichen Umsatzes** zugewiesen sind. Die tatsächlichen Stunden werden direkt für die Aufgabe protokolliert.

* Bei Mehrfachüberschreibung der Abrechnungsrate verwendet Workfront die Abrechnungsrate der Auftragrolle, deren Zeitrahmen mit dem **Einstiegsdatum** der Stunden übereinstimmt, die für die Aufgabe protokolliert wurden, um den **tatsächlichen Umsatz** zu berechnen.

* Da es keinen Zeitstempel am **Einstiegsdatum** der angemeldeten Stunden gibt und es keinen Zeitstempel für die Datumsbereiche mehrerer Außerkraftsetzungen der Abrechnungsrate gibt, sind **Tatsächlicher Umsatz**-Berechnungen nicht von der Zeitzone betroffen, die mit Benutzern verknüpft ist.

Weitere Informationen dazu, welche Auftragsrolle zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt &quot;Grundlagen zu den Umsatzberechnungen für Aufgaben, die auf Benutzer- und Rollenzuweisungen basieren&quot;im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Projektfinanzierungen neu berechnen

Die Finanzierung wird für ein Projekt berechnet, da Änderungen in den für das Projekt protokollierten Stunden stattfinden.

Wenn die Beträge während der Laufzeit eines Projekts geändert werden, können Sie die Kosten und Einnahmen des Projekts manuell neu berechnen, indem Sie für ein Projekt die Option Finanzen neu berechnen verwenden. Darüber hinaus wird bei einigen Aktionen eine automatische Neuberechnung Trigger.

Weitere Informationen zur Neuberechnung der Projektfinanzen finden Sie im Artikel [Neuberechnung der Projektfinanzen vornehmen](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Hinzufügen einer neuen Abrechnungsrate mithilfe der API

Um mithilfe der API eine neue Abrechnungsrate für eine Auftragsrolle hinzuzufügen, führen Sie eine *setRatesForRole* -Aktion für das Objekt **Rate** durch, indem Sie die *PUT-Methode* verwenden.
Die Aktion und die Datumsfelder für das Objekt **Rate** sind in der API-Version 8.0 verfügbar.
Wenn Sie bereits mehrere Abrechnungsraten für eine Auftragsrolle in einem Projekt definiert haben und eine neue Abrechnungsrate für dieses Projekt mit einem neuen Datumsbereich hinzufügen möchten, müssen Sie sowohl die bestehende Rate als auch die Rate angeben, die im selben API-Aufruf hinzugefügt werden soll. Dies ähnelt der Aktualisierung von Sammlungen für Objekte.

Der folgende API-Aufruf ist ein Beispiel, bei dem **attachmentID** die **Projekt-ID** des Projekts ist, in dem Sie die Rate hinzufügen, und **RoleID** die **Auftrags-Rolle-ID**, für die Sie die neue Abrechnungsrate hinzufügen.<pre>{</pre><pre>&quot;attachmentID&quot;:&quot;593f0150000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachmentObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df00014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Weitere Informationen zur Verwendung der Workfront-API finden Sie im Artikel [API-Grundlagen](https://experience.workfront.com/s/article/API-Basics-638808549).
