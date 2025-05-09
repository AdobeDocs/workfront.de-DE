---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Verzögerungsarten
description: Verzögerung ist die Zeit, die nach dem Abschluss eines erzwungenen Vorgängers vergehen muss, bis die abhängige Aufgabe beginnen kann (positive Verzögerung), oder die Zeit, die eine abhängige Aufgabe beginnen könnte, bevor die Vorgängeraufgabe beginnt (negative Verzögerung).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# Übersicht über Verzögerungsarten

<!-- Audited: 01/2024 -->

Verzögerung ist die Zeit, die nach dem geplanten Abschluss eines Vorgängers vergehen muss, bis die abhängige Aufgabe beginnen kann (positive Verzögerung), oder die Zeit, die eine abhängige Aufgabe beginnen könnte, bevor die Vorgängeraufgabe beginnt (negative Verzögerung).

Die geplanten, erwarteten und geschätzten Termine der Nachfolgeaufgaben werden unter Berücksichtigung der Zeitverzögerung sowie der geplanten, geplanten und geschätzten Anfangs- (Fertigstellungs-) Termine der Vorgängeraufgaben berechnet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
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
   <td> <p>Verwalten der Berechtigungen für die Aufgaben und das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verzögerungstypen {#lag-types}

Ein Beispiel für eine Aufgabe, für die eine Zeitverzögerung erforderlich wäre, könnte das Sägen von Bäumen in Bauholz sein. Wenn das frisch geschnittene Holz vor dem Schneiden eine Zeit lang trocknen muss, dann würde es eine Zeitverzögerung zwischen dem Schneiden der Bäume und dem Sägen in Holz geben.

Die folgende Tabelle veranschaulicht die Verzögerungsarten und zeigt, wie die Zeitdauer für jede Zeitverzögerung angegeben wird:

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
   <td> <p>Die Verzögerung zwischen zwei durch Abhängigkeit verknüpften Aufgaben wird in Arbeitstagen gemessen. Dies ist der standardmäßige Verzögerungstyp. </p> <p>Wenn beispielsweise eine Ende-Anfang-Abhängigkeit mit einer Verzögerung von 2 Arbeitstagen besteht und die Vorgängeraufgabe am Freitag abgeschlossen wird, beginnt die abhängige Aufgabe am Mittwoch. Die Wochenendtage zählen nicht als Teil der Verzögerung. </p> <p>Hinweis: Die maximale Verzögerungszeit für Tage beträgt 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalendertage (c oder ce)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird in Kalendertagen gemessen, einschließlich Feiertagen und Wochenenden. </p> <p>Hinweis: Obwohl dieser Verzögerungstyp arbeitsfreie Tage als Teil der Verzögerung zählt, kann eine abhängige Aufgabe nie an einem arbeitsfreien Tag beginnen. Wenn dieser Verzögerungstyp den Beginn der abhängigen Aufgabe auf einen arbeitsfreien Tag festlegt, wird das geplante Startdatum der abhängigen Aufgabe für den folgenden Arbeitstag geplant. </p> <p>Wenn beispielsweise eine Ende-Anfang-Abhängigkeit mit einer Verzögerung von 2 Kalendertagen besteht und die Vorgängeraufgabe am Donnerstag abgeschlossen wird, beginnt die abhängige Aufgabe am Montag anstelle eines Sonntags. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prozent (p oder pE)</p> </td> 
   <td> <p>Die Verzögerung wird als Prozentsatz der geschätzten Zeit zum Abschließen der Vorgängeraufgabe ausgedrückt. </p> <p>Wenn beispielsweise eine Ende-Anfang-Abhängigkeit mit einer Verzögerung von 20 % bei einer 10-tägigen Vorgängeraufgabe vorliegt, berechnet das System, wie viele Tage 20 % der Aufgabendauer des Vorgängers repräsentieren, und verwendet diese als Verzögerung. In diesem Fall liegt der Zeitpunkt 2 Tage nach Abschluss der Aufgabe. </p>

<p><b>NOTIZ</b></p> Die maximale Verzögerungsgrenze für Prozent beträgt 2.000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag (mit oder ohne Woche) </p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird gemessen, indem die Wochentage für die Woche angegeben werden, die das geplante Abschlussdatum des Vorgängers enthält.</p> <p>Für diesen Verzögerungstyp ist jeder Wochentag mit einer Zahl verknüpft:</p> 
    <ul> 
     <li>Sonntag=1</li> 
     <li>Montag=2</li> 
     <li>Dienstag=3</li> 
     <li>Mittwoch=4</li> 
     <li>Donnerstag=5</li> 
     <li>Freitag=6</li> 
     <li>Samstag=7</li> 
    </ul> <p>Wenn Sie angeben möchten, dass das geplante Startdatum des Nachfolgers auf einen Dienstag der aktuellen Woche fallen soll und der Dienstag vor dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>NOTIZ</b></p>

Wenn das Startdatum des Nachfolgers auf einen bestimmten Dienstag berechnet wird und dieser Tag für die aktuelle Woche vergangen ist, dann ist das geplante Startdatum der Nachfolger-Aufgabe derselbe Tag (Dienstag) der folgenden Woche, falls verfügbar. </p> <p>Wenn Sie angeben möchten, dass die Verzögerung auf einen Samstag der aktuellen Woche fallen soll und der Samstag nach dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren:</p> <p><code>4fs+7w</code> </p> <p>Wenn Samstag ein arbeitsfreier Tag ist, wird der nächste verfügbare Tag nach Samstag (um eine positive Verzögerung anzugeben) als geplantes Startdatum des Nachfolgers ausgewählt. </p>

<p>Dies gilt nicht für Zeitplanausnahmen. Wenn ein Datum auch eine Zeitplanausnahme ist und als Startdatum des Nachfolgers dieser Tag berechnet wird, versucht das System, das nächste verfügbare Datum zu finden, nämlich den im Vorgängerausdruck angegebenen Wochentag.</p>

<p>Wenn beispielsweise das Startdatum für einen bestimmten Dienstag berechnet wird und dieser Tag eine Zeitplanausnahme ist und die Verzögerung des Vorgängers positiv ist, wählt er den folgenden Dienstag (wenn dies auch ein Arbeitstag ist) als Startdatum des Nachfolgers. Wenn die Verzögerung negativ ist, wählt das System den vorherigen Dienstag als Startdatum.</p>

<p>Um vergangene oder zukünftige Wochen anzugeben, können Sie für den Verzögerungstyp eine Zahl vor der Tagesnummer hinzufügen. </p> <p>Um beispielsweise den Montag vor 10 Wochen anzugeben, können Sie diesen Code verwenden, um den Vorgänger Ihres Nachfolgers anzugeben:</p> <p><code>4fs-102w</code> </p> <p>10 gibt an, dass dies vor 10 Wochen erfolgte, und 2 ist die Zahl, die Montag zugewiesen wurde. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag ungleich null (k oder k)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird genauso gemessen wie der Tag des Wochentyps „lag“, es sei denn, die Zeit des Vorgängers endet am selben Tag der angegebenen Woche. Die Verzögerungszeit wird dann auf die angrenzende Woche (+/-) berechnet. </p> <p>In diesem Fall kann die Verzögerungszeit nie 0 sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## negative Verzögerung

Sie können eine negative Verzögerung verwenden, um anzugeben, ob die Aufgabe vor dem Ende der Vorgängeraufgabe beginnen muss oder kann.

Beachten Sie bei der Verwendung negativer Zeitabstände die folgenden Regeln:

* Negative Verzögerung kann nicht erzwingen, dass Start-/Enddaten eines Vorgangs vor oder nach den geplanten Start-/Enddaten des Projekts liegen. Diese Daten werden im Feld Zeitplan ab im Projekt angegeben.

  Beachten Sie in diesem Fall Folgendes:

   * Planen Sie das Projekt ab Abschlussdatum.
   * Für die letzte Aufgabe im Projekt sollte die Einschränkung Muss abgeschlossen sein für Aufgabe verwendet werden. Es wird empfohlen, der Aufgabe eine ausreichend lange Dauer zu geben, um alle Aufgaben im Projekt zu erfassen. Die verbleibenden Aufgaben funktionieren gut mit der Einschränkung So bald wie möglich .

* Die Verwendung einer Finish-Start-Vorgängerbeziehung mit Aufgaben kann zu einer Fehlermeldung führen.

  Beachten Sie in diesem Fall Folgendes:

   * Legen Sie eine Beenden-Beenden-Vorgängerbeziehung zwischen Aufgaben fest.
   * Die Dauer der Nachfolgeaufgabe sollte der vorgesehenen Anzahl an Verzögerungstagen zwischen Aufgaben entsprechen oder diese überschreiten.

## Angeben der Verzögerungsarten bei Aufgaben

Sie können Verzögerungstypen für Aufgaben angeben, wenn Sie deren Vorgängerbeziehungen definieren.

### Verzögerungstypen im Abschnitt „Vorgänger“ einer Aufgabe angeben {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Wechseln Sie zu einer Aufgabe, für die Sie den Vorgänger und den Verzögerungstyp definieren möchten.
1. Klicken Sie **linken Bedienfeld auf** Vorgänger“.
1. Klicken Sie **Vorgänger hinzufügen**.
1. (Optional) Wenn Sie einen projektübergreifenden Vorgänger hinzufügen möchten, ersetzen Sie den Namen **Übergeordnetes Projekt** durch ein anderes Projekt.
1. Beginnen Sie mit der Eingabe des Namens der Vorgängeraufgabe und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.
1. Wählen Sie den **Abhängigkeitstyp**.

   Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie einen **Lag**-Betrag mithilfe eines numerischen Werts an. Sie können negative Zahlen angeben, um eine negative Verzögerung anzugeben.
1. Wählen Sie aus den folgenden Optionen, um die Art der Verzögerung zu bestimmen, die Sie für Ihren Vorgänger angeben möchten:

   * **Tage**
   * **Kalendertage**
   * **Prozent**
   * **Wochentag**
   * **Wochentag (ungleich null)**

     Weitere Informationen zu diesen Verzögerungsarten und deren Berechnung finden Sie im Abschnitt [Verzögerungsarten](#lag-types) in diesem Artikel.

1. Klicken Sie auf **Speichern**.

### Verzögerungstypen in einer Aufgabenliste angeben  {#indicate-lag-types-in-a-task-list}

1. Wechseln Sie zu einer Aufgabenliste und wählen Sie die Ansicht **Standard** aus.

1. Klicken Sie in die Spalte **Vorgänger**, die der Aufgabe entspricht, für die Sie einen Vorgänger und einen Verzögerungsbetrag angeben möchten.
1. Geben Sie Folgendes ohne Leerzeichen ein:

   * Die Nummer der Aufgabe, die Sie als Vorgänger der ausgewählten Aufgabe angeben möchten
   * Die Abkürzung für den Abhängigkeitstyp, den Sie zwischen den Aufgaben angeben möchten

     Weitere Informationen zu den Abkürzungen für Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * Entweder ein **+** für eine positive Verzögerung oder ein **-** für eine negative Verzögerung

   * Der Betrag der Verzögerung
   * die Abkürzung für den Verzögerungstyp, den Sie verwenden möchten

     Weitere Informationen zu den Abkürzungen für Verzögerungsarten finden Sie im Abschnitt [Verzögerungsarten](#lag-types) in diesem Artikel.

   Um beispielsweise anzugeben, dass eine Aufgabe einen Vorgänger und eine positive Verzögerung von 2 Tagen hat, geben Sie in der Spalte „Vorgänger“ `1fs+2d` ein.

1. Drücken Sie die Eingabetaste auf der Tastatur, um die Änderungen an der Aufgabe zu speichern.
