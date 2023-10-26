---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kosten verfolgen
description: Sie können Kosten für Projekte, Aufgaben und Probleme in Adobe Workfront verfolgen.
author: Alina, Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 1%

---

# Kosten verfolgen

Sie können Kosten für Projekte, Aufgaben und Probleme in Adobe Workfront verfolgen.

## Kostenberechnung durch Workfront

Um die Kosten zu verfolgen, müssen Sie Benutzer und Stellenrollen mit stündlichen Kostensätzen verknüpfen.

Stündliche Kostensätze sind Beträge der Kosten pro Arbeitseinheit, die mit den Rollen oder Benutzern in einem Job verbunden sind. Die Multiplikation der Raten mit den Arbeitsstunden generiert Kosten für Ihre Projekte, Aufgaben oder Probleme.

Die folgenden Szenarien existieren:

* Wenn der Kostentyp Ihrer Aufgaben &quot;Benutzer stündlich&quot;ist, berechnet der Benutzer die Aufgaben- und Projektkosten mit der Stundenrate.

  Informationen zur Zuordnung von Benutzern zu Kostenstellen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn der Kostentyp Ihrer Aufgaben die Rolle Stündlich ist, berechnet der Stundensatz für die Rolle &quot;Auftrag&quot;die Aufgaben- und Projektkosten.

  Informationen zum Verknüpfen von Stellenrollen mit Kostenstellen finden Sie unter [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront berechnet nur die tatsächlichen Kosten für Probleme und Probleme ohne Kostentyp. Weitere Informationen finden Sie im Abschnitt . [So verfolgt Workfront Kosten für Probleme](#how-workfront-tracks-costs-for-issues) in diesem Artikel.

>[!TIP]
>
>Sie können die Kostensätze für Projekte nicht überschreiben. Sobald Sie die Kosten pro Stunde für einen Benutzer oder eine Rolle im Arbeitsbereich ermitteln, berechnet diese Rate alle Kosten im System.

## Workfront-Indizes zur Kosteneffizienz

Workfront berechnet eine Reihe von Kostenleistungsindizes für Projekte, damit Projekte im Hinblick auf Kosteneffizienz verfolgt werden können.\
Weitere Informationen zur Berechnung von Kosten-Performance-Indizes finden Sie unter:

* [CPI (Cost Performance Index) berechnen](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calculate Cost Schedule Performance Index (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Berechnung des Zeitplan-Leistungsindex (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## So verfolgt Workfront Kosten für Aufgaben und Projekte

* [Wie Workfront Kosten verfolgt](#how-workfront-tracks-costs)
* [Berechnung der geplanten, budgetierten und tatsächlichen Kosten durch Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [So berechnet Workfront Kostentypen für Aufgaben](#how-workfront-calculates-cost-types-for-tasks)

### Wie Workfront Kosten verfolgt  {#how-workfront-tracks-costs}

Sie können mehrere Kostentypen für Aufgaben und Projekte in Workfront verfolgen. Die Gesamtkosten werden nach folgender Formel berechnet:

`Costs = Labor Costs + Expense Costs`

* **Arbeitskosten** sind mit den Stunden für Aufgaben und Projekte sowie den Kosten pro Stunde der mit Aufgaben verbundenen Ressourcen verknüpft. Im Allgemeinen berechnet Workfront die folgenden Arbeitskosten:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Geplante Arbeitskosten</td> 
     <td> <p>Sie werden mit der folgenden Formel berechnet:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Veranschlagte Arbeitskosten</td> 
     <td> <p>Sie werden mit der folgenden Formel berechnet:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Tatsächliche Arbeitskosten</td> 
     <td> <p>Sie werden mit der folgenden Formel berechnet:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  Weitere Informationen finden Sie unter [Berechnung der geplanten, budgetierten und tatsächlichen Kosten durch Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs) in diesem Artikel beschrieben.

* **Kosten** sind mit Ausgaben für Projekte und Aufgaben verknüpft.\
  Wenn Sie ein Projekt erstellen, können Sie geplante Ausgaben für das gesamte Projekt festlegen. Zusätzlich können Sie Ausgaben mit neuen oder bestehenden Aufgaben verknüpfen. Weitere Informationen finden Sie unter [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Feste Kosten** sind als fester Kostenbetrag für ein Projekt definiert. Dies ist Teil der geplanten Kosten des Projekts, die den Geldbetrag darstellen, den Sie zum Abschluss des Projekts benötigen.

  >[!TIP]
  >
  >Beim Anhängen einer Vorlage an ein Projekt werden die Festkosten einer Vorlage zu den Festkosten des Projekts hinzugefügt. Weitere Informationen finden Sie unter [Übersicht über das Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Berechnung der geplanten, budgetierten und tatsächlichen Kosten durch Workfront {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront berechnet die geplanten Kosten und die tatsächlichen Kosten für jede einzelne Aufgabe eines Projekts. Workfront verwendet diese Berechnungen für einzelne Aufgaben zur Berechnung der geplanten Kosten und der tatsächlichen Kosten für das Projekt.

* [Geplante Kosten](#planned-cost)
* [Budgetierte Kosten](#budgeted-cost)
* [Istkosten](#actual-cost)

#### Geplante Kosten {#planned-cost}

Die geplanten Kosten eines Projekts sind die Kosten im Zusammenhang mit der geplanten Arbeit (geplante Stunden) des Projekts.

Die Plankosten eines Projekts werden nach folgender Formel berechnet:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Sie haben beispielsweise im Tab Ausgaben einer Aufgabe die folgenden Ausgaben: 100 $ Marketing-Ausgaben und 50 $ Verwaltungsausgaben. Wählen Sie auf der Registerkarte Finanzen den Kostentyp Benutzer Stündlich aus. Ein Benutzer wird der Aufgabe zugewiesen und die Stundenrate des Benutzers beträgt 15 USD. Der Benutzer wird fünf Stunden an dieser Aufgabe zugewiesen. Auf dem Tab Ausgaben des Projekts erhalten Sie Kosten in Höhe von 100 USD für eine so genannte Consulting-Ausgabe. Sie haben außerdem Festkosten in Höhe von 200 USD für das Projekt.

Die geplanten Kosten des Projekts werden wie folgt berechnet:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

Bei der Stundenrate in der Formel werden alle Datumsänderungen des Satzes berücksichtigt.

#### Budgetierte Kosten {#budgeted-cost}

Die budgetierten Kosten eines Projekts sind die Kosten im Zusammenhang mit der geplanten Arbeit (Budgetzeit) des Projekts.

Die veranschlagten Kosten des Projekts entsprechen den geplanten Kosten des Projekts, wenn die beiden folgenden Bedingungen erfüllt sind:

* Die geplanten Stunden der Aufgaben im Projekt stimmen mit den geplanten Stunden überein (im Ressourcenplaner)
* Die Aufgabe &quot;Rechnungsstellung&quot;lautet &quot;Rolle stündlich&quot;.

Die budgetierten Kosten des Projekts werden mit der folgenden Formel berechnet, wenn die folgenden Bedingungen erfüllt sind:

* Die geplanten Stunden der Aufgaben im Projekt stimmen nicht mit den geplanten Stunden überein (im Ressourcenplaner)
* Der Abrechnungstyp der Aufgaben ist &quot;Stündlich&quot;.

Wenn die oben genannten Bedingungen erfüllt sind, berechnet Workfront die budgetierten Projektkosten anhand der folgenden Formel:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Istkosten {#actual-cost}

Die tatsächlichen Kosten eines Projekts sind die Kosten, die mit der tatsächlichen Arbeit (angemeldete Stunden) des Projekts verbunden sind.

Die tatsächlichen Kosten werden anhand der folgenden Formel berechnet:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Sie haben beispielsweise im Tab Ausgaben einer Aufgabe die folgenden Ausgaben: eine Marketingaufwendung mit tatsächlichen Kosten von 110 USD und eine Verwaltungsaufwendung mit tatsächlichen Kosten von 40 USD. Sie wählen den Kostentyp Stündliche Rolle aus und weisen der Aufgabe die Rolle Berater-Job zu. Der Anteil der Berater-Job-Rolle beträgt 15 USD pro Stunde und es werden 6 Stunden für die Aufgabe als Berater-Job-Rolle protokolliert. Mit dem Projekt verbundene Beratungskosten (auf der Registerkarte &quot;Ausgaben&quot;) mit tatsächlichen Kosten von 100 USD und ein Benutzer mit einer Kosten pro Stunde von 20 USD in seinem Benutzerprofil protokolliert 10 Stunden im Projekt. Sie haben außerdem Festkosten in Höhe von 200 USD für das Projekt.

Die tatsächlichen Kosten des Projekts werden wie folgt berechnet:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

Bei der Stundenrate in der Formel werden alle Datumsänderungen des Satzes berücksichtigt.

>[!NOTE]
>
>Die tatsächlichen Kosten des Projekts werden wie folgt berechnet:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Diese Kosten werden in der Berechnung der tatsächlichen Kosten nicht dupliziert. Wenn beispielsweise ein Festbetrag zu den tatsächlichen Kosten des Projekts gehört, wird er nicht separat zu den tatsächlichen Kosten hinzugefügt.

>[!NOTE]
>
>Beim Protokollieren der Zeit in einem Projekt gibt es bei der Berechnung der tatsächlichen Arbeitskosten für das Projekt die folgenden Szenarien:
>
>* Standardmäßig verwendet Workfront die Kosten pro Stunde des Benutzers zur Berechnung der tatsächlichen Arbeitskosten.
>* Wenn der Benutzer, der die Uhrzeit protokolliert, keinen Kosten zugeordnet ist, verwendet Workfront die Kosten pro Stunde der Primären Rolle des Benutzers.
>* Wenn Ihr Workfront-Administrator die **Manuelles Zuweisen von Vorgangsrollen zu Stundeneinträgen** im Bereich &quot;Voreinstellungen&quot;für Timesheets und Stunden festlegen und die Zeit für die Benutzerprotokollierung im Projekt eine andere Rolle auswählt, die dieser Zeit zugeordnet werden soll, werden die tatsächlichen Kosten des Projekts basierend auf der Rolle berechnet, die bei der Aufzeichnung der Stunden angegeben wurde. Informationen zum Aktivieren der Protokollierungszeit für eine bestimmte Auftragsrolle finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### So berechnet Workfront Kostentypen für Aufgaben {#how-workfront-calculates-cost-types-for-tasks}

Die Planungs- und tatsächlichen Kosten der Aufgaben und ihre Arbeitskosten werden durch den Kostentyp jeder Aufgabe bestimmt.

Sie können den Kostentyp für einzelne Aufgaben innerhalb des Projekts konfigurieren. Jeder Kostentyp wirkt sich auf die Werte für geplante Kosten und tatsächliche Kosten aus.

Informationen zum Ändern des Kostentyps einer Aufgabe finden Sie unter [Aktualisierungstyp für Aufgaben](../../../manage-work/tasks/task-information/update-task-cost-type.md).

In der folgenden Tabelle werden die in Workfront verfügbaren Aufgabenkostentypen beschrieben:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Task Cost Type</strong> </p> </th> 
   <th> <p><strong>Beschreibung</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzer pro Stunde</p> </td> 
   <td> <p>Dies ist der Standardkostentyp beim Erstellen einer Aufgabe.</p> <p><strong>Geplante Kosten</strong> wird mit der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Wenn die geplanten Arbeitskosten berechnet werden durch:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Notiz: <p>Beachten Sie die folgenden Auswirkungen der Verwendung des User Stündlich-Kostentyps und der Berechnung der geplanten Kosten:</p> 
     <ul> 
      <li>Wenn Sie einer Aufgabe mehrere Ressourcen zuweisen, passt Workfront die Berechnungen für geplante Kosten basierend auf dem Prozentsatz der Aufgabe an, die jeder Ressource zugewiesen ist.</li>
      <li>Für die geltenden Kostensätze entsprechen die geplanten Arbeitskosten der Summe der geplanten Kosten für jeden Zeitraum, der von der Aufgabe abgedeckt wird.</li>
      <li>Der Wert des Felds Geplante Kosten kann davon abweichen, ob Sie die geplanten Kosten aus der Aufgabe selbst oder aus dem Bericht Verwendung anzeigen.<br><strong>Beim Anzeigen der geplanten Kosten aus der Aufgabe selbst:</strong> Das Feld Plante Kosten berücksichtigt das auf der Ebene der Auftragsrolle festgelegte Feld Kosten/Stunde (wenn das Feld Kosten/Stunde nicht auf Benutzerebene festgelegt wurde).<br><strong>Beim Anzeigen der geplanten Kosten aus dem Nutzungsbericht für das Projekt:</strong> Das Feld Plante Kosten berücksichtigt nicht das Kosten-/Stunden-Feld, das auf der Ebene der Auftragsrolle festgelegt wurde. Wenn Sie stattdessen möchten, dass der Nutzungsbericht das auf der Ebene der Auftragsrolle eingestellte Kosten-/Stunden-Feld berücksichtigt, müssen Sie den Kostentyp für die Aufgabe auf Stündlich Rolle festlegen. </li> 
     </ul> </p> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wenn die tatsächlichen Arbeitskosten berechnet werden durch:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Beispiel: Ein Benutzer hat in seinem Profil eine Kosten-pro-Stunde-Rate von 20 USD. Wenn sie 5 Stunden für eine Aufgabe protokollieren, beträgt die tatsächliche Arbeitskosten 100 USD für diese Aufgabe. Wenn dem Benutzer kein Kostensatz pro Stunde zugeordnet ist, werden die tatsächlichen Kosten anhand der Kosten pro Stunde ihrer Primären Auftragsrolle berechnet. Wenn sie keine Arbeitsplatzrolle haben oder die Kosten pro Stunde-Rate ihrer Arbeitsplatzrolle nicht definiert ist, beträgt die tatsächliche Kosten der Aufgabe null. </p> <p>Hinweis: Die tatsächlichen Kosten werden basierend auf der Rate der Kosten pro Stunde für den Benutzer berechnet, der die Zeit protokolliert, unabhängig davon, wer der Aufgabe zugewiesen ist. Außerdem berücksichtigt der Abrechnungsstundensatz in der Formel alle Datumsänderungen des Satzes.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stundensatz nach Funktion</p> </td>
   <td> <p><strong>Geplante Kosten</strong> wird mit der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Dabei werden die geplanten Arbeitskosten berechnet durch:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Hinweis: Wenn Sie einer Aufgabe mehrere Ressourcen zuweisen, passt Workfront die Berechnungen für "Geplante Stunden"basierend auf dem Prozentsatz der Aufgabe an, die jeder Ressource zugewiesen ist. Außerdem berücksichtigt der Stundensatz in der Formel alle Datumsänderungen des Satzes.</p> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wenn die tatsächlichen Arbeitskosten der Aufgabe berechnet werden durch:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Beispielsweise wird eine Aufgabe einer Auftragsrolle oder einem Benutzer mit einer Auftragsrolle zugewiesen, deren Kosten pro Stunde 20 USD betragen. Wenn ein Benutzer 5 Stunden für eine Aufgabe protokolliert, beträgt die tatsächliche Arbeitskosten 100 USD für diese Aufgabe. Wenn dem Benutzer, der der Aufgabe zugewiesen wurde, keine Aufgabenrolle zugeordnet ist, werden die tatsächlichen Kosten anhand der Kosten pro Stunde ihrer Primären Auftragsrolle berechnet. Wenn sie keine Arbeitsplatzrolle haben oder die Kosten pro Stunde-Rate ihrer Arbeitsplatzrolle nicht definiert ist, beträgt die tatsächliche Kosten der Aufgabe null. </p> <p>Notiz:   <p> Die tatsächlichen Stunden einer rollenbasierten Aufgabe berechnen sich auf der Basis der Vorgangsrollen der mit der Aufgabe verknüpften Benutzer und nicht anhand der Rollen des Benutzers, der die Zeit protokolliert. Außerdem berücksichtigt der Abrechnungsstundensatz in der Formel alle Datumsänderungen des Satzes.</p> <p>Wenn Ihr Workfront-Administrator die <strong>Manuelles Zuweisen von Vorgangsrollen zu Stundeneinträgen</strong> im Bereich "Voreinstellungen"für Timesheets und Stunden festlegen und die Zeit für die Benutzerprotokollierung in der Aufgabe eine andere Rolle auswählt, die dieser Zeit zugeordnet werden soll, wird die tatsächliche Kosten einer Aufgabe "Stündlich"basierend auf der Rolle berechnet, die bei der Aufzeichnung der Stunden angegeben wurde. Informationen zum Aktivieren der Protokollierungszeit für eine bestimmte Auftragsrolle finden Sie im Artikel <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Zeitblatt- und Stundenvoreinstellungen konfigurieren</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festgelegt pro Stunde</p> </td> 
   <td> <p><strong>Geplante Kosten</strong> wird mit der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Wo die Task Labour Cost berechnet werden durch:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Wenn die tatsächlichen Arbeitskosten der Aufgabe berechnet werden durch:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Dieser Kostentyp berücksichtigt keine einzelnen Benutzer oder Auftragsrollen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Keine Kosten</p> </td> 
   <td> <p>Dieser Kostentyp hat keine Auswirkungen auf die Kosten. Wenn eine übergeordnete Aufgabe diesen Kostentyp hat, berechnen Unteraufgaben mit einem anderen Kostentyp entsprechend ihren individuellen Kostentypen und die Kosten der übergeordneten Aufgabe werden entsprechend beeinflusst. </p> <p>Wenn ein Benutzer ohne Zugriff auf Finanzdaten oder ein Benutzer ohne finanzielle Berechtigungen für eine Vorlage ein Projekt aus dieser Vorlage erstellt, ist dies der Standardkostentyp für die Aufgaben im Projekt.</p> <p>Informationen zum Zugriff auf Finanzdaten finden Sie im Artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> <p>Weitere Informationen zu finanziellen Berechtigungen für Objekte finden Sie im Artikel <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Freigeben von Finanzberechtigungen für ein Objekt</a>.</p> <p>Informationen zum Erstellen von Projekten aus Vorlagen finden Sie im Artikel <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Erstellen eines Projekts mit einer Vorlage</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## So verfolgt Workfront Kosten für Probleme {#how-workfront-tracks-costs-for-issues}

Probleme haben keine Auswirkungen auf die folgenden Kostentypen eines Projekts:

* Geplante Kosten
* Budgetierte Kosten

Probleme können jedoch **Tatsächliche Kosten** was sich auch auf die tatsächlichen Kosten des Projekts auswirkt.

In der folgenden Tabelle wird erläutert, wie die tatsächlichen Kosten für Probleme berechnet werden, je nach Art der Zuweisung zu dem Problem:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Tatsächliche Kosten des Problems</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerzuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Die Kosten pro Stunde des Benutzers, der die Zeit protokolliert, wird hier berücksichtigt, unabhängig davon, wer dem Problem zugewiesen ist. </p> <p>Wenn der Benutzer, der die Zeit protokolliert, keine Kosten pro Stunde in seinem Profil hat, berechnet die Kostensatz pro Stunde seiner Primären Auftragsrolle die tatsächlichen Kosten des Problems. Wenn der Benutzer, der die Zeit protokolliert, in seinem Profil keine Rolle hat oder keine zugehörige Rate zugeordnet ist, werden die tatsächlichen Stunden anhand der Kosten pro Stunde-Rate der Primären Auftragsrolle des Primären Bevollmächtigten für das Problem berechnet. Wenn für diese Rolle kein Prozentsatz definiert ist, liegen die tatsächlichen Kosten des Problems bei null. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rollenzuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Die Kosten pro Stunde des Benutzers, der die Zeit für das Problem protokolliert, wird hier berücksichtigt, unabhängig davon, welche Rolle dem Problem zugewiesen ist. </p> <p>Wenn dem Benutzer, der die Zeit protokolliert, keine Kosten pro Stunde zugeordnet ist, berechnet die Kostensatz pro Stunde seiner Primären Rolle die tatsächlichen Kosten des Problems.<br>Wenn der Benutzer, der die Zeit protokolliert, keine Rolle in seinem Profil hat oder keine Quote damit verknüpft ist, beträgt die tatsächliche Ausgabe des Problems null. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Keine Zuweisung</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Tatsächliche Kosten</strong> wird mit der folgenden Formel berechnet:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Wenn dem Benutzer, der die Uhrzeit protokolliert, keine Kosten pro Stunde mit seinem Profil verbunden ist, berechnet die Kostensatz pro Stunde seiner Primären Auftragsrolle die tatsächlichen Kosten des Problems. </p> <p>Wenn dem Benutzer, der die Zeit protokolliert, keine Stellenrolle mit seinem Profil zugeordnet ist oder dessen Primäre Rolle "Job"keine Kostensätze pro Stunde definiert hat, beträgt die tatsächliche Kosten des Problems null. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
