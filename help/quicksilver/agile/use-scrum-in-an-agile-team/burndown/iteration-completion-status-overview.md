---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Übersicht über den Iteration-Abschlussstatus
description: Die in diesem Artikel beschriebenen Vervollständigungsinformationen werden oberhalb der Abbruchgrafik angezeigt.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Übersicht über den Iteration-Abschlussstatus

Die in diesem Artikel beschriebenen Vervollständigungsinformationen werden oberhalb der Abbruchgrafik angezeigt.

Abschlussprozentsatz bei einer Iteration:

![](assets/burndown-percentcomplete-350x47.png)

Diese Informationen geben den Abschlussstatus der Iteration für den Tag an, der aktuell in der Abbruchgrafik ausgewählt ist. Standardmäßig wird der Abschlussstatus basierend auf dem Datum des aktuellen Tages angezeigt.

Die folgenden Informationen sind verfügbar:

* **[!UICONTROL Percent Complete]:** Gesamtfortschritt der Iteration

  [!UICONTROL Prozent abgeschlossen] passt sich an den prozentualen Abschluss jeder Geschichte oder Aufgabe innerhalb der Iteration an, einschließlich Geschichten oder Aufgaben, die nur teilweise abgeschlossen sind.

  Die Farbe der Statusleiste [!UICONTROL Prozent abgeschlossen] wird rot oder grün angezeigt, um der Farbe der tatsächlichen Abbruchrate zu entsprechen. Er wird rot angezeigt, wenn die Abbruchrate kleiner als das Ideal ist (mehr Punkte oder Stunden, die pro Tag verbleiben, als die ideale Abbruchberechnung), und grün angezeigt, wenn die Abbruchrate gleich oder besser als das Ideal ist (entspricht oder weniger Punkten, die pro Tag verbleiben, als die ideale Abbruchberechnung).

* **[!UICONTROL Abgeschlossene Geschichten]:** (Nur in Ausführungen verfügbar) Die Anzahl der Meldungen, die mit [!UICONTROL Abgeschlossen] markiert sind. Dies wird in Bezug auf die Gesamtzahl der Meldungen in der Iteration angezeigt. Beispielsweise zeigt &quot;3 von 6&quot;an, dass 3 der 6 Geschichten in der Iteration mit [!UICONTROL Complete] markiert wurden.
* **[!UICONTROL Abgeschlossene Punkte/Stunden]:** (Nur in Ausführungen verfügbar) Die Anzahl der Punkte oder Stunden, die mit [!UICONTROL Abgeschlossen] markiert sind. Wird in Bezug auf die Gesamtzahl der Punkte oder Stunden in der Iteration angezeigt. Beispielsweise zeigt &quot;5 von 11&quot;an, dass 5 der 11 Meldungen in der Iteration mit [!UICONTROL Complete] markiert wurden. Diese Zahl steht in direktem Zusammenhang zur Berechnung [!UICONTROL Prozent abgeschlossen] und wird gleichzeitig aktualisiert, wenn [!UICONTROL Prozent abgeschlossen] aktualisiert wird.

  Punkte und Stunden sind mit Geschichten verknüpft. Wenn eine Meldung mit [!UICONTROL Complete] markiert ist, werden die Punkte oder Stunden, die mit dieser Meldung verbunden sind, als &quot;Complete&quot;markiert.

  Standardmäßig werden Punkte verwendet. Sie können dies ändern, indem Sie die Einstellungen für Ihr Team ändern, wie unter [Erstellen eines agilen Teams](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md) beschrieben.

* **[!UICONTROL Punkte/Stunden pro Tag]:** (Nur in Ausführungen verfügbar) Die durchschnittliche Anzahl der Punkte oder Stunden, die an jedem Tag seit Beginn der Iteration durch den aktuellen Tag mit [!UICONTROL Complete] markiert sind.

  Dies wird anhand der Gesamtpunkte oder Stunden berechnet, die abgeschlossen sind, geteilt durch die Gesamtanzahl der Tage bis zum aktuellen Tag. (Teiltage werden als ganzer Tag aufgezeichnet.)

  Diese Informationen können bei der Planung einer zukünftigen Iteration nützlich sein.

* **[!UICONTROL Geschätzter Abschluss]:** Das geschätzte Datum, an dem die Iteration abgeschlossen wird, basierend auf der aktuellen Rate in den Punkten/Stunden pro Tag (für Iterationen).

  Wenn das Datum des [!UICONTROL geschätzten Abschlusses] nach dem für die Iteration definierten Enddatum liegt, wird die Anzahl der verbleibenden Arbeitstage in Klammern neben dem Datum des [!UICONTROL geschätzten Abschlusses] rot angezeigt.

  Wenn das Datum des [!UICONTROL geschätzten Abschlusses] vor dem geplanten Enddatum der Iteration liegt, wird die Anzahl der verbleibenden Arbeitstage grün angezeigt. (Das Enddatum für die Iteration wird bei der Planung der Iteration angegeben, wie unter [Iteration erstellen](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) beschrieben. Das Enddatum für das Projekt ist das [!UICONTROL geplante Abschlussdatum], oder es ist das aktuelle Datum, wenn das [!UICONTROL geplante Abschlussdatum] in der Vergangenheit liegt. Das [!UICONTROL geplante Abschlussdatum] für das Projekt wird anhand der Dauer der Aufgaben im Projekt berechnet.) Wenn Sie bei der Planung der Iteration das Enddatum der Iteration für einen nicht funktionierenden Tag festlegen und die Iteration die pünktliche Fertigstellung verfolgt, wird das geschätzte Abschlussdatum für den letzten Arbeitstag vor dem von Ihnen festgelegten Iterationsenddatum festgelegt (da die Arbeit nicht für Nichtarbeitstage geplant ist).

  Beispiel: &quot;(+9 Tage)&quot;gibt an, dass das geschätzte Abschlussdatum 9 Arbeitstage nach dem geplanten Enddatum der Iteration liegt.

  Weitere Informationen finden Sie unter [Übersicht über den Iteration-Abschlussstatus](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
