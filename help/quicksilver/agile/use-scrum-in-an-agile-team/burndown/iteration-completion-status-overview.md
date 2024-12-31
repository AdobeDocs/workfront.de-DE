---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Übersicht über den Abschlussstatus der Iteration
description: Die in diesem Artikel beschriebenen Informationen zum Abschluss werden über dem Burndown-Diagramm angezeigt.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Übersicht über den Abschlussstatus der Iteration

Die in diesem Artikel beschriebenen Informationen zum Abschluss werden über dem Burndown-Diagramm angezeigt.

Prozentsatz der Fertigstellung einer Iteration:

![](assets/burndown-percentcomplete-350x47.png)

Diese Informationen geben den Abschlussstatus der Iteration für den Tag an, der derzeit im Burndown-Diagramm ausgewählt ist. Standardmäßig wird der Abschlussstatus basierend auf dem aktuellen Datum angezeigt.

Folgende Informationen sind verfügbar:

* **[!UICONTROL Prozent abgeschlossen]:** Gesamtfortschritt der Iteration

  [!UICONTROL Prozent abgeschlossen] wird auf der Grundlage des Prozentsatzes der Fertigstellung jeder Story oder Aufgabe innerhalb der Iteration angepasst, einschließlich Storys oder Aufgaben, die nur teilweise abgeschlossen sind.

  Die Farbe der Statusleiste [!UICONTROL Prozent abgeschlossen] wird als Rot oder Grün angezeigt, um sie an die Farbe der tatsächlichen Burndown-Rate anzupassen. Er wird rot angezeigt, wenn die Burndown-Rate kleiner als das Ideal ist (mehr Punkte oder Stunden pro Tag als die ideale Burndown-Berechnung), und er wird grün angezeigt, wenn die Burndown-Rate gleich oder besser als das Ideal ist (gleich oder weniger Punkte pro Tag als die ideale Burndown-Berechnung).

* **[!UICONTROL Abgeschlossene Storys]:** (nur in Iterationen verfügbar) Die Anzahl der Storys, die als &quot;[!UICONTROL &quot; ] sind. Dies wird im Verhältnis zur Gesamtzahl der Storys in der Iteration angezeigt. Beispiel: „3 von 6“ zeigt an, dass 3 der 6 Geschichten in der Iteration als „Abgeschlossen[!UICONTROL  gekennzeichnet ].
* **[!UICONTROL Abgeschlossene Punkte/Stunden]:** (nur in Iterationen verfügbar) Die Anzahl der Punkte oder Stunden, die als &quot;[!UICONTROL &quot; ] sind. Wird im Verhältnis zur Gesamtzahl der Punkte oder Stunden in der Iteration angezeigt. Beispiel: „5 von 11“ zeigt an, dass 5 der 11 Geschichten in der Iteration als „Abgeschlossen[!UICONTROL  gekennzeichnet ]. Diese Zahl bezieht sich direkt auf die Berechnung [!UICONTROL Prozent abgeschlossen] und wird gleichzeitig mit der Aktualisierung [!UICONTROL Prozent abgeschlossen] aktualisiert.

  Punkte und Stunden sind mit Storys verknüpft. Wenn ein Artikel oder eine Story [!UICONTROL Abgeschlossen] gekennzeichnet ist, werden die mit diesem Artikel oder dieser Story verknüpften Punkte oder Stunden als Abgeschlossen markiert.

  Standardmäßig werden Punkte verwendet. Sie können dies ändern, indem Sie die Einstellungen für Ihr Team ändern, wie in [Erstellen eines agilen Teams](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md) beschrieben.

* **[!UICONTROL Punkte/Stunden pro Tag]:** (Nur in Iterationen verfügbar) Die durchschnittliche Anzahl der Punkte oder Stunden, die [!UICONTROL Abgeschlossen] jeden Tag seit Beginn der Iteration durch den aktuellen Tag markiert sind.

  Dies wird durch die Gesamtzahl der abgeschlossenen Punkte oder Stunden dividiert durch die Gesamtzahl der Tage bis zum aktuellen Tag berechnet. (Teiltage werden als ganzer Tag erfasst.)

  Diese Informationen können bei der Planung einer zukünftigen Iteration nützlich sein.

* **[!UICONTROL Geschätzter Abschluss]:** Das geschätzte Datum, an dem die Iteration abgeschlossen wird, basierend auf der aktuellen Rate in den Punkten/Stunden pro Tag (für Iterationen).

  Wenn das [!UICONTROL Geschätzte Abschlussdatum] nach dem für die Iteration definierten Enddatum liegt, wird die Anzahl der verbleibenden Arbeitstage in Klammern neben dem Datum [!UICONTROL Geschätzter Abschluss] angezeigt.

  Wenn das [!UICONTROL Geschätzte Abschlussdatum] vor dem geplanten Enddatum der Iteration liegt, wird die Anzahl der verbleibenden Arbeitstage grün angezeigt. (Das Enddatum für die Iteration wird bei der Planung der Iteration angegeben, wie in [Iteration erstellen](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) beschrieben. Das Enddatum für das Projekt ist das [!UICONTROL Geplantes Abschlussdatum] oder das aktuelle Datum, wenn das [!UICONTROL Geplantes Abschlussdatum] in der Vergangenheit liegt. Das [!UICONTROL geplante Abschlussdatum] für das Projekt wird anhand der Dauer der Aufgaben im Projekt berechnet.) Wenn Sie bei der Planung der Iteration das Enddatum der Iteration für einen arbeitsfreien Tag festgelegt haben und die Iteration so verfolgt, dass sie pünktlich abgeschlossen wird, wird das geschätzte Abschlussdatum für den letzten Arbeitstag vor dem von Ihnen festgelegten Enddatum der Iteration festgelegt (da die Arbeit nicht an arbeitsfreien Tagen abgebrannt werden soll).

  Beispiel: „(+9 Tage)“ zeigt an, dass das geschätzte Abschlussdatum 9 Arbeitstage nach dem geplanten Enddatum der Iteration liegt.

  Weitere Informationen finden Sie unter [Übersicht über den Iterationsabschluss](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
