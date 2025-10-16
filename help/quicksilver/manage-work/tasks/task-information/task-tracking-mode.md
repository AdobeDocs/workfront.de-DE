---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über den Aufgabenverfolgungsmodus
description: Beim Erstellen oder Bearbeiten einer Aufgabe können Sie die Einstellung für den Überwachungsmodus einer Aufgabe anpassen, um zu steuern, wie und wann die Fortschrittsstatusanzeigen einer Aufgabe angezeigt werden. Adobe Workfront zeigt Statusanzeigen an, wenn Sie bestimmte Einstellungen für das Verfolgen des Aufgabenfortschritts konfigurieren.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 3%

---

# Übersicht über den Aufgabenverfolgungsmodus

<!-- Audited: 01/2024 -->

Beim Erstellen oder Bearbeiten einer Aufgabe können Sie die Einstellung für den Überwachungsmodus einer Aufgabe anpassen, um zu steuern, wie und wann die Fortschrittsstatusanzeigen einer Aufgabe angezeigt werden. Adobe Workfront zeigt Statusanzeigen an, wenn Sie bestimmte Einstellungen für das Verfolgen des Aufgabenfortschritts konfigurieren.

Weitere Informationen zum Fortschrittsstatus von Aufgaben finden Sie unter [Übersicht über den Aufgabenstatus](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Tracking-Modus-Optionen {#tracking-mode-options}

Als Aufgabenbesitzer oder Projekt-Manager können Sie auswählen, wie Workfront den Fortschrittsstatus für jede Aufgabe anzeigt. Informationen zum Festlegen des Tracking-Modus für Aufgaben finden Sie unter [Festlegen des Tracking-Modus für Aufgaben](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Sie können aus den folgenden Optionen auswählen:

* [Benutzer muss aktualisieren](#user-must-update)
* [Annahme: Pünktlich](#assume-on-time)
* [Späte Warnungen ignorieren](#ignore-late-warnings)
* [Automatisch vervollständigen](#auto-complete)
* [Vorgänger](#predecessor)

### Benutzer muss aktualisieren {#user-must-update}

Wenn diese Option ausgewählt ist, verwendet Workfront die protokollierten Werte für „Prozent abgeschlossen“ und „Tatsächliche Stunden“, um den Fortschrittsstatus der Aufgabe zu ermitteln. Dies ist die Standardoption.

### Annahme: Im Zeitplan {#assume-on-time}

Workfront geht davon aus, dass eine Aufgabe unabhängig vom aktuellen Abschlussstatus termingerecht abgeschlossen wird. Wenn die Aufgabe nicht rechtzeitig (am geplanten Abschlussdatum) abgeschlossen wird, geht Workfront automatisch von einem geplanten Abschlussdatum des nächsten Arbeitstages aus. Sie müssen weiterhin angeben, wann die Aufgabe abgeschlossen ist. Verwenden Sie diese Option, wenn Benutzer ihre Aufgaben nicht regelmäßig aktualisieren.

### Späte Warnungen ignorieren {#ignore-late-warnings}

Der Fortschrittsstatus einer Aufgabe ist Pünktlich, bis es zu spät ist. Wenn Sie beispielsweise eine Aufgabe so planen, dass sie 10 Tage dauert und an dem Tag, an dem sie abgeschlossen werden soll, 60 % der abgeschlossenen Aufgaben angezeigt werden, aktualisiert Workfront das voraussichtliche Abschlussdatum, indem vier Tage hinzugefügt werden. Der Fortschrittsstatus der Aufgabe wird zu „spät“.

### Automatisch abschließen {#auto-complete}

Workfront geht davon aus, dass Aufgaben wie geplant erledigt werden, und markiert sie als erledigt am fälligen oder geplanten Abschlussdatum. Bis dahin verwendet Workfront die Protokollierung von Prozent abgeschlossen und Tatsächliche Stunden, um den Fortschrittsstatus zu bestimmen. Unabhängig vom Fortschrittsstatus vor dem geplanten Abschlussdatum markiert Workfront die Aufgabe jedoch weiterhin als abgeschlossen.

Die folgenden Ausnahmen sind vorhanden:

* Wenn die Aufgabe unvollständige Vorgänger hat, wird sie erst automatisch abgeschlossen, wenn alle ihre Vorgänger abgeschlossen sind. Vorgänger müssen durchgesetzt werden.
* Wenn für den Vorgang ein festes Datum gilt, wird der Vorgang immer am geplanten Abschlussdatum abgeschlossen, unabhängig davon, ob die Vorgänger abgeschlossen sind.

>[!IMPORTANT]
>
>Wenn Sie auswählen, dass Aufgaben automatisch abgeschlossen werden sollen, wird die Aufgabe als abgeschlossen markiert, wenn die Projektzeit neu berechnet wird. Wenn der Aktualisierungstyp des Projekts auf „Automatisch“ oder „Automatisch“ und „Bei Änderung“ festgelegt ist, wird die Zeitleiste des Projekts täglich berechnet. Informationen zu Neuberechnungen der Zeitleiste für Projekte finden Sie unter [Neuberechnen von Projektzeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>Der Zeitpunkt des tatsächlichen Abschlussdatums ist Mitternacht des Tages, an dem die Timeline automatisch berechnet wird. Die Zeit, die zum Generieren dieses Zeitstempels verwendet wird, ist die Zeitzone Ihres Systems, wie sie von Ihrem Workfront-Administrator im Abschnitt „Kundeninformationen“ von Setup definiert wurde. Informationen zum Festlegen der Zeitzone Ihres Systems finden Sie unter [Konfigurieren grundlegender Informationen für Ihr System](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Vorgänger {#predecessor}

Workfront schätzt das voraussichtliche Abschlussdatum einer Aufgabe entsprechend ihrer Vorgängerbeziehung. Der Fortschrittsstatus einer Aufgabe wird auf Grundlage dieser Schätzung bestimmt. Beispielsweise hat Aufgabe B eine Dauer von 1 Tag und soll zwei Tage nach dem Vorgänger von Aufgabe A abgeschlossen werden, was fünf Tage dauern sollte. Ein Benutzer aktualisiert dann Aufgabe B auf 50 % abgeschlossen, aber der Vorgänger, Aufgabe A, hat noch nicht begonnen. Workfront plant den Abschluss der abhängigen Aufgabe B sechs Tage nach dem Startdatum der Vorgängeraufgabe. Dabei werden 5 Tage für Aufgabe A und 1 Tag für Aufgabe B eingeräumt.
