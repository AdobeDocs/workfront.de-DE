---
content-type: reference
navigation-topic: workfront-navigation
title: Übersicht über die Projekt-, Aufgaben- und Problemdaten in [!DNL Workfront]
description: Dieser Artikel enthält Definitionen zu den häufigsten Daten, die mit Projekten, Aufgaben und Problemen in [!DNL Adobe Workfront] verknüpft sind.
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Übersicht über die Projekt-, Aufgaben- und Problemdaten in [!DNL Workfront]

<!-- Audited: 05/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc) </p>
-->

Dieser Artikel enthält Definitionen zu den häufigsten Daten, die mit Projekten, Aufgaben und Problemen in [!DNL Adobe Workfront] verknüpft sind. Die hier enthaltenen Bilder zeigen, wo die Daten in Workfront angezeigt werden und nicht vollständig sind. Es gibt andere Bereiche, in denen die Daten angezeigt werden. Alle Daten sind auch in Projekt-, Aufgaben- und Problemberichten und Listen sichtbar.

Informationen zu Berichten und Listen finden Sie in den folgenden Artikeln:

* [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [Erste Schritte mit Berichten](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

Weitere Informationen zu Projekt-, Aufgaben- und Problemfeldern finden Sie im [Glossar der  [!DNL Adobe Workfront] Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## [!UICONTROL Geplantes Startdatum]

Das [!UICONTROL geplante Startdatum] ist das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem beginnen soll.

Abhängig von der [!UICONTROL Task Constraint] können Sie das [!UICONTROL geplante Startdatum] einer Aufgabe möglicherweise nicht bearbeiten. Je nach dem [!UICONTROL Planmodus] des Projekts können Sie möglicherweise das [!UICONTROL geplante Startdatum] eines Projekts nicht bearbeiten.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Geplantes Startdatum]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

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

## [!UICONTROL Einstiegsdatum]

Das [!UICONTROL Einstiegsdatum] ist das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem in Workfront erstellt wurde.

Das [!UICONTROL Einstiegsdatum] hat keinen Einfluss auf die Zeitleiste von Projekten, Aufgaben oder Problemen, aber es ist für Tracking- und Berichtszwecke wichtig. [!DNL Workfront] generiert automatisch das [!UICONTROL Entrypdatum], wenn das Objekt erstellt wird, und Sie können es nicht manuell bearbeiten.

![](assets/entry-date-in-task-details-highlighted-nwe.png)

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

## [!UICONTROL Datum der Übermittlung]

Das [!UICONTROL Datum für die Übermittlung] ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen. Dies unterscheidet sich vom [!UICONTROL geplanten Abschlussdatum], da es eine realistischere Schätzung des Abschlussdatums ist, das nur vom Benutzer angegeben wird, der für die Arbeit verantwortlich ist. Weitere Informationen finden Sie unter [[!UICONTROL Commit Date] overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

>[!NOTE]
>
>Eine Änderung des [!UICONTROL Veröffentlichungsdatums] wirkt sich auf das [!UICONTROL vorgeschlagene Abschlussdatum] aus, nicht jedoch auf das [!UICONTROL geplante Abschlussdatum] einer Aufgabe oder eines Problems. Der Projektmanager kann die vom Verantwortlichen am [!UICONTROL Veröffentlichungsdatum] vorgenommenen Änderungen verwenden, um das [!UICONTROL geplante Abschlussdatum] einer Aufgabe oder eines Problems zu aktualisieren.

## [!UICONTROL Projiziertes Startdatum]

Das [!UICONTROL vorgeschlagene Startdatum] ist ein Echtzeit-Datum für den Beginn des Projekts, der Aufgabe oder des Problems und berücksichtigt alle Verzögerungen. Dies ist ein genaueres Startdatum für das Projekt, die Aufgabe oder das Problem als das geplante Startdatum [!UICONTROL 1}. ] Das [!UICONTROL geplante Startdatum] berücksichtigt keine Verzögerungen oder vergangene Daten.

Wenn Sie ein Projekt zum ersten Mal planen, sind das [!UICONTROL geplante Startdatum] und das [!UICONTROL vorgeschlagene Startdatum] der Aufgaben und des Projekts identisch. Da Verzögerungen auftreten können oder Aufgaben früher abgeschlossen werden können, kann sich das [!UICONTROL vorgeschlagene Startdatum] vom [!UICONTROL geplanten Startdatum] unterscheiden.

Bei einer Aufgabe kann sich das vorgeschlagene Startdatum ] auch vom geplanten Startdatum [!UICONTROL unterscheiden, wenn einer ihrer Vorgänger hinter dem Zeitplan liegt.

>[!TIP]
>
>Sie können das [!UICONTROL vorgeschlagene Startdatum] eines Problems nur in einer Liste oder einem Bericht anzeigen.

Weitere Informationen finden Sie unter [Überblick über das Projekt [!UICONTROL Projiziertes Startdatum]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

## [!UICONTROL Voraussichtliches Abschlussdatum]

Das [!UICONTROL vorgeschlagene Abschlussdatum] ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das [!UICONTROL vorgeschlagene Abschlussdatum] in das Datum des [!UICONTROL tatsächlichen Abschlussdatums].

Wenn alles reibungslos und wie geplant verläuft, sollte das [!UICONTROL vorgeschlagene Abschlussdatum] mit dem [!UICONTROL geplanten Abschlussdatum] übereinstimmen. Andernfalls kann sich das geplante Abschlussdatum ] aufgrund der Verzögerungen bei den Vorgängeraufgaben vom [!UICONTROL geplanten Abschlussdatum] unterscheiden.[!UICONTROL 

Weitere Informationen finden Sie unter [Überblick über das [!UICONTROL vorgeschlagene Abschlussdatum] für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL Stunden des Einstiegsdatums]

Wenn Sie die Zeit für Projekte, Aufgaben und Probleme protokollieren, um anzugeben, wie viel Zeit (in Stunden) Sie mit der Arbeit an dem Projekt, der Aufgabe oder dem Problem verbringen, wird die Zeit, die Sie protokollieren, zur [!UICONTROL tatsächlichen Stunde] des Projekts, der Aufgabe oder des Problems.

Das Datum, für das Sie die Uhrzeit protokollieren, ist das Feld [!UICONTROL Stündliches Einstiegsdatum] für den Stundeneintrag. In einigen Stundenlisten und Berichten wird das stündliche Einstiegsdatum als Datum angezeigt.

>[!TIP]
>
>Das [!UICONTROL Stunden-Einstiegsdatum] unterscheidet sich vom [!UICONTROL Einstiegsdatum] insofern, als es sich nicht um das Datum der Erstellung des Stundenprotokolls, sondern um das Datum handelt, mit dem die Stunden verknüpft werden sollen.

Sie können die Zeit in den folgenden Bereichen von Workfront protokollieren und anzeigen:

* Protokollieren und Anzeigen der Zeit im Abschnitt [!UICONTROL Projekt], [!UICONTROL Aufgabe] oder [!UICONTROL Problemaktualisierungen] oder im Abschnitt [!UICONTROL Stunden] . Bei der Protokollierung der Zeit im Abschnitt [!UICONTROL Stunden] können Sie manuell das Einstiegsdatum und den Benutzer, zu dem die Stunden gehören, angeben.

  ![](assets/log-time-box-task-hours-section-nwe-350x500.png)

  Weitere Informationen finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).

  >[!TIP]
  >
  >Es wird empfohlen, keine übergeordneten Aufgaben oder Projekte mehr mit Arbeitsaufgaben und Problemen zu protokollieren. Die in den Arbeitsaufgaben protokollierte Zeit aggregiert zu den übergeordneten Aufgaben und zum Projekt als [!UICONTROL Tatsächliche Stunden] für die übergeordneten Aufgaben und das Projekt. Die bei Problemen angemeldete Zeit wird für das Projekt als [!UICONTROL Tatsächliche Stunden] berechnet.

* Protokollieren der Zeit im Aktualisierungsstream einer Aufgabe oder eines Problems.

  ![](assets/log-time-in-update-stream-task-nwe-350x185.png)

* Zeigen Sie die [!UICONTROL Stunden-Entrypages] in Stunden-Berichten und -Listen an.

  ![](assets/hour-entry-date-in-view-nwe-350x173.png)
