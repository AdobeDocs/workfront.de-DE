---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über die Lag-Typen
description: Lag ist die Zeit, die nach dem Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann (Positive Lag), oder die Zeit, die eine abhängige Aufgabe vor dem Start des Vorgängers beginnen könnte (Negative Lag).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# Übersicht über die Lag-Typen

Lag ist die Zeit, die nach dem Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann (Positive Lag), oder die Zeit, die eine abhängige Aufgabe vor dem Start des Vorgängers beginnen könnte (Negative Lag).

Die geplanten, geplanten und geschätzten Termine der Nachfolgeaufgaben werden unter Berücksichtigung der Verzögerungen sowie der geplanten, geplanten und geschätzten Start- (Abschluss-)Daten der Voraufgaben berechnet.

## Zugriffsanforderungen

<!--drafted - replace table at P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben und Projekte verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen von Lag- und Lag-Typen für Aufgaben

Sie können bei der Definition der Vorgängerbeziehungen bei Aufgaben die Art der Verzögerung angeben.

* [Anzeigen von Lag-Typen im Abschnitt &quot;Vorgänger&quot;einer Aufgabe](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [Anzeigen von Lag-Typen in einer Aufgabenliste](#indicate-lag-types-in-a-task-list)

### Anzeigen von Lag-Typen im Abschnitt &quot;Vorgänger&quot;einer Aufgabe {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Gehen Sie zu einer Aufgabe, für die Sie den Vorgänger und den Lag-Typ definieren möchten.
1. Klicken **Vorgänger** im linken Bereich. Möglicherweise müssen Sie auf **Mehr anzeigen**, und dann **Vorgänger**.
1. Klicken **Vorgänger hinzufügen**.
1. (Optional) Wenn Sie einen projektübergreifenden Vorgänger hinzufügen möchten, ersetzen Sie die **Übergeordnetes Projekt** mit einem anderen Projekt.
1. Beginnen Sie mit der Eingabe des Namens der Vorgängeraufgabe und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.
1. Wählen Sie die **Abhängigkeitstyp**.

   Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie eine **Lag** Betrag unter Verwendung eines numerischen Werts. Sie können negative Zahlen angeben, um eine negative Verzögerung anzugeben.
1. Wählen Sie aus den folgenden Optionen aus, um den Verzögerungstyp zu identifizieren, den Sie für Ihren Vorgänger angeben möchten:

   * **Tage**
   * **Kalendertage**
   * **Prozent**
   * **Wochentag**
   * **Wochentag (nicht null)**

      Weitere Informationen zu diesen Lag-Typen und deren Berechnung finden Sie im Abschnitt . [Übersicht über Launch-Typen](#lag-types-overview) in diesem Artikel.

1. Klicken Sie auf **Speichern**.

### Anzeigen von Lag-Typen in einer Aufgabenliste  {#indicate-lag-types-in-a-task-list}

1. Wechseln Sie zu einer Aufgabenliste und wählen Sie die **Standard** Ansicht über **Ansicht** Dropdown-Menü.

1. Klicken Sie in die **Vorgänger** -Spalte, die der Aufgabe entspricht, für die Sie einen Vorgänger und einen Latenzbetrag angeben möchten.
1. Geben Sie Folgendes ohne Leerzeichen ein:

   * die Nummer der Aufgabe, die als Vorgänger der ausgewählten Aufgabe angegeben werden soll
   * die Abkürzung für den Abhängigkeitstyp, den Sie zwischen den Aufgaben anzeigen möchten

      Weitere Informationen zu den Abkürzungen für Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * entweder ein **+** für eine positive Verzögerung oder **-** für eine negative Verzögerung

   * die Zeitspanne, in der die Verzögerung
   * die Abkürzung für den zu verwendenden Lag-Typ.

      Weitere Informationen zu den Abkürzungen für Lag-Typen finden Sie im Abschnitt . [Übersicht über Launch-Typen](#lag-types-overview) in diesem Artikel.
   Um beispielsweise anzugeben, dass eine Aufgabe einen Vorgänger und eine positive Verzögerung von 2 Tagen hat, geben Sie

   ```
   1fs+2d
   ```

   in der Spalte &quot;Vorgänger&quot;.

1. Klicken Sie auf die Eingabetaste, um die Änderungen an der Aufgabe zu speichern.

## Übersicht über Launch-Typen {#lag-types-overview}

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
   <td> <p>Tage (d)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei durch Abhängigkeit bedingten Aufgaben wird in Arbeitstagen gemessen. Dies ist der standardmäßige Lag-Typ. </p> <p>Wenn es beispielsweise eine Finish-Start-Abhängigkeit mit einer Verzögerung von zwei Arbeitstagen gibt und die Vorgängeraufgabe am Freitag abgeschlossen wird, beginnt die abhängige Aufgabe am Mittwoch. Die Wochenendtage zählen nicht als Teil der Verzögerung. </p> <p>Hinweis: Die maximale Verzögerung für Tage beträgt 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalendertage (c)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird in Kalendertagen gemessen, einschließlich Feiertagen und Wochenenden. </p> <p>Hinweis: Dieser Verzögerungstyp zählt zwar als Teil der Verzögerung Nicht-Arbeitstage, eine abhängige Aufgabe kann jedoch nie an einem nicht funktionierenden Tag beginnen. Wenn dieser Verzögerungstyp dazu führt, dass die abhängige Aufgabe an einem nicht funktionierenden Tag beginnt, wird das geplante Startdatum der abhängigen Aufgabe für den folgenden Arbeitstag geplant. </p> <p>Wenn es beispielsweise eine Finish-Start-Abhängigkeit mit einer Verzögerung von 2 Kalendertagen gibt und die Vorgängeraufgabe am Donnerstag abgeschlossen wird, beginnt die abhängige Aufgabe am Montag und nicht am Sonntag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prozent (p oder pe)</p> </td> 
   <td> <p>Die Verzögerung wird als Prozentsatz der geschätzten Zeit zum Abschließen der vorherigen Aufgabe ausgedrückt. </p> <p>Wenn es beispielsweise eine Abhängigkeit zwischen Fertigstellung und Start mit einer Verzögerung von 20 % zwischen einer 10-tägigen Vorgängeraufgabe gibt, berechnet das System, wie viele Tage 20 % der vorherigen Aufgabendauer beträgt, und verwendet dies als Verzögerung. In diesem Fall wäre es 2 Tage nach Abschluss der Aufgabe. </p> <p>Hinweis: Die maximale Latenzgrenze beträgt 2000 %.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag (w) </p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird durch Angabe der Wochentage der Woche gemessen, die das geplante Abschlussdatum des Vorgängers enthält.</p> <p>Für diesen Lag-Typ wird jeder Wochentag mit einer Zahl verknüpft:</p> 
    <ul> 
     <li>Sonntag=1</li> 
     <li>Montag = 2</li> 
     <li>Dienstag=3</li> 
     <li>Mittwoch=4</li> 
     <li>Donnerstag=5</li> 
     <li>Freitag=6</li> 
     <li>Samstag=7</li> 
    </ul> <p>Wenn Sie angeben möchten, dass das geplante Startdatum des Nachfolgers auf einen Dienstag der aktuellen Woche fällt und der Dienstag vor dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren: </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>Hinweis: Wenn der Dienstag für die Woche des geplanten Abschlussdatums des Vorgängers verstrichen ist, ist das geplante Startdatum der Nachfolgeaufgabe der erste verfügbare Arbeitstag dieser Woche. </p> <p>Wenn Sie angeben möchten, dass die Verzögerung auf einen Samstag der aktuellen Woche fällt und der Samstag nach dem geplanten Abschlussdatum des Vorgängers liegt, würden Sie Ihren Nachfolger mit der folgenden Formel codieren:</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>Wenn Samstag ein nicht funktionierender Tag ist, wird der nächste verfügbare Tag nach Samstag (um eine positive Verzögerung anzugeben) als geplantes Startdatum des Nachfolgers ausgewählt. </p> <p>Um vergangene oder zukünftige Wochen anzugeben, können Sie eine Zahl vor der Tagesnummer für den Verzögerungstyp hinzufügen. </p> <p>Um beispielsweise den Montag von 10 Wochen anzugeben, können Sie diesen Code verwenden, um den Vorgänger Ihres Nachfolgers anzugeben:</p> <p><code>4fs-102w</code> </p> <p>10 bedeutet, dass vor 10 Wochen und 2 die Zahl ist, die Montag zugewiesen ist. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Wochentag ungleich null (k)</p> </td> 
   <td> <p>Die Verzögerung zwischen zwei Aufgaben wird identisch mit dem Tag des Wochenzeitraums gemessen, es sei denn, die Zeit des Vorgängers endet am angegebenen Wochentag. Die Latenzzeit wird dann auf die angrenzende Woche (+/-) berechnet. </p> <p>In diesem Fall kann die Zeitverzögerung nie 0 betragen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Übersicht über Negative Lag

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
