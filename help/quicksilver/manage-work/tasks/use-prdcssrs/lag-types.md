---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Launch-Typen
description: Lag ist die Zeit, die nach dem Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann (Positive Lag), oder die Zeit, die eine abhängige Aufgabe vor dem Start des Vorgängers beginnen könnte (Negative Lag).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Übersicht über Launch-Typen

<!-- Audited: 01/2024 -->

Lag ist die Zeit, die nach dem geplanten Abschluss eines Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann (Positive Lag), oder die Zeit, die eine abhängige Aufgabe vor dem Start des Vorgängers beginnen könnte (Negative Lag).

Die geplanten, geplanten und geschätzten Daten der Nachfolgeaufgaben werden unter Berücksichtigung der Zeitverzögerung und der geplanten, geplanten und geschätzten Startdaten (Ende) der Voraufgaben berechnet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgaben und das Projekt verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Launch-Typen {#lag-types}

Ein Beispiel für eine Aufgabe, für die eine Zeitverzögerung erforderlich wäre, könnte das Sägen von Bäumen in Holz sein. Wenn das frisch geschnittene Holz eine Zeit lang trocknen muss, bevor es gefällt werden kann, dann würde es eine Zeitverzögerung zwischen dem Schneiden der Bäume und dem Sägen in Holz geben.

Die folgende Tabelle zeigt die Lag-Typen und wie die Zeitdauer für jede einzelne angegeben wird:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Wert</strong> </p> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tage (d oder de)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei durch Abhängigkeit bedingten Aufgaben wird in Arbeitstagen gemessen. Dies ist der standardmäßige Lag-Typ. </p> <p>Wenn es beispielsweise eine Finish-Start-Abhängigkeit mit einer Verzögerung von zwei Arbeitstagen gibt und die Vorgängeraufgabe am Freitag abgeschlossen wird, beginnt die abhängige Aufgabe am Mittwoch. Die Wochenendtage zählen nicht als Teil der Verzögerung. </p> <p>Hinweis: Die maximale Latenzgrenze für Tage beträgt 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalendertage (c oder ce)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird in Kalendertagen gemessen, einschließlich Feiertagen und Wochenenden. </p> <p>Hinweis: Dieser Verzögerungstyp zählt zwar Nicht-Arbeitstage als Teil der Verzögerung, eine abhängige Aufgabe kann jedoch nie an einem nicht funktionierenden Tag beginnen. Wenn dieser Verzögerungstyp dazu führt, dass die abhängige Aufgabe an einem nicht funktionierenden Tag beginnt, wird das geplante Startdatum der abhängigen Aufgabe für den folgenden Arbeitstag geplant. </p> <p>Wenn es beispielsweise eine Finish-Start-Abhängigkeit mit einer Verzögerung von 2 Kalendertagen gibt und die Vorgängeraufgabe am Donnerstag abgeschlossen wird, beginnt die abhängige Aufgabe am Montag und nicht am Sonntag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prozent (p oder pe)</p> </td> 
   <td> <p>Die Verzögerung wird als Prozentsatz der geschätzten Zeit zum Abschließen der vorherigen Aufgabe ausgedrückt. </p> <p>Wenn es beispielsweise eine Abhängigkeit von der Fertigstellung einer 10-tägigen Vorgängeraufgabe mit einer Verzögerung von 20 % gibt, berechnet das System, wie viele Tage 20 % der Aufgabendauer des Vorgängers ausmachen, und verwendet dies als Verzögerung. In diesem Fall wäre es 2 Tage nach Abschluss der Aufgabe. </p>

<p><b>NOTIZ</b></p> Die maximale Latenzgrenze beträgt 2000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag (w oder wir) </p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird durch Angabe der Wochentage der Woche gemessen, die das geplante Abschlussdatum des Vorgängers enthält.</p> <p>Für diesen Lag-Typ wird jeder Wochentag mit einer Zahl verknüpft:</p> 
    <ul> 
     <li>Sonntag=1</li> 
     <li>Montag = 2</li> 
     <li>Dienstag=3</li> 
     <li>Mittwoch=4</li> 
     <li>Donnerstag=5</li> 
     <li>Freitag=6</li> 
     <li>Samstag=7</li> 
    </ul> <p>Wenn Sie angeben möchten, dass das geplante Startdatum des Nachfolgers auf einen Dienstag der aktuellen Woche fällt und der Dienstag vor dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTIZ</b></p>

Wenn das Startdatum des Nachfolgers als ein bestimmter Dienstag berechnet wird und dieser Tag für die aktuelle Woche verstrichen ist, ist das geplante Startdatum der Nachfolgeaufgabe derselbe Tag (Dienstag) der folgenden Woche, sofern verfügbar. </p> <p>Wenn Sie angeben möchten, dass die Verzögerung auf einen Samstag der aktuellen Woche fällt und der Samstag nach dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren:</p> <p><code>4fs+7w</code> </p> <p>Wenn Samstag ein nicht funktionierender Tag ist, wird der nächste verfügbare Tag nach Samstag (um eine positive Verzögerung anzugeben) als geplantes Startdatum des Nachfolgers ausgewählt. </p>

<p>Dies gilt nicht für die Planung von Ausnahmen. Wenn ein Datum auch eine planmäßige Ausnahme ist und das Startdatum des Nachfolgers als dieser Tag berechnet wird, versucht das System, das nächste verfügbare Datum zu finden, das dem Wochentag entspricht, der im vorherigen Ausdruck angegeben ist.</p>

<p>Wenn beispielsweise das Startdatum als ein bestimmter Dienstag berechnet wird und dieser Tag eine planmäßige Ausnahme ist und die Verzögerung des Vorgängers positiv ist, wird der folgende Dienstag (wenn es auch ein Arbeitstag ist) als Startdatum des Nachfolgers ausgewählt. Wenn die Verzögerung negativ ist, wählt das System den vorherigen Dienstag als Startdatum aus.</p>

<p>Um vergangene oder zukünftige Wochen anzugeben, können Sie eine Zahl vor der Tagesnummer für den Verzögerungstyp hinzufügen. </p> <p>Um beispielsweise den Montag von 10 Wochen anzugeben, können Sie diesen Code verwenden, um den Vorgänger Ihres Nachfolgers anzugeben:</p> <p><code>4fs-102w</code> </p> <p>10 bedeutet, dass vor 10 Wochen und 2 die Zahl ist, die Montag zugewiesen ist. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag ungleich null (k oder ke)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird identisch mit dem Tag des Wochenzeitraums gemessen, es sei denn, die Zeit des Vorgängers endet am angegebenen Wochentag. Die Latenzzeit wird dann auf die angrenzende Woche (+/-) berechnet. </p> <p>In diesem Fall kann die Zeitverzögerung nie 0 betragen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Negativer Schwung

Sie können einen negativen Lag verwenden, um anzugeben, ob die Aufgabe vor dem Ende der Vorgängeraufgabe beginnen muss oder nicht.

Beachten Sie bei der Verwendung negativer Abstände die folgenden Regeln:

* Das negative Lag kann nicht erzwingen, dass das Start-/Enddatum einer Aufgabe vor oder nach dem geplanten Start-/Enddatum des Projekts liegt. Diese Daten werden im Feld Zeitplan von des Projekts angegeben.

  Beachten Sie in diesem Fall Folgendes:

   * Planen Sie das Projekt ab dem Abschlussdatum.
   * Die letzte Aufgabe im Projekt sollte die &quot;Must Finish on Task Constraint&quot;verwenden. Es wird empfohlen, der Aufgabe eine ausreichend lange Dauer zuzuweisen, damit alle Aufgaben im Projekt berücksichtigt werden können. Die verbleibenden Aufgaben funktionieren mit der so bald wie möglich geltenden Beschränkung.

* Die Verwendung einer Finish-Start-Vorgängerbeziehung mit Aufgaben kann zu einer Fehlermeldung führen.

  Beachten Sie in diesem Fall Folgendes:

   * Legen Sie eine Fertigstellen-Finish-Vorgängerbeziehung zwischen Aufgaben fest.
   * Die Dauer der Nachfolgeaufgabe sollte der vorgesehenen Anzahl von Verzögerungen zwischen Aufgaben entsprechen oder diese überschreiten.

## Anzeigen von Lag- und Lag-Typen für Aufgaben

Sie können bei der Definition der Vorgängerbeziehungen bei Aufgaben die Art der Verzögerung angeben.

### Anzeigen von Lag-Typen im Abschnitt &quot;Vorgänger&quot;einer Aufgabe {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Gehen Sie zu einer Aufgabe, für die Sie den Vorgänger und den Lag-Typ definieren möchten.
1. Klicken Sie im linken Bereich auf **Vorgänger** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Vorgänger** klicken.
1. Klicken Sie auf **Vorgänger hinzufügen**.
1. (Optional) Wenn Sie einen projektübergreifenden Vorgänger hinzufügen möchten, ersetzen Sie den Namen des **übergeordneten Projekts** durch einen anderen Projekt.
1. Geben Sie den Namen der Vorgängeraufgabe ein und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.
1. Wählen Sie den **Abhängigkeitstyp** aus.

   Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie einen Betrag vom Typ **Lag** mithilfe eines numerischen Werts an. Sie können negative Zahlen angeben, um eine negative Verzögerung anzugeben.
1. Wählen Sie aus den folgenden Optionen aus, um den Verzögerungstyp zu identifizieren, den Sie für Ihren Vorgänger angeben möchten:

   * **Tage**
   * **Kalendertage**
   * **Prozent**
   * **Wochentag**
   * **Wochentag (nicht null)**

     Weitere Informationen zu diesen Lag-Typen und deren Berechnung finden Sie im Abschnitt [Lag-Typen](#lag-types) in diesem Artikel.

1. Klicken Sie auf **Speichern**.

### Anzeigen von Lag-Typen in einer Aufgabenliste  {#indicate-lag-types-in-a-task-list}

1. Wechseln Sie zu einer Aufgabenliste und wählen Sie die Ansicht **Standard** aus.

1. Klicken Sie in die Spalte **Vorgänger** , die der Aufgabe entspricht, für die Sie einen Vorgänger und einen Verzögerungsbetrag angeben möchten.
1. Geben Sie Folgendes ohne Leerzeichen ein:

   * die Nummer der Aufgabe, die als Vorgänger der ausgewählten Aufgabe angegeben werden soll
   * die Abkürzung für den Abhängigkeitstyp, den Sie zwischen den Aufgaben anzeigen möchten

     Weitere Informationen zu den Abkürzungen für Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * entweder eine **+** für eine positive Verzögerung oder eine **-** für eine negative Verzögerung

   * die Zeitspanne, in der die Verzögerung
   * die Abkürzung für den gewünschten Lag-Typ

     Weitere Informationen zu den Abkürzungen für Lag-Typen finden Sie im Abschnitt [Lag-Typen](#lag-types) in diesem Artikel.

   Um beispielsweise anzugeben, dass eine Aufgabe einen Vorgänger und eine positive Verzögerung von 2 Tagen aufweist, geben Sie in die Spalte &quot;Vorgänger&quot;den Wert &quot;`1fs+2d`&quot;ein.

1. Drücken Sie die Eingabetaste auf der Tastatur, um die Änderungen an der Aufgabe zu speichern.