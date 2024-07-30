---
content-type: reference
navigation-topic: workfront-navigation
title: Übersicht über die Projekt-, Aufgaben- und Problemdaten in [!DNL Workfront]
description: Dieser Artikel enthält Definitionen zu den häufigsten Daten, die mit Projekten, Aufgaben und Problemen in [!DNL Adobe Workfront] verknüpft sind.
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 6f1f669f7e2235637864a92a40aadbfb19b4310b
workflow-type: tm+mt
source-wordcount: '2301'
ht-degree: 3%

---

# Übersicht über die Projekt-, Aufgaben- und Problemdaten in [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

Dieser Artikel enthält Definitionen zu den häufigsten Daten, die mit Projekten, Aufgaben und Problemen in [!DNL Adobe Workfront] verknüpft sind. Die hier enthaltenen Bilder zeigen, wo die Daten in Workfront angezeigt werden und nicht vollständig sind. Es gibt andere Bereiche, in denen die Daten angezeigt werden. Alle Daten sind auch in Projekt-, Aufgaben- und Problemberichten und Listen sichtbar.

Informationen zu Berichten und Listen finden Sie in den folgenden Artikeln:

* [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Erste Schritte mit Berichten](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Weitere Informationen zu Projekt-, Aufgaben- und Problemfeldern finden Sie unter [Glossar der  [!DNL Adobe Workfront] Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).


## [!UICONTROL Tatsächliches Startdatum]

Das [!UICONTROL tatsächliche Startdatum] ist das Datum, an dem ein Benutzer mit der Bearbeitung eines Projekts, einer Aufgabe oder eines Problems beginnt. Das [!UICONTROL tatsächliche Startdatum] ist beim Erstellen des Projekts, der Aufgabe oder des Problems leer.

Sie können manuell angeben, wann die Arbeit an einer Aufgabe oder einem Problem gestartet wurde, oder das [!UICONTROL tatsächliche Startdatum] wird automatisch ausgefüllt, wenn sich der Status der Aufgabe oder des Problems von [!UICONTROL Neu] in [!UICONTROL In Bearbeitung] oder [!UICONTROL Abgeschlossen] ändert. Das [!UICONTROL tatsächliche Startdatum] eines Projekts entspricht dem Datum, an dem die erste Aufgabe des Projekts gestartet wird.

>[!TIP]
>
>Das [!UICONTROL tatsächliche Startdatum] entspricht möglicherweise nicht dem [!UICONTROL geplanten Startdatum] eines Projekts, einer Aufgabe oder eines Problems, da der Benutzer seine Arbeit möglicherweise später oder früher als geplant starten kann.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Tatsächliches Startdatum]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md).

>[!NOTE]
>
>Die &quot;[!UICONTROL Muss am]&quot;-Aufgabe oder die Beschränkungen für &quot;Feste Datumswerte&quot;wirken sich auf das &quot;[!UICONTROL geplante Startdatum]&quot; einer Aufgabe aus, nicht auf das &quot;[!UICONTROL tatsächliche Startdatum]&quot;. Dadurch wird das geplante Startdatum [!UICONTROL 1} auf ein von Ihnen angegebenes Datum aktualisiert. ] Das [!UICONTROL tatsächliche Startdatum] wird unabhängig vom [!UICONTROL geplanten Startdatum] aktualisiert, wie oben beschrieben.

![](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL Tatsächliches Abschlussdatum]

Das [!UICONTROL tatsächliche Abschlussdatum] ist das Datum, an dem ein Benutzer ein Projekt, eine Aufgabe oder ein Problem tatsächlich abgeschlossen hat. Das [!UICONTROL tatsächliche Abschlussdatum] ist beim Erstellen des Projekts, der Aufgabe oder des Problems leer.

Sie können manuell angeben, wann die Arbeit an einer Aufgabe oder einem Problem abgeschlossen ist, oder das [!UICONTROL tatsächliche Abschlussdatum] wird automatisch ausgefüllt, wenn eines der folgenden Ereignisse eintritt:

* Der Projekt-, Aufgaben- oder Problemstatus ändert sich in &quot;[!UICONTROL Complete]&quot;, &quot;[!UICONTROL Closed]&quot;oder &quot;[!UICONTROL Resolved]&quot;.
* Der prozentuale Abschluss der Aufgabe bzw. des Projekts beträgt 100 %.

Das [!UICONTROL tatsächliche Abschlussdatum] eines Projekts entspricht dem Datum, an dem Sie die letzte Aufgabe im Projekt abgeschlossen haben.

>[!TIP]
>
>Das [!UICONTROL tatsächliche Abschlussdatum] stimmt möglicherweise nicht mit dem [!UICONTROL geplanten Abschlussdatum] überein.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Tatsächliches Abschlussdatum]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

![](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## Genehmigungspfad – Abschlussdatum

Das Abschlussdatum des Genehmigungspfads ist das Datum, an dem die Genehmigung eines Projekts, einer Aufgabe oder eines Problems erteilt und der Status des Elements geändert wurde.

Das Abschlussdatum des Genehmigungspfads wird in Projekt-, Aufgaben- und Problemlisten und Berichten angezeigt.

## Genehmigungspfad – Startdatum

Das Startdatum des Genehmigungspfads ist das Datum, an dem das Projekt, die Aufgabe oder der Ausgabestatus in &quot;Genehmigung ausstehend&quot;geändert und die Projektgenehmigungsanforderung an die Genehmiger gesendet wurde.

Das Startdatum des Genehmigungspfads ist in Projekt-, Aufgaben- und Problemlisten und Berichten sichtbar.

<!--## Auto Closure Date -->

## Budgetiertes Abschlussdatum

Dies ist ein veraltetes Feld für Projekte. Alle Informationen, die dieses Feld in einer Liste oder einem Bericht anzeigen kann, beziehen sich auf eine Funktion, die von Workfront entfernt wurde. Dieses Feld kann nicht aktualisiert werden.

Das Feld ist in Projektberichten und -listen sichtbar.

## Budgetiertes Startdatum

Dies ist ein veraltetes Feld für Projekte. Alle Informationen, die in diesem Feld angezeigt werden, beziehen sich auf eine Funktion, die von Workfront entfernt wurde. Dieses Feld kann nicht aktualisiert werden.

Das Feld ist in Projektberichten und -listen sichtbar.

## [!UICONTROL Datum der Übermittlung]

Das [!UICONTROL Datum für die Übermittlung] ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen. Dies unterscheidet sich vom [!UICONTROL geplanten Abschlussdatum], da es eine realistischere Schätzung des Abschlussdatums ist, das nur vom Benutzer angegeben wird, der für die Arbeit verantwortlich ist. Weitere Informationen finden Sie unter [[!UICONTROL Commit Date] overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

>[!NOTE]
>
>Eine Änderung des [!UICONTROL Veröffentlichungsdatums] wirkt sich auf das [!UICONTROL vorgeschlagene Abschlussdatum] aus, nicht jedoch auf das [!UICONTROL geplante Abschlussdatum] einer Aufgabe oder eines Problems. Der Projektmanager kann die vom Verantwortlichen am [!UICONTROL Veröffentlichungsdatum] vorgenommenen Änderungen verwenden, um das [!UICONTROL geplante Abschlussdatum] einer Aufgabe oder eines Problems zu aktualisieren.

<!--## Completion Pending Date-->

## Einschränkungsdatum

Wenn Sie eine Aufgabenbegrenzung verwenden, die an ein bestimmtes Datum gebunden ist, wird dieses spezifische Datum zum Beschränkungsdatum der Aufgabe.

Mit den folgenden Aufgabenbegrenzungen wird das Feld Beschränkungsdatum aktualisiert:

* Muss beginnen am
* Muss beendet werden am
* Nicht später anfangen als
* Nicht früher anfangen als

>[!TIP]
>
>Eine Aufgabe mit einer Begrenzung von festen Datumswerten hat kein Beschränkungsdatum.
>

Das Beschränkungsdatum wird in einer Aufgabenliste oder einem Bericht angezeigt.

## Problem-Eingabedatum konvertiert

Das Datum, an dem das Problem, das in das Projekt oder die Aufgabe konvertiert wurde, erstellt wurde.

Das Einstiegsdatum des konvertierten Problems ist in Projekt-, Aufgabenlisten und Berichten sichtbar.

## Fälligkeitsdatum

Das Datum, an dem eine Aufgabe oder ein Problem abgeschlossen werden soll. Das Fälligkeitsdatum einer Aufgabe oder eines Problems ist dasselbe Datum wie das geplante Abschlussdatum.

Die Aufgabe und das Problem Fälligkeitsdatum sind in den Aufgaben- und Problemlisten und Berichten sichtbar.

Weitere Informationen finden Sie im Abschnitt [Geplantes Abschlussdatum](#planned-completion-date) in diesem Artikel.

## Fällig am

Das Datum, an dem das Projekt abgeschlossen sein soll. Das Fälligkeitsdatum eines Projekts ist dasselbe Datum wie das geplante Abschlussdatum des Projekts.

Das Projekt Fälligkeitsdatum ist in Projektlisten und Berichten sichtbar.

Weitere Informationen finden Sie im Abschnitt [Geplantes Abschlussdatum](#planned-completion-date) in diesem Artikel.

## [!UICONTROL Einstiegsdatum]

Das [!UICONTROL Einstiegsdatum] ist das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem in [!DNL Workfront] erstellt wurde.

Das [!UICONTROL Einstiegsdatum] hat keinen Einfluss auf die Zeitleiste von Projekten, Aufgaben oder Problemen, aber es ist für Tracking- und Berichtszwecke wichtig. [!DNL Workfront] generiert automatisch das [!UICONTROL Entrypdatum], wenn das Objekt erstellt wird, und Sie können es nicht manuell bearbeiten.

![](assets/entry-date-in-task-details-highlighted-nwe.png)

## Geschätztes Fälligkeitsdatum

Das geschätzte Fälligkeitsdatum der Aufgabe und des Projekts zeigt ein realistischeres Datum für den Zeitpunkt, zu dem das Projekt oder die Aufgabe abgeschlossen werden soll.

Die geschätzten Daten entsprechen eher der Realität des Projekts und der Aufgabe, da sie berücksichtigen, welche Auswirkungen auf die tatsächliche Fertigstellung des Projekts oder der Aufgabe haben. Die geschätzten Fälligkeitsdaten ähneln den prognostizierten Abschlussdaten.

Weitere Informationen finden Sie unter [Überblick über die prognostizierten und geschätzten Datumswerte](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Das Projekt und die Aufgabe Geschätzte Fälligkeitsdaten sind in Projekt- und Aufgabenlisten und Berichten sichtbar.

## Voraussichtliches Startdatum

Das geschätzte Startdatum der Aufgabe und des Projekts zeigt ein realistischeres Datum für den Beginn des Projekts oder der Aufgabe.

Die voraussichtlichen Daten entsprechen eher der Realität des Projekts und der Aufgabe, da sie berücksichtigen, was den tatsächlichen Beginn des Projekts oder der Aufgabe beeinflusst. Die geschätzten Startdaten ähneln den prognostizierten Startdaten.

Weitere Informationen finden Sie unter [Überblick über die prognostizierten und geschätzten Datumswerte](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md).

Das Projekt und die Aufgabe Geschätzte Startdaten sind in Projekt- und Aufgabenlisten und Berichten sichtbar.

<!--## Exchange Rate Date-->

## Festes Enddatum

Der Projektanfragende oder Projektinhaber identifiziert beim Abschließen des Geschäftsfeldes das Festende Enddatum eines Projekts. Es ist das Datum, bis zu dem sie empfehlen, das Projekt abzuschließen.

Dies ist eine manuelle Schätzung, bei der der tatsächliche Fortschritt der Aufgaben im Projekt nicht berücksichtigt wird.

Das feste Enddatum eines Projekts ist im Abschnitt &quot;Geschäftsszenario&quot;des Projekts sowie in Projektlisten und Berichten sichtbar.

![](assets/fixed-end-date-business-case-highlight.png)

## Festes Startdatum

Der Projektanfragende oder -eigentümer identifiziert beim Abschließen des Geschäftsszenarios das feste Startdatum eines Projekts. Es ist das Datum, an dem sie empfehlen, mit dem Projekt zu beginnen.

Dies ist eine manuelle Schätzung, bei der der tatsächliche Fortschritt der Aufgaben im Projekt nicht berücksichtigt wird.

Das feste Startdatum eines Projekts ist im Abschnitt &quot;Geschäftsszenario&quot;des Projekts sowie in Projektlisten und Berichten sichtbar.

![](assets/fixed-start-date-business-case-highlight.png)

## Übergabedatum

Das Datum, an dem eine Aufgabe zur Arbeit verfügbar wird. Dies bedeutet, dass alle Begrenzungen, Genehmigungen und Abhängigkeiten abgeschlossen sind und Benutzer mit der Arbeit beginnen können.

Das Übergabedatum ist eine Berechnung, die nicht manuell festgelegt werden kann.

Weitere Informationen zum Übergabedatum finden Sie unter [Übersicht über das Übergabedatum für Aufgaben](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md).

Das Übergabedatum einer Aufgabe wird in Aufgabenlisten und Berichten angezeigt.

## Datum der letzten Finanzaktualisierung

Das Datum, an dem die Finanzinformationen zu einem Projekt aktualisiert wurden. Dazu gehört die Aktualisierung von Finanzfeldern im Abschnitt &quot;Finanzen&quot;oder im Abschnitt &quot;Geschäftsfall&quot;des Projekts.

Das Datum der letzten Finanzaktualisierung ist in Projektlisten und Berichten sichtbar.

## Datum der letzten Aktualisierung

Das Datum, an dem das Projekt, die Aufgabe oder das Problem zuletzt aktualisiert wurde Eine Aktualisierung gilt als Änderung, bei der ein Projekt, eine Aufgabe oder ein Problem zur Speicherung Trigger wird. Dazu gehören Änderungen von Status, Bedingung, Timeline, Finanzen oder anderen Feldern.

Das Datum der letzten Aktualisierung ist in Projekt-, Aufgaben- und Problemlisten und Berichten sichtbar.

## [!UICONTROL Stunden des Einstiegsdatums]

Wenn Sie die Zeit für Projekte, Aufgaben und Probleme protokollieren, um anzugeben, wie viel Zeit (in Stunden) Sie mit der Arbeit an dem Projekt, der Aufgabe oder dem Problem verbringen, wird die Zeit, die Sie protokollieren, zur [!UICONTROL tatsächlichen Stunde] des Projekts, der Aufgabe oder des Problems.

Das Datum, für das Sie die Uhrzeit protokollieren, ist das Feld [!UICONTROL Stündliches Einstiegsdatum] für den Stundeneintrag.

Das stündliche Einstiegsdatum wird in Stunden-Listen und Berichten angezeigt.

>[!TIP]
>
>Das [!UICONTROL Einstiegsdatum] einer Stunde unterscheidet sich vom [!UICONTROL Einstiegsdatum] eines anderen Workfront-Objekts insofern, als es sich nicht um das Datum der Erstellung des Stundenprotokolls, sondern um das Datum handelt, mit dem die Stunden verknüpft werden sollen.
>
>Sie können beispielsweise Stunden für eine Aufgabe am 5. September protokollieren, die Stunden jedoch mit dem 1. September verknüpfen. Das Entrypdatum der Stunde ist der 1. September.

Informationen zur Protokollzeit in Workfront finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Es wird empfohlen, keine übergeordneten Aufgaben oder Projekte mehr mit Arbeitsaufgaben und Problemen zu protokollieren. Die in den Arbeitsaufgaben protokollierte Zeit aggregiert zu den übergeordneten Aufgaben und zum Projekt als [!UICONTROL Tatsächliche Stunden] für die übergeordneten Aufgaben und das Projekt. Die bei Problemen angemeldete Zeit wird für das Projekt als [!UICONTROL Tatsächliche Stunden] berechnet.

## [!UICONTROL Geplantes Abschlussdatum]

Das Datum [!UICONTROL Geplantes Abschlussdatum] oder das Datum [!UICONTROL Fällig am] ist das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem abgeschlossen werden soll.

Abhängig von der [!UICONTROL Task Constraint] können Sie das [!UICONTROL geplante Abschlussdatum] einer Aufgabe möglicherweise nicht bearbeiten. Je nach dem [!UICONTROL Zeitplan-Modus] des Projekts können Sie möglicherweise das [!UICONTROL geplante Abschlussdatum] eines Projekts nicht bearbeiten.

Das geplante Abschlussdatum ] wird in einigen Bereichen von [!DNL Workfront] als Fälligkeitsdatum angezeigt.[!UICONTROL 

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Übersicht über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Festlegen des geplanten Abschlussdatums für das Projekt ](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Überblick über das Problem [!UICONTROL Geplantes Abschlussdatum]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## Ausrichtung am geplanten Datum

Dies ist ein automatischer Indikator, mit dem Workfront Projekte, Aufgaben und Probleme zuweist, um anzuzeigen, wann ein Element in Bezug auf das geplante Abschlussdatum abgeschlossen wird.

Die folgenden Werte sind für den Indikator Geplante Datumsausrichtung möglich:

* Wird zum geplanten Abschlussdatum fertiggestellt
* Wird vor dem geplanten Abschlussdatum fertiggestellt
* Wird nach dem geplanten Abschlussdatum fertiggestellt

Die geplante Datumsausrichtung ist in Projekt-, Aufgaben- und Problemlisten und Berichten sichtbar.

## [!UICONTROL Geplantes Startdatum]

Das [!UICONTROL geplante Startdatum] ist das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem beginnen soll.

Abhängig von der [!UICONTROL Task Constraint] können Sie das [!UICONTROL geplante Startdatum] einer Aufgabe möglicherweise nicht bearbeiten. Je nach dem [!UICONTROL Planmodus] des Projekts können Sie möglicherweise das [!UICONTROL geplante Startdatum] eines Projekts nicht bearbeiten.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Geplantes Startdatum]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL Voraussichtliches Abschlussdatum]

Das [!UICONTROL vorgeschlagene Abschlussdatum] ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das [!UICONTROL vorgeschlagene Abschlussdatum] in das Datum des [!UICONTROL tatsächlichen Abschlussdatums].

Wenn alles reibungslos und wie geplant verläuft, sollte das [!UICONTROL vorgeschlagene Abschlussdatum] mit dem [!UICONTROL geplanten Abschlussdatum] übereinstimmen. Andernfalls kann sich das geplante Abschlussdatum ] aufgrund der Verzögerungen bei den Vorgängeraufgaben vom [!UICONTROL geplanten Abschlussdatum] unterscheiden.[!UICONTROL 

Weitere Informationen finden Sie unter [Überblick über das [!UICONTROL vorgeschlagene Abschlussdatum] für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Projiziertes Startdatum]

Das [!UICONTROL vorgeschlagene Startdatum] ist ein Echtzeit-Datum für den Beginn des Projekts, der Aufgabe oder des Problems und berücksichtigt alle Verzögerungen. Dies ist ein genaueres Startdatum für das Projekt, die Aufgabe oder das Problem als das geplante Startdatum [!UICONTROL 1}. ] Das [!UICONTROL geplante Startdatum] berücksichtigt keine Verzögerungen oder vergangene Daten.

Wenn Sie ein Projekt zum ersten Mal planen, sind das [!UICONTROL geplante Startdatum] und das [!UICONTROL vorgeschlagene Startdatum] der Aufgaben und des Projekts identisch. Da Verzögerungen auftreten können oder Aufgaben früher abgeschlossen werden können, kann sich das [!UICONTROL vorgeschlagene Startdatum] vom [!UICONTROL geplanten Startdatum] unterscheiden.

Bei einer Aufgabe kann sich das vorgeschlagene Startdatum ] auch vom geplanten Startdatum [!UICONTROL unterscheiden, wenn einer ihrer Vorgänger hinter dem Zeitplan liegt.

>[!TIP]
>
>Sie können das [!UICONTROL vorgeschlagene Startdatum] eines Problems nur in einer Liste oder einem Bericht anzeigen.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Projiziertes Startdatum]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## Slack-Datum

Aufgaben können manchmal erst spät beginnen und abgeschlossen werden, ohne dass sich dies auf das Abschlussdatum des Projekts auswirkt.

Das Slack-Datum zeigt das genaue Datum an, an dem eine Aufgabe das Abschlussdatum des Projekts definitiv beeinflussen könnte.

Informationen zum Slack-Datum einer Aufgabe finden Sie unter [Task Slack Date overview](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md).

Aufgabendaten werden in Aufgabenlisten und Berichten angezeigt.

## Starten am

Das Datum, an dem das Projekt beginnen soll. Das Datum des Projektstarts ist das Datum des geplanten Projektstarts.

Dieses Feld ist in Projektlisten und Berichten sichtbar.

Weitere Informationen finden Sie im Abschnitt [Geplantes Startdatum](#planned-start-date) in diesem Artikel.



