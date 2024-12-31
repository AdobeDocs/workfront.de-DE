---
content-type: overview
product-area: projects
navigation-topic: financials
title: Übersicht über Abrechnung und Umsatz
description: Als Projekt-Manager können Sie Abrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu erfassen.
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '3691'
ht-degree: 0%

---

# Übersicht über Abrechnung und Umsatz

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

Als Projekt-Manager können Sie Abrechnungssätze verwenden, um den Umsatz Ihrer Projekte zu erfassen.

In diesem Artikel wird das Tracking des Umsatzes für Projekte beschrieben. Der Umsatz wird im Auslastungsbericht anders berechnet. Informationen zu Umsatzberechnungen im Auslastungsbericht finden Sie unter [Ressourcenauslastungsinformationen anzeigen](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Übersicht über Abrechnungssätze

Beachten Sie beim Arbeiten mit Abrechnungssätzen Folgendes:

* Sie benötigen eine Plan- oder Standardlizenz mit Bearbeitungszugriff auf Finanzdaten, um Abrechnungssätze verwalten zu können.\
  Weitere Informationen zum Gewähren des Zugriffs auf Finanzdaten finden Sie unter [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Abrechnungssätze sind Umsatzbeträge pro Arbeitseinheit, die mit Aufgabengebieten oder Benutzern verknüpft sind.

  Das Multiplizieren der Sätze mit den für die Arbeit aufgewendeten Stunden generiert Umsätze für Ihre Projekte.

* Nachdem Sie Ihre Abrechnungssätze festgelegt haben, können Sie den Umsatz verfolgen, indem Sie Abrechnungs-Datensätze erstellen, um zu erfassen, was in Rechnung gestellt wurde und was nicht.

  >[!TIP]
  >
  >Wenn Sie einen Rechnungsnachweis als In Rechnung gestellt markieren, kann er nie bearbeitet werden. Dies ist wichtig, wenn Ihre Sätze variieren und Sie die Umsatz- und Ausgabeninformationen für Ihr Projekt sperren möchten. Wenn Sie ihn zu einem Rechnungsnachweis hinzufügen und als „In Rechnung gestellt“ markieren, wird er nicht aktualisiert, wenn die Tarife in Ihrem System aktualisiert werden.

  Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md).

* Sie können Abrechnungssätze für Benutzer, Aufgabengebiete oder einen einmaligen Abrechnungssatz für ein Projekt oder eine Aufgabe erstellen.

>[!IMPORTANT]
>
>Die Sätze, mit denen der Umsatz berechnet wird, gehören dem Benutzer, der die Zeit protokolliert, oder seinen Aufgabengebieten.

* [Benutzer-Abrechnungssätze](#user-billing-rates)
* [Abrechnungssätze für Aufgabengebiete](#job-role-billing-rates)
* [Feste Abrechnungssätze für Projekte oder Aufgaben](#fixed-billing-rates-for-projects-or-tasks)
* [Abrechnungssätze überschreiben](#override-billing-rates)

### Benutzer-Abrechnungssätze {#user-billing-rates}

Wenn Sie als Benutzeradministrator einen Benutzer erstellen, können Sie ihn mit datumswirksamen Abrechnungssätzen verknüpfen, indem Sie Werte für die Felder Abrechnung pro Stunde und die Datumsangaben für die Sätze angeben.

Weitere Informationen zum Erstellen von Benutzern finden Sie im Artikel [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![Benutzerkosten und Abrechnungssätze bearbeiten](assets/edit-user-cost-billing-rate-1.png)

### Abrechnungssätze für Aufgabengebiete {#job-role-billing-rates}

Wenn Sie als Adobe Workfront-Administrator ein Aufgabengebiet erstellen, können Sie es mit datumswirksamen Abrechnungssätzen verknüpfen, indem Sie Werte für die Felder „Abrechnung pro Stunde“ und die Datumsangaben für die Sätze angeben.

Sie können den Wert eines Abrechnungssatzes für Aufgabengebiete mithilfe der Basiswährung Ihres Workfront-Systems oder einer anderen benutzerdefinierten Währung definieren.

Weitere Informationen zum Erstellen von Aufgabengebieten und zum Überschreiben ihrer Währung finden Sie im Artikel [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

![Bearbeiten der Kosten und Abrechnungssätze für Aufgabengebiete](assets/edit-job-role-multiple-billing-rates-new.png)

### Feste Abrechnungssätze für Projekte oder Aufgaben {#fixed-billing-rates-for-projects-or-tasks}

Zusätzlich zu den Stundensätzen für Benutzer und Aufgabengebiete können Sie auch die folgenden festen Abrechnungssätze haben:

* Fester Betrag für Umsatztyp „Fester Stundenbetrag“
* Fester Betrag für Umsatztyp Feste Einnahmen

Weitere Informationen dazu, wie die festen Abrechnungssätze zur Berechnung des Umsatzes verwendet werden, finden Sie unter [Übersicht über Aufgabenumsatztypen](#overview-of-task-revenue-types).

### Abrechnungssätze überschreiben {#override-billing-rates}

>[!IMPORTANT]
>
>Sie können die mit Aufgabengebieten verknüpften Abrechnungssätze überschreiben. Sie können Benutzer-Abrechnungssätze oder Festsätze nicht überschreiben.

Sie können Abrechnungssätze für Aufgabengebiete überschreiben für:

* Ein bestimmtes Unternehmen

  Weitere Informationen zum Erstellen unternehmensspezifischer Abrechnungssätze für Aufgabengebiete finden Sie unter [Firmen erstellen und bearbeiten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Ein bestimmtes Projekt

  Weitere Informationen zum Erstellen projektspezifischer Abrechnungssätze für Aufgabengebiete finden Sie im Artikel [Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Umsatzbeträge verfolgen

Workfront kann den geplanten Umsatz automatisch verfolgen, wenn Aufgaben basierend auf den geplanten Stunden der Aufgaben erstellt werden.

Es kann auch den tatsächlichen Umsatz automatisch verfolgen, wenn die tatsächlichen Stunden für Aufgaben, Probleme und für das Projekt protokolliert werden.

Die folgende Tabelle zeigt die Umsatztypen, die mit Aufgaben, Problemen und Projekten verbunden sind.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Geplante Einnahmen</td> 
   <td> <p>Bei Aufgaben ist dies der Umsatz, der mit den geplanten Stunden an Aufgaben verknüpft ist. Die geplanten Stunden aller Aufgaben summieren sich auf die geplanten Stunden des Projekts, um zur Berechnung der geplanten Stunden des Projekts beizutragen. </p> <p>Weitere Informationen zu den geplanten Stunden in Workfront finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Übersicht über die geplanten Stunden</a>. </p> <ul><li><p>Workfront berechnet den geplanten Umsatz für Aufgaben anhand der folgenden Formel:</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>HINWEIS</strong></br> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen des Satzes.</p> </li><li><p>Workfront berechnet die geplanten Einnahmen für Projekte anhand der folgenden Formel:</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>NOTIZ</b>

<p>Die geplanten Projekteinnahmen, die im Bereich „Projektdetails“ und in Projektberichten angezeigt werden, unterscheiden sich von den geplanten Einnahmen, die im Auslastungsbericht angezeigt werden. </p></li></ul> <p>Die geplanten Einnahmen im Bereich „Projektdetails“ spiegeln die mit den geplanten Stunden für die Aufgabe verbundenen Einnahmen sowie die Festeinnahmen des Projekts wider. Der geplante Umsatz im Auslastungsbericht zeigt den geplanten Umsatz an, der nur den geplanten Stunden aus den Aufgabenzuordnungen des Projekts zugeordnet ist. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Wenn das Projekt 1 Aufgabe mit 10 Stunden hat, einem Berater mit einem Stundensatz von 20 US-Dollar zugewiesen ist und das Projekt einen festen Umsatz von 100 US-Dollar hat, zeigt der Auslastungsbericht 200 US-Dollar für den geplanten Umsatz an (der geplante Umsatz, der mit den Stunden für die Aufgabe verknüpft ist). Im Abschnitt Projektdetails werden 300 $ angezeigt (der geplante Umsatz aus der Aufgabe und der feste Umsatz für das Projekt). </p> 
     </div> </p> <p>Der geplante Aufgabenumsatz wird anhand der Stundensätze für die Abrechnung der Benutzenden oder Aufgabengebiete berechnet, die den Aufgaben zugewiesen wurden. Der Umsatztyp der Aufgaben beeinflusst, welche Rate (Benutzer oder Funktion) für die Berechnung des geplanten Umsatzes verwendet wird. Weitere Informationen finden Sie in den folgenden Abschnitten in diesem Artikel:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Übersicht über Aufgabenumsatztypen</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen</a> </p> </li> 
    </ul> <p>Weitere Informationen zu Berechnungen des geplanten Umsatzes im Auslastungsbericht finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Informationen zur Ressourcenauslastung anzeigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tatsächliche Einnahmen*</td> 
   <td> <p>Der Umsatz, der mit den tatsächlichen Stunden an Aufgaben, Problemen und Projekten verbunden ist. </p> <p>Im Allgemeinen berechnet Workfront den tatsächlichen Umsatz anhand der folgenden Formel:</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>HINWEIS</strong></br> Der Stundensatz für die Abrechnung in der Formel berücksichtigt alle Datumsänderungen des Satzes.</p> <p>Informationen zu den Berechnungen des tatsächlichen Umsatzes im Auslastungsbericht finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Informationen zur Ressourcenauslastung anzeigen</a>. </p> <p><b>TIPP</b>

Sie können den tatsächlichen Umsatz auf Anfrageebene nicht anzeigen. Der mit den tatsächlichen Stunden für die Probleme verknüpfte Umsatz trägt jedoch zum tatsächlichen Umsatz des Projekts bei. </p> </td>
</tr> 
 </tbody> 
</table>

*Für tatsächliche Stunden beziehen sich die Tarife der Benutzenden immer auf die Benutzenden, die die Stunden protokollieren, oder auf die Tarife ihrer Aufgabengebiete. Informationen dazu, wann Workfront die Raten der Benutzenden verwendet und wann es die Raten ihrer Aufgabengebiete verwendet, finden Sie im Abschnitt [Umsatzberechnungen](#revenue-calculations) dieses Artikels.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Beispiel: Wenn für eine Aufgabe mit dem Umsatztyp „Benutzer pro Stunde“ eine Dauer von 2 Stunden geplant ist und der ihr zugewiesene Benutzer einen Stundensatz von 30 USD pro Stunde hat, beträgt der geplante Umsatz der Aufgabe 60 USD. Wenn nach Abschluss der Aufgabe der Benutzer nur 1,5 Stunden als tatsächliche Zeit für die Fertigstellung der Aufgabe protokolliert, beträgt der tatsächliche Umsatzbetrag 45 USD. Wenn ein anderer Benutzer, der der Aufgabe nicht zugewiesen ist, die Zeit protokolliert, wird der tatsächliche Umsatz anhand der Abrechnungssätze dieses Benutzers berechnet.

Sie können den Umsatz wie folgt erfassen:

* Indem Sie den Umsatztyp Ihrer Aufgaben definieren und Benutzende oder Rollen, die Arbeitselementen zugewiesen sind, mit Abrechnungssätzen verknüpfen. Dieser berechnet den Umsatz anhand der geplanten oder tatsächlichen Stunden für die Arbeitselemente. Sie können eine Obergrenze auf den Höchstbetrag festlegen, der für Stundensätze berechnet wird, oder nicht.\
  Weitere Informationen zum Festlegen des Umsatztyps einer Aufgabe finden Sie im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Durch Fakturierung eines pauschalen Festeinnahmensatzes für Aufgaben oder Projekte.\
  Wenn Sie Aufgaben mit Festeinnahmen haben, wird der Festeinnahmenbetrag als geplanter Umsatz einer Aufgabe oder eines Projekts hinzugefügt, und der geplante Umsatz einer Aufgabe kann einem Rechnungsnachweis als Festeinnahme hinzugefügt werden.
* Indem Sie einen festen Einnahmensatz für die pauschale Abrechnung für ein Projekt festlegen und anschließend Stundensätze für die Aufgaben innerhalb des Projekts festlegen. Workfront fügt die Stundensätze für die Aufgaben zur Pauschale des Projekts hinzu.\
  So könnte ein Mechaniker, der Workfront verwendet, beispielsweise Kosten für Teile als Festeinnahmen für das Projekt eingeben und dann die für die Reparatur eines Fahrzeugs aufgewendete Zeit stündlich in Rechnung stellen. Feste Einnahmen aus Projekten oder Aufgaben werden dann nach Abschluss realisiert.

Sie können Ihre Aufgaben auch als „Nicht fakturierbar“ markieren. In diesem Fall sind keine geplanten oder tatsächlichen Einnahmen mit ihnen verbunden.

## Übersicht über Aufgabenumsatztypen {#overview-of-task-revenue-types}

Standardmäßig wird der Umsatztyp für alle neuen Aufgaben gemäß den von Ihrem Workfront- oder Gruppenadministrator festgelegten Aufgaben- und Problemeinstellungen festgelegt.\
Weitere Informationen zum Definieren der Aufgaben- und Problemvoreinstellungen für Ihre Workfront-Instanz finden Sie im Artikel [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Der Projektbesitzer kann den Umsatztyp von Aufgaben und den Festeinnahmen für Projekte ändern.\
Weitere Informationen zur Angabe der Festeinnahmen eines Projekts finden Sie im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).\
Weitere Informationen zum Festlegen des Umsatztyps einer Aufgabe finden Sie im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Sie können die folgenden Umsatztypen auf Ihre Aufgaben oder Projekte anwenden:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Umsatztyp</strong> </p> </th> 
   <th> <p><strong>Beschreibung</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Festeinnahmen</p> </td> 
   <td> <p>Dieser Typ kann mit Projekten und Aufgaben verwendet werden. </p> <p>Wenn Sie eine Vorlage an ein Projekt anhängen, wird der feste Umsatz der Vorlage zum festen Umsatz des Projekts hinzugefügt. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Übersicht über das Anhängen einer Vorlage an ein Projekt</a>. </p> <p>Bei Vorgängen wird unabhängig von den Aufgabenzuordnungen der Umsatz für die Aufgabe immer unter Verwendung des Festbetrags berechnet, der für die Aufgabe angegeben wurde. </p> <p>Der feste Umsatz aus untergeordneten Aufgaben summiert sich zum Umsatz der übergeordneten Aufgabe und dann zum Umsatz des Projekts. Wenn für die übergeordnete Aufgabe und/oder das Projekt ein fester Betrag definiert ist, wird der Betrag zu den geplanten Einnahmen addiert, die aus allen untergeordneten Aufgaben aggregiert werden.</p> <p>Der Betrag der Festeinnahmen aus Vorgängen kann in einem Rechnungsnachweis für das Projekt enthalten sein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer pro Stunde</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden. </p> <p>Der Abrechnungssatz, den Sie für einen bestimmten Benutzer festlegen, multipliziert mit der Anzahl der geplanten Stunden für diese Aufgabe, wird zum geplanten Umsatzbetrag der Aufgabe. Der Abrechnungssatz, den Sie für einen bestimmten Benutzer festlegen, multipliziert mit der Anzahl der Stunden, die der Benutzer für die Aufgabe protokolliert, ist der tatsächliche Umsatzbetrag der Aufgabe. <br>Wenn Sie beispielsweise einen Benutzer erstellen und für sein Feld Abrechnung pro Stunde $20 festlegen, und der Benutzer fünf Stunden für eine Aufgabe auf der Arbeitszeittabelle einreicht, beträgt der tatsächliche Abrechnungsbetrag der Aufgabe $100.</p>
   <p>Ein Benutzerprofil kann mehrere Abrechnungssätze mit Gültigkeitsdaten enthalten. Beispielsweise endet der erste Benutzer-Abrechnungssatz von 20 $ am 30. April 2023 und der zweite Benutzer-Abrechnungssatz von 25 $ beginnt am 1. Mai 2023. Wenn der Benutzer 2 Stunden am 28. April und 3 Stunden am 2. Mai für eine Aufgabe einreicht, beträgt der tatsächliche Rechnungsbetrag der Aufgabe 40 $ + 75 $ = 115 $.</p>
   <p><b>TIPP</b>

Dies ist der standardmäßige Umsatztyp beim Erstellen einer Aufgabe.</p> </td>
</tr> 
  <tr> 
   <td> <p>Stundensatz nach Funktion</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden.</p> <p>Dieser Typ ähnelt dem „Benutzer pro Stunde“, verwendet jedoch Tarife für Aufgabengebiete anstelle von Benutzerraten.</p> <p><strong>HINWEIS</strong><br> Ein Aufgabengebiet kann auch mehrere Abrechnungssätze mit Datum des Wirksamwerdens aufweisen.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer pro Stunde mit Obergrenze</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden.</p> <p>Aufgaben werden stündlich wie in „Benutzer stündlich“ abgerechnet, sie haben jedoch einen maximalen Höchstbetrag, den Sie angeben können. <br>Beispiel: Wenn der Abrechnungssatz eines Benutzers 25 USD beträgt, der Höchstbetrag für die Aufgabe jedoch 20 USD beträgt und der Benutzer eine Stunde protokolliert, beträgt der tatsächliche Umsatz für die Aufgabe 20 USD. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stundensatz nach Funktion mit Obergrenze</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden.</p> <p>Dieser Typ ähnelt dem Benutzer „Stündlich mit Begrenzung“, verwendet jedoch Vorgangsrollensätze anstelle von Benutzerraten. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzer pro Stunde plus festgelegt</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden. </p> <p>Aufgaben werden stündlich wie in „Benutzer stündlich“ abgerechnet, haben jedoch einen festen Betrag, den Sie zum Benutzertarif hinzufügen können. Der für die Aufgabe angegebene Festbetrag kann in den Rechnungsnachweisen für das Projekt enthalten sein. Der Festbetrag wird nicht mit den Stunden für die Aufgabe multipliziert. Nur der Abrechnungssatz des Benutzers tut das. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stundensatz nach Funktion plus fest</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden. </p> <p>Aufgaben werden stündlich wie in Funktion „Stündlich“ abgerechnet, es gibt jedoch einen zusätzlichen festen Betrag, den Sie zum Abrechnungssatz hinzufügen können. Der für die Aufgabe angegebene Festbetrag kann in den Rechnungsnachweisen für das Projekt enthalten sein. Der Festbetrag wird nicht mit den Stunden für die Aufgabe multipliziert. Nur der Abrechnungssatz für das Aufgabengebiet ist gültig. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festgelegt pro Stunde</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden.</p> <p>Die Obergrenze oder der feste Betrag, die Sie für die Aufgabe festlegen, multipliziert mit der Anzahl der für die Aufgabe eingegebenen Stunden (unabhängig von Benutzer oder deren Aufgabengebiet) ist der Fakturierungsbetrag.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nicht fakturierbar</p> </td> 
   <td> <p>Dieser Typ kann nur für Aufgaben verwendet werden.</p> <p>Dieser Umsatztyp hat keine Auswirkungen auf den Umsatz. </p> <p>Wenn ein übergeordnetes Objekt diese Einstellung aufweist, werden untergeordnete Aufgaben mit einem Abrechnungstyp weiterhin normal angewendet.</p> <p>Wenn ein(e) Benutzende(r) ohne Zugriff auf Finanzdaten oder ein(e) Benutzende(r) ohne Finanzberechtigungen für eine Vorlage ein Projekt aus dieser Vorlage erstellt, ist dies der standardmäßige Umsatztyp für die Aufgaben im Projekt.</p> <p>Informationen zum Zugriff auf Finanzdaten finden Sie im Artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.<br>Informationen zu finanziellen Berechtigungen für Objekte finden Sie im Artikel <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über Freigabeberechtigungen für Objekte</a>.<br>Informationen zum Erstellen von Projekten aus Vorlagen finden Sie im Artikel <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Erstellen eines Projekts mithilfe einer Vorlage</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Übersicht über den Umsatz für übergeordnete Aufgaben

Wenn Sie eine eigenständige Aufgabe mit Fakturierungsinformationen in eine übergeordnete Aufgabe ändern, behält die neue übergeordnete Aufgabe weiterhin alle Rechnungsinformationen bei, die zuvor auf sie angewendet wurden, zusammen mit den zuvor angewendeten Stunden. Rechnungsinformationen, die aus Stunden stammen, die für untergeordnete Aufgaben protokolliert wurden, werden als tatsächlicher Umsatz für die neue übergeordnete Aufgabe aggregiert.

Der geplante Umsatz aus den untergeordneten Aufgaben wird ebenfalls auf die übergeordnete Aufgabe angerechnet.

## Überblick über den Umsatz für Probleme

Probleme haben keine geplanten oder tatsächlichen Umsatzbeträge, können aber Istkosten aufweisen.

Wenn Sie Stunden für ein Problem protokollieren und einen Stundentyp verwenden, der als „Als Umsatz zählen“ gekennzeichnet ist, berechnet Workfront einen Istkostenbetrag entsprechend der Rate des Benutzers, der sich in der Zeit anmeldet. Diese Zahl wird den Ist-Kosten des Projekts hinzugefügt. Die Stunden können auch in einem Rechnungsnachweis enthalten sein.

Weitere Informationen zur Kostennachverfolgung finden Sie im Artikel [Kosten nachverfolgen](../../../manage-work/projects/project-finances/track-costs.md).

Weitere Informationen zu Stundentypen finden Sie im Artikel [Verwalten von Stundentypen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Einnahmenberechnungen

* [Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Umsatzberechnungen für Aufgaben basierend auf Benutzer- und Rollenzuweisungen {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Berücksichtigen Sie bei der Berechnung des Umsatzes für eine Aufgabe Folgendes:

* Wenn ein(e) Benutzende(r) oder ein Aufgabengebiet eine Rate von 0,00 $ anzeigt, liest Workfront dies als gültigen Betrag ein und multipliziert diesen Betrag mit der Anzahl der Stunden für die Aufgabe, um den Umsatz zu berechnen. Wenn Sie für Ihre Aufgaben keinen Umsatz anzeigen möchten, stellen Sie sicher, dass das Feld für den Abrechnungssatz für Ihre Benutzerin bzw. Ihren Benutzer oder Ihr Aufgabengebiet leer ist.
* Wenn Abrechnungssätze für Aufgabengebiete gelten, verwendet Workfront bei jedem Überschreiten eines Abrechnungssatzes für das Projekt den Überschreibungssatz auf Projektebene anstelle des auf Systemebene definierten Abrechnungssatzes für diese Funktion.
* Wenn der Benutzer oder das Aufgabengebiet für den tatsächlichen Umsatz über mehrere Abrechnungssätze mit effektiven Datumsangaben verfügt, ist der Aufgabenumsatz die Summe der Einnahmen jedes Zeitraums, in dem der Benutzer die Zeit erfasst hat. Der geplante Umsatz basiert auf den geplanten Stunden für die Zeiträume.
* Im Falle mehrerer Bevollmächtigter für die Aufgaben gelten die unten beschriebenen Szenarien für jeden Bevollmächtigten.

Es gibt eine Hierarchie darüber, welcher Satz in Umsatzberechnungen verwendet wird, die auf Aufgabenzuweisungen basieren.

Wenn Ihr Workfront-Administrator die Einstellung **Aufgabengebiete zu Stundeneinträgen manuell zuweisen** im Bereich Arbeitszeittabellen- und Stunden-Voreinstellungen aktiviert hat und die Benutzenden, die für das Projekt die Zeit erfassen, eine andere Rolle auswählen, die mit dieser Zeit verknüpft werden soll, wird der tatsächliche Umsatz der Aufgabe oder des Projekts immer auf der Grundlage der Rolle berechnet, die mit dem Stundeneintrag verknüpft ist. Informationen zur Aktivierung der Protokollierungszeit für ein bestimmtes Aufgabengebiet finden Sie im Artikel [Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Bei der Berechnung des Aufgabenumsatzes basierend auf dem Umsatztyp und der Art der Aufgabenzuweisung gibt es die folgenden Szenarien:

* **Der Umsatztyp der Aufgabe lautet „Benutzer pro Stunde“**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Abrechnung pro Stundensatz</td> 
     <td>Keine Zuweisung</td> 
     <td>Benutzerzuweisung</td> 
     <td>Zuweisung eines Aufgabengebiets</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Abrechnung des Satzes pro Stunde für den geplanten Umsatz</td> 
     <td>0,00 $</td> 
     <td> Wenn ein Benutzer einen Abrechnungssatz in seinem Profil hat, wird dieser Satz zur Berechnung des geplanten Umsatzes verwendet. Andernfalls wird der Abrechnungssatz des Systems für das primäre Aufgabengebiet verwendet. <br><p><b>HINWEIS</b> Der Benutzer kann der Aufgabe mit einem seiner sekundären Aufgabengebiete zugewiesen werden, hier wird jedoch stattdessen die Rate des primären Aufgabengebiets verwendet.</p><p>Wenn sich die Rolle des/r Benutzenden während der Zuweisung geändert hat, werden bei der Neuberechnung der Projektfinanzen die richtigen Sätze angewendet.</p></td> 
     <td><p><span class="preview">Wenn dem Projekt eine Tarifkarte beigefügt ist, wird der geplante Umsatz anhand des Aufgabengebiets der Tarifkarte berechnet.</span></p> <p><span class="preview">Die Abrechnungssätze können auf Projektebene überschrieben werden.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Abrechnungssatz pro Stunde für tatsächlichen Umsatz</td> 
     <td>Wenn der Benutzer, der die Stunden erfasst, einen Abrechnungssatz in seinem Profil hat, wird dieser Satz verwendet. 
     <br><span class="preview">Wenn die Zeit für einen Benutzer oder eine Funktion protokolliert wird, der bzw. die in den erweiterten Zuweisungen eine standortspezifische Zuweisung hat, wird die Rate des Standorts verwendet.</span>
     <br>Andernfalls wird der Abrechnungssatz ihrer primären Aufgabengebiete verwendet. Wenn mit dem Benutzer oder seiner primären Rolle kein Abrechnungssatz verknüpft ist, beträgt der tatsächliche Umsatz 0,00 USD. <br><p><b>NOTIZ</b>

  Für die Berechnung werden nur die Tarife berücksichtigt, die dem Benutzer zugeordnet sind, der die Zeit erfasst hat, auch wenn der Aufgabe ein anderer Benutzer zugeordnet ist.</p></td>
  <td>Wenn der Benutzer, der die Stunden erfasst, einen Abrechnungssatz in seinem Profil hat, wird dieser Satz verwendet. <br><span class="preview">Wenn die Zeit für einen Benutzer oder eine Funktion protokolliert wird, der bzw. die in den erweiterten Zuweisungen eine standortspezifische Zuweisung hat, wird die Rate des Standorts verwendet.</span><br>Andernfalls wird der Abrechnungssatz ihrer primären Aufgabengebiete verwendet. Wenn mit dem Benutzer oder seiner primären Rolle kein Abrechnungssatz verknüpft ist, beträgt der tatsächliche Umsatz 0,00 USD. <br><p><b>NOTIZ</b>

  Für die Berechnung werden nur die Tarife berücksichtigt, die dem Benutzer zugeordnet sind, der die Zeit erfasst hat, auch wenn der Aufgabe ein anderer Benutzer zugeordnet ist.</p></td>
  <td>Wenn der Benutzer, der die Stunden erfasst, einen Abrechnungssatz in seinem Profil hat, wird dieser Satz verwendet. Andernfalls wird der Abrechnungssatz ihrer primären Aufgabengebiete verwendet.<br><p><b>NOTIZ</b>

  Wenn der Benutzerprotokollierungszeit kein Abrechnungssatz zugeordnet ist und sie kein Aufgabengebiet oder keinen Abrechnungssatz für ihr Aufgabengebiet hat, wird der Satz aus dem Aufgabengebiet verwendet, das mit der Aufgabe verknüpft ist. Wenn für diese Rolle kein Abrechnungssatz vorhanden ist, beträgt der Umsatz 0,00 USD</p></td>
  </tr> 
   </tbody> 
  </table>

* **Der Umsatztyp der Aufgabe lautet „Stundensatz nach Funktion“**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Abrechnung pro Stundensatz</td> 
     <td>Keine Zuweisung</td> 
     <td>Benutzerzuweisung</td> 
     <td>Zuweisung eines Aufgabengebiets</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Abrechnung des Satzes pro Stunde für den geplanten Umsatz</td> 
     <td>0,00 $</td> 
     <td><p>Workfront prüft das Aufgabengebiet, das der Benutzer bei der Berechnung des geplanten Umsatzes erfüllt. <br>Wenn der/die Benutzende mit keiner Rolle in der Aufgabe verknüpft ist, beträgt der Umsatz 0,00 $.</p> <p><strong>HINWEIS</strong><br> Wenn sich die Rolle des Benutzers während der Zuweisung geändert hat, werden bei der Neuberechnung der Projektfinanzen die richtigen Sätze angewendet.</p> </td> 
     <td><p><span class="preview">Wenn dem Projekt eine Tarifkarte beigefügt ist, wird der geplante Umsatz anhand des Aufgabengebiets der Tarifkarte berechnet.</span></p> <p><span class="preview">Die Abrechnungssätze können auf Projektebene überschrieben werden.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Abrechnungssatz pro Stunde für tatsächlichen Umsatz</td> 
     <td>Workfront verwendet den Abrechnungssatz des primären Aufgabengebiets des Benutzers, der die Zeit protokolliert. <br><span class="preview">Wenn die Zeit für einen Benutzer oder eine Funktion protokolliert wird, der bzw. die in den erweiterten Zuweisungen eine standortspezifische Zuweisung hat, wird die Rate des Standorts verwendet.</span> <br>Wenn dem Benutzer, der die Zeit erfasst, kein Aufgabengebiet zugeordnet ist oder wenn das primäre Aufgabengebiet keinen Abrechnungssatz hat, beträgt der tatsächliche Umsatz 0,00 USD. </td> 
     <td> Wenn der Benutzer, der die Zeit erfasst, der Aufgabe zugewiesen ist, wird der Abrechnungssatz des Aufgabengebiets, das dem Benutzer in der Aufgabe zugeordnet ist, zur Berechnung des tatsächlichen Umsatzes verwendet. <br><span class="preview">Wenn die Zeit für einen Benutzer oder eine Funktion protokolliert wird, der bzw. die in den erweiterten Zuweisungen eine standortspezifische Zuweisung hat, wird die Rate des Standorts verwendet.</span> <br>Andernfalls wird der Abrechnungssatz ihrer primären Aufgabengebiete verwendet. Wenn der Benutzer kein primäres Aufgabengebiet hat oder sein primäres Aufgabengebiet keinen Abrechnungssatz hat, beträgt der tatsächliche Umsatz 0,00 USD. </td> 
     <td>Wenn eine der Aufgabengebiete des Benutzers, der die Zeit protokolliert, der Aufgabe zugewiesen wird, wird diese Aufgabengebietsrate verwendet. Wenn das der Aufgabe zugewiesene Aufgabengebiet nicht mit dem Benutzer verknüpft ist, der die Zeit erfasst hat, wird der Abrechnungssatz der primären Funktion des Benutzers verwendet, um den tatsächlichen Umsatz zu berechnen. Wenn der/die Benutzende kein Aufgabengebiet hat oder mit seinem/ihrem primären Aufgabengebiet keine Rate verknüpft ist, wird die Rate des Aufgabengebiets verwendet, das der Aufgabe zugewiesen wurde. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Einnahmenberechnungen für Projekte

Sie können die folgenden Umsatztypen für Projekte verfolgen:

* Die geplanten Einnahmen für ein Projekt werden nach folgender Formel berechnet:

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  Informationen zur Berechnung des geplanten Aufgabenumsatzes finden Sie im Abschnitt [Umsatzberechnungen für Aufgaben basierend auf Benutzer- und ](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)) in diesem Artikel.

* Die tatsächlichen Einnahmen für ein Projekt werden anhand der folgenden Formel berechnet:

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

Informationen zur Berechnung des tatsächlichen Aufgabenumsatzes finden Sie im Abschnitt [Umsatzberechnungen für Aufgaben basierend auf Benutzer- und ](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)) in diesem Artikel.

Für den tatsächlichen Umsatz in Verbindung mit den Stunden, die direkt im Projekt erfasst werden, oder mit den Problemen verwendet Workfront den Abrechnungssatz der Person, die die Zeit im Projekt erfasst. Wenn dem/der Benutzenden kein Abrechnungssatz zugeordnet ist, verwendet Workfront den Abrechnungssatz des Primären Aufgabengebiets. Wenn beide Sätze null sind, ist der tatsächliche Umsatz, der mit den für das Projekt oder die Probleme protokollierten Stunden verbunden ist, null.
