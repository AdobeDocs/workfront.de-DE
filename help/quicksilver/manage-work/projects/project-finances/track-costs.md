---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kosten nachverfolgen
description: Sie können Kosten für Projekte, Aufgaben und Probleme in Adobe Workfront verfolgen.
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 23a5c90b9321b72a20f21752f957b3be0a9f3a02
workflow-type: tm+mt
source-wordcount: '2499'
ht-degree: 0%

---

# Kosten nachverfolgen

<!-- Audited: 02/2024 -->

Sie können Kosten für Projekte, Aufgaben und Probleme in Adobe Workfront verfolgen.

## So berechnet Workfront Kosten

Um Kosten zu verfolgen, müssen Sie Benutzer und Aufgabengebiete mit Stundenkostensätzen verknüpfen.

Stundenkostensätze sind Kostenbeträge pro Arbeitseinheit, die mit Aufgabengebieten oder Benutzern verknüpft sind. Das Multiplizieren der Sätze mit den für die Arbeit aufgewendeten Stunden verursacht Kosten für Ihre Projekte, Aufgaben oder Probleme.

Die folgenden Szenarien sind vorhanden:

* Wenn der Kostentyp Ihrer Aufgaben „Benutzer pro Stunde“ ist, berechnet der Benutzer-Stundensatz die Aufgaben- und Projektkosten.

  Informationen zum Verknüpfen von Benutzern mit Kostensätzen finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn der Kostentyp Ihrer Aufgaben „Funktion pro Stunde“ lautet, berechnet der Stundensatz für Aufgabengebiete die Aufgaben- und Projektkosten.

  Informationen zum Verknüpfen von Aufgabengebieten mit Kostensätzen finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront berechnet nur die Ist-Kosten für Probleme, und Probleme haben keinen Kostentyp. Weitere Informationen finden Sie im Abschnitt [So verfolgt Workfront die Kosten für Probleme](#how-workfront-tracks-costs-for-issues) in diesem Artikel.

>[!TIP]
>
>Sie können Kostensätze für Projekte nicht überschreiben. Sobald Sie den Stundensatz für einen Benutzer oder ein Aufgabengebiet festgelegt haben, berechnet dieser Satz alle Kosten im System.

## Workfront-Kostenentwicklungsindizes

Workfront berechnet eine Reihe von Kostenleistungsindizes für Projekte, damit Projekte im Hinblick auf Kosteneffizienz verfolgt werden können.\
Weitere Informationen zur Berechnung von Kosten-Performance-Indizes finden Sie unter:

* [Kostenentwicklungsindex (Cost Performance Index, CPI) berechnen](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Kostenplan-Leistungsindex (CSI) berechnen](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Planleistungsindex (SPI) berechnen](../../../manage-work/projects/project-finances/calculate-spi.md)

## Wie Workfront Kosten für Aufgaben und Projekte verfolgt

Die Kostenarten werden für Aufgaben und Projekte unterschiedlich berechnet.

### So verfolgt Workfront Kosten {#how-workfront-tracks-costs}

Sie können verschiedene Arten von Kosten für Aufgaben und Projekte in Workfront verfolgen. Die Gesamtkosten werden nach folgender Formel berechnet:

`Costs = Labor Costs + Expense Costs`

* **Arbeitskosten** sind mit den Stunden für Aufgaben und Projekte und den Kosten pro Stunde der Ressourcen verknüpft, die mit Aufgaben verknüpft sind. Im Allgemeinen berechnet Workfront die folgenden Lohnkosten:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Geplante Arbeitskosten</td> 
     <td> <p>Sie werden nach folgender Formel berechnet:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Budgetierte Arbeitskosten</td> 
     <td> <p>Sie werden nach folgender Formel berechnet:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Ist-Lohnkosten</td> 
     <td> <p>Sie werden nach folgender Formel berechnet:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> 
     <p><strong>HINWEIS</strong>
     <p>Workfront berechnet die Ist-Lohnkosten anhand der Legacy-Iststunden. Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Tatsächliche Stunden anzeigen</a>. </p>

  </td> 
    </tr> 
   </tbody> 
  </table>

  Weitere Informationen finden Sie [ Abschnitt „Wie Workfront geplante, budgetierte und Istkosten berechnet](#how-workfront-calculates-planned-budgeted-and-actual-costs) in diesem Artikel.

* **Ausgabenkosten** sind mit Ausgaben für Projekte und Aufgaben verknüpft.\
  Wenn Sie ein Projekt erstellen, können Sie geplante Ausgaben für das gesamte Projekt festlegen. Darüber hinaus können Sie Ausgaben neuen oder vorhandenen Aufgaben zuordnen. Weitere Informationen finden Sie unter [Projektausgaben verwalten](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Fixkosten** werden als fester Kostenbetrag für ein Projekt definiert. Dies ist Teil der geplanten Kosten des Projekts, d. h. der Summe, die Sie für die Durchführung des Projekts benötigen.

  >[!TIP]
  >
  >Wenn Sie eine Vorlage einem Projekt zuordnen, werden die Festkosten einer Vorlage zu den Festkosten des Projekts hinzugefügt. Weitere Informationen finden Sie unter [Übersicht über das Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### So berechnet Workfront geplante, budgetierte und Ist-Kosten {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront berechnet die geplanten Kosten und Istkosten für jede einzelne Aufgabe in einem Projekt. Workfront verwendet diese Berechnungen für einzelne Vorgänge, um die geplanten Kosten und Istkosten für das Projekt zu berechnen.

#### Geplante Kosten {#planned-cost}

Die geplanten Kosten eines Projekts sind die Kosten, die mit den geplanten Arbeiten (geplante Stunden) für das Projekt verbunden sind.

Die geplanten Kosten eines Projekts werden nach folgender Formel berechnet:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Beispiel: Auf der Registerkarte „Ausgaben“ einer Aufgabe befinden sich folgende Ausgaben: Marketing-Ausgaben 100 $ und Verwaltungsausgaben 50 $. Auf der Registerkarte „Finanzen“ wählen Sie den Kostentyp „Benutzer pro Stunde“. Ein Benutzer wird der Aufgabe zugewiesen und der Stundensatz des Benutzers beträgt 15 $. Der/die Benutzende wird mit 5 Stunden Arbeit an dieser Aufgabe beauftragt. Auf der Registerkarte Ausgaben des Projekts fallen für eine Ausgabe namens Beratung Kosten in Höhe von 100 US-Dollar an. Sie haben außerdem Fixkosten von 200 $ für das Projekt.

Die geplanten Kosten des Projekts werden wie folgt berechnet:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

Der Stundensatz in der Formel berücksichtigt alle Datumsänderungen, die wirksam sind.

#### Budgetierte Kosten {#budgeted-cost}

Die budgetierten Kosten eines Projekts sind die Kosten, die mit der budgetierten Arbeit (budgetierte Stunden) für das Projekt verknüpft sind.

Die budgetierten Kosten des Projekts entsprechen den geplanten Kosten des Projekts, wenn die beiden folgenden Bedingungen erfüllt sind:

* Die geplanten Stunden der Aufgaben im Projekt entsprechen den budgetierten Stunden (im Ressourcenplaner).
* Der Abrechnungstyp der Aufgaben ist „Stundensatz nach Funktion“.

Die budgetierten Kosten des Projekts werden anhand der folgenden Formel berechnet, wenn die folgenden Bedingungen erfüllt sind:

* Die geplanten Stunden der Aufgaben im Projekt stimmen nicht mit den budgetierten Stunden überein (im Ressourcenplaner).
* Der Abrechnungstyp der Aufgaben ist „Stundensatz nach Funktion“.

Wenn die oben genannten Bedingungen erfüllt sind, berechnet Workfront die budgetierten Kosten des Projekts anhand der folgenden Formel:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Ist-Kosten {#actual-cost}

Die Ist-Kosten eines Projekts sind die Kosten, die mit der tatsächlichen Arbeit (protokollierte Stunden) für das Projekt verbunden sind.

Die Ist-Kosten werden anhand der folgenden Formel berechnet:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Beispiel: Auf der Registerkarte „Ausgaben“ einer Aufgabe befinden sich folgende Ausgaben: eine Marketing-Ausgabe mit Istkosten von 110 $ und eine Verwaltungsausgabe mit Istkosten von 40 $. Sie wählen den Kostentyp „Stundensatz nach Funktion“ aus und weisen der Aufgabe das Aufgabengebiet „Berater“ zu. Der Satz für das Aufgabengebiet Berater beträgt 15 USD pro Stunde, und für das Aufgabengebiet Berater sind 6 Stunden protokolliert. Mit dem Projekt sind Beratungskosten verbunden (auf der Registerkarte „Ausgaben„), mit tatsächlichen Kosten von 100 $ und einem Benutzer mit einem Stundensatz von 20 $ in seinen Benutzerprofilprotokollen, die 10 Stunden für das Projekt enthalten. Sie haben außerdem Fixkosten von 200 $ für das Projekt.

Die Ist-Kosten des Projekts werden wie folgt berechnet:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

Der Stundensatz in der Formel berücksichtigt alle Datumsänderungen, die wirksam sind.

>[!NOTE]
>
>Die tatsächlichen Kosten des Projekts werden wie folgt berechnet:
>&#x200B;>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Diese Kosten werden in der Istkostenberechnung nicht dupliziert. Wenn beispielsweise Fixkosten Teil der Ist-Ausgaben des Projekts sind, werden sie nicht separat zu den Ist-Kosten hinzugefügt.

>[!NOTE]
>
>Beim Protokollieren der Zeit für ein Projekt ergeben sich bei der Berechnung der tatsächlichen Lohnkosten für das Projekt die folgenden Szenarien:
>
>* Standardmäßig verwendet Workfront den Stundensatz des Benutzers zur Berechnung der tatsächlichen Lohnkosten.
>* Wenn die Benutzerin oder der Benutzer, die oder der die Zeit protokolliert, keine Kosten verursacht, verwendet Workfront den Stundensatz der Primären Rolle der Benutzerin oder des Benutzers.
>* Wenn Ihr Workfront-Administrator die Einstellung **Aufgabengebiete zu Stundeneinträgen manuell zuweisen** im Bereich „Arbeitszeittabellen- und Stunden-Voreinstellungen“ von „Setup“ aktiviert hat und die Benutzenden, die für das Projekt protokollieren, eine andere Rolle auswählen, die dieser Zeit zugeordnet werden soll, werden die Istkosten des Projekts auf der Grundlage der Rolle berechnet, die beim Protokollieren der Stunden angegeben wurde. Informationen zur Aktivierung der Protokollierungszeit für ein bestimmtes Aufgabengebiet finden Sie im Artikel [Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### So berechnet Workfront Kostentypen für Aufgaben {#how-workfront-calculates-cost-types-for-tasks}

Die geplanten Kosten und Istkosten der Aufgaben sowie deren Lohnkosten werden durch den Kostentyp jeder Aufgabe bestimmt.

Sie können den Kostentyp für einzelne Aufgaben innerhalb des Projekts konfigurieren. Jeder Kostentyp wirkt sich auf die Werte der geplanten Kosten und Istkosten aus.

Informationen zum Ändern des Kostentyps einer Aufgabe finden Sie unter [Kostentyp der Aufgabe aktualisieren](../../../manage-work/tasks/task-information/update-task-cost-type.md).

In der folgenden Tabelle werden die in Workfront verfügbaren Aufgabenkostentypen beschrieben:

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>Kostenart der Aufgabe</strong> </p> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>Benutzer pro Stunde</p> </td> 
   <td> <p>Dies ist der Standardkostentyp beim Erstellen einer Aufgabe.</p> <p><strong>Geplante Kosten</strong> werden anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Wenn die geplanten Lohnkosten wie folgt berechnet werden:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Hinweis: <p>Beachten Sie die folgenden Auswirkungen der Verwendung des Kostentyps „Benutzer pro Stunde“ und der Berechnung der geplanten Kosten:</p> 
     <ul> 
      <li>Wenn Sie einem Vorgang mehrere Ressourcen zuordnen, passt Workfront die Berechnungen für die geplanten Kosten auf der Grundlage des Prozentsatzes des Vorgangs an, der jeder Ressource zugewiesen wurde.</li>
      <li>Bei effektiven Datumskostensätzen sind die geplanten Lohnkosten die Summe der geplanten Kosten jedes Zeitraums, der von der Aufgabe abgedeckt wird.</li>
      <li>Der Wert des Felds Geplante Kosten kann variieren, je nachdem, ob Sie die geplanten Kosten aus der Aufgabe selbst oder aus dem Auslastungsbericht anzeigen.<br><strong>Beim Anzeigen der geplanten Kosten aus der Aufgabe selbst:</strong> Das Feld „Geplante Kosten“ berücksichtigt das Feld „Kosten/Std.“, das auf der Ebene des Aufgabengebiets festgelegt wurde (wenn das Feld „Kosten/Std.“ nicht auf Benutzerebene festgelegt wurde).<br><strong>Beim Anzeigen der geplanten Kosten aus dem Auslastungsbericht für das Projekt: </strong> Feld „Geplante Kosten“ berücksichtigt nicht das Feld „Kosten/Std.“, das auf der Ebene des Aufgabengebiets festgelegt wurde. Wenn der Auslastungsbericht stattdessen das Feld „Kosten/Std.“ berücksichtigen soll, das auf Aufgabengebiet-Ebene festgelegt wurde, müssen Sie für den Kostentyp in der Aufgabe „Stundensatz“ festlegen. </li> 
     </ul> </p> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wenn die tatsächlichen Lohnkosten wie folgt berechnet werden:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Beispielsweise hat ein Benutzer in seinem Profil einen Stundensatz von 20 US-Dollar. Wenn 5 Stunden für eine Aufgabe protokolliert werden, betragen die tatsächlichen Lohnkosten für diese Aufgabe 100 USD. Wenn dem/der Benutzenden kein Stundensatz „Kosten pro Stunde“ zugeordnet ist, werden die Istkosten auf der Grundlage des Stundensatzes für das Primäre Aufgabengebiet berechnet. Wenn er kein Aufgabengebiet hat oder der Stundensatz des Aufgabengebiets nicht definiert ist, sind die Istkosten der Aufgabe gleich null. </p> <p>Hinweis: Die Istkosten werden auf der Grundlage des Stundensatzes des Benutzers berechnet, der die Zeit protokolliert, und zwar unabhängig davon, wer der Aufgabe zugewiesen ist. Außerdem berücksichtigt der Stundensatz für die Abrechnung in der Formel alle Datumsänderungen, die wirksam sind.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stundensatz nach Funktion</p> </td>
   <td> <p><strong>Geplante Kosten</strong> werden anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Wo die geplanten Lohnkosten für die Aufgabe wie folgt berechnet werden:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Hinweis: Wenn Sie einem Vorgang mehrere Ressourcen zuordnen, passt Workfront die Berechnungen für geplante Stunden auf der Grundlage des Prozentsatzes des Vorgangs an, der jeder Ressource zugewiesen wurde. Außerdem berücksichtigt der Stundensatz in der Formel alle Datumsänderungen, die wirksam sind.</p> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wo die Ist-Lohnkosten der Aufgabe wie folgt berechnet werden:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Beispielsweise wird eine Aufgabe einem Aufgabengebiet oder einem Benutzer mit einem Aufgabengebiet zugewiesen, für das der Kostensatz pro Stunde 20 $ beträgt. Wenn ein(e) Benutzende(r) 5 Stunden für eine Aufgabe protokolliert, betragen die tatsächlichen Lohnkosten für diese Aufgabe 100 USD. Wenn dem Benutzer, der der Aufgabe zugewiesen wurde, kein Aufgabengebiet zugeordnet ist, das dieser Aufgabe zugeordnet ist, werden die Istkosten auf der Grundlage des Stundensatzes für das Primäre Aufgabengebiet berechnet. Wenn er kein Aufgabengebiet hat oder der Stundensatz des Aufgabengebiets nicht definiert ist, sind die Istkosten der Aufgabe gleich null. </p> <p>Hinweis: Die tatsächlichen Stunden einer stündlichen Aufgabe mit Funktion werden basierend auf den Aufgabengebieten der Benutzer berechnet, die mit der Aufgabe verknüpft sind, nicht auf den Rollen, die mit dem Benutzer verknüpft sind, der die Zeit erfasst. Außerdem berücksichtigt der Stundensatz für die Abrechnung in der Formel alle Datumsänderungen, die wirksam sind.</p> <p>Wenn Ihr Workfront-Administrator bei Setup die Einstellung <strong>Aufgabengebiete zu Stundeneinträgen manuell zuweisen</strong> im Bereich Arbeitszeittabellen- und Stunden-Voreinstellungen aktiviert hat und die Benutzenden, die die Zeit für die Aufgabenerfassung protokollieren, eine andere Rolle auswählen, die dieser Zeit zugeordnet werden soll, werden die Istkosten für eine Stundenaufgabe für Aufgabengebiete auf der Grundlage der Rolle berechnet, die beim Protokollieren der Stunden angegeben wurde. Informationen zur Aktivierung der Protokollierungszeit für ein bestimmtes Aufgabengebiet finden Sie im Artikel <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festgelegt pro Stunde</p> </td> 
   <td> <p><strong>Geplante Kosten</strong> werden anhand der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Dabei werden die Lohnkosten für die Aufgabe wie folgt berechnet:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Wo die Ist-Arbeitskosten der Aufgabe wie folgt berechnet werden:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Dieser Kostentyp berücksichtigt keine einzelnen Benutzer oder Aufgabengebiete.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Keine Kosten</p> </td> 
   <td> <p>Dieser Kostentyp hat keine Auswirkungen auf die Kosten. Wenn ein übergeordneter Vorgang diesen Kostentyp hat, werden Teilvorgänge mit einem anderen Kostentyp entsprechend ihren individuellen Kostentypen berechnet, und die Kosten des übergeordneten Vorgangs werden entsprechend beeinflusst. </p> <p>Wenn ein(e) Benutzende(r) ohne Zugriff auf Finanzdaten oder ein(e) Benutzende(r) ohne Finanzberechtigungen für eine Vorlage ein Projekt basierend auf dieser Vorlage erstellt, ist dies der Standardkostentyp für die Aufgaben im Projekt.</p> <p>Informationen zum Zugriff auf Finanzdaten finden Sie im Artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> <p>Informationen zu Finanzberechtigungen für Objekte finden Sie im Artikel <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Freigeben von Finanzberechtigungen für ein Objekt</a>.</p> <p>Informationen zum Erstellen von Projekten aus Vorlagen finden Sie im Artikel <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Erstellen eines Projekts mithilfe einer Vorlage</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Wie Workfront Kosten für Probleme nachverfolgt {#how-workfront-tracks-costs-for-issues}

Probleme haben keine Auswirkungen auf die folgenden Kostentypen in einem Projekt und wirken sich auch nicht darauf aus:

* Geplante Kosten
* Budgetierte Kosten

Probleme können jedoch &quot;**Kosten“ aufweisen** was sich auch auf die Ist-Kosten des Projekts auswirkt.

In der folgenden Tabelle wird erläutert, wie die Ist-Kosten für Probleme je nach Art der Zuweisung für das Problem berechnet werden:

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>Benutzerzuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Der Stundensatz des Benutzers, der die Zeit erfasst, wird hier berücksichtigt, unabhängig davon, wer dem Problem zugewiesen ist. </p> <p>Wenn der/die Benutzende, der/die die Zeit protokolliert, in seinem/ihrem Profil keinen Stundensatz „Kosten pro Stunde“ hat, berechnet der Stundensatz seines/ihres Primären Aufgabengebiets die Ist-Kosten des Problems.</p> <p>Wenn der/die Benutzende, der/die die Zeit protokolliert, in seinem/ihrem Profil keine Funktion hat oder ihm kein Stundensatz zugeordnet ist, werden die Iststunden anhand des Stundensatzes des Primären Aufgabengebiets des/r Primären Verantwortlichen für das Problem berechnet. Wenn für diese Funktion kein Satz definiert ist, sind die Istkosten des Problems gleich null. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Funktionszuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Der Stundensatz des Benutzers, der die Zeit in Bezug auf das Problem protokolliert, wird hier berücksichtigt, unabhängig davon, welche Rolle dem Problem zugewiesen ist. </p> <p>Wenn dem Benutzer, der die Zeit protokolliert, kein Stundensatz „Kosten pro Stunde“ zugeordnet ist, berechnet der Stundensatz seiner Primären Funktion die Ist-Kosten des Problems.</p><p>Wenn der/die Benutzende, der/die die Zeit protokolliert, in seinem/ihrem Profil keine Rolle oder keinen Satz hat, der damit verknüpft ist, sind die tatsächlichen Kosten des Problems gleich null. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Keine Zuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Istkosten</strong> werden anhand der folgenden Formel berechnet:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Wenn dem/der Benutzenden, der/die die Zeit protokolliert, kein Stundensatz „Kosten pro Stunde“ zugeordnet ist, berechnet der Stundensatz seines/ihres Primären Aufgabengebiets die Ist-Kosten des Problems. </p> <p>Wenn dem/der Benutzenden, der/die die Zeit protokolliert, kein Aufgabengebiet mit seinem/ihrem Profil zugeordnet ist oder für das sein/ihr Primäres Aufgabengebiet kein Stundensatz definiert ist, sind die Istkosten des Problems Null. </p> </td> 
  </tr> 
 </tbody> 
</table>
