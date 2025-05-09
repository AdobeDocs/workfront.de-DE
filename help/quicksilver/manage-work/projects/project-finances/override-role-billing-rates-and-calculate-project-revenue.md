---
product-area: projects
navigation-topic: financials
title: Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt
description: Sie können Verrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu berechnen, wenn Sie sie mit den für das Projekt aufgewendeten Stunden multiplizieren. Weitere Informationen zu Abrechnungssätzen und Umsatz finden Sie im Artikel Übersicht über Abrechnung und Umsatz .
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '3860'
ht-degree: 0%

---

# Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt

{{highlighted-preview}}

Sie können Verrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu berechnen, wenn Sie sie mit den für das Projekt aufgewendeten Stunden multiplizieren. Weitere Informationen zu Abrechnungssätzen und Umsatz finden Sie im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

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

## Übersicht über Abrechnungssätze für Aufgabengebiete und Umsatztypen für Stundensätze für Aufgabengebiete

Als Adobe Workfront-Administrator können Sie Abrechnungssätze sowohl mit Benutzern als auch mit Aufgabengebieten verknüpfen.\
Weitere Informationen zum Erstellen von Benutzern und zum Verknüpfen mit Abrechnungssätzen finden Sie im Artikel [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Weitere Informationen zum Erstellen von Aufgabengebieten und deren Verknüpfung mit Abrechnungssätzen finden Sie im Artikel [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Die mit Benutzenden verknüpften Abrechnungssätze können nicht überschrieben werden.

Abrechnungssätze für Aufgabengebiete können auf Unternehmens- oder Projektebene überschrieben werden.

Um den Umsatz aus Projekten auf der Grundlage der Abrechnungssätze für Aufgabengebiete zu berechnen, muss **Umsatztyp** der Aufgaben für die Projekte einer der folgenden sein:

* Stundensatz nach Funktion
* Stundensatz nach Funktion mit Begrenzung
* Stundensatz nach Funktion plus fest

Weitere Informationen zu **Umsatztyp** und Abrechnungssätzen finden Sie unter [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hierarchie der Abrechnungssatz-Überschreibungen bei der Berechnung des Umsatzes

Einem Aufgabengebiet kann auf folgende Weise ein Abrechnungssatz zugeordnet werden:

* Als Workfront-Administrator können Sie den Abrechnungssatz auf Systemebene definieren, der mit einem Aufgabengebiet verknüpft ist, wenn Sie dieses Aufgabengebiet erstellen.\
  Weitere Informationen zum Erstellen von Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Als Workfront-Administrator können Sie bei der Erstellung eines Unternehmens den Abrechnungssatz auf Firmenebene für dasselbe Aufgabengebiet definieren.\
  Wenn Workfront den Umsatz für die mit diesem Unternehmen verbundenen Projekte berechnet, wird der Abrechnungssatz des Unternehmens verwendet, wenn die Funktion Aufgaben zugewiesen wird, und nicht der Abrechnungssatz auf Systemebene für dieses Aufgabengebiet.\
  Die auf Unternehmensebene geänderten Tarife für Aufgabengebiete wirken sich auf alle mit dieser Firma verbundenen Projekte aus.

  >[!NOTE]
  >
  >Wenn Sie den Abrechnungssatz der Firma aktualisieren müssen, wird der Satz für das Projekt nicht automatisch aktualisiert. Sie müssen die Firma aus dem Projekt entfernen, den Satz für die Firma aktualisieren und dann die Firma erneut an das Projekt anhängen, bevor der neue Firmensatz für das Projekt wirksam wird. Anweisungen zum Anhängen einer Firma an ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

  Weitere Informationen zum Erstellen unternehmensspezifischer Abrechnungssätze für Aufgabengebiete finden Sie unter [Firmen erstellen und bearbeiten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Als Workfront-Administrator können Sie beim Bearbeiten eines Projekts eine Option aktivieren, um Änderungen an den Abrechnungssätzen auf Firmenebene auf das Projekt anzuwenden, wenn Benutzer die Projektfinanzen manuell neu berechnen.\
  Weitere Informationen finden Sie unter [Überschreiben von Abrechnungssätzen auf Projektebene mit Abrechnungssätzen auf Firmenebene](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Als Workfront-Administrator können Sie Tarifkarten mit mehreren Abrechnungssätzen pro Rolle definieren, basierend auf Standort und Datum. Wenn einem Projekt eine Tarifkarte beigefügt ist, werden alle Funktionen (nach Standort, wenn Standorte verwendet werden) und die zugehörigen Abrechnungssätze zum Abschnitt Abrechnungssätze des Projekts hinzugefügt. Durch das Anhängen einer Tarifkarte werden alle vorhandenen Abrechnungssätze für das Projekt überschrieben.

  Weitere Informationen finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) und [Eine Tarifkarte an ein Projekt anhängen](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Als Projekt-Manager können Sie auf Projektebene den Abrechnungssatz für dasselbe Aufgabengebiet definieren.\
  Die im Projekt geänderten Tarife für Aufgabengebiete wirken sich nur auf dieses Projekt aus.

  Informationen zum Überschreiben von Abrechnungssätzen für Aufgabengebiete für das Projekt finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Wenn ein Aufgabengebiet auf Systemebene, Unternehmensebene und Projektebene mit einem Abrechnungssatz verknüpft ist, berechnet Workfront den Umsatz der Aufgaben anhand des Abrechnungssatzes des Aufgabengebiets auf Projektebene, wenn es die Abrechnungssätze für Aufgabengebiete verwendet. Die Einnahmen aus allen Aufgaben summieren sich zu den Einnahmen des Projekts.

## Aufgabengebiet-Abrechnungssätze auf Projektebene überschreiben

Als Projekt-Manager können Sie den Abrechnungssatz für ein Aufgabengebiet in einem bestimmten Projekt angeben. Dieser Abrechnungssatz auf Projektebene überschreibt den Abrechnungssatz auf Systemebene für dieses Aufgabengebiet. Workfront verwendet zur Berechnung des Umsatzes den Abrechnungssatz auf Projektebene des Aufgabengebiets, anstatt den Abrechnungssatz auf Systemebene zu verwenden.

<span class="preview">Sie können dem Projekt auch eine Tarifkarte hinzufügen, mit der die Abrechnungssätze für das Aufgabengebiet von der Tarifkarte in das Projekt importiert werden.</span>

Informationen zum Überschreiben der Abrechnungssätze für Aufgabengebiete auf Projektebene finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des Umsatzes für das Projekt verwendet wird, finden Sie im Abschnitt „Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ in [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Informationen zum Anhängen einer Tarifkarte an ein Projekt finden Sie unter [Anhängen einer Tarifkarte an ein Projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>Bei tatsächlichen Einnahmen sollten die Abrechnungssätze, die auf Stunden angewendet werden, die einem als „In Rechnung gestellt“ markierten Abrechnungs-Datensatz hinzugefügt werden, nicht von Abrechnungssatz-Überschreibungen beeinflusst werden, die nach der Abrechnung des Abrechnungs-Datensatzes auftreten.

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
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. </p> </li>
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

## Übersicht über den Abschnitt Abrechnungssätze eines Projekts

Nachdem Sie die Verrechnungssätze für die mit dem Projekt verknüpften Aufgabengebiete überschreiben haben, können Sie alle Aufgabengebiete und deren Überschreibungen auf der Registerkarte **Verrechnungssätze** des Projekts anzeigen.

Beachten Sie die folgenden Informationen in der Liste **Abrechnungssätze**:

* [Aufgabengebiet-Gruppierung](#job-role-grouping)
* [Projekt-Abrechnungssatzwert](#project-billing-rate-value)
* [Standardwert für Abrechnungssatz](#default-billing-rate-value)
* [Wert des Abrechnungssatzes des Unternehmens](#company-billing-rate-value)
* [Mehrere Abrechnungssatzwerte und Zeitrahmen](#multiple-billing-rate-values-and-timeframes)

### Aufgabengebiet-Gruppierung {#job-role-grouping}

Abrechnungssätze werden im Bereich „Abrechnungssätze **nach** Aufgabengebiet gruppiert. <span class="preview">Wenn dem Projekt eine Tarifkarte beigefügt ist, werden die Aufgabengebiete ebenfalls nach Tarifkarte gruppiert. Wenn Standorte auf Aufgabengebiete angewendet werden, wird der Standortname als Teil des Aufgabengebietsnamens eingeschlossen. Dasselbe Aufgabengebiet könnte für mehrere Standorte aufgelistet sein.</span>

### Projekt-Abrechnungssatzwert {#project-billing-rate-value}

Beachten Sie in der Gruppierungsposition, die einem Aufgabengebiet entspricht, den Abrechnungssatz für dieses Aufgabengebiet auf Projektebene in der Spalte **Projekt-Abrechnungssatz**. Wenn das Aufgabengebiet mehrere Überschreibungssätze hat, wird der Überschreibungssatz für das aktuelle Datum in der Gruppierungsposition in der Spalte **Projekt-Abrechnungssatz** angezeigt.

### Standardwert für Abrechnungssatz {#default-billing-rate-value}

Beachten Sie in der Gruppierungsposition eines Aufgabengebiets den Abrechnungssatz für dieses Aufgabengebiet auf Systemebene in der Spalte **Standardabrechnungssatz**.

>[!NOTE]
>
>Wenn für ein Aufgabengebiet Abrechnungssätze für ein Projekt vorhanden sind, wird **Standard-Abrechnungssatz** nie auf die Berechnung des Umsatzes für das Projekt angewendet. Zur Berechnung **Umsatzes werden nur die** Projekt-Abrechnungssätze“ angewendet.

### Wert des Abrechnungssatzes der Firma {#company-billing-rate-value}

Beachten Sie in der Gruppierungsposition eines Aufgabengebiets den Abrechnungssatz für dieses Aufgabengebiet auf Unternehmensebene in der Spalte **Abrechnungssatz des Unternehmens**. Dies bedeutet, dass mit diesem Projekt eine Firma verknüpft ist und dieses Aufgabengebiet einen anderen Abrechnungssatz für diese Firma hat. Der Abrechnungssatz für die Firma wird angezeigt, auch wenn er mit dem Projektsatz identisch ist.

>[!NOTE]
>
><span class="preview">Wenn dem Projekt eine Tarifkarte beigefügt ist, werden **Abrechnungssätze des Unternehmens** nicht in die Abrechnungssätze importiert. Die Berechnungen basieren entweder auf Tarifkartensätzen oder Firmensätzen für die Aufgabengebiete.</span>
>
>Wenn für ein Aufgabengebiet Projekt-Abrechnungssätze vorhanden sind, wird **Abrechnungssatz des Unternehmens** nie auf die Berechnung des Umsatzes für das Projekt angewendet. Zur Berechnung **Umsatzes werden nur die** Projekt-Abrechnungssätze“ angewendet.

### Mehrere Abrechnungssatzwerte und Zeitrahmen {#multiple-billing-rate-values-and-timeframes}

Wenn Sie für ein bestimmtes Aufgabengebiet mehrere Abrechnungssätze überschreiben, werden diese unter der Gruppierung für dieses Aufgabengebiet aufgeführt. Bei der Inline-Bearbeitung können Sie auf dieser Registerkarte die Überschreibungssätze und **Start** **Datum** und **Enddatum** der Überschreibungssätze ändern.

>[!NOTE]
>
>Sie können kein **Startdatum** für den ersten Überschreibungssatz und kein **Enddatum** für den letzten Überschreibungssatz angeben. Workfront geht davon aus, dass die erste Überschreibungsrate auf alle Stunden angewendet wird, deren Datum älter als das **Enddatum** der ersten Überschreibungsrate ist, und dass die letzte Überschreibungsrate auf alle Stunden angewendet wird, deren Datum neuer als das **Startdatum** der letzten Überschreibungsrate ist.\
>Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird der erste Abrechnungssatz verwendet.\
>Wird eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert, wird der letzte Abrechnungssatz verwendet.

## Geplanten Umsatz berechnen

* [Berechnung des geplanten Umsatzes basierend auf einer einmaligen Abrechnungssatz-Überschreibung](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Berechnung des geplanten Umsatzes basierend auf Überschreibungen mehrerer Abrechnungssätze](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Verteilung der geplanten Stunden über die Dauer einer Aufgabe](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Berechnung des geplanten Umsatzes basierend auf einer einmaligen Abrechnungssatz-Überschreibung {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Beachten Sie bei der Berechnung des geplanten Umsatzes auf der Grundlage einer einmaligen Abrechnungssatz-Überschreibung Folgendes:

* Wenn der **Umsatztyp** einer Aufgabe &quot;**pro Stunde“**, multipliziert Workfront die geplanten Stunden einer Aufgabe mit dem Abrechnungssatz des Aufgabengebiets, das der Aufgabe zugeordnet ist, um den geplanten Umsatz für die Aufgabe zu berechnen.

* Wenn der Abrechnungssatz des Aufgabengebiets auf Projektebene überschrieben wurde, verwendet Workfront den Überschreibungssatz aus dem Projekt, um den geplanten Umsatz zu berechnen.
* Wenn eine Aufgabe mehrere Zuordnungen hat, wird der geplante Umsatz durch Multiplikation des Abrechnungssatzes des Aufgabengebiets jeder Zuordnung und der entsprechenden Zuordnung der geplanten Stunde berechnet.

>[!NOTE]
>
>Die geplanten Stunden pro Arbeitsauftrag sind bei mehreren Arbeitsaufträgen nicht mit den geplanten Stunden für die Aufgabe identisch.

Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des geplanten Umsatzes verwendet wird, finden Sie im Abschnitt „Grundlagen zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Berechnung des geplanten Umsatzes basierend auf Überschreibungen mehrerer Abrechnungssätze {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Beachten Sie bei der Berechnung des geplanten Umsatzes auf der Grundlage mehrerer Abrechnungssatzüberschreibungen Folgendes:

* Wenn der **Umsatztyp** einer Aufgabe &quot;**pro Stunde“**, multipliziert Workfront die geplanten Stunden einer Aufgabe mit dem Abrechnungssatz des Aufgabengebiets, das der Aufgabe zugeordnet ist, um den geplanten Umsatz für die Aufgabe zu berechnen.

  Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des geplanten Umsatzes verwendet wird, finden Sie im Abschnitt „Grundlagen zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Bei Überschreibungen mehrerer Abrechnungssätze ändert sich der Satz, mit dem die geplanten Stunden multipliziert werden, während der Dauer einer Aufgabe. Standardmäßig verteilt Workfront die geplanten Stunden gleichmäßig auf die Dauer einer Aufgabe, wobei für jeden Aufgabentag die gleiche Anzahl von Stunden zugewiesen wird. Bei der Berechnung **Geplanter Umsatz** für eine Aufgabe multipliziert Workfront die geplante Stunde pro Tag mit dem Abrechnungssatz des Tages. Bei mehreren Abrechnungssätzen kann dieser Satz jeden Tag anders sein.

  Sie haben beispielsweise eine Aufgabe mit der Funktion „Stündlich“ **Umsatztyp**. Die Aufgabe hat eine Dauer von 5 Tagen und einen Wert für Geplante Stunden von 40 Stunden. Die geplanten Stunden pro Tag betragen 8 Stunden. Weisen Sie der Aufgabe ein Aufgabengebiet als Projekt-Manager zu und überschreiben Sie den Abrechnungssatz dieses Aufgabengebiets für die letzten 3 Tage der Aufgabe, sodass Sie für die ersten zwei Tage einen Abrechnungssatz von Satz 1 und für dieses Aufgabengebiet einen Abrechnungssatz von Satz 2 für die verbleibenden 3 Tage der Aufgabe haben.

  Die Formel zur Berechnung der **geplanten Einnahmen** dieser Aufgabe lautet:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Weitere Informationen zum Ermitteln der geplanten Stunden pro Tag in Workfront finden Sie im Abschnitt [Verteilung der geplanten Stunden über die Dauer einer Aufgabe](#distribution-of-planned-hours-across-the-duration-of-a-task) in diesem Artikel.

>[!NOTE]
>
>Wenn Sie mehrere Beauftragte für die Aufgabe haben, wird die Anzahl der geplanten Stunden zuerst auf jeden Beauftragten und dann während der Dauer der Aufgabe auf jeden Tag verteilt. In diesem Fall werden bei der Berechnung der geplanten Einnahmen die Anzahl der täglichen Stunden für jeden Verantwortlichen und der Abrechnungssatz für jedes Aufgabengebiet berücksichtigt, der sich bei mehreren Abrechnungssätzen während der Laufzeit der Aufgabe ändern könnte.

### Verteilung der geplanten Stunden über die Dauer einer Aufgabe {#distribution-of-planned-hours-across-the-duration-of-a-task}

Beachten Sie beim Verstehen der Verteilung der geplanten Stunden über die Dauer einer Aufgabe Folgendes:

* Standardmäßig verteilt Workfront die geplanten Stunden gleichmäßig auf die Dauer einer Aufgabe, wobei für jeden Aufgabentag die gleiche Anzahl geplanter Stunden entsprechend der Verfügbarkeit des Projektplans zugewiesen wird.

  Weitere Informationen zum Verständnis der Verteilung der geplanten Stunden über die Dauer einer Aufgabe finden Sie im Abschnitt „Grundlegendes zur Verteilung der geplanten Stunden über die Dauer einer Aufgabe“ im Artikel [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >Die „Geplante Stunden pro Tag“ ist die Zuordnung der geplanten Stunden für jeden Tag während der Aufgabendauer. Wenn die Aufgabe über eine Zuweisung verfügt, stellt diese Zahl auch die geplanten Stunden pro Tag und Zuweisung dar. Wenn die Aufgabe mehrere Zuweisungen hat, unterscheidet sich die geplante Stunde pro Tag und Zuweisung von der geplanten Stunde pro Tag für die Aufgabe. In Workfront gibt es keine visuelle Darstellung der geplanten Stunden pro Tag und Zuweisung für Aufgaben mit mehreren Zuweisungen.
  >
  >
  >Die geplanten Stunden pro Tag werden mit dem Abrechnungssatz für das Aufgabengebiet multipliziert, das der Aufgabe für diesen Tag zugewiesen wurde, um den geplanten Umsatz pro Tag für diese Aufgabe zu berechnen. Die Summe aller auf diese Weise berechneten täglichen geplanten Einnahmen entspricht den geplanten Einnahmen für diese Aufgabe.

## Tatsächlichen Umsatz berechnen

* [Berechnen Sie den tatsächlichen Umsatz anhand einer einmaligen Überschreibung des Abrechnungssatzes](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Berechnung des tatsächlichen Umsatzes basierend auf Überschreibungen mehrerer Abrechnungssätze](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Berechnung des tatsächlichen Umsatzes basierend auf einer einmaligen Abrechnungssatz-Überschreibung {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Beachten Sie Folgendes bei der Berechnung der tatsächlichen Einnahmen auf der Grundlage einer einmaligen Überschreibung des Abrechnungssatzes:

* Wenn der **Umsatztyp** einer Aufgabe &quot;**pro Stunde“**, multipliziert Workfront die **Ist-Stunden** einer Aufgabe mit dem Abrechnungssatz des Aufgabengebiets, das der Aufgabe zugeordnet ist, um **Ist-Umsatz** der Aufgabe zu berechnen. Tatsächliche Stunden sind Stunden, die direkt in der Aufgabe protokolliert werden.

  Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt „Grundlagen zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Wenn der Abrechnungssatz des Aufgabengebiets auf Projektebene überschrieben wurde, berechnet Workfront den tatsächlichen Umsatz anhand des Überschreibungssatzes aus dem Projekt. Wenn Sie den Abrechnungssatz des Aufgabengebiets für das Projekt überschreiben, wird der **tatsächliche Umsatz** des Projekts automatisch unter Verwendung des neuen angepassten Satzes neu berechnet.

  Informationen zum Überschreiben von Abrechnungssätzen für Aufgabengebiete für das Projekt finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Wenn Sie die Stunden, die Sie bereits für das Projekt angemeldet haben, beibehalten möchten, bevor Sie den ursprünglichen, zum ursprünglichen Satz in Rechnung gestellten Abrechnungssatz überschreiben, müssen Sie sie in einen **Abrechnungsdatensatz** einbeziehen und den **Abrechnungsdatensatz** als **In Rechnung gestellt** markieren. Andernfalls wird der **tatsächliche Umsatz** der Stunden, die protokolliert wurden, bevor der Abrechnungssatz für das Projekt überschrieben wurde, bei der Neuberechnung der Finanzen der Projekte mit dem neuen Satz neu berechnet.\
>Weitere Informationen zum Einschließen von Stunden in einen Abrechnungs-Datensatz und zum Kennzeichnen als **Abgerechnet** finden Sie im Artikel [Erstellen von Abrechnungs-Datensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

### Berechnung des tatsächlichen Umsatzes basierend auf Überschreibungen mehrerer Abrechnungssätze {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Beachten Sie Folgendes bei der Berechnung der tatsächlichen Einnahmen auf der Grundlage mehrerer Abrechnungssatzüberschreibungen:

* Wenn der **Umsatztyp** einer Aufgabe &quot;**pro Stunde“**, multipliziert Workfront die **Ist-Stunden** der Aufgabe mit dem Abrechnungssatz der Aufgabengebiete, die der Aufgabe zugewiesen wurden, um **Ist-Umsatz** der Aufgabe zu berechnen. Tatsächliche Stunden sind Stunden, die direkt in der Aufgabe protokolliert werden.

* Bei Überschreibungen mehrerer Abrechnungssätze kann sich der Satz, mit dem die **Ist-Stunden** multipliziert werden, um den **Ist-Umsatz** während der Dauer einer Aufgabe ändern. Workfront verwendet den Abrechnungssatz des Aufgabengebiets, dessen Zeitrahmen mit dem **Eingabedatum) der** für die Aufgabe protokollierten Stunden übereinstimmt, um den **tatsächlichen Umsatz“**

  Beispielsweise hat eine Aufgabe den **Umsatztyp** &quot;**Stündlich** und ist dem Aufgabengebiet des Projekt-Managers zugewiesen. Überschreiben Sie den Abrechnungssatz dieses Aufgabengebiets mit Satz 1 für die Daten zwischen dem 19. Juni und dem 25. Juni. Überschreiben Sie ab dem 26. Juni den Abrechnungssatz mit Satz 2. Protokollieren Sie 2 Stunden für den 20. Juni und 3 Stunden für den 28. Juni.

  Workfront berechnet den **tatsächlichen Umsatz** für diese Aufgabe anhand der folgenden Formel:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt „Grundlagen zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Auswirkungen von Zeitzonen bei der Berechnung des Umsatzes basierend auf mehreren Abrechnungssätzen

Benutzende sehen andere geplante Stunden pro Tag als andere Benutzende, wenn Zeitzonenunterschiede zwischen ihnen und anderen Entitäten in Workfront auftreten. Die folgenden Szenarien können die Informationen zu „Geplante Stunden pro Tag“ für eine Benutzerin oder einen Benutzer von dem unterscheiden, was eine andere Person sieht:

* Die Computer der beiden Benutzer sind möglicherweise für zwei verschiedene Zeitzonen eingerichtet
* Die beiden Benutzerprofile in Workfront können auf zwei verschiedene Zeitzonen festgelegt sein
* Die mit dem Benutzerprofil verknüpfte Zeitzone kann sich von der Systemzeitzone in Workfront unterscheiden
* Die mit dem Benutzerprofil verknüpfte Zeitzone kann sich von der Zeitzone des Zeitplans des Projekts unterscheiden.

In diesen Fällen kann die Anzahl der geplanten Stunden pro Tag zwischen zwei Benutzenden unterschiedlich sein, die nicht dieselben Einstellungen für Zeitzonen verwenden. Bei Verwendung mehrerer Abrechnungssatz-Überschreibungen für ein Projekt werden auch andere Zahlen für den geplanten Umsatz angezeigt.

* [Berechnung des geplanten Umsatzes für Benutzer in verschiedenen Zeitzonen](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Berechnen des tatsächlichen Umsatzes für Benutzer in verschiedenen Zeitzonen](#calculate-actual-revenue-for-users-in-different-time-zones)

### Berechnung des geplanten Umsatzes für Benutzer in verschiedenen Zeitzonen {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Wenn Sie Benutzende in verschiedenen Zeitzonen haben, die an denselben Projekten arbeiten, empfehlen wir, die Überschreibungen des Abrechnungssatzes für Ihre Projekte während der Woche nicht zu ändern. Dadurch kann die falsche Menge an geplantem Umsatz für Ihr Projekt angezeigt werden, da Ihre Unterschiede zwischen den Zeitzonen im Zeitplan der Benutzenden und der Zeitzone des Workfront-Systems bestehen. Die meisten Zeitpläne ermöglichen den Ausschluss von Wochenenden aus den Berechnungen für geplante Stunden. Wenn eine Änderung in der Außerkraftsetzung des Abrechnungssatzes für ein Aufgabengebiet auftritt, ist es besser, dass die Änderung an einem Wochenende erfolgt als mitten in einer Woche, wenn sie mit der Mitte der Dauer einer Aufgabe zusammenfallen könnte.

Beachten Sie bei der Berechnung des geplanten Umsatzes für Benutzer in verschiedenen Zeitzonen Folgendes:

* Bei Aufgaben mit dem **Umsatztyp** &quot;**Stündlich**, die Aufgabengebieten zugewiesen sind, wird **Geplanter Umsatz** durch Multiplikation der **Geplanten Stunden** einer Aufgabe mit dem Abrechnungssatz des Aufgabengebiets berechnet.

* Die **Geplanten Stunden** werden gleichmäßig über die **Dauer** der Aufgabe verteilt.

* Die **Dauer** ist der Zeitraum zwischen dem **geplanten Start****Datum** und dem **geplanten Abschlussdatum** der Aufgabe. Da das **Geplantes Startdatum** und **Geplantes Abschlussdatum** der Aufgaben je nach Zeitzonen der Benutzer, die die Aufgabe angezeigt haben, unterschiedlich sein können, kann die Anzahl der geplanten Stunden pro Tag für zwei Benutzer in zwei verschiedenen Zeitzonen unterschiedlich sein.

* Der Betrag der geplanten Stunden pro Tag ändert den geplanten Umsatz eines Projekts nicht, wenn der Abrechnungssatz des Aufgabengebiets nicht geändert wird oder wenn nur eine Überschreibung des Abrechnungssatzes erfolgt. Selbst wenn zwei Benutzer aus zwei verschiedenen Zeitzonen unterschiedliche geplante Stunden pro Tag sehen, sind die geplanten Gesamteinnahmen des Projekts zwischen den beiden Benutzern identisch.

  Bei mehreren Überschreibungen des Abrechnungssatzes kann der **Geplante Umsatz** des Projekts für zwei Benutzer in zwei verschiedenen Zeitzonen jedoch unterschiedlich aussehen, da er von der Menge der geplanten Stunden pro Tag (die für die beiden Benutzer unterschiedlich sein könnte) und der Überschreibungsrate (die für denselben Tag unterschiedlich sein könnte, wenn jeder Benutzer die Aufgabe in seiner eigenen Zeitzone betrachtet) abhängt.

* Der genaue **Geplanter Umsatz** ist der Betrag, der von der Benutzerin bzw. dem Benutzer gesehen wird, die/der dieselbe Zeitzone wie die Zeitzone Ihrer Workfront-Instanz hat. Ihr Workfront-Administrator definiert die Workfront-Zeitzone im Bereich „System-Kundeninformationen“.\
  Weitere Informationen zum Definieren der Zeitzone für Ihr System finden Sie im Artikel [Konfigurieren grundlegender Informationen für Ihr System](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Berechnen des tatsächlichen Umsatzes für Benutzer in verschiedenen Zeitzonen {#calculate-actual-revenue-for-users-in-different-time-zones}

Beachten Sie bei der Berechnung der tatsächlichen Einnahmen für Benutzer in verschiedenen Zeitzonen Folgendes:

* Wenn der **Umsatztyp** einer Aufgabe &quot;**pro Stunde“**, multipliziert Workfront die **Ist-Stunden** der Aufgabe mit dem Abrechnungssatz der Aufgabengebiete, die der Aufgabe zugewiesen wurden, um den **Ist-Umsatz**. Tatsächliche Stunden sind Stunden, die direkt in der Aufgabe protokolliert werden.

* Bei Überschreibungen mehrerer Abrechnungssätze verwendet Workfront den Abrechnungssatz des Aufgabengebiets, dessen Zeitrahmen mit dem **Eingabedatum) der** für die Aufgabe übereinstimmt, um den **tatsächlichen Umsatz** zu berechnen.

* Da für protokollierte Stunden kein Zeitstempel am **Eingabedatum** und für die Datumsbereiche mehrerer Überschreibungen von Abrechnungssätzen kein Zeitstempel vorhanden ist, sind **Berechnungen des tatsächlichen** von der Zeitzone, die mit Benutzenden verknüpft ist, nicht betroffen.

Weitere Informationen dazu, welches Aufgabengebiet zur Berechnung des **tatsächlichen Umsatzes** verwendet wird, finden Sie im Abschnitt „Grundlagen zu Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Projektfinanzen neu berechnen

Finanzen werden für ein Projekt berechnet, wenn Änderungen in den für das Projekt protokollierten Stunden auftreten.

Wenn Sätze während der Laufzeit eines Projekts geändert werden, können Sie Kosten und Einnahmen für das Projekt manuell neu berechnen, indem Sie die Option Finanzen neu berechnen für ein Projekt verwenden. Darüber hinaus wird bei einigen Aktionen eine automatische Neuberechnung Trigger.

Weitere Informationen zur Neuberechnung der Projektfinanzen finden Sie im Artikel [Neuberechnen der Projektfinanzen](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Hinzufügen eines neuen Abrechnungssatzes mithilfe der API

Um mithilfe der API einen neuen Abrechnungssatz für ein Aufgabengebiet hinzuzufügen, führen Sie eine Aktion *setRatesForRole* für das Objekt **Rate** mithilfe der Methode *PUT*.
Die Aktion und die Datumsfelder im Objekt **Rate** sind in der API-Version 8.0 verfügbar.
Wenn Sie bereits mehrere Abrechnungssätze für ein Aufgabengebiet in einem Projekt definiert haben und einen neuen Abrechnungssatz mit einem neuen Datumsbereich hinzufügen möchten, müssen Sie sowohl den vorhandenen Satz als auch den Satz einbeziehen, der in demselben API-Aufruf hinzugefügt werden soll. Dies ähnelt dem Aktualisieren von Sammlungen auf Objekten.

Der folgende API-Aufruf ist ein Beispiel, wobei **attachableID** die **Projekt-ID** des Projekts ist, bei dem Sie den Satz hinzufügen, und **RoleID** die **Aufgabengebiet-ID** ist, für die Sie den neuen Abrechnungssatz hinzufügen.<pre>{</pre><pre>„attachableID“:„593f01500000557d75fdd4fdfcc624f2“,</pre><pre>„attachableObjCode“:„PROJ“,</pre><pre>„roleID“:„544820df000014148cda5136d4b79d09“, </pre><pre>„Tarife“:[</pre><pre>         {„rateValue“:„0.00“,„startDate“:null,„endDate“:„2017-06-11“},</pre><pre>         {„rateValue“:„45.00“,„startDate“:„2017-06-12“,„endDate“:„2017-06-17“},</pre><pre>         {„rateValue“:„95.00“,„startDate“:„2017-06-21“,„endDate“:null}</pre><pre>]</pre><pre>}</pre>Weitere Informationen zur Verwendung der Workfront-API finden Sie im Artikel [API-Grundlagen](https://experience.workfront.com/s/article/API-Basics-638808549).
