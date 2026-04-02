---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossar der Terminologie von  [!DNL Adobe Workfront] '
description: Das Glossar für [!DNL Adobe Workfront] enthält Begriffe, die häufig in der Benutzeroberfläche von  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] oder in Berichten verwendet werden, oder die verwendet werden, wenn Sie versuchen, die Bedeutung der Konzepte von [!DNL Workfront] zu verstehen, die in der Dokumentation zu [!DNL Workfront] definiert sind.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '21621'
ht-degree: 99%

---


# Glossar der Terminologie von [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Dieser Artikel sollte als Referenz verwendet werden, um die Begriffe zu verstehen, die Ihnen in der Anwendung [!DNL Adobe Workfront], in der Dokumentation zu [!DNL Workfront] oder allgemein im Zusammenhang mit der Planung und Verwaltung von Arbeit begegnen können. Diese Informationen werden derzeit aktualisiert, sodass diese Tabelle möglicherweise nicht vollständig ist. Wir werden diesen Haftungsausschluss entfernen, sobald wir diese Informationen für vollständig halten.

In der folgenden Tabelle finden Sie eine Liste häufig verwendeter Begriffe in Adobe Workfront:

## A–C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objektname</strong></th> 
   <th><strong>Beschreibung</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Zugriffsebene]</td> 
   <td>Ein Benutzerprofil, das bestimmt, wie Benutzende mit verschiedenen Objekten und Tools in Workfront interagieren können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktive Aufgabe]</td> 
   <td>Eine unvollständige Aufgabe in einem aktuellen Projekt, deren Bearbeitung nicht durch eine Vorgängeraufgabe verhindert wird, und die keine Aufgabenbeschränkung mit einem zukünftigen geplanten Startdatum aufweist. Mit anderen Worten, die Aufgabe kann heute bearbeitet werden.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Aktivität]</td> 
   <td>In [!DNL Workfront Goals] ist eine Aktivität eine Fortschrittsanzeige für ein Ziel. Dabei kann es sich um eine Fortschrittsleiste handeln, die Sie manuell aktualisieren, oder um ein Projekt, das mit dem Ziel verknüpft ist. Sie können Aktivitäten nicht in einem Bericht anzeigen und nicht über die [!DNL Workfront]-API darauf zugreifen. Informationen zu Aktivitäten finden Sie unter <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Kosten]</td> 
   <td> <p>Bei Aufgaben und Problemen sind dies die Kosten, die mit den tatsächlich protokollierten Stunden verknüpft sind, und zwar in Bezug auf den Stundensatz der Ressource, die der Aufgabe oder dem Problem zugewiesen wurde. Bei Projekten entspricht dies der Summe aller [!UICONTROL tatsächlichen Kosten] aus Aufgaben und Problemen des Projekts. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Nachverfolgen der Kosten</a>.</p>

<p>Bei der Berechnung der [!UICONTROL tatsächlichen Kosten] werden [!UICONTROL frühere tatsächliche Stunden] berücksichtigt. Weitere Informationen finden Sie unter „[!UICONTROL Tatsächliche Stunden]“ oder „[!UICONTROL Frühere tatsächliche Stunden]“ in dieser Tabelle. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Ausgabenkosten]</td> 
   <td> <p>Die Summe der [!UICONTROL tatsächlichen Beträge] für alle für ein Projekt oder eine Aufgabe protokollierten Ausgaben.</p> <b>BEISPIEL </b>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und 600,00 € in das Feld „[!UICONTROL Tatsächliche Kosten]“ eingeben, ist der Wert im Feld „[!UICONTROL Tatsächliche Ausgabenkosten]“ für diese Aufgabe 600,00 €. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um die [!UICONTROL tatsächlichen Ausgabenkosten] zu berechnen:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    -->
    </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächliche Stunden]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht sind die [!UICONTROL tatsächlichen Stunden] die Summe aller Stunden, die nach Mai 2021 für das Projekt, die Aufgabe oder das Problem protokolliert wurden.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> Wenn Sie auf der Registerkarte [!UICONTROL Updates] für Aufgabe 1 auf „Zeit erfassen“ klicken und 25 Stunden eingeben, sind die tatsächlichen Stunden von Aufgabe 1 = 25 Stunden. </p> <p>[!DNL Workfront] berechnet die [!UICONTROL tatsächlichen Stunden] für übergeordnete Aufgaben oder Projekte mithilfe der folgenden Formeln:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Siehe auch <strong>[!UICONTROL Frühere tatsächliche Stunden]</strong>.
    <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Anzeigen der tatsächlichen Stunden</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Arbeitskosten]</td> 
   <td> <p>Die [!UICONTROL tatsächlichen Kosten], die mit den in eine Aufgabe oder ein Projekt investierten Arbeitskräften verbunden sind. </p> <p>Für eine Aufgabe berechnet [!DNL Workfront] die [!UICONTROL tatsächlichen Arbeitskosten] mithilfe der folgenden Formel:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Wenn für die Aufgabe als [!UICONTROL Kostenart] die Option „[!UICONTROL Benutzer pro Stunde]“ gewählt ist, verwendet [!DNL Workfront] den Benutzersatz. Wenn für die Aufgabe als [!UICONTROL Kostenart] die Option „[!UICONTROL Stundensatz nach Funktion]“ gewählt ist, verwendet [!DNL Workfront] den Tarif des Aufgabengebiets, um die [!UICONTROL tatsächlichen Arbeitskosten] zu berechnen. </p> <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um die [!UICONTROL tatsächlichen Arbeitskosten] zu berechnen:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Nachverfolgen der Kosten</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel:</b></span></span> Wenn ein Benutzer bzw. eine Benutzerin 5 Stunden für eine Aufgabe protokolliert und für die [!UICONTROL Kostenart] die Option „[!UICONTROL Benutzer pro Stunde]“ gewählt ist und der Stundensatz 100 € beträgt, dann sind die [!UICONTROL tatsächlichen Arbeitskosten] gleich 500 €.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächlicher Umsatz] </td> 
   <td> <p>Der [!UICONTROL tatsächliche Umsatz] eines Projekts oder einer Aufgabe ist der Geldbetrag, der mit den [!UICONTROL tatsächlichen Stunden] des Projekts oder der Aufgabe verknüpft ist. </p> <p>Informationen zur Nachverfolgung von Umsätzen in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Überblick über Abrechnung und Umsatz</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächlicher Start]</td> 
   <td>Der Zeitstempel, zu dem ein Benutzer bzw. eine Benutzerin ein Objekt in einer ihm zugewiesenen laufenden Arbeit ändert.</td> 
  </tr> 
  <!--
  <tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile-Methode]</td> 
   <td>Eine Methodik, die auf der gemeinsamen Entwicklung von Anforderungen und Lösungen mit funktionsübergreifenden Teams basiert. Sie fördert Flexibilität und Veränderungen auf der Grundlage einer festen Timeline.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile-Team]</td> 
   <td>Unterscheidet sich von einem herkömmlichen Team, da es seine voraussichtliche Arbeit aus einem Rückstand übernimmt und diese innerhalb eines bestimmten Zeitraums bearbeitet, der als [!UICONTROL Iteration] bezeichnet wird.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alle meine Teams]</td> 
   <td> <p>Wenn unter „[!UICONTROL Filter]“ darauf verwiesen wird, zeigt dieses Feld entweder Benutzende an, die zu einem der Teams gehören, zu denen der angemeldete Benutzer bzw. die angemeldete Benutzerin gehört, oder Arbeitselemente, die einem der Teams zugewiesen sind, zu denen der angemeldete Benutzer bzw. die angemeldete Benutzerin gehört. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzende allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer bzw. die angemeldete Benutzerin angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuteilungsdatum]</td> 
   <td> <p>Dieses Feld finden Sie in den folgenden Berichtstypen:</p> 
    <ul>
    <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Projekt] (Finanzdaten)</li> 
     <li>[!UICONTROL Budgetierte Stunde]</li> 
    </ul> <p>Für eine
    <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->
     [!UICONTROL Project (Financial Data)]-Bericht: </p>
    <ul> 
     <li>Diesen Bericht erstellen, wenn Sie Folgendes verstehen möchten
     <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      -->
      Der Betrag von [!UICONTROL Geplante Stunden], der Ihren Ressourcen zugewiesen ist.</li>
     <li> <p>Das [!UICONTROL Zuteilungsdatum] ist der erste Tag (Sonntag) einer Woche, in der die Zuteilung eines [!UICONTROL Aufgabengebiets] zu einer Aufgabe beginnt. Das ([!UICONTROL Aufgabengebiet]) einer Ressource kann so viele [!UICONTROL Zuteilungstermine] haben, wie es Wochen während der [!UICONTROL Dauer] der Aufgaben hat, denen es zugewiesen ist. Wenn sich Aufgaben über mehrere Monate erstrecken, kann der erste Tag eines Monats auch zu einem [!UICONTROL Zuteilungsdatum] werden, wenn er in die [!UICONTROL Dauer] der Aufgabe fällt.</p> <p>Sie können beispielsweise ein [!UICONTROL Aufgabengebiet] einer Aufgabe zuweisen, die sich über 3 Wochen erstreckt und 90 [!UICONTROL geplante Stunden] hat. Diese Stunden werden während der Aufgabendauer gleichmäßig verteilt, sodass Sie Ihrem Aufgabengebiet täglich 6 [!UICONTROL geplante Stunden] zuweisen:</p> <p><em> [!UICONTROL Tägliche geplante Stunden] = [!UICONTROL Gesamte geplante Stunden] / Anzahl der [!UICONTROL Arbeitstage] während der [!UICONTROL Dauer] der Aufgabe </em> </p> <p>Infolgedessen gibt es drei [!UICONTROL Zuteilungstermine], einen für jeden Sonntag jeder Woche während der [!UICONTROL Dauer] der Aufgabe, wobei jedem eine bestimmte Anzahl unter „[!UICONTROL Geplante Stunden]“ zugeordnet ist.<br>Wenn die Aufgabe in der Mitte der letzten Woche eines Monats beginnt und zwei Wochen nach dem Beginn eines neuen Monats endet, hat die Aufgabe vier [!UICONTROL Zuteilungstermine]: einen für jeden Sonntag jeder Woche während der [!UICONTROL Dauer] der Aufgabe und einen für den ersten Tag des neuen Monats.</p> <p>Um diese Informationen optimal zu nutzen, empfehlen wir, eine
     <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       -->
       Erstellen Sie einen Bericht zu den (finanziellen) Daten des Projekts und fügen Sie eine Matrix-Gruppierung für das [!UICONTROL Zuteilungsdatum] hinzu. Gruppieren Sie dann die Ergebnisse wöchentlich, monatlich, vierteljährlich oder jährlich, um die genauesten Daten zu erhalten.<br>Informationen zum Erstellen einer Matrixgruppierung finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Erstellen eines Matrixberichts</a>.</p> </li>
    </ul> <p>Finanzinformationen werden nur dann in Berichten zum [!UICONTROL Projekt (Finanzdaten)] übernommen, wenn die damit verbundenen Daten weniger als 5 Jahre alt sind. Wenn beispielsweise einer Aufgabe im Januar 2015 ein Aufgabengebiet zugewiesen wurde und jetzt September 2021 ist, wird ein Finanzfeld wie das [!UICONTROL Zuteilungsdatum] für das Aufgabengebiet im Bericht zum [!UICONTROL Projekt (Finanzdaten)] nicht mit Daten gefüllt. </p> 
    <div> 
     <p>Für einen Bericht des Typs „[!UICONTROL Budgetierte Stunde]“:</p> 
     <ul> 
      <li>Erstellen Sie diesen Bericht, wenn Sie versuchen, die Menge unter „[!UICONTROL Budgetierte Stunden]“ zu verstehen, die Ihren Ressourcen oder Ihren Projekten im Ressourcenplaner zugewiesen ist.</li> 
      <li> <p>Das [!UICONTROL Zuteilungsdatum] ist der erste Tag (ein Sonntag) der Woche, für die Sie die Stunden im [!UICONTROL Ressourcenplaner] budgetiert haben. </p> <p><b>TIPP</b></p> <p>Wenn sich eine Woche über zwei Monate erstreckt, werden zwei Zeilen im Bericht generiert: eine Zeile, die dem ersten Wochentag entspricht (Sonntag der ersten Woche, die im ersten Monat liegt), und die zweite Zeile zeigt den ersten Tag des zweiten Monats an. </p> <p>Wenn Sie beispielsweise 8 Stunden für einen Benutzer bzw. eine Benutzerin für die Woche vom 30. Juni (Sonntag) bis zum 6. Juli (Samstag) budgetieren, wird in den beiden Zeilen als [!UICONTROL Zuteilungsdatum] der 30. Juni und der 1. Juli angezeigt. </p> </p> <p>Informationen zur Budgetierung von Ressourcen im [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetieren von Ressourcen im [!DNL Resource Planner] mithilfe der Ansichten [!UICONTROL Projekt] und [!UICONTROL Rolle</a>.</p> <p>Informationen zum Erstellen eines Berichts vom Typ [!UICONTROL Budgetierte Stunde] finden Sie unter <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ankündigungen]</td> 
   <td> <p>Eine Möglichkeit, Benutzerinformationen innerhalb des Systems zu kommunizieren. Diese Informationen werden häufig von [!DNL Workfront] an Admins übermittelt bzw. von Admins an die Benutzenden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Senden von Ankündigungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App-Integration]</td> 
   <td>Eine App stellt in den meisten Fällen einen Connector zu einer Software-Anwendung dar, kann aber auch spezielle Funktionen zur Datenbearbeitung darstellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entscheidung der genehmigenden Person]</td> 
   <td> <p>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld Entscheidungen zur Genehmigung von Korrekturabzügen für Korrekturabzüge an, die nicht mehr aktiv sind.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigungsstatus]</td> 
   <td>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld Informationen zur aktuellen Phase eines Korrekturabzugs an.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigung]</td> 
   <td> <p>Für ein bestimmtes Arbeitselement, z. B. eine Aufgabe, ein Dokument oder eine Arbeitszeittabelle, kann es erforderlich sein, dass eine verantwortliche Person oder ein anderer Benutzer bzw. eine andere Benutzerin das Arbeitselement abzeichnet. Dieser Prozess der Abzeichnung wird als Genehmigung bezeichnet. </p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Überblick über den Genehmigungsprozess</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigung]</td> 
   <td>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld das Datum an, an dem ein Korrekturabzug genehmigt wurde.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigende Person]</td> 
   <td>Ein Benutzer bzw. eine Benutzerin oder ein Aufgabengebiet, der, die oder das ein bestimmtes Arbeitselement abzeichnen muss oder Stundeneinträge in Arbeitszeittabellen genehmigt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zugewiesen zu]</td> 
   <td> <p>In einem Bericht des Typs [!UICONTROL „Aufgabe“ oder „Problem“] zeigt dieses Feld den Inhaber bzw. die Inhaberin der Aufgabe oder des Problems oder die Person unter „[!UICONTROL Primäre zugewiesene Person]“ an. Sie können auch nach diesem Feld filtern oder gruppieren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrag]</td> 
   <td>Ein Benutzer bzw. eine Benutzerin, ein Aufgabengebiet oder ein Team, die, der oder das einem Problem oder einer Aufgabe zugewiesen ist. Projekte, Portfolios oder Programme dürfen keine Arbeitsaufträge haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsaufträge]</td> 
   <td> <p>In einem Bericht zu [!UICONTROL Aufgabe] oder [!UICONTROL Problem] zeigt dieses Feld eine Liste aller Entitäten (Benutzende, Aufgabengebiete, Teams) an, die der Aufgabe oder dem Problem zugewiesen sind. Sie können mithilfe der Felder [!UICONTROL Arbeitsauftrag – Benutzer] und [!UICONTROL Arbeitsauftrag – Aufgabengebiete] nach diesem Feld filtern. Sie können über das Feld „Team“ nach dem Team filtern, das der Aufgabe oder dem Problem zugewiesen wurde. Sie können einen Bericht nicht nach diesem Feld gruppieren.</p> <p>Arbeitselemente, die in den [!UICONTROL Papierkorb] gelegt wurden, werden weiterhin in einigen Berichten angezeigt, die sich auf das Objekt [!UICONTROL Arbeitsauftrag] beziehen, in dem ein [!DNL OR]-Filtermodifikator verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrag – Aufgabengebiete]</td> 
   <td>
   <p>In einem Bericht zu [!UICONTROL Aufgabe] oder [!UICONTROL Problem] zeigt dieses Feld Informationen zu den Aufgabengebieten an, die den Aufgaben oder Problemen zugewiesen sind. In diesem Feld werden [!UICONTROL primäre Verantwortliche] sowie andere Aufgabengebiete angezeigt, die Aufgaben oder Problemen zugewiesen sind.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrag – Status]</td> 
   <td> <p>In einem Arbeitsauftrags-, Aufgaben- oder Problembericht wird unter „[!UICONTROL Arbeitsauftrag – Status]“ angezeigt, ob die einem Arbeitselement zugewiesenen Benutzenden auf die Schaltfläche „[!UICONTROL Bearbeiten]“ oder „[!UICONTROL Fertig]“ geklickt haben, um die Arbeit zu akzeptieren oder abzuschließen. Unter „[!UICONTROL Arbeitsauftrag – Status]“ gibt es folgende Möglichkeiten:</p> 
    <ul> 
     <li><b>[!UICONTROL Angefordert]</b>: Der Benutzer bzw. die Benutzerin wurde der Aufgabe oder dem Problem zugewiesen, hat jedoch noch nicht auf die Schaltfläche „[!UICONTROL Bearbeiten]“ geklickt, um mit der Bearbeitung zu beginnen.</li> 
     <li><b>[!UICONTROL In Arbeit]</b>: Der Benutzer bzw. die Benutzerin hat auf die Schaltfläche „[!UICONTROL Bearbeiten]“ geklickt und arbeitet derzeit an dem Element. </li> 
     <li><b>[!UICONTROL Fertig]</b>: Der Benutzer bzw. die Benutzerin hat auf die Schaltfläche „[!UICONTROL Fertig]“ geklickt und seine bzw. ihre Arbeit am Element abgeschlossen. </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Überblick über die Schaltflächen [!UICONTROL Bearbeiten] und [!UICONTROL Fertig]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrags-Teams]</td> 
   <td>
   <p>In einem Bericht zu [!UICONTROL Aufgabe] oder [!UICONTROL Problem] zeigt dieses Feld Informationen zu den Teams an, die den Aufgaben oder Problemen zugewiesen wurden. Das Feld zeigt [!UICONTROL primäre Verantwortliche] sowie andere Teams an, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrag – Benutzer]</td> 
   <td>
   <p>In einem Bericht zu [!UICONTROL Aufgabe] oder [!UICONTROL Problem] zeigt dieses Feld Informationen zu den Benutzenden an, die den Aufgaben oder Problemen zugewiesen wurden. In diesem Feld werden [!UICONTROL primäre Verantwortliche] sowie andere Benutzende angezeigt, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribut]</td> 
   <td>Ein Attribut ist ein Merkmal eines Objekts in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auditbereich]</td> 
   <td> <p>Audits sind Systemmeldungen, die eine Aktion aufzeichnen, die in Workfront stattgefunden hat. Die folgenden Audittypen werden aufgezeichnet:</p> 
    <ul> 
     <li>[!UICONTROL Umfangsänderung]</li> 
     <li>[!UICONTROL Anhangaktion]</li> 
     <li>[!UICONTROL Allgemeine Bearbeitung]</li> 
     <li>[!UICONTROL Statusänderung]</li> 
     <li>[!UICONTROL Notiz]</li> 
     <li>[!UICONTROL Kombinierter Eintrag]</li> 
     <li>[!UICONTROL Fehlereintrag]</li> 
     <li>[!UICONTROL Statusänderung]</li> 
     <li>[!UICONTROL Abonnementänderung]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit-Protokoll]</td> 
   <td>Die Sammlung von Notizen, die automatisch von Ereignissen generiert werden, die durch die ([!UICONTROL Auditbereiche]) für aufgezeichneten Änderungen verfolgt werden. In jeder Notiz wird aufgezeichnet, wer die Aktion ausgeführt hat, was getan wurde und wann die Aktion ausgeführt wurde.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatisch und bei Änderung]</td> 
   <td> <p>Eine Art der [!UICONTROL Projektaktualisierung]. Dadurch werden die erwarteten und geplanten Timelines des Projekts neu berechnet, wenn der Prozess der nächtlichen Neuberechnung ausgeführt wird und wenn am Projekt oder an den Aufgaben innerhalb des Projekts Aktualisierungen vorgenommen werden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps eines Projekts</a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Verfügbarkeit</p></td> 
   <td> <p>Dieser Begriff wird in Bezug auf „Benutzerverfügbarkeit“ oder „Ressourcenverfügbarkeit“ verwendet und veranschaulicht den Zeitraum, in dem die Ressource (Person oder Aufgabengebiet) für die Arbeit verfügbar ist. </p> 
   <p>Workfront berechnet die Benutzerverfügbarkeit anhand mehrerer Felder und abhängig von den Einstellungen in den Voreinstellungen des Ressourcen-Managements in Ihrem System. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurieren von Voreinstellungen für das Ressourcen-Management</a>. </p>
   <p>Weitere Informationen zur Ressourcenverfügbarkeit finden Sie unter <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit dem Ressourcen-Management</a></p>
   Alternativ wird auch „Kapazität“ verwendet, um auf die Verfügbarkeit von Ressourcen zu verweisen. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Nur automatisch]</td> 
   <td> <p>Eine Art der [!UICONTROL Projektaktualisierung]. Dadurch werden die prognostizierten und geplanten Timelines bei der nächtlichen Neuberechnung neu berechnet.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps eines Projekts</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>„Business as usual“ bezeichnet Arbeit, die dazu beiträgt, die alltäglichen primären Geschäftsziele zu erreichen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Rückstand]</td> 
   <td>Der Bereich in einer Agile-Umgebung, in dem neue Probleme abgelegt werden, bis sie bereit zur Bearbeitung sind.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Eine Datenquelle für die Messung von Iterationen in einer Agile-Umgebung.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Abrechenbare Kosten]</td> 
   <td> <p>Eine Ausgabe, die für den Kunden bzw. die Kundin als fakturierbar gekennzeichnet ist. Dies kann entweder eine geplante Ausgabe oder eine tatsächliche Ausgabe sein.</p> <p>Die Felder „Geplante abrechenbare Kosten“ und „Tatsächliche abrechenbare Kosten“ können zu Ansichten und Berichten hinzugefügt werden. Sie werden nicht auf den Seiten mit den Projekt- oder Aufgabendetails angezeigt.</p>
   <p>Diese Felder finden Sie in den folgenden Berichtstypen:</p>
   <ul>
   <li>Baseline</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Kennzeichnen einer Ausgabe als fakturierbar finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Verwalten von Projektausgaben</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Abrechnungseintrag]</td> 
   <td> <p>Erfasst den Umsatz, die Stunden oder die Ausgaben, die fakturiert werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchhaltungssystem verwendet werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Erstellen von Abrechnungseinträgen</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status des Abrechnungseintrags</td> 
   <td> <p>In einem Abrechnungseintrag oder Stundenbericht gibt der Status eines Abrechnungseintrags an, ob der Abrechnungseintrag fakturiert wurde oder nicht. Sie können ein Projekt nicht löschen und die mit einem fakturierten Abrechnungseintrag verknüpfte Zeit nicht bearbeiten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Erstellen von Abrechnungseinträgen</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Der Prozess der Anpassung von [!DNL Workfront], um der Benutzeroberfläche ein Erscheinungsbild zu verleihen, das Ihr Unternehmen widerspiegelt, indem Ihre Farben und Logos verwendet werden.</p><p><strong>HINWEIS</strong><br> Wenn Ihre Organisation in [!DNL Adobe Experience Cloud] integriert wurde, ist kein Branding verfügbar.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Der Bereich oben auf der Seite, der die hierarchische Position anzeigt, an der sich der Benutzer bzw. die Benutzerin in der Anwendung befindet.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Überblick über Breadcrumbs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetstatus]</td> 
   <td> <p>Dieses Feld ist veraltet. Alle Informationen, die in diesem Feld möglicherweise angezeigt werden, beziehen sich auf eine Funktion, die aus [!DNL Workfront] entfernt wurde. Das Feld kann nicht aktualisiert werden. </p> <p>Dieses Feld zeigt, ob das Projekt dem [!UICONTROL Kapazitätsplaner] hinzugefügt wurde und ob die Budgetberechnung dafür abgeschlossen wurde. Der [!UICONTROL Kapazitätsplaner] wurde aus [!DNL Workfront] entfernt. </p> 
    <ul>
    <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  not added to the capacity planner, its value is <i>Not Included</i>.  </li>
     -->
     <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  added to the Capacity Planner but is excluded from the budget calculation,  the value is <i>Included but not Calculated</i>.  </li>
     -->
     <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is  added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Aufschlüsselung]</td> 
   <td> <p>In Workfront-Planung können Sie mithilfe der Aufschlüsselungsfunktion verbundene Einträge in der Timeline-Ansicht eines Eintrags anzeigen. </p>
   <p>Wenn Sie Einträge nach ihren Verbindungen aufschlüsseln, können Sie die Timelines anderer verbundener Einträge anzeigen und verstehen, wie sich diese auf die Leistung und die Fristen Ihrer Einträge auswirken können. </p>
   <p>Verbundene Einträge werden verschachtelt unter ihrem jeweiligen Eintrag angezeigt. </p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Verwalten der Timeline-Ansicht</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Budgetiertes Fertigstellungsdatum]</td> 
   <td> <p>Dieses Feld ist veraltet. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die aus [!DNL Workfront] entfernt wurde. Dieses Feld kann nicht aktualisiert werden. </p>
   <p> Dieses Feld ist weiterhin in Berichten zum [!UICONTROL Projekt] und entsprechenden Listen sichtbar.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Kosten]</td>

<td> <p>Dies sind die Kosten für die Budgetierung von Ressourcen für ein Projekt. </p>
   <p>Das Feld wird in den folgenden Bereichen von [!DNL Workfront] unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL Budgetierte Kosten]</strong>: im Panel [!UICONTROL Business Case-Zusammenfassung]</li>
   <li><strong>[!UICONTROL Kosten]</strong>: in den Bereichen für die [!UICONTROL Auslastung], wenn Sie Informationen nach [!UICONTROL Kosten] anzeigen</li>
   <li><strong>[!UICONTROL Budgetierte Projektkosten]</strong>: in Listen und Berichten</li>
   </ul>   
    <p>Unter „[!UICONTROL Budgetierte Kosten]“ für das Projekt erfolgt die Berechnung mithilfe der folgenden Formel:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Weitere Informationen zur Berechnung von [!UICONTROL budgetierten Kosten] und zu den verschiedene Namen für dieses Konzept in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Berechnen der budgetierten Projektkosten</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgetierte Stunden]</td> 
   <td> <p>Die budgetierten Stunden der Ressourcen für die Arbeit, die sie an Projekten durchführen müssen. Dieses Feld bezieht sich auf die budgetierten Stunden im Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case] (oder im [!UICONTROL Ressourcenplaner]) für das Projekt oder die Projektressourcen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Grundlegendes zu [!UICONTROL budgetierten Arbeitskosten] und [!UICONTROL Budgetierte Stunden] für Projekte</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Informationen zur Budgetierung von Ressourcen im [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetieren von Ressourcen im [!DNL Resource Planner] mithilfe der Ansichten [!UICONTROL Projekt] und [!UICONTROL Rolle]</a>. </p> 
    <p>Die budgetierten Stunden im Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case] oder im [!UICONTROL Ressourcenplaner] werden in den folgenden Bereichen von [!DNL Workfront] und unter den folgenden Namen angezeigt:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgetierte Stunden] Anzeigename</strong></td> 
        <td><strong>Bereiche von [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Stunden]</td> 
        <td>Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Ressourcenplaner] angezeigt nach [!UICONTROL Stunden]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgetierte Stunden]</td> 
        <td> <p>Ansicht „Auslastungsbericht – [!UICONTROL Stunden]“</p> <p>Weitere Informationen zum Bericht zur [!UICONTROL Auslastung] finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Überblick über den Bericht zur [!UICONTROL Ressourcenauslastung</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Stunden]</td> 
        <td> <p>Bericht [!UICONTROL Budgetierte Stunde]</p><p>Das Objekt [!UICONTROL Budgetierte Stunde] im Bericht für budgetierte Stunden bezieht sich auf Informationen zu einem veralteten Ressourcen-Management-Tool. Nur das Feld „[!UICONTROL Bud. Stunden] in diesem Bericht bezieht sich auf die budgetierten Stunden im Bereich „[!UICONTROL Ressourcenplaner]“ oder „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case] des Projekts. </p> <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ressourcenplaner für budgetierte Stunden] </td> 
        <td> <p>In den folgenden Berichten enthalten:</p>
        <ul>
        <li>Bericht [!UICONTROL Projekt]
        <li>Bericht [!UICONTROL Projekt (Finanzdaten)]
        <li>Bericht [!UICONTROL Aufgabe]
        <li>Bericht [!UICONTROL Problem]
        <li>Bericht [!UICONTROL Budgetierte Stunde]</li>
        </ul>
         <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Jede andere Erwähnung von [!UICONTROL budgetierten Stunden] in [!DNL Adobe Workfront] bezieht sich auf Stunden, die mit veralteten Funktionen budgetiert wurden, die aus Workfront entfernt wurden. Diese Felder sind schreibgeschützt und werden nicht mit aktuellen Informationen aktualisiert, wenn Sie die aktuellen Tools für die Ressourcenbudgetierung verwenden. </p>
    <!--
    <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the  Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy  Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy  Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial  Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul>
      -->
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Lohnkosten]</td> 
   <td> <p>Dies sind die Kosten im Zusammenhang mit den Stunden, die Sie im Ressourcen-Management für Ihre Aufgabengebiete für die Arbeit budgetieren, die Mitarbeitende in Projekten erledigen müssen. </p> <p>[!UICONTROL Budgetierte Lohnkosten] in einem Projektbericht werden nach folgender Formel berechnet:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Dieses Feld kann sich auf Folgendes beziehen:</p> 
    <ul> 
     <li> <p>Arbeitskosten, die im Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case] oder im [!UICONTROL Ressourcenplaner] angezeigt werden und mit den Kosten für Aufgabengebiete in einem Projekt verknüpft sind. Informationen zur Berechnung der [!UICONTROL budgetierten Lohnkosten] finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Grundlegendes zu budgetierten Lohnkosten] und [!UICONTROL Budgetierte Stunden] für Projekte</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Im Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case] werden Arbeitskosten angezeigt, die die geschätzten [!UICONTROL Personalkosten] in einer mit dem Projekt verknüpften Initiative aus dem [!DNL Scenario Planner] widerspiegeln, wenn Sie den Szenarienplaner zur Budgetierung Ihrer Projektressourcen verwenden. Informationen zu Initiativen finden Sie unter <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Überblick über Initiativen im Szenarienplaner</a>. </p> <p>Für den [!DNL Scenario Planner] ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick über den [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Er wird in den folgenden Bereichen von unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL Budgetierte Lohnkosten]</strong>: im Bereich „[!UICONTROL Ressourcenbudgetierung]“ des [!UICONTROL Business-Case].
   <li><strong>[!UICONTROL Budgetierte Kosten]</strong>: im Bericht zur [!UICONTROL Auslastung], Ansicht [!UICONTROL Kosten]
   <p>Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Anzeigen von Informationen zur Ressourcenauslastung</a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in den Ansichten „Projekt“ oder „[!DNL Role]“ im [!DNL Resource Planner] bei der Anzeige nach Kosten
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in den folgenden Berichten: 
   <ul>
    <li>Bericht [!UICONTROL Projekt]</li>
    <li>Bericht [!UICONTROL Projekt (Finanzdaten)]</li>
    <li>Bericht [!UICONTROL Aufgabe]</li>
    <li>Bericht [!UICONTROL Problem]</li>
    <li>Bericht [!UICONTROL Budgetierte Stunde]</li> 
    </ul>
    <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in  Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>  .  </p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgetiertes Startdatum]</td> 
  <td> <p>Dieses Feld ist veraltet. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die aus [!DNL Workfront] entfernt wurde. Dieses Feld kann nicht aktualisiert werden.</p>
  <p>Diese Bereiche wurden aus [!DNL Workfront] entfernt. </p> 
  <p>Das Feld ist weiterhin in Berichten zum [!UICONTROL Projekt] und entsprechenden Listen sichtbar.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown-Diagramm]</td> 
   <td>Ein Liniendiagramm, das die abgeschlossenen und verbleibenden Arbeiten visuell darstellt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business-Case]</td> 
   <td> <p>Ein Tool, mit dem ausgewertet wird, ob ein Projekt vom Status [!UICONTROL Idee] zum Status [!UICONTROL Planung] weitergeleitet werden soll. Mit anderen Worten: Ein [!UICONTROL Business-Case] hilft der Organisation bei der Entscheidung, ob es sich lohnt, das Projekt zu starten und abzuschließen oder nicht, insbesondere beim Vergleich von Projekten mit anderen in einem Portfolio.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Erstellen eines [!UICONTROL Business-Case] für ein </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgetierte Kosten für Business-Case]</td> 
   <td> <p>Dieses Feld ist veraltet. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die aus [!DNL Workfront] entfernt wurde. Dieses Feld kann nicht aktualisiert werden.</p> <p>Dieses Feld ist weiterhin in Listen und Berichten zu Projekten und [!UICONTROL Aufgaben] sichtbar. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechneter Arbeitsauftrag]</td> 
   <td> <p>Einer der [!UICONTROL Dauertypen] für Aufgaben. Damit wird der Prozentsatz eines 8-Stunden-Arbeitstags berechnet, den der Benutzer bzw. die Benutzerin, der bzw. die der Aufgabe zugewiesen ist, für die Aufgabe zugeteilt bekommt, basierend auf der [!UICONTROL Dauer] der Aufgabe und der Angabe unter „[!UICONTROL Erforderliche Arbeit]“.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Überblick über die [!UICONTROL Dauer] und den [!UICONTROL Dauertyp] einer Aufgabe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechnete Arbeit]</td> 
   <td> <p>Einer der [!UICONTROL Dauertypen] einer Aufgabe. Damit wird die [!UICONTROL erforderliche Arbeit] für eine Aufgabe unter Berücksichtigung der [!UICONTROL Dauer] und des prozentualen Anteils an einem [!UICONTROL Arbeitsauftrag] für Benutzende (basierend auf einem 8-Stunden-Arbeitstag) berechnet.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Überblick über die [!UICONTROL Dauer] und den [!UICONTROL Dauertyp] einer Aufgabe</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender]</td> 
   <td> <p>In Workfront ist ein Kalenderbericht ein dynamischer Bericht, in dem Benutzende das Datum und andere wichtige Details eines Ereignisses anzeigen können, einschließlich des Fälligkeitsdatums, des Arbeitsstatus und der Benutzenden, denen das Ereignis zugewiesen ist.</p> <p> Weitere Informationen zu Kalenderberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Überblick über Kalenderberichte</a>.</p>
   <p> In Workfront-Planung ist eine Kalenderansicht eine Art von Ansicht für einen Eintragstyp, der Einträge in einem Kalender anzeigt. Sie benötigen eine zusätzliche Lizenz, um auf Workfront-Planung zugreifen zu können. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Kann beginnen]</td> 
   <td> <p>Dieses Feld gibt an, ob eine Aufgabe bereit für die Bearbeitung ist. Wenn mit der Bearbeitung begonnen werden kann, wird das Feld „[!UICONTROL Kann beginnen]“ der Aufgabe auf „[!UICONTROL Wahr]“ festgelegt. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Überblick über die Option „[!UICONTROL Kann beginnen]“ für Aufgaben</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    -->
    <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.  </li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.  </li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    -->
    <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    -->
    </td>
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Kapazität</p> </td> 
   <td> <p>Die verfügbare Zeit einer Ressource, in der sie für die Arbeit zugewiesen werden kann. Siehe „Verfügbarkeit“. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Kategorie]</p> </td> 
   <td> <p>Eine Kategorie ist ein benutzerdefiniertes Formular. Sie können Berichte für dieses Objekt erstellen und sie auch in anderen Objektberichten anzeigen. Nicht alle Objekte können ein benutzerdefiniertes Formular oder eine benutzerdefinierte Kategorie haben. Die folgenden Objekte können ein benutzerdefiniertes Formular haben: <br></p> 
    <ul> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Aufgabe]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Dokument]</li> 
     <li>[!UICONTROL Ausgabe]</li> 
     <li>[!UICONTROL Programm]</li> 
     <li>[!UICONTROL Benutzende]</li> 
     <li>[!UICONTROL Unternehmen]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kategoriename]</td> 
   <td> <p>Wenn dieser als Spalte zur Ansicht eines der folgenden Objekte hinzugefügt wird, wird eine Liste aller benutzerdefinierten Formulare angezeigt, die mit diesen Objekten verknüpft sind:</p> 
    <ul> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Aufgabe]<br></li> 
     <li>[!UICONTROL Problem]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Dokument]<br></li> 
     <li>[!UICONTROL Ausgabe]<br></li> 
     <li>[!UICONTROL Programm]<br></li> 
     <li>[!UICONTROL Benutzende]<br></li> 
     <li>[!UICONTROL Unternehmen]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Änderungs-Management]</td> 
   <td>Ein Tätigkeitsbereich, der sich auf die Definition, das Verständnis und die Anpassung geplanter Arbeiten an Änderungen in Bezug auf Umfang, Zeitplan, Kosten und Ressourcenfaktoren konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Änderungsanforderung]</td> 
   <td>Eine Art von Problem, das für ein Projekt vorgebracht wird und eine angefragte Änderung des vereinbarten Umfangs skizziert.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nur Änderung]</td> 
   <td>Einer der [!UICONTROL Aktualisierungstypen] für Projekte. Die Timelines [!UICONTROL Projiziert] und [!UICONTROL Geplant] des Projekts werden nur dann aktualisiert, wenn Aktualisierungen an Aufgaben vorgenommen oder Änderungen am Projekt oder an Aufgaben durchgeführt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Änderungsanforderung]</td> 
   <td> <p>Einer der Typen für ein [!UICONTROL Problem], der normalerweise angibt, dass vor dem Abschluss des Projekts ungeplanter Arbeitsaufwand erforderlich ist.</p> <p>Weitere Informationen zu Typen für ein [!UICONTROL Problem] finden Sie im Abschnitt „Standardproblemtypen“ im Artikel<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Anpassen von Standardproblemtypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Untergeordnete Aufgabe]</td> 
   <td>Eine Aufgabe, die eine [!UICONTROL Unteraufgabe] einer [!UICONTROL übergeordneten Aufgabe] ([!UICONTROL Übersichtsaufgabe]) ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Untergeordnete Elemente]</td> 
   <td>Die Sammlung [!UICONTROL Unteraufgaben] für eine [!UICONTROL übergeordnete Aufgabe] ([!UICONTROL Übersichtsaufgabe]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] und [!UICONTROL Training]</td> 
   <td>Lernmodule, Zertifizierungen, Standards oder eine Community von Anwendenden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verpflichtung]</td> 
   <td>Ein Kommunikations-Tool für Benutzende, mit dem sie Erwartungen an die zu erbringenden Aufgaben definieren können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verpflichtungsdatum]</td> 
   <td>Ein Kommunikations-Tool für Benutzende, mit dem sie Erwartungen im Zusammenhang mit den zu erbringenden Aufgaben definieren können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommunikation] und [!UICONTROL Reporting]</td> 
   <td>Standards zur Überprüfung der Ausnahmen und des Zustands eines Projekts, Programms oder Portfolios</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unternehmen]</td> 
   <td> <p>Ein [!UICONTROL Unternehmen] ist eine Organisationseinheit in [!DNL Workfront]. </p> 
   <p> Sie können einen Benutzer bzw. eine Benutzerin oder ein Projekt mit einer Firma verknüpfen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Erstellen und Bearbeiten von Unternehmen</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussdatum]</td> 
   <td> <p>Das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem abgeschlossen sein soll. Es gibt mehrere Typen von [!UICONTROL Abschlussdaten] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Tatsächliches Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Überblick über das [!UICONTROL tatsächliche Abschlussdatum] des Projekts</a>.</li> 
     <li>[!UICONTROL Geplantes Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Einrichten des [!UICONTROL geplanten Abschlussdatums]</a> des Projekts und <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Überblick über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]</a>.</li> 
     <li>[!UICONTROL Voraussichtliches Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Überblick über das [!UICONTROL voraussichtliche Abschlussdatum] für Projekte, Aufgaben und Probleme</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fertigstellungstag]</td> 
   <td>Der Tag, relativ zum Beginn der [!UICONTROL Vorlage], an dem eine [!UICONTROL Vorlagenaufgabe] oder eine [!UICONTROL Vorlage] abgeschlossen sein soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fertigstellungsmodus]</td> 
   <td> <p>Dieses Objekt gibt an, wie ein Projekt als „[!UICONTROL Abgeschlossen]“ gekennzeichnet wird. Es kann zwei Werte haben:</p> 
    <ul> 
     <li>[!UICONTROL Manuell]: Ein Benutzer bzw. eine Benutzerin muss den Projektstatus in [!UICONTROL Abgeschlossen] ändern.</li> 
     <li>[!UICONTROL Automatisch]: Der Projektstatus ändert sich automatisch in [!UICONTROL Abgeschlossen], wenn alle Aufgaben im Projekt zu 100 % abgeschlossen sind und alle Probleme geschlossen sind.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bedingung]</td> 
   <td> <p>Dies ist eine visuelle Darstellung des Fortschritts einer Aufgabe, eines Problems oder Projekts.</p> <p>Bei Projekten kann die Bedingung von Projektverantwortlichen manuell festgelegt werden oder automatisch von [!DNL Workfront] auf der Grundlage des Fortschrittsstatus des Projekts festgelegt werden. </p> <p>Die möglichen Werte für die Projektbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL Im Zielbereich]</li> 
     <li>[!UICONTROL Gefährdet]</li> 
     <li>[!UICONTROL In Schwierigkeiten]</li> 
    </ul> <p>Weitere Informationen zu Projektbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Überblick über die [!UICONTROL Projektbedingung] und den [!UICONTROL Bedingungstyp]</a>.</p>
     <p>Sie können Aufgaben- und Problembedingungen mit einer Zahl verknüpfen, die in Berichten angezeigt werden kann. In den folgenden Listen werden die Standardnamen und -nummern für Aufgaben- und Problembedingungen angezeigt. Ihre bzw. Ihr Systemadmin kann die Namen der Bedingungen aktualisieren und neue Bedingungen mit unterschiedlichen Nummern hinzufügen. Nachdem eine Nummer mit einer Bedingung verknüpft wurde, kann sie nicht mehr bearbeitet werden.  </p> 
     <p>Für Aufgaben wird die Bedingung vom Aufgabenbesitzer bzw. der Aufgabenbesitzerin manuell festgelegt. Die möglichen Werte für die Aufgabenbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL Keine Probleme] (0)<br></li> 
     <li> [!UICONTROL Kleinere Probleme] (1)<br></li> 
     <li>[!UICONTROL Größere Probleme] (2)</li> 
    </ul> <p>Weitere Informationen zu Aufgabenbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisieren der [!UICONTROL Bedingung] für Aufgaben und Probleme</a>.</p> <p>Bei Problemen wird die Bedingung manuell vom Probleminhaber bzw. der Probleminhaberin festgelegt. Die möglichen Werte für die Problembedingung sind:<br></p> 
    <ul> 
     <li>[!UICONTROL Keine Probleme] (0)<br></li> 
     <li>[!UICONTROL Kleinere Probleme] (1)<br></li> 
     <li>[!UICONTROL Größere Probleme] (2)</li> 
    </ul> 
   <p><b>HINWEIS</b></p>
    <p>Wenn das Feld „[!UICONTROL Bedingung]“ in Berichten zum [!UICONTROL Journaleintrag] nachverfolgt wird, wird unter „[!UICONTROL Neu]“ und „[!UICONTROL Alte Zahlenwerte]“ die mit der Bedingung verknüpfte Zahl anstelle ihres Namens angezeigt. Wenn eine Bedingung ursprünglich nicht für eine Aufgabe oder ein Problem definiert ist und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den [!UICONTROL alten Zahlenwert] des Feldes „[!UICONTROL Bedingung]“ als -2.147.483648 an. Siehe auch „[!UICONTROL Neuer Zahlenwert]“, „[!UICONTROL Alter Zahlenwert]“ und „[!UICONTROL Journaleintrag]“ in diesem Artikel. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bedingungs-Aktualisierung]</td> 
   <td> <p>In diesem Feld wird die aktuelle Bedingung von Aufgaben, Projekten oder Problemen angezeigt. Diese Option zeigt die neuesten Aktualisierungen, die die Verantwortlichen für Aufgaben, Projekte oder Probleme im Feld „[!UICONTROL Aktualisierungsstatus]“ bereitgestellt haben, zusammen mit der neuen Bedingung an.</p> <p>Kommentare zu Bedingungs-Aktualisierungen werden nicht in der Spalte [!UICONTROL Bedingungs-Aktualisierung] angezeigt, sondern nur die Hauptaktualisierung.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Verbundene Eintragstypen]</td> 
   <td> <p>In Workfront-Planung können Sie eine Verbindung zwischen folgenden Elementen erstellen: </p>
   <ul>
   <li>Zwei Eintragstypen</li>
   <li>Einem Eintragstyp und einem Workfront-Objekttyp</li>
   <li>Einem Eintragstyp und einem Adobe Experience Manager-Asset</li></ul>
   <p>Durch das Verbinden von Eintragstypen können Sie Informationen aus einem Eintrag oder Objekttyp in einem anderen Eintragstyp anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Überblick über verbundene Eintragstypen</a>  </p>
  <p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Verbundene Einträge]</td> 
   <td> <p>In Workfront-Planung können Sie nach dem Verbinden von zwei Eintragstypen zwei einzelne Einträge dieser Typen miteinander verbinden.  </p>
   <p>Durch das Verbinden von Einträgen können Sie Informationen aus einem Eintrag oder Objekt einer anderen Anwendung in einem anderen Eintrag anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Überblick über verbundene Einträge</a>. </p>

<p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Verbindungen]</td> 
   <td> <p>In Workfront-Planung können Verbindungen auf verbundene Eintragstypen oder verbundene Einträge verweisen. Workfront-Planung benötigt eine zusätzliche Lizenz.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Einschränkungsdatum]</td> 
   <td> <p>Wenn Sie eine [!UICONTROL Aufgabenbeschränkung] verwenden, die mit einem bestimmten Datum verknüpft ist, z. B. [!UICONTROL Muss beginnen am], wird dieses bestimmte Datum zum [!UICONTROL Einschränkungsdatum] der Aufgabe.</p> <p>Die folgenden Aufgabenbeschränkungen aktualisieren das Feld „[!UICONTROL Einschränkungsdatum]“:</p> 
    <ul> 
     <li>[!UICONTROL Muss beginnen am]</li> 
     <li>[!UICONTROL Muss beendet werden am]</li> 
     <li>[!UICONTROL Nicht später anfangen als]</li> 
     <li>[!UICONTROL Nicht früher anfangen als]</li> 
    </ul> <p><b>TIPP</b></p>   
     <ul> 
      <li> <p>Eine Aufgabe mit einer [!UICONTROL Einschränkung] von „[!UICONTROL Feste Daten]“ hat kein [!UICONTROL Einschränkungsdatum]. </p> </li> 
      <li> <p> [!UICONTROL Einschränkungsdatum] kann nur in einem Bericht oder in einer angepassten Ansicht angezeigt werden.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einschränkungstag]</td> 
   <td> <p>Wenn Sie eine Aufgabenbeschränkung in einer Vorlagenaufgabe verwenden, die an einen bestimmten Tag gebunden ist, z. B. „Muss beginnen am“, wird dieser Tag zum Einschränkungstag der Vorlagenaufgabe.</p> <p>Die folgenden Aufgabenbeschränkungen aktualisieren das Feld „[!UICONTROL Einschränkungstag]“:</p> 
    <ul> 
     <li>[!UICONTROL Muss beginnen am]</li> 
     <li>[!UICONTROL Muss beendet werden am]</li> 
     <li>[!UICONTROL Nicht später anfangen als]</li> 
     <li>[!UICONTROL Nicht früher anfangen als]</li> 
    </ul> <p><b>TIPP</b></p> <p>  [!UICONTROL Einschränkungstag] kann nur in einem Bericht oder in einer benutzerdefinierten Ansicht angezeigt werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einschränkungstyp]</td> 
   <td> <p>Die Planungstendenz einer Aufgabe. Beispielsweise wird mit [!UICONTROL So bald wie möglich] eine Aufgabe so geplant, dass sie baldmöglichst beginnt, und mit [!UICONTROL Nicht später beenden als] wird eine Aufgabe so geplant, dass sie spätestens am [!UICONTROL Einschränkungsdatum] beendet wird.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Überblick über [!UICONTROL Aufgabenbeschränkungen]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kontextmenü]</td> 
   <td>Ein Menü links im Bildschirm, in dem sich die Elemente ändern, sodass sie mit dem aktiven Inhalt korrelieren. Wenn ein Benutzer bzw. eine Benutzerin beispielsweise ein Projekt anzeigt, enthält das [!UICONTROL Kontextmenü] Links zu projektbezogenen Informationen und Tools.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Konvertiertes Problem – Urheber]</td> 
   <td>Ein Feld in einem Projekt- oder Aufgabenbericht, das Informationen zu dem Benutzer bzw. der Benutzerin anzeigt, der bzw. die [!UICONTROL primärer Kontakt] für ein Problem ist, wenn das Problem in ein Projekt oder eine Aufgabe konvertiert wird. Das Feld wird auch im Abschnitt [!UICONTROL Projektdetails] angezeigt, wo es den Namen des [!UICONTROL primären Kontakts] des konvertierten Problems anzeigt. Siehe auch „[!UICONTROL Primärer Kontakt]“ in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Kosten]</td> 
   <td> <p>Der Geldbetrag, den Sie beim Abschluss eines Projekts, einer Aufgabe oder eines Problems ausgeben müssen. </p> <p>Sie können verschiedene Arten von Kosten für Arbeit, Ausgaben und Risiken im Zusammenhang mit dem Projekt verfolgen. Informationen zur Kostennachverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Nachverfolgen der Kosten</a>.</p> 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Kostenentwicklungsindex (Cost Performance Index, CPI)]</td> 
   <td> <p>Der [!UICONTROL Kostenentwicklungsindex (Cost Performance Index, CPI)] beschreibt die Beziehung zwischen den geplanten Kosten und den tatsächlichen Kosten auf Projekt- oder Aufgabenebene. Das Projekt-Management überprüft diese Metrik, um Aufgaben oder Projekte zu ermitteln, die zu einem bestimmten Zeitpunkt unter oder über den Kosten liegen. Die Kosten können je nach [!UICONTROL Performance-Index-Methode (PIM)] in Stunden oder Währungen gemessen werden.</p> 
    <p> Informationen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-cpi.md">Berechnen des Kostenentwicklungsindex (Cost Performance Index, CPI)</a>.</p>

</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Terminentwicklungsindex (CSI, Cost Schedule Performance Index)]</td> 
   <td> <p>Der [!UICONTROL Terminentwicklungsindex (Cost Schedule Performance Index, CSI)] ist eine automatische Berechnung, die den [!UICONTROL Kostenentwicklungsindex (Cost Performance Index, CPI)] und den [!UICONTROL Zeitplan-Leistungsindex (Schedule Performance Index, SPI)] zu einer allgemeinen Metrik kombiniert, die Kosten und Zeitplan ausgleicht. Durch Multiplikation dieser Werte kann eine einzige Metrik einen verlängerten Zeitplan bei geringerem Budget oder umgekehrt berücksichtigen. Das Projekt-Management kann dieses Objekt verwenden, um den allgemeinen Projekt- oder Aufgabenzustand zu bestimmen, wenn Kosten geopfert werden, um den Zeitplan während des Projekts voranzutreiben.</p> 
    <p> Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-csi.md">Berechnen des Terminentwicklungsindex (Cost Schedule Performance Index, CSI)</a>.</p>
    </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Kostenart]</td> 
   <td>Bei einer Aufgabe bestimmt die [!UICONTROL Kostenart], wie Kosten für die Aufgabe entstehen. Einige Beispiele sind [!UICONTROL Festgelegt pro Stunde], [!UICONTROL Benutzer pro Stunde] und [!UICONTROL Benutzer pro Stunde plus festgelegt]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektübergreifende Abhängigkeiten]</td> 
   <td> <p>Eine Aufgabe eines Projekts ist von einer Aufgabe aus einem anderen Projekt abhängig.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Erstellen von projektübergreifenden Vorgängern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefinierte Daten]</td> 
   <td> <p>Daten, die für eine Organisation eindeutig sind. Organisationen können [!DNL Workfront] anpassen, indem sie benutzerdefinierte Formulare und Felder erstellen. Diese benutzerdefinierten Informationen können das Reporting für KPIs, Auditing und den Nachfrage-Mix vorantreiben. </p> <p>[!UICONTROL Benutzerdefinierte Daten] können mit folgenden Elementen verknüpft werden:</p> 
    <ul> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Benutzende]</li> 
     <li>[!UICONTROL Unternehmen]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Iterationen]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Art der benutzerdefinierten Daten]</td> 
   <td>Mit dieser Option wird angegeben, ob das Feld „[!UICONTROL Benutzerdefinierte Daten]“ in der Datenbank als Text, Datum, Zahl oder Währung gespeichert wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Art des benutzerdefinierten Displays]</td> 
   <td>Der Feldanzeigetyp eines benutzerdefinierten Feldes. Beispiele sind [!UICONTROL Dropdown], [!UICONTROL Textfeld], [!UICONTROL Textbereich], [!UICONTROL Optionsfelder] usw.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefiniertes Feld]</td> 
   <td>Bei benutzerdefinierten Daten, mit denen Benutzende aus mehreren Optionen auswählen können, sind dies die Werte, aus denen Benutzende auswählen können. Benutzerdefinierte Optionen sind nur für [!UICONTROL Dropdown], [!UICONTROL Mehrfachauswahl-Dropdown], [!UICONTROL Optionsfelder] und [!UICONTROL Kontrollkästchen] gültig.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierte Formularbeschriftung]</td> 
   <td>Wenn Sie eine „Art des benutzerdinierten Displays“ mit benutzerdefinierten Optionen verwenden, ist dies der Benutzeroberflächentext, der im Dropdown-Menü, den Kontrollkästchen oder den Optionsfeldern für diese benutzerdefinierte Option angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierter Wert]</td> 
   <td>Bei Verwendung eines benutzerdefinierten Feldes mit benutzerdefinierten Optionen ist dies der Wert, der für eine bestimmte Option in der Datenbank gespeichert wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierte Ansicht]</td> 
   <td>Eine Definition der Datenfelder oder Spalten, die für jedes Objekt in einer Liste angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kundin bzw. Kunde]</td> 
   <td>Eine Organisation, die eine Instanz von Workfront verwendet.</td> 
  </tr> 
 </tbody> 
</table>

## D–F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> Sie können dieses Feld einem Bericht oder einer Ansicht des Berichtsobjekts hinzufügen, um die Dashboards anzuzeigen, in denen der Bericht in einer Liste aufgeführt ist. </p> <p> Sie können dieses Feld auch verwenden, um nach Berichten zu filtern, die in einem bestimmten Dashboard aufgeführt sind. </p> <p> Weitere Informationen zum Einschließen von Dashboard-Informationen in Berichte zu Berichtsobjekten finden Sie im Abschnitt „Verstehen, welche Berichte in Dashboards aufgelistet sind“ im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Zugriff auf und Organisieren von Berichten</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datentyp]</td> 
   <td>Siehe „[!UICONTROL Art der benutzerdefinierten Daten]“.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tage Verspätung]</td> 
   <td> <p>Dieses Feld zeigt eine Datumsabweichung zwischen [!UICONTROL Geplanter Start] und [!UICONTROL Heute] an, wenn [!UICONTROL Tatsächliches Fertigstellungsdatum] fehlt.</p> <p>Zeigt auch eine Datumsabweichung zwischen [!UICONTROL Tatsächlicher Abschluss] und [!UICONTROL Geplanter Abschluss], wenn ein [!UICONTROL tatsächliches Fertigstellungsdatum] vorhanden ist.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Standardzeitplan]</td> 
   <td> <p>Anpassbare Standardarbeitsstunden, die Benutzenden und Projekten in einer Organisation zugewiesen werden können. </p> <p>Zeitpläne werden verwendet, um das geplante Datum sowie das Start- und das Fertigstellungsdatum von Aufgaben zu berechnen, die Benutzenden zugewiesen werden.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Zu erbringende Leistung]</td> 
   <td>Quantifizierbare Waren oder Dienstleistungen, die nach Abschluss eines Projekts bereitgestellt werden müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Bedarfs-Management]</td> 
   <td>Bewertung und Priorisierung der Aufnahmeprozesse.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Abteilungsziele]</td> 
   <td>Eindeutige Ziele für eine bestimmte Abteilung, die sich auf die Verbesserung der Betriebsmetriken innerhalb der Abteilung konzentrieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abhängigkeit]</td> 
   <td>Die Verknüpfung zwischen zwei Aufgaben, für die der Status einer Aufgabe geändert werden muss, bevor der Status der anderen Aufgabe ebenfalls geändert werden kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abhängigkeitstyp]</td> 
   <td> <p>Der Typ der Planungsbeziehung zwischen einer Aufgabe und ihren Vorgängern. Ein Beispiel ist [!UICONTROL Beenden-Start]. Dies setzt voraus, dass die erste Aufgabe beendet wird, bevor die zweite Aufgabe beginnen kann.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Überblick über Typen von Aufgabenabhängigkeiten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokument]</td> 
   <td>Jede Datei, die an ein Objekt in [!DNL Workfront] angehängt ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokumentversion]</td> 
   <td> <p>Jedes Mal, wenn dasselbe Dokument in dasselbe Objekt hochgeladen wird, wird ihm eine Versionsnummer zugewiesen. Benutzende können mehrere Optionen für eine frühere Version eines Dokuments anzeigen und ändern.</p> <p>Weitere Informationen finden Sie unter <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Verwalten von Dokumentversionen</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe oder ein Problem abgeschlossen sein soll. Das Fälligkeitsdatum einer Aufgabe oder eines Problems entspricht dem geplanten Abschlussdatum.</p>
    <p>Das Fälligkeitsdatum von Aufgaben und Problemen ist in Aufgaben- und Problemlisten und Berichten sichtbar.</p> 
    <p>Siehe auch „Geplantes Abschlussdatum“ in dieser Tabelle. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer]</td> 
   <td> <p>Das Zeitfenster, das für den Abschluss einer Aufgabe, eines Problems oder eines Projekts zugewiesen wurde (bestimmt durch die Anzahl der Tage zwischen dem [!UICONTROL geplanten Start] und dem geplanten Abschluss).</p> 
    <ul> 
     <li>Bei Aufgaben ist die Dauer ein bearbeitbares Feld, wenn der Dauertyp der Aufgabe nicht „Einfach“ ist. Wenn der Dauertyp der Aufgabe „Einfach“ ist oder die Aufgabenbeschränkung „Feste Daten“ ist, wird die Berechnung der Dauer von Workfront durchgeführt.</li> 
     <li>Bei Problemen ist die Dauer immer ein bearbeitbares Feld und sollte eine Schätzung der Anzahl der Tage darstellen, innerhalb derer das Problem gelöst werden muss.</li> 
     <li>Bei Projekten wird die Dauer von [!DNL Workfront] berechnet. Es handelt sich dabei um die Differenz in Tagen zwischen dem geplanten Beginn der frühesten Aufgabe und dem [!UICONTROL geplanten Abschluss] der spätesten Aufgabe des Projekts.</li> 
    </ul> <p>Weitere Informationen zum Unterschied zwischen „[!UICONTROL Dauer]“ und „[!UICONTROL Geplante Dauer]“ für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Unterschied zwischen [!UICONTROL geplanter Dauer] und [!UICONTROL Dauer] für Aufgaben</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer in Minuten]</td> 
   <td>Dieses Feld zeigt dieselben Informationen wie das Feld „[!UICONTROL Dauer]“ in Minuten anstelle von Tagen an. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Dauer pro Termin]</td> 
   <td> <p>Wird in den Feldern [!UICONTROL Aufgabendetails] und [!UICONTROL Aufgabe bearbeiten] eines übergeordneten Elements wiederkehrender Aufgaben angezeigt. Angezeigt wird die Dauer jeder wiederkehrenden Aufgabe. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Erstellen wiederkehrender Aufgaben</a>. </p> <p> <span>Eine in einzelnen wiederkehrenden Aufgaben geänderte Dauer zeigt nicht den in diesem Feld angegebenen Wert an.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Dauer – Typ]</td> 
   <td> <p>Ein Aufgabenfeld, das angibt, wie die zur Erledigung der Aufgabe erforderliche Arbeit den Personen, denen die Aufgabe zugewiesen wurde, über die Dauer der Aufgabe hinweg zugeteilt wird. Es stellt die Beziehung zwischen der [!UICONTROL Dauer] der Aufgabe, dem [!UICONTROL Arbeitsaufwand] und der Zeit oder der [!UICONTROL Zuteilung] dar, die die zugewiesenen Ressourcen für die Aufgabe aufwenden sollen, um sie abzuschließen. </p> <p>Dieses Feld wird auf der Registerkarte [!UICONTROL Details] einer Aufgabe angezeigt. </p> <p>Die Optionen für den Dauertyp einer Aufgabe sind:</p> 
    <ul> 
     <li>[!UICONTROL Berechneter Arbeitsauftrag]</li> 
     <li>[!UICONTROL Berechnete Arbeit]</li> 
     <li>[!UICONTROL Leistungsgesteuert]</li> 
     <li>[!UICONTROL Einfach]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Überblick über die [!UICONTROL Dauer] und den [!UICONTROL Dauertyp]</a> einer Aufgabe.</p> 
    --&gt;
    </td>
   </tr> 
   <tr> 
   <td>[!UICONTROL Dauer – Einheit]</td> 
   <td>Die Einheit, die zur Zeitmessung in einer Power-Suche verwendet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Leistungsgesteuert]</td> 
   <td>Die Beziehung zwischen der Anzahl der Benutzenden und der Zeit, die für die Erledigung der Aufgabe benötigt wird. Je mehr Benutzende Sie hinzufügen, desto kürzer wird die für die Erledigung der Aufgabe geplante Gesamtzeit. Die Dauer der Aufgabe bleibt jedoch gleich. Wenn eine Aufgabe beispielsweise darin besteht, eine Tüte Erdnüsse zu schälen, verringert sich durch den Einsatz weiterer Personen die geplante Zeit. Die Dauer in Personentagen bleibt jedoch gleich.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verstrichene Zeit]</td> 
   <td> <p>[!UICONTROL Verstrichene Zeit] ist eine Zeiteinheit für die [!UICONTROL Dauer] einer Aufgabe. Dies ist die Zeit zwischen [!UICONTROL Geplantes Startdatum] und [!UICONTROL Geplantes Abschlussdatum] einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen. </p> <p>[!DNL Workfront] unterstützt die folgenden Einheiten verstrichener Zeit für die Dauer einer Aufgabe:</p> 
    <ul> 
     <li> <p>[!UICONTROL Verstrichene Minuten]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Stunden]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Tage]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Wochen]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Monate]</p> </li> 
    </ul> <p>Weitere Informationen zur Dauer von Aufgaben, einschließlich der verstrichenen Zeit, finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Überblick über die [!UICONTROL Dauer] und den [!UICONTROL Dauertyp]</a> einer Aufgabe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> In einem Bericht zum [!UICONTROL Tarif] ist dies das Datum, an dem ein neuer Abrechnungssatz für ein Aufgabengebiet auf Projektebene endet. Die mit dem Projekt verknüpften Stunden vor diesem Datum werden mit diesem Abrechnungssatz multipliziert, um den Projektumsatz zu berechnen. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Interaktion]</td> 
   <td>Der [!UICONTROL Arbeitsleistungsindikator] (Work Performance Indicator, WPI), der angibt, wann das Engagement und die Überzeugung für die Aufgabe, das Projekt, das Team oder die Organisation nachlassen. Dies zeigt, dass Sie handeln müssen, um diese Überzeugung und dieses Engagement wiederzubeleben. Der WPI wird anhand der einfachen Frage gemessen: „Haben Sie verstanden, was von Ihnen erwartet wurde? Hat die Ihnen zugewiesene Arbeit einen Unterschied für die Organisation gemacht? Haben Sie großartige Arbeit geleistet?“</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Unternehmensziele]</td> 
   <td>Funktionsübergreifende Ziele, die zur Metrik der Unternehmensziele beitragen.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Geschätzter Gesamtaufwand (Estimate at Completion, EAC)]</td> 
   <td><p>Als Leistungskennzahl für Projekte stellt „Geschätzter Gesamtaufwand (Estimate at Completion, EAC)“ die voraussichtlichen Gesamtkosten bei Abschluss Ihrer Aufgabe oder Ihres Projekts dar.</p>
   <p>Als Projekteinstellung können Sie festlegen, wie der EAC-Wert berechnet werden soll.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-eac.md">Berechnen des geschätzten Gesamtaufwands (Estimate at Completion, EAC)</a>. </p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Geschätztes Fälligkeitsdatum]</td> 
   <td>In Projekt-, Aufgaben- und Problemberichten ist das geschätzte Fälligkeitsdatum das Datum, bis zu dem Workfront die Fertigstellung des Elements voraussichtlich erwartet.</td> 
  </tr>


<tr> 
   <td>[!UICONTROL Ereignis]</td> 
   <td>Jede Änderung in einem Projekt oder einer Aufgabe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-Handler]</td> 
   <td>Automatisierte Aufgaben, die ausgeführt werden, wenn Ereignisse stattfinden. Ein gängiges Beispiel ist eine automatisierte E-Mail-Benachrichtigung.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignisbenachrichtigung]</td> 
   <td>Von einem Ereignis-Handler generierte E-Mail.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td>Sonstige Kosten für Aufgaben oder Projekte.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Extern]</td> 
   <td> <p>In der Regel handelt es sich um einen Lizenztyp oder einen Benutzer bzw. eine Benutzerin mit einer solchen Lizenz. Benutzende mit einem solchen Lizenztyp können nur Informationen im System überprüfen. Sie können nicht aktiv an der Arbeit teilnehmen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Überblick über Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externes System]</td> 
   <td>Alle Dienste oder Software, die außerhalb des vorgesehenen System of Record gespeichert sind und verwaltet werden.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Feld]</td> 
   <td><p>Alle Workfront-Objekte oder die damit verbundenen Informationen, wie sie in der Datenbank angezeigt werden. </p>
   <p>Beispielsweise sind „Projekt“, „Benutzerin bzw. Benutzer“, „Stunde“ sowohl Workfront-Objekte als auch Felder. „Name“, „Status“, „Besitzerin bzw. Besitzer“, „Startdatum“ sind Workfront-Felder, die mit den oben genannten Objekten verknüpft sind. </p>

<p>Bei der Bezugnahme auf Objekte können die Begriffe „Objekte“ und „Felder“ synonym verwendet werden.</p>
   <p>Im Rahmen des Reportings beziehen sich die „Felder“ auf die Objekte oder die Informationen über das Objekt, die Sie im Bericht erfassen möchten.</p>

<p><b>HINWEIS</b></p>

<p>Beim textbezogenen Reporting beziehen sich Felder auf die Objekte oder deren Informationen, wie sie in der Datenbank angezeigt werden.</p>
   <p>Manchmal unterscheidet sich der Name, den Sie in der Benutzeroberfläche sehen, vom Namen des Feldes in der Datenbank. Beispielsweise ist „Problem“ der Name des Objekts in der Workfront-Benutzeroberfläche, aber „opTask“ ist der Name des Objekts (oder des Feldes) in der Workfront-Datenbank. </p> 
   <p> Es ist wichtig, das Feld so zu verwenden, wie es in der Datenbank angezeigt wird, wenn Sie einen Textmodusbericht verfassen und eine Ansicht, einen Filter oder eine Gruppierung oder ein berechnetes Feld erstellen.</p>

<p>Weitere Informationen finden Sie unter <a href="../../../wf-api/general/api-explorer.md">API-Explorer</a> und <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Überblick über den Textmodus</a>.</p>

<p>Standardmäßig enthält Workfront eine Reihe von Feldern, die sowohl Objekte als auch deren Informationen definieren. Sie können auch benutzerdefinierte Felder zum Definieren von Objekten erstellen, jedoch keine benutzerdefinierten Objekte.</p>

<p>In Workfront-Planung können Sie benutzerdefinierte Felder für alle Eintragstypen erstellen. Workfront-Eintragstypen verfügen nur über eine sehr begrenzte Anzahl von Feldern. Sie müssen alle Felder von Grund auf neu erstellen und Eintragstypen zuordnen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/fields/fields-overview.md">Überblick über Felder</a>. </p> <p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Einer der Hauptbausteine eines Berichts oder eines Listenelements, der bzw. das definiert, welche Informationen auf dem Bildschirm angezeigt werden. Weitere Informationen zu Berichtselementen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting-Elemente: Filter, Ansichten und Gruppierungen</a>.</p> <p>Der Filter bestimmt die Ergebnisse, die in einem Bericht oder in einer Liste eines [!DNL Workfront]-Panels angezeigt werden, wie z. B. Projekte, Aufgaben oder Probleme.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Arbeits-Management – Finanzen]</td> 
   <td>Prozess zur Verwaltung von Lohnkosten, Ausgaben und Umsatzdaten in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Festkosten]</td> 
   <td>Sie können einen festen Kostenbetrag für ein Projekt definieren. Dies ist Teil der [!UICONTROL geplanten Kosten] des Projekts, die den Betrag darstellen, den Sie zum Abschließen des Projekts benötigen. Informationen zu den Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Nachverfolgen von Kosten</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fester Umsatz]</td> 
   <td>Sie können einen festen Umsatzbetrag für ein Projekt definieren. Dies ist Teil des [!UICONTROL geplanten Umsatzes] des Projekts, der dem Geldbetrag entspricht, den Sie möglicherweise erhalten, wenn Sie das Projekt abschließen. Informationen zum Umsatz finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Überblick über Abrechnung und Umsatz</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Dies ist dasselbe Feld wie [!UICONTROL Status-Symbole], es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL Vorlagen] </li> 
     <li> [!UICONTROL Ausgaben] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Status-Symbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner]</td> 
   <td>Mit Ordnern können Sie Dokumente oder Berichte organisieren, die mit einem Objekt verknüpft sind.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Vollzeitäquivalent)</td> 
   <td>Dies ist das Vollzeitäquivalent, das angibt, für wie lange eine Ressource für die Arbeit verfügbar ist. 
   Das Feld „[!UICONTROL FTE]“ wird in den folgenden Bereichen angezeigt: 
  <ul>
   <li> Benutzerprofil beim Bearbeiten oder Erstellen des Benutzers bzw. der Benutzerin </li>
   <li> [!UICONTROL Ressourcenplaner] </li>
   <li> [!UICONTROL Szenarienplaner] (erfordert eine zusätzliche Lizenz für den Szenarienplaner von Workfront) </li>
   <li> Benutzerlisten und Berichte </li> </ul>

<p>Der [!UICONTROL FTE] muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. </p>
   <p> Ein [!UICONTROL FTE] von 1 (der Standardwert für das Feld „[!UICONTROL FTE]“ einer Person gemäß der Definition in ihrem Profil) bedeutet, dass eine Ressource (Person oder Funktion) die gesamte Anzahl von Stunden arbeitet, basierend auf dem Zeitplan, anhand dessen ihre Verfügbarkeit berechnet wird. </p>
   <p>Ihr bzw. Ihre Workfront-Admin entscheidet, welcher Zeitplan zur Bestimmung der Benutzerverfügbarkeit verwendet werden soll.  </p>
   <ul>
   <li> Wenn der [!UICONTROL Standardzeitplan] genutzt wird, verwendet Workfront den [!UICONTROL FTE] der Person, der in ihrem Profil gefunden wurde, um die Verfügbarkeit zu berechnen. </li>
   <li> Wenn der Zeitplan der Person genutzt wird, verwendet Workfront ihre Ausfallzeit, denn Wert unter „[!UICONTROL Arbeitszeit]“ und die Stunden im [!UICONTROL Standardzeitplan], um den [!UICONTROL FTE] der Person zu ermitteln. </li> </ul>

<p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Konfigurieren von Voreinstellungen für das Ressourcen-Management</a>.  </p>
   <p>Weitere Informationen zum Erstellen eines Zeitplans in [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>

<p><b>HINWEIS</b></p>
   <p>Für alle Berechnungen im [!UICONTROL Szenarienplaner] verwendet Workfront den folgenden Wert: 1 [!UICONTROL FTE] = 8 Stunden.</p>
   <p>Weitere Informationen finden Sie unter <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Erste Schritte mit dem [!UICONTROL Szenarienplaner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G–I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gantt-Diagramm]</td> 
   <td> <p>Eine visuelle Timeline der Projekttermine in einer Kalenderansicht, die auf den geplanten oder voraussichtlichen Terminen basiert, wie sie derzeit für die Aufgaben des Projekts geplant sind.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ziel]</td> 
   <td><p>In [!DNL Workfront] gibt es zwei Konzepte von Zielen: </p> 
    <ul> 
     <li> <p><b>Projektziele</b>: Eine Reihe von Geschäftszielen, die von den entsprechenden Verantwortlichen eines Projekts vereinbart wurden. Projektziele sind Teil des Business-Case eines Projekts. </p> <p>Sie können Projektziele nicht in Listen oder Berichten anzeigen, aber Sie können über die API darauf zugreifen. </p> <p>Informationen zu Business-Case-Projektzielen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Erstellen von Business-Case-Zielen</a>. </p> </li> 
     <li> <p><b>Strategische Ziele</b>: Ein strategisches Ziel ist ein Ziel, das Sie erstellen, um Ihre Arbeitsstrategie für einen bestimmten Zeitraum zu planen. Sie können diese Arten von Zielen mithilfe von [!DNL Workfront Goals] erstellen. Ihr Unternehmen muss eine zusätzliche Lizenz erwerben und Sie müssen Zugriff auf diese Funktion haben, um strategische Ziele erstellen zu können. [!DNL Workfront Goals] ist nur mit einer zusätzlichen Lizenz verfügbar.</p> 
     <p>Weitere Informationen finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] </a>“. </p> 
     <p>Sie können strategische Ziele in einem Ziel- oder Projektbericht anzeigen und über die API darauf zugreifen. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Zielhierarchie]</td> 
   <td> <p>In Berichten zu [!UICONTROL Ziel] und [!UICONTROL Projekt] ist dies ein Sammlungsfeld, das die Ziele in der Hierarchie anzeigt, zu der ein strategisches Ziel gehört, wenn es an anderen Zielen ausgerichtet wird. Die Ziele werden durch das Trennzeichen ▸ voneinander getrennt. </p> <p>In diesem Feld werden nur die übergeordneten Elemente des Ziels und das Ziel selbst angezeigt. Untergeordnete Ziele werden nicht angezeigt. </p> <p>Informationen zum Ausrichten von Zielen in [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Überblick über die Zielausrichtung in [!DNL Workfront Goals]</a>. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihre Organisation [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>“. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Bewertung der Zielerfüllung]</td> 
   <td> In einem [!UICONTROL Projektbericht] wird dieses Feld verwendet, um auf die Ziele auf Projektebene zu verweisen, die mit dem [!UICONTROL Business]-Case verknüpft sind. Derzeit ist dies ein veraltetes Feld, das mit keiner Funktion verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziele] </td> 
   <td> <p>In einem Bericht zum [!UICONTROL Projekt] ist dies ein Sammlungsfeld, das alle strategischen Ziele anzeigt, die mit einem Projekt verbunden sind. Die Ziele werden durch Kommas getrennt.</p> <p>Dieses Feld ist nur sichtbar, wenn Ihre Organisation [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>“. Weitere Informationen zu strategischen Zielen und Projektzielen in [!DNL Workfront] finden Sie unter „[!UICONTROL Ziel]“ in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Schnittstelleneinstellungen]</td> 
   <td>Einstellungen der Benutzeroberfläche, die sich auf alle Benutzenden auswirken. [!UICONTROL Globale Schnittstelleneinstellungen] können durch die [!UICONTROL Benutzeroberflächeneinstellungen] überschrieben werden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gruppe]</td> 
   <td> <p>Eine Sammlung von Benutzenden (möglicherweise aus derselben Abteilung oder Geschäftseinheit), die Zugriff auf dieselben Objekte haben. Zusätzlich zu den Benutzenden können Gruppen mit Portfolios, Programmen, Projekten, <span> Projektvorlagen, </span> Unternehmen, Teams, Zeitplänen, Layout-Vorlagen und Arbeitszeittabellen-Profilen verknüpft werden.</p> <p>Sie können auch Berechtigungen für Objekte nach Gruppe erteilen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Überblick über Gruppen</a>.</p> <p>In einer Liste oder einem Bericht mit Objekten eines der folgenden Typen können Sie mithilfe des Feldes „[!UICONTROL Gruppe]“ auflisten, welche Objekte dieses Typs einer bestimmten Gruppe zugeordnet sind: Benutzerin bzw. Benutzer, Portfolio, Programm, Projekt, <span>Projektvorlage</span>, Unternehmen, Team, Zeitplan, Layout-Vorlage oder Arbeitszeittabellenprofil.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gruppen-Administrator]</td> 
   <td> <p>Benutzende, die die Objekte, den Zugriff und die Benutzer bzw. Benutzerinnen bestimmter Benutzergruppen verwalten.</p> <p> In einem Bericht des Typs „[!UICONTROL Gruppe]“ zeigt dieses Feld die Namen der Benutzenden an, die in der Gruppe als [!UICONTROL Gruppenadmins] angegeben sind. Weitere Informationen zu Gruppenadmins finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadmins</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gruppe mit Administratorzugriff]</td> 
   <td> <p> In einer [!UICONTROL Layout-Vorlage], einem [!UICONTROL Arbeitszeittabellenprofil] oder einem [!UICONTROL Zeitplanbericht] enthält dieses Feld die Gruppen, deren Gruppenadmins über die Zugriffsrechte zum Bearbeiten der Vorlage verfügen. Sie können diesen Bericht auch nach diesem Feld filtern. </p> <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gruppierung]</td> 
   <td> <p>Ein Reporting-Element, mit dem Informationen in einer Liste anhand eines gemeinsamen Kriteriums kategorisiert werden.</p> <p>Weitere Informationen finden Sie im Abschnitt „[!UICONTROL Gruppierungen]“ im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Reporting-Elemente: Filter, Ansichten und Gruppierungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergabedatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe für die Arbeit verfügbar wird. Das [!UICONTROL Übergabedatum] wird berechnet und kann nicht manuell festgelegt werden. <br>Weitere Informationen zum [!UICONTROL Übergabedatum] finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Überblick über das [!UICONTROL Übergabedatum der Aufgabe]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Helpdesk]</td> 
   <td>Ein alternativer Name für den Bereich „[!UICONTROL Anfragen]“ von [!DNL Workfront]. Im Bereich „[!UICONTROL Anfragen]“ können Sie Kunden-Support-Tickets, Projektanfragen, Helpdesk-Tickets usw. verarbeiten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Besitzerin bzw. Besitzer]</td> 
   <td>In einem Bericht des Typs „[!UICONTROL Stunde]“ bezeichnet „[!UICONTROL Besitzerin bzw. Besitzer]“ die Person, der die Stunden zugeordnet sind. Dies unterscheidet sich von der Person, die die Zeit tatsächlich erfasst. Diese beiden Entitäten können manchmal zwei verschiedene Benutzende sein. <br>Weitere Informationen zur Erfassung der Zeit für andere Benutzende finden Sie im Artikel <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Erfassen von Zeit</a>.</td> 
  </tr>

<tr> 
   <td>Stundenstatus</td> 
   <td> <p>Ein Attribut, das von Workfront für die tatsächlichen Stunden festgelegt wird, die Benutzende für Aufgaben, Probleme oder Projekte erfassen. </p>

Stundeneinträge können einen der folgenden Status in Workfront aufweisen:
<ul>
   <li><b>Gesendet</b>: Die Stunden wurden für ein Projekt, eine Aufgabe oder ein Problem erfasst. Sie sind entweder Teil eines Abrechnungseintrags oder wurden noch nicht zu einem Abrechnungseintrag hinzugefügt.</li>
   <li><b>Genehmigt</b>: Die Stunden wurden erfasst und vom Projektbesitzer bzw. der Projektbesitzerin genehmigt. Sie sind entweder Teil eines Abrechnungseintrags oder wurden noch nicht zu einem Abrechnungseintrag hinzugefügt.</li> 
   <li><b>Nicht genehmigt</b>: Die Stunden wurden erfasst und vom Projektbesitzer bzw. der Projektbesitzerin abgelehnt. Sie sind entweder Teil eines Abrechnungseintrags oder wurden noch nicht zu einem Abrechnungseintrag hinzugefügt.</li>
   <li><b>Abgerechnet</b>: Die Stunden wurden erfasst, einem Abrechnungseintrag hinzugefügt, und der Status des Abrechnungseintrags wurde als „Abgerechnet“ gekennzeichnet. Sie mussten nicht vom Projektbesitzer bzw. von der Projektbesitzerin genehmigt werden.</li>
   <li><b>Abgerechnet und genehmigt</b>: Die Stunden wurden erfasst und vom Projektbesitzer bzw. der Projektbesitzerin genehmigt, und der Status des Abrechnungseintrags wurde als „Abgerechnet“ gekennzeichnet.</li>
   </ul>

<p>Wenn Stunden Teil eines Abrechnungseintrags sind, gibt der Stundenstatus an, ob die Stunden genehmigt wurden oder ob der Abrechnungseintrag, zu dem sie gehören, in Rechnung gestellt wurde. Der Stundenstatus eines Stundeneintrags ist nur in einer Stundenliste oder einem Bericht sichtbar. </p>

<p>Weitere Informationen zum Hinzufügen von Stunden zu Abrechnungseinträgen finden Sie im Abschnitt „Hinzufügen von Stunden zu Abrechnungseinträgen“ im Artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Erstellen von Abrechnungseinträgen</a>.</p>

<p>Weitere Informationen zur Genehmigung der Zeit für Projekte finden Sie unter <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Anfordern der Genehmigung des Zeitaufwands für ein Projekt</a>.</p>

<p><b>TIPP</b></p>

<p>Für allgemeine Stunden, die nicht direkt für Arbeitselemente erfasst werden, wird kein Stundenstatus angezeigt. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Stundentyp]</td> 
   <td> <p>Ein Attribut, das für die tatsächlichen Stunden festgelegt werden kann, die Benutzende für Aufgaben, Probleme oder Projekte erfassen. Dies ist auch ein Attribut für die erfassten Stunden, die nicht direkt mit der Arbeit verknüpft sind, z. B. [!UICONTROL Urlaub] und [!UICONTROL Ausfallzeit].</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Verwalten von Stundentypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Die ID ist ein alphanumerischer Indikator, der mit jedem Objekt in [!DNL Workfront] verknüpft ist. Jedes Objekt in der Datenbank von [!DNL Workfront] wird eindeutig identifiziert. Sie können die ID eines beliebigen Objekts in einem Bericht oder einer Liste für jedes Objekt anzeigen. </p> <p><b>TIPP</b></p>   <p>Sie können die ID auch in der URL der Objektseite anzeigen. Wenn Sie beispielsweise auf die Seite „[!UICONTROL Projektdetails]“ zugreifen, könnte die ID eines Projekts in etwa wie die Zahl in der folgenden URL aussehen:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Identitäts-Management-System. Das Adobe-IMS verlangt, dass Sie sich bei Workfront über Adobe anmelden, anstatt Ihren Benutzernamen und Ihr Passwort für Workfront zu verwenden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Persönliche Ziele]</td> 
   <td>Persönliche Ziele, die zu den Metriken der Team-Ziele beitragen, aber nicht mit der persönlichen oder beruflichen Entwicklung zusammenhängen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Übernommener Zugriff]</td> 
   <td>Freigabefunktion, mit der der Zugriff von einem Objekt zu einem anderen übertragen werden kann. Beispielsweise übernehmen Projektbenutzende die in Programm- und Portfolio-Einträgen definierten Zugriffsrechte.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>Im [!DNL Workfront Scenario Planner] können Sie einen Plan in mehrere Initiativen unterteilen, um die Verwaltung des Plans zu vereinfachen. <span>Sie können einen Bericht des Typs „[!UICONTROL Initiative]“ erstellen und auf Informationen zu einer [!UICONTROL Initiative] in einem Bericht zum [!UICONTROL Projekt] zugreifen.</span></p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick über den [!DNL Scenario Planner]</a>. </p> <p>Der Berichtstyp „[!DNL Initiative]“ ist in Ihrer Instanz von [!DNL Workfront] nur sichtbar, wenn Ihr Unternehmen eine Lizenz für den [!DNL Workfront Scenario Planner] erworben hat. Sie können nicht über die API auf [!UICONTROL Initiativen] zugreifen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Aufgabengebiet der Initiative]</span> </td> 
   <td> <p><span>Der Berichtstyp [!UICONTROL Aufgabengebiet der Initiative] zeigt Informationen zu den Aufgabengebieten an, die einer Planinitiative im [!DNL Workfront Scenario Planner] zugeordnet sind.</span> </p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Scenario Planner]</a>. </p> <p><span>Dieser Berichtstyp ist in Ihrer Instanz von [!DNL Workfront] nur sichtbar, wenn Ihr Unternehmen eine Lizenz für den [!DNL Workfront Scenario Planner] erworben hat.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Stunden für die Aufgabengebiete der Initiative]</span> </td> 
   <td> <p><span> In einem Bericht des Typs „[!UICONTROL Aufgabengebiet der Initiative]“ zeigt diese Option die Anzahl der Stunden an, die mit einem Aufgabengebiet in einer Initiative verknüpft sind.</span> </p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Scenario Planner]</a>. </p> <p>Dieses Feld und der Berichtstyp [!UICONTROL Aufgabengebiet der Initiative] sind in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine Lizenz für den [!DNL Workfront Scenario Planner] erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabengebiet der Initiative – Anzahl]</td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Aufgabengebiet der Initiative]“ wird die Anzahl der spezifischen Aufgabengebiete angezeigt, die einer Initiative zugeordnet sind.</p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Scenario Planner]</a>. </p> <p>Dieses Feld und der Berichtstyp „[!UICONTROL Aufgabengebiet der Initiative]“ sind in Ihrer Instanz von [!DNL Workfront] nur sichtbar, wenn Ihr Unternehmen eine Lizenz für den [!DNL Workfront Scenario Planner] erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datum der letzten Veröffentlichung der Initiative]</td> 
   <td> <p>Ein Feld in einem Bericht des Typs „[!UICONTROL Initiative]“, „[!UICONTROL Aufgabengebiet der Initiative]“ und „[!UICONTROL Projekt]“, das das Datum anzeigt, an dem eine Initiative in einem Plan zuletzt für ein Projekt veröffentlicht wurde. Sie können Initiativen veröffentlichen, um Projekte zu erstellen oder Projekte zu aktualisieren, die mit den Initiativen verknüpft sind.</p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Scenario Planner]</a>. </p> <p><span>Informationen zur Veröffentlichung von Initiativen finden Sie unter </span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Veröffentlichen von Szenarien zum Erstellen und Aktualisieren von Projekten im [!DNL Workfront Scenario Planner]</a>. Dieses Feld ist in Ihrer Instanz von [!DNL Workfront] nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner]-Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline-Suche]</td> 
   <td>Eine Suche, die beim Ausfüllen eines Formulars durchgeführt wird, um mögliche Einträge für ein bestimmtes Feld zu finden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup der Benutzeroberfläche]</td> 
   <td>Der Bereich der Anwendung, in dem Sie benutzerdefinierte Ansichten, Filter, Gruppierungen, Listensteuerelemente usw. definieren können.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Ist Unternehmensziel]</p></td> 
   <td> <p>In [!DNL goal reports] wird für jedes strategische Ziel ein Wert „[!UICONTROL Wahr]/ [!UICONTROL Falsch]“ angezeigt, um anzugeben, ob Ihre Organisation dem Ziel als Inhaber bzw. Inhaberin zugewiesen ist. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]</a>“.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problem]</td> 
   <td> <p>Ein ungeplantes Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Er wird triagiert und hinsichtlich des weiteren Arbeitsaufwands bewertet</p> <p>Ein [!UICONTROL Problem] kann auch eine Anfrage an den [!UICONTROL Helpdesk] sein. [!UICONTROL Änderungsanforderungen], [!UICONTROL Anfragen] und [!UICONTROL Fehler] sind ebenfalls [!UICONTROL Probleme].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problem-Management]</td> 
   <td> <p>Der Prozess und die Regeln für die Definition der Problemtypen und des Routing-, Triage- oder Traffic-Prozesses, der mit jedem Typ verknüpft ist.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Probleminhaber]</td> 
   <td>Das Team oder die Benutzenden, das bzw. die für die Triagierung und den Abschluss eines Problems verantwortlich ist bzw. sind.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Ein Zeitraum, in dem ein Team einen vordefinierten Satz von Arbeitsergebnissen erbringt.</td> 
  </tr> 
 </tbody> 
</table>

## J–L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabengebiet]</td> 
   <td> <p>Wird verwendet, um die alltäglichen Aufgabenbereiche und Aufgaben eines Benutzers bzw. einer Benutzerin zu identifizieren. Aufgabengebiete können Arbeitselementen zugewiesen werden, um die für den Abschluss eines Arbeitsverfahrens erforderlichen Fertigkeiten zu ermitteln, ohne sie einer bestimmten Person zuzuweisen. </p> <p>Ein Benutzer bzw. eine Benutzerin kann über mehrere Rollen verfügen. Beispiele hierfür sind Grafik-Designer bzw. Grafik-Designerin oder Berater bzw. Beraterin.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journaleintrag]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Informationen zu Systemaktualisierungen für nachverfolgte Felder bereitstellt, die im Bereich „[!UICONTROL Aktualisierungen]“ von Projekten, Aufgaben, Problemen und anderen Objekten angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Bericht über den Bereich „Aktualisierungen“ mit einem Bericht zum Journaleintrag</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban-Flag]</td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Aufgabe]“ oder „[!UICONTROL Problem]“ zeigt das Feld „[!UICONTROL Kanban-Flag]“ den Markierungsstatus an, der für die Story im [!UICONTROL Kanban-Board] festgelegt ist. Mögliche Werte sind „[!UICONTROL Auf Kurs]“, „[!UICONTROL Bereit, abzuziehen]“ und „[!UICONTROL Ist gesperrt]“.</p> <p>Weitere Informationen zum Festlegen des Flag-Status für Storys im [!UICONTROL Kanban-Story-Board] finden Sie im Artikel <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Verwenden von Markierungen für Storys auf dem [!UICONTROL Kanban-Board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Ein messbarer Wert, der zeigt, wie effektiv ein Unternehmen wichtige Geschäftsziele erreicht.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitabstand]</td> 
   <td>Der Zeitraum, der nach Ablauf des [!UICONTROL geplanten Abschlussdatums] der Vorgängeraufgabe verstreichen muss, bevor die abhängige Aufgabe beginnen kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitabstandstypen]</td> 
   <td> <p>Die Methode zur Berechnung des [!UICONTROL Zeitabstands]. Es kann sich handeln um:</p> 
    <ul> 
     <li>[!UICONTROL Tage] (Arbeitstage)</li> 
     <li>[!UICONTROL Kalendertage] (Feiertage ignorieren)</li> 
     <li>[!UICONTROL Prozent]</li> 
     <li>[!UICONTROL Tag der Woche]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Überblick über Zeitabstandstypen</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Große Miniaturansicht]</td> 
   <td> <p> In einer Liste oder einem Bericht zu einem [!UICONTROL Dokument] wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p>Wählen Sie <strong>[!UICONTROL Große Miniaturansicht]</strong> aus, um eine 400 Pixel breite Miniaturansicht im Bericht anzuzeigen.</p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch „[!UICONTROL Miniaturansicht]“ in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzten 10 anzeigenden Benutzer]</td> 
   <td> <p>In einer Berichtsliste enthält dieses Feld die Namen von bis zu 10 Benutzenden, die den Bericht zuletzt angezeigt haben.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte Bedingung – Notiz]</td> 
   <td> <p>Dieses Feld zeigt die letzte Aktualisierung an, die der Inhaber bzw. die Inhaberin des Objekts für ein Objekt eingegeben hat. Dies ist die letzte Aktivität oder Interaktion des Inhabers bzw. der Inhaberin für ein Objekt.</p> <p>Die Spalte [!DNL Last Condition Note] ist leer, wenn der Notiztext der letzten Notiz eines Objekts gelöscht wurde. Wenn eine neue Notiz für das Objekt eingegeben wird, wird sie zur letzten Notiz und wird erneut in der Spalte angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datum der letzten Finanzaktualisierung]</td> 
   <td>In einem Bericht des Typs „[!UICONTROL Projekt]“ werden in diesem Feld das Datum und die Uhrzeit der letzten Berechnung und Aktualisierung der Projektfinanzen erfasst. Informationen zu den Projektfinanzen finden Sie unter <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Überblick über die Projektfinanzen</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte Notiz]</td> 
   <td> <p>Dieses Feld zeigt die letzte Aktualisierung an, die ein Benutzer bzw. eine Benutzerin für ein Objekt eingegeben hat. Dies ist die neueste Aktivität oder Interaktion mit einem Objekt.</p> <p>Die Spalte [!UICONTROL Letzte Notiz] ist leer, wenn der Text der letzten Notiz für ein Objekt gelöscht wurde. Wenn eine neue Notiz für das Objekt eingegeben wird, wird sie zur letzten Notiz und wird erneut in der Spalte angezeigt.</p>
   <p>Wenn dieses Feld zu einem [!UICONTROL Task]-Bericht hinzugefügt wird, werden alle Aktualisierungen, die bei untergeordneten Objekten der Aufgabe verbleiben - z. B. Probleme, Unteraufgaben oder Dokumente -, nicht in dieser Spalte angezeigt.</p> 
   <p><b>NOTIZ</p>
   <p>Die letzte Anmerkung, die einem Objekt mithilfe der API hinzugefügt wurde, wird nicht in einem Bericht in Workfront angezeigt. Das Feld [!DNL Last Note] ist leer, wenn die letzte Aktualisierung für ein Objekt mithilfe der API hinzugefügt wurde. </p>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuletzt angezeigt von]</td> 
   <td> <p>In einer Berichtsliste enthält dieses Feld Informationen zu der Person, die den Bericht zuletzt angezeigt hat.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuletzt angezeigt am]</td> 
   <td> <p>In einer Berichtsliste wird in diesem Feld das Datum angezeigt, an dem der Bericht zuletzt angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout-Vorlage]</td> 
   <td>Wird vom Systemadmin oder Gruppenadmin definiert, um die Registerkarten und Berichte zu ermitteln, die im Arbeitsbereich eines bestimmten Benutzers bzw. einer bestimmten Benutzerin angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout-Typ]</td> 
   <td>In Verbindung mit [!UICONTROL benutzerdefinierten Ansichten] gibt der [!UICONTROL Layout-Typ] den Typ der [!UICONTROL benutzerdefinierten Ansicht] an. Derzeit ist nur eine Liste verfügbar. In Zukunft wird möglicherweise „[!UICONTROL Detail]“ (die Ansicht „[!UICONTROL Detail]“ eines Objekts) verfügbar.</td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--
  <tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there  are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.   
     </p> </td> </tr>
     -->
  <!--
  <tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.  </p>
    -->
    <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    -->
    <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    -->
    <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>    </p>
    -->
    </td>
  </tr> 
  <tr> 
   <!--
    <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection  of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    -->
    </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächliche Legacy-Stunden]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht handelt es sich bei den [!UICONTROL tatsächlichen Legacy-Stunden] um die Summe aller Stunden, die zu einem beliebigen Zeitpunkt (auch vor Mai 2021) für das Projekt, die Aufgabe oder das Problem erfasst wurden.</p>  
   <p>„Tatsächliche Legacy-Stunden“ wird als „Tatsächliche Stunden“ im Detailbereich eines Projekts, einer Aufgabe oder eines Problems angezeigt. </p>
   <p>Siehe auch <strong>Tatsächliche Stunden</strong>.
    <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Anzeigen der tatsächlichen Stunden</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL Lizenztyp]</td> 
   <td>Der Typ der Lizenz, die einer [!UICONTROL Zugriffsebene] zugeordnet ist. Entweder „[!UICONTROL Vollständiger Benutzer]“, „[!UICONTROL Eingeschränkter Benutzer]“ oder „[!UICONTROL Anforderer]“.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lizenz-Limit-Plan]</td> 
   <td> <p>In einer Ansicht oder einem Bericht des Typs „[!UICONTROL Gruppe]“ enthält dieses Feld die maximale Anzahl der Lizenzen des Typs „[!UICONTROL Plan]“, die Benutzenden zugewiesen werden können, für die die entsprechende Gruppe als ihre [!UICONTROL Hauptgruppe] festgelegt ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lizenz-Limit Arbeit]</td> 
   <td> <p>In einer Ansicht oder einem Bericht des Typs „[!UICONTROL Gruppe]“ enthält dieses Feld die maximale Anzahl der Lizenzen des Typs „[!UICONTROL Arbeit]“, die Benutzenden zugewiesen werden können, für die die entsprechende Gruppe als ihre [!UICONTROL Hauptgruppe] festgelegt ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eingeschränkte Benutzerrechte]</td> 
   <td>Ein Lizenztyp, der die Erstellung einer [!DNL Access Level] ermöglicht, die schreibgeschützte Berechtigungen enthält, mit der Möglichkeit, Probleme zu senden, Notizen einzugeben und Dokumente hochzuladen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Listensteuerelemente]</td> 
   <td> <p>Ein Teil des [!UICONTROL Setups der Benutzeroberfläche], der die Verknüpfung benutzerdefinierter Filter, Ansichten und Gruppierungen mit einzelnen Benutzenden oder global mit allen Benutzenden ermöglicht.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Suchfelder]</td> 
   <td> <p>Nachdem Sie in Workfront-Planung die Verbindung zwischen zwei Eintragstypen hergestellt und einzelne Einträge miteinander verknüpft haben, können Sie in dem Eintrag, von dem aus Sie die Verbindung herstellen, auf die Felder der verknüpften Einträge verweisen.</p>
   <p>Wenn Sie beispielsweise einen Kampagneneintragstyp mit einem Workfront-Projektobjekttyp verbinden, können Sie das Feld „Budget“ der verbundenen Projekte in den Kampagneneinträgen anzeigen. Das Projektfeld „Budget“ ist ein Suchfeld aus Projekten in einer Kampagne.</p> <p>Die Werte der Suchfelder werden automatisch in die Einträge übernommen, mit denen sie verbunden sind.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Überblick über verbundene Einträge</a>.</p>
   <p>Workfront-Planung benötigt eine zusätzliche Lizenz.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

## M–O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nur manuell]</td> 
   <td> <p>Einer der [!UICONTROL Aktualisierungstypen] eines [!UICONTROL Projekts]. Diese Einstellung ermöglicht, dass die Timelines „[!UICONTROL Projiziert]“ und „[!UICONTROL Geplant]“ des Projekts nur dann aktualisiert werden, wenn auf „[!UICONTROL Neuberechnete Timeline]“ geklickt wird. Auf diese Weise eingerichtete Projekte werden bei der nächtlichen Neuberechnung und beim Aktualisieren des Projekts bzw. der Aufgaben im Projekt ignoriert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des [!UICONTROL Aktualisierungstyps] eines Projekts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ich]</td> 
   <td> <p>Dies bezieht sich auf die aktuell angemeldete Person. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzende allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer bzw. die angemeldete Benutzerin angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max. Benutzer]</td> 
   <td> <p>Dieses Feld ist veraltet. Alle Informationen, die in diesem Feld möglicherweise angezeigt werden, beziehen sich auf eine Funktion, die aus [!DNL Workfront] entfernt wurde, und das Feld kann nicht aktualisiert werden. </p> <p>In früheren Versionen von [!DNL Workfront] konnten Sie dieses Feld beim Erstellen oder Bearbeiten eines Aufgabenfeldes aktualisieren. Es enthielt die Gesamtzahl der Benutzenden, die in jedem Projekt einer Rolle zugeordnet werden können. Der Wert null ermöglicht eine unbegrenzte Anzahl von Benutzenden, die einem Projekt zugewiesen werden können. </p>Das Feld ist weiterhin in einigen Berichten und Listen sichtbar, die angezeigten Informationen können jedoch nicht aktualisiert werden. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Meilenstein]</td> 
   <td> <p>Eine Markierung, die Sie mit einer Aufgabe verknüpfen können, um anzugeben, dass nach Abschluss der Aufgabe ein wichtiger Punkt im Projekt erreicht wurde. Im Allgemeinen können Sie Meilensteine verwenden, um ein bedeutendes Ereignis anzuzeigen, z. B. den Abschluss einer Projektphase oder einer Reihe wichtiger Aktivitäten. [!UICONTROL Meilensteine] sind normalerweise mit übergeordneten Aufgaben verknüpft. Sie müssen die Meilensteine erstellen, bevor Sie sie Aufgaben zuordnen können. Weitere Informationen zu Meilensteinen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Erstellen eines Meilensteinpfads</a> und <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Zuordnen von Meilensteinen zu Aufgaben</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Meilensteinpfad]</td> 
   <td>Eine Sammlung von [!UICONTROL Meilensteinen]. [!UICONTROL Meilensteinpfade] werden für Projekte verwendet, um Projekte mit bestimmten Arten von [!UICONTROL Meilensteinen] von Projekten mit einem anderen Satz an [!UICONTROL Meilensteinen] zu unterscheiden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Meilensteinaufgabe]</td> 
   <td>Eine Aufgabe mit einer Markierung für die Angabe eines zu messenden berichtspflichtigen Ereignisses.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Modul]</td> 
   <td>Ein einzelner Schritt in einem Szenario in [!DNL Workfront Fusion], der einige Funktionen basierend auf der verknüpften Anwendung durchführt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meine primäre Funktion]</td> 
   <td> <p>Wenn in Filtern auf dieses Objekt verwiesen wird, zeigt es entweder Benutzende an, die dieselbe [!UICONTROL primäre Funktion] haben wie die angemeldete Person, oder Arbeitselemente, die der [!UICONTROL primären Funktion] der angemeldeten Person zugewiesen sind.</p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzende allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer bzw. die angemeldete Benutzerin angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mein Haupt-Team]</td> 
   <td> <p>Wenn in Filtern darauf verwiesen wird, zeigt dieses Feld entweder Benutzende an, die zum [!UICONTROL Haupt-Team] der angemeldeten Person gehören, oder Arbeitselemente, die dem [!UICONTROL Haupt-Team] der angemeldeten Person zugewiesen sind. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzende allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer bzw. die angemeldete Benutzerin angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Namenskonvention]</td> 
   <td>Ein organisationsweiter Regelsatz, der Daten zur Erstellung von Namen von Projekten, Aufgaben und Arbeitsergebnissen verwendet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Eine Integration, die keine manuelle Codierung oder API-Konfiguration erfordert. Wird auch als vorkonfigurierte Integration bezeichnet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigationsmenü]</td> 
   <td>Das Panel oben in der Mitte der Anwendung, das Links zu den Hauptbereichen von [!UICONTROL Workfront] enthält.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Zahlenwert]</td> 
   <td>In einem Bericht des Typs „[!UICONTROL Journaleintrag]“ zeigt dies den aktualisierten Wert eines Feldes an, der den [!UICONTROL alten Zahlenwert] ersetzt.
   Weitere Informationen finden Sie unter „[!UICONTROL Alter Zahlenwert]“ in diesem Artikel.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Nicht fakturierbare Kosten]</td> 
   <td> <p>Eine Ausgabe, die für den Kunden bzw. die Kunden nicht als fakturierbar gekennzeichnet ist. Dies kann entweder eine geplante Ausgabe oder eine tatsächliche Ausgabe sein.</p> <p>Sie können die Felder „Geplante nicht fakturierbare Kosten“ und „Tatsächliche nicht fakturierbare Kosten“ zu Ansichten und Berichten hinzuzufügen. Sie werden nicht auf den Seiten mit den Projekt- oder Aufgabendetails angezeigt.</p>
   <p>Diese Felder finden Sie in den folgenden Berichtstypen:</p>
   <ul>
   <li>Baseline</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Kennzeichnen einer Ausgabe als fakturierbar finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Verwalten von Projektausgaben</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Arbeitsfreier Tag]</td> 
   <td>Ein Tag, der nicht für den Abschluss von Arbeitsaufträgen zugewiesen ist. Dies ist normalerweise ein Urlaubstag, ein Feiertag oder ein Wochenende. Der Begriff wird im API-Explorer angezeigt. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notiz]</td> 
   <td>Ein Kommentar oder eine Aktualisierung zu einem Objekt in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notizentext]</td> 
   <td> <p>Dadurch wird der Text einer Aktualisierung angezeigt, die von einer Person für ein beliebiges Objekt eingegeben wurde. </p> </td> 
  </tr>

<tr data-mc-conditions="">

<td>[!UICONTROL Anzahl der verknüpften Ziele]</td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Projekt]“ ist dies die Anzahl der strategischen Ziele, die mit dem Projekt verknüpft sind. Informationen zum Verknüpfen von Projekten mit strategischen Zielen finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Hinzufügen von Projekten zu Zielen in [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Informationen zu strategischen Zielen finden Sie auch unter „[!UICONTROL Ziel]“ in diesem Artikel.</p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihre Organisation [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Hinzufügen von Projekten zu Zielen in [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr>

<tr>

<td>[!UICONTROL Anzahl der untergeordneten Elemente]</td> 
   <td> <p>In einem [!UICONTROL Project]-Bericht ist dies die Anzahl der untergeordneten Elemente oder Unteraufgaben, die eine Aufgabe hat. 
   <p><b>TIPP</b></p>
   Sie können die <code>{numberOfChildren}</code> Berechnung einem berechneten benutzerdefinierten Feld im benutzerdefinierten Formular einer Aufgabe hinzufügen, um in einem benutzerdefinierten Feld die Anzahl der untergeordneten Elemente der Aufgabe anzuzeigen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md">Hinzufügen eines berechneten Felds zu einem Formular</a>. 
    </td>


</tr> 
  <tr> 
   <td>[!UICONTROL Objekt]</td> 
   <td> <p>Die in [!DNL Adobe Workfront] angezeigten Informationen werden durch Objekte dargestellt, die in der Datenbank von [!DNL Workfront] gespeichert sind. Die Informationen in Workfront werden durch Objekte gesteuert. Beispiele für Objekte:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Berichte]</li> 
     <li>[!UICONTROL Gruppen]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Benutzende]</li> 
     <li>[!UICONTROL Unternehmen]</li> 
     <li>[!UICONTROL Benutzerdefinierte Formulare]</li>
     <li>[!UICONTROL Benutzerdefinierte Felder]</li>  
     <li>[!UICONTROL Stunden]</li> 
     <li>[!UICONTROL Abrechnungssätze]</li> 
     <li>[!UICONTROL Vorlagen]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li>

<p><b>HINWEIS</b></p>
  <p>Dies ist keine vollständige Liste. </p>

</ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Grundlegendes zu Objekten in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objekttypen]</td> 
   <td>Wenn Sie einen Bericht oder eine Liste mit allen Ihren benutzerdefinierten Formularen erstellen, können Sie dieses Feld als Ansicht oder Filter verwenden, um zu sehen, welche Objekttypen mit den einzelnen Formularen verknüpft sind. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Alter Zahlenwert]</td> 
   <td>In einem Bericht des Typs „[!UICONTROL Journaleintrag]“ wird der ursprüngliche Wert eines Feldes vor seiner Aktualisierung angezeigt. Nachdem der Wert eines Feldes aktualisiert wurde, wird es als [!UICONTROL neuer Zahlenwert] in einem Bericht des Typs „[!UICONTROL Journaleintrag]“ angezeigt. Weitere Informationen finden Sie auch unter „[!UICONTROL Neuer Zahlenwert]“.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Nur bei Änderung]</td> 
   <td> <p>Eine Art der [!UICONTROL Projektaktualisierung]. Wenn diese Option ausgewählt ist, werden die Timelines „[!UICONTROL Projiziert]“ und „[!UICONTROL Geplant]“ des Projekts nur dann aktualisiert, wenn eine Aktualisierung oder Änderung am Projekt oder an einer Aufgabe innerhalb des Projekts vorgenommen wird. Das Projekt wird nicht jede Nacht aktualisiert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps eines Projekts </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op-Aufgabe]</td> 
   <td> <p>Der Name für das [!UICONTROL Problem] in der Datenbank von [!DNL Workfront], der in Textmodusberichten oder berechneten benutzerdefinierten Daten verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Offen]</td> 
   <td>Ein Problem oder eine Aufgabe, das bzw. die noch nicht abgeschlossen ist, aber bearbeitet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigramm]</td> 
   <td>Abkürzung für Organigramm. Dies ist ein Diagramm, das die Hierarchie einer Organisation zeigt. Es befindet sich auch auf der Registerkarte im Detailbildschirm „[!UICONTROL Benutzerin bzw. Benutzer]“, der angezeigt wird, und ermöglicht die Festlegung der Beziehungen für das [!UICONTROL Reporting] und das [!UICONTROL Unternehmen] der [!UICONTROL Benutzenden].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organisations-Setup]</td> 
   <td>Dadurch werden die [!UICONTROL Unternehmen], [!UICONTROL Gruppen] und [!UICONTROL Sicherheitsprofile] für Ihre Organisation definiert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Andere Gruppen]</td> 
   <td> <p>In einem Bericht oder einer Ansicht, in dem Benutzende aufgelistet werden, zeigt dieses Feld alle Gruppen an, in denen jede einzelne Person Mitglied ist. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Überschreibungswährung]</span> </td> 
   <td> 
    <div> 
     <p>In einem Bericht des Typs „[!UICONTROL Aufgabengebiet]“ ist dies die Währung, die mit einem Aufgabengebiet verknüpft ist. Sie überschreibt die [!UICONTROL Basiswährung], die von dem oder der Admin in [!DNL Workfront] im Bereich „[!UICONTROL Setup]“ festgelegt wurde. </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Überschreibungswährung Abrechnung/Stunde]</span> </td> 
   <td> 
    <div> 
     <p>In einem Bericht des Typs „[!UICONTROL Aufgabengebiet]“ ist dies der Abrechnungssatz pro Stunde des Aufgabengebiets, das die ausgewählte [!UICONTROL Überschreibungswährung] des Aufgabengebiets verwendet.</p> 
     <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Überschreibungswährung Kosten/Stunde]</span> </td> 
   <td> 
    <div> 
     <p>In einem Bericht des Typs „[!UICONTROL Aufgabengebiet]“ ist dies der Stundensatz des Aufgabengebiets unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung] des Aufgabengebiets. </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Besitzerin bzw. Besitzer]</td> 
   <td>Die Person, die für die Fertigstellung des angegebenen Objekts verantwortlich ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Besitzertyp]</span> </td> 
   <td> 
    <div> 
     <p>In einem Bericht des Typs „[!UICONTROL Ziel]“ wird der Besitzertyp angezeigt, der einem strategischen Ziel zugewiesen ist. Im Folgenden finden Sie die Typen von Zielbesitzenden:</p> 
     <ul> 
      <li> <p>[!UICONTROL Benutzende]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Gruppe]</p> </li> 
     </ul> 
     <p>In diesem Feld wird kein Wert angezeigt, wenn der Inhaber bzw. die Inhaberin des Ziels Ihr Unternehmen ist. </p> 
     <p>Dies erfordert eine zusätzliche Lizenz. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]</a>“. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P–R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Ein [!UICONTROL Parameter] ist ein benutzerdefiniertes Feld. Sie können einen Bericht für alle Parameter oder für benutzerdefinierte Felder in Ihrem System erstellen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnet]</td> 
   <td>In einem Bericht zeigt dieses Feld Informationen zum übergeordneten Element des Objekts an. Beispielsweise werden in einem Bericht des Typs „[!UICONTROL Problem]“ möglicherweise Informationen zu der Aufgabe oder dem Projekt angezeigt, unter der bzw. dem das Problem erfasst ist. In einem Aufgabenbericht werden möglicherweise Informationen zur direkt übergeordneten Aufgabe oder zum Projekt angezeigt. Weitere Informationen dazu, welche Objekte in [!DNL Workfront] übergeordnete Elemente haben könnten, finden Sie im Abschnitt „Interdependenz und Hierarchie von Objekten“ im Artikel <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Grundlegendes zu Objekten in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitabstand zwischen über- und untergeordneter Aufgabe]</td> 
   <td>Die Zeit, die zwischen dem Start der [!UICONTROL übergeordneten Aufgabe] und dem Start der [!UICONTROL Unteraufgabe] vergehen muss.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnete Aufgabe]</td> 
   <td>Wird auch als [!UICONTROL Übersichtsaufgabe] bezeichnet. Dies ist eine Aufgabe mit Unteraufgaben (auch als „[!UICONTROL Untergeordnete Aufgaben]“ bezeichnet). Die [!UICONTROL Dauer], die [!UICONTROL erforderliche Arbeit] und der Wert von „[!UICONTROL Prozent abgeschlossen]“ der übergeordneten Aufgabe werden aus den Unteraufgaben berechnet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Teilzeitressourcen]</td> 
   <td>Ein lizenzierter Benutzer bzw. eine lizenzierte Benutzerin, deren Kapazität unter dem im System definierten Standardzeitplan liegt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prozent abgeschlossen]</td> 
   <td> <p>Ein Projekt, eine Aufgabe oder ein Problem, das bzw. die anzeigt, welcher Prozentsatz der mit der Aufgabe, dem Projekt oder dem Problem verbundenen Arbeit abgeschlossen ist.</p> <p>Sie können dieses Feld für Probleme und Arbeitsaufgaben manuell aktualisieren. </p> <p>Für Projekte und übergeordnete Aufgaben ist dieses Feld eine Zusammenfassung aller laufenden Aufgaben. Sie können es nicht manuell aktualisieren. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Überblick über den [!UICONTROL Prozentwert des Projektabschlusses</a>.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Performance Index Method (PIM)]</td> 
   <td> <p>Die [!UICONTROL Performance Index Method (PIM)] für das Projekt steuert die Methode, die Adobe Workfront zur Berechnung von Projektleistungsmetriken wie Kostenentwicklungsindex (Cost Performance Index, CPI), Terminentwicklungsindex (Cost Schedule Performance Index, CSI), Zeitplan-Leistungsindex (Schedule Performance Index, SPI) und Estimate at Completion (EAC) verwendet.</p> 
   <p>Workfront berechnet diese Werte anhand der Stunden oder der Kosten.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/set-pim.md">Festlegen der Performance Index Method (PIM)</a>.</p>
   </td> 
  </tr>
 <tr> 
   <td>[!UICONTROL Berechtigung]</td> 
   <td> <p>Rechte, die einem Benutzer bzw. einer Benutzerin für ein Objekt gewährt werden, in der Regel damit er bzw. sie die Arbeit an dem Objekt abschließen oder das Objekt anzeigen kann. Berechtigungen können für folgende Elemente erteilt werden:</p> 
    <ul> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Berichte]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Benutzerdefinierte Formulare]</li> 
     <li>[!UICONTROL Ansichten]</li> 
     <li>[!UICONTROL Filter]</li> 
     <li>[!UICONTROL Gruppierungen]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Überblick über Freigabeberechtigungen für Objekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Dies ist ein vollständiger Lizenztyp im [!DNL Workfront]-System. Diese Berechtigung ist für den Zugriff auf alle Funktionen in [!DNL Workfront] erforderlich.</p> <p>Weitere Informationen finden Sie unter „Überblick über <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]</a>“.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (im [!DNL Scenario Planner])</td> 
   <td> <p>Ein Plan ist das Hauptobjekt bei der Arbeit mit dem Szenarienplaner in [!DNL Workfront]. Sie können die Strategie für die kurz- und langfristige Zukunft Ihres Unternehmens skizzieren, jedes Ergebnis auf allgemeiner Ebene identifizieren und es als Plan zum Szenarienplaner in [!DNL Workfront] hinzufügen. </p> <p>Sie können [!DNL Scenario Planner]-Pläne nicht in einem Bericht anzeigen und Sie können nicht über die [!DNL Workfront]-API darauf zugreifen. </p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplant]</td> 
   <td> <p>Der Zeitrahmen, innerhalb dessen etwas stattfinden soll. Beim Erstellen von Projekten, Aufgaben oder Problemen in [!DNL Workfront] legen Sie die geplanten Start- und Endtermine sowie den geplanten Zeitrahmen fest, in dem sie stattfinden. Diese Werte stellen Ihre ursprüngliche Absicht oder Schätzung dar, wie lange es dauern soll, bis ein Element abgeschlossen ist. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Nutzen]</td> 
   <td>Dies ist eine manuelle Eingabe für das Projekt-Management, um einzuschätzen, ob die Fertigstellung eines Projekts der Organisation einen finanziellen Vorteil bringen würde. Die Angabe dieses Wertes kann Teil der Erstellung eines [!UICONTROL Business-Case] für das Projekt sein. Sie müssen über Berechtigungen zum [!UICONTROL Verwalten] des Projekts verfügen, um diesen Wert zu aktualisieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Budgetierte Stunden – geplant]</td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Budgetierte Stunden]“ wird die Anzahl der budgetierten Stunden für Projekte oder [!UICONTROL Aufgabengebiete] im [!UICONTROL Ressourcenplaner] angezeigt. </p> <p>Informationen zur Budgetierung von Projekten oder Funktionen im [!UICONTROL Ressourcenplaner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetieren von Ressourcen im [!UICONTROL Ressourcenplaner] mithilfe der Ansichten „[!UICONTROL Projekt]“ und „[!UICONTROL Rolle]“</a>. Informationen zum Bericht des Typs „[!UICONTROL Budgetierte Stunden]“ finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>Sie können das [!UICONTROL geplante Abschlussdatum] einer Aufgabe, eines Projekts oder eines Problems manuell auf ein Datum Ihrer Wahl setzen. Wenn Sie das [!UICONTROL geplante Abschlussdatum] nicht festlegen, wird es von [!DNL Workfront] automatisch festgelegt. Bei automatischer Festlegung ist das [!UICONTROL geplante Abschlussdatum]: [!UICONTROL Geplantes Startdatum] + [!UICONTROL Dauer]</p> <p>Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Überblick über das [!UICONTROL geplante Abschlussdatum] der Aufgabe</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Festlegen des [!UICONTROL geplanten Abschlussdatums] für das Projekt</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Kosten]</td> 
   <td> <p>Summe von „[!UICONTROL Geplante Arbeitskosten]“ und „[!UICONTROL Geplante Ausgabenkosten]“ des Projekts. Dies umfasst nicht die [!UICONTROL geplanten Risikokosten] für das Projekt.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausrichtung am geplanten Datum]</td> 
   <td> <p>Hierbei handelt es sich um einen automatischen Indikator, mit dem Workfront Projekte, Aufgaben und Probleme zuweist, um zu zeigen, wann ein Element in Bezug auf das geplante Abschlussdatum abgeschlossen wird. </p>
   <p>Im Folgenden finden Sie mögliche Werte für den Indikator für die Ausrichtung am geplanten Datum: </p>
<ul>
<li>Wird zum geplanten Abschlussdatum fertiggestellt</li>
<li>Wird vor dem geplanten Abschlussdatum fertiggestellt</li>
<li>Wird nach dem geplanten Abschlussdatum fertiggestellt</li></ul>
<p>Die Ausrichtung am geplanten Datum ist in Projekt-, Aufgaben- und Problemlisten und -berichten sichtbar. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Dauer]</td> 
   <td> <p>Die [!UICONTROL geplante Dauer] einer Aufgabe ist in der Regel mit der [!UICONTROL Dauer] einer Aufgabe identisch. Sie stellt die Differenz in Tagen zwischen dem [!UICONTROL geplanten Start] und dem [!UICONTROL geplanten Abschlussdatum] der Aufgabe dar. </p> <p>Wenn für die Aufgabe als [!UICONTROL Dauer] der Typ „[!UICONTROL Leistungsgesteuert]“ verwendet wird, kann die [!UICONTROL geplante Dauer] von der [!UICONTROL Dauer] der Aufgabe abweichen, je nachdem, wie viele Ressourcen Sie der Aufgabe zuweisen. </p> <p>Wenn beispielsweise eine Aufgabe, deren [!UICONTROL Dauer] den Typ „[!UICONTROL Leistungsgesteuert]“ verwendet, eine [!UICONTROL Dauer] von 3 Tagen hat und Sie der Aufgabe eine Ressource mit einem Vollzeitplan zuweisen, ist die [!UICONTROL geplante Dauer] ebenfalls 3 Tage. Wenn Sie derselben Aufgabe drei Ressourcen mit einem Vollzeitplan zuweisen, bleibt die [!UICONTROL Dauer] 3 Tage, aber die [!UICONTROL geplante Dauer] wird zu 1 Tag. Die [!UICONTROL geplante Dauer] ändert auch die Termine unter „[!UICONTROL Geplanter Start]“ und „[!UICONTROL Geplanter Abschluss]“ für die Aufgabe, um die neue [!UICONTROL geplante Dauer] widerzuspiegeln. Daher ist auch die Timeline des Projekts betroffen. </p> <p>Weitere Informationen zum Unterschied zwischen der [!UICONTROL Dauer] und der [!UICONTROL geplanten Dauer] für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Unterschied zwischen [!UICONTROL geplanter Dauer] und [!UICONTROL Dauer] für Aufgaben</a>.</p> <p>Projekte und Probleme haben keine [!UICONTROL geplante Dauer]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Dauer in Minuten]</td> 
   <td> <p>Die [!UICONTROL geplante Dauer in Minuten] eines Projekts oder Problems entspricht der [!UICONTROL Dauer] des Projekts oder Problems in Minuten. </p> <p>Aufgaben haben kein Feld „[!UICONTROL Geplante Dauer in Minuten]“. </p> <p>[!UICONTROL Vorlagenaufgaben] haben ein Feld „[!UICONTROL Geplante Dauer in Minuten]“, das die [!UICONTROL geplante Dauer] der Aufgabe in Minuten anzeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Ausgabenkosten]</td> 
   <td> <p>Die Summe der [!UICONTROL geplanten Beträge] für alle Ausgaben, die für ein Projekt oder eine Aufgabe erfasst wurden.</p> <p><b>BEISPIEL</b></p>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und 600,00 € in das Feld „[!UICONTROL Geplanter Betrag]“ eingeben, betragen die [!UICONTROL geplanten Ausgabenkosten] für diese Aufgabe 600,00 €. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um [!UICONTROL geplante Ausgabenkosten] zu berechnen:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    -->
    </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Stunden]</td> 
   <td> <p>Dieses Feld wird in den Bereichen für [!UICONTROL Projekte], [!UICONTROL Aufgaben] und Probleme, in Berichten für Projekte, Aufgaben und Probleme und in Ressourcen-Management-Tools wie dem [!UICONTROL Ressourcenplaner], dem [!UICONTROL Workload Balancer] und dem Bericht zur [!UICONTROL Auslastung] angezeigt. </p> <p>Darin wird die Anzahl der Stunden angezeigt, die Projektbesitzende für die Erledigung jeder Aufgabe oder jedes Problems veranschlagen. Bei Projekten ist dies in der Regel eine Zusammenfassung der [!UICONTROL geplanten Stunden] aus den Aufgaben des Projekts. </p> <p>Das Feld „[!UICONTROL Geplante Stunden]“ enthält möglicherweise unterschiedliche Informationen, je nachdem, wo Sie es anzeigen. Informationen zu den geplanten Stunden finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Überblick über geplante Stunden</a>.</p> <p>Geplante Stunden werden in der Datenbank von [!DNL Workfront] in Minuten gespeichert. Berücksichtigen Sie beim Erstellen von Berechnungen mit diesem Feld, dass die Stunden als Minuten angezeigt werden.<br></p> <p>Standardmäßig werden die geplanten Stunden gleichmäßig auf alle Tage während der Dauer eines Arbeitselements und auch gleichmäßig auf alle Ressourcen verteilt, die der Aufgabe zugewiesen sind. Benutzende können die tägliche Anzahl der geplanten Stunden für ein Arbeitselement oder die individuellen geplanten Stunden für jede zugewiesene Person aktualisieren.</p> <p>Die Aktualisierung dieses Feldes erfolgt für Projekte, Aufgaben und Probleme auf unterschiedliche Weise: </p> 
    <ul> 
     <li> <p>Bei Problemen können Sie dieses Feld manuell aktualisieren. Die geplanten Stunden für das Problem werden nicht zu den geplanten Stunden des Projekts hinzugefügt. </p> <p><b>TIPP</b></p> <p>In einem Problembericht wird eines der Felder „[!UICONTROL Geplante Stunden]“ durch das Feld „[!UICONTROL Arbeit]“ ersetzt. Das Feld enthält die Anzahl der für das Problem geplanten Stunden. Weitere Informationen finden Sie unter den Feldern „work“ oder „[!UICONTROL Arbeit]“ in dieser Tabelle. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Bei Aufgaben können Sie dieses Feld manuell aktualisieren, wenn der [!UICONTROL Dauertyp] der Aufgabe „[!UICONTROL Berechneter Arbeitsauftrag]“ oder „[!UICONTROL Einfach]“ ist. Dieses Feld wird von [!DNL Workfront] berechnet, wenn der [!UICONTROL Dauertyp] der Aufgabe „[!UICONTROL Berechnete Arbeit]“ oder „[!UICONTROL Leistungsgesteuert]“ ist.<br>Informationen zur [!UICONTROL Aufgabendauer] finden Sie im Artikel <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Überblick über die [!UICONTROL Dauer] und den [!UICONTROL Dauertyp] einer Aufgabe</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Bei Projekten berechnet [!DNL Workfront] die geplanten Stunden, indem alle geplanten Stunden aus allen Aufgaben im Projekt hinzugefügt werden. </p> </li> 
    </ul> <p><b>TIPP</b></p> <p>Sie können [!UICONTROL geplante Stunden] in Berichten des Typs „[!UICONTROL Projekt]“, „[!UICONTROL Aufgabe]“ oder „[!UICONTROL Problem]“ auch mithilfe des Textmodus anzeigen und auf zusätzliche Felder verweisen. Weitere Informationen finden Sie unter den Feldern „<code>work</code>“, „[!UICONTROL Arbeit]“ und „<code>workRequiredExpression</code>“ in dieser Tabelle. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Arbeitskosten]</td> 
   <td> 
    <p>Bei einer Aufgabe entspricht dies dem Stundensatz der Person oder der Rolle multipliziert mit der Anzahl der Stunden, die der Person oder der Rolle zugewiesen wurden.</p> <p>Bei einem Projekt entspricht dies der Summe der kompletten [!UICONTROL geplanten Arbeitskosten] aller Aufgaben.</p> <p>Ob der Satz der Person oder der Rolle verwendet wird, hängt vom Kostentyp ab, der für die jeweilige Aufgabe ausgewählt wurde. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Nachverfolgen der Kosten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Umsatz]</td> 
   <td> <p>Für Aufgaben und Projekte kann in [!DNL Workfront] ein Wert für den [!UICONTROL geplanten Umsatz] angezeigt werden. Der [!UICONTROL geplante Umsatz] stellt den Geldbetrag dar, der mit den [!UICONTROL geplanten Stunden] der Aufgaben im Projekt verbunden ist. Bei Projekten kann dies auch die [!UICONTROL Festeinnahmen] des Projekts beinhalten. </p> <p>Bei Aufgaben ist dies der Umsatz, der mit den [!UICONTROL geplanten Stunden] der Aufgaben verbunden ist. Die geplanten Stunden aller Aufgaben werden zu den geplanten Stunden des Projekts zusammengefasst und fließen in die Berechnung der [!UICONTROL geplanten Stunden] des Projekts ein. </p> 
   <p>[!DNL Workfront] berechnet den [!UICONTROL geplanten Umsatz] für Aufgaben und Projekte mithilfe der folgenden Formeln:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Der [!UICONTROL geplante Umsatz] des Projekts, der im Bereich „[!UICONTROL Projektdetails]“ und in den Projektberichten angezeigt wird, unterscheidet sich von dem geplanten Umsatz, der im Bericht zur [!UICONTROL Auslastung] angezeigt wird. </p> <p>Der [!UICONTROL geplante Umsatz] im Bereich „[!UICONTROL Projektdetails]“ spiegelt sowohl den Umsatz für die Aufgabe als auch die Festeinnahmen des Projekts wider. Der [!UICONTROL geplante Umsatz] im [!UICONTROL Auslastungsbericht] stellt nur den [!UICONTROL geplanten Umsatz] dar, der mit den Aufgaben im Projekt verknüpft ist. </p> 
     <p><b>BEISPIEL</b></p>  
      <p>Wenn das Projekt 1 Aufgabe mit 10 Stunden umfasst, die einem Berater bzw. einer Beraterin mit einem Stundensatz von 20 € zugewiesen wurde, und das Projekt [!UICONTROL Festeinnahmen] in Höhe von 100 € aufweist, weist der Bericht zur [!UICONTROL Auslastung] 200 € als [!UICONTROL geplanten Umsatz] aus (der mit den Stunden für die Aufgabe verknüpfte [!UICONTROL geplante Umsatz]). Der Abschnitt „[!UICONTROL Projektdetails]“ zeigt 300 € an (der [!UICONTROL geplante Umsatz] aus der Aufgabe und den Festeinnahmen für das Projekt). </p> 
    <p>Informationen zur Umsatznachverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Überblick über Abrechnung und Umsatz</a>. </p> 
    <p>Informationen zu den Berechnungen für den [!UICONTROL geplanten Umsatz] im [!UICONTROL Auslastungsbericht] finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Anzeigen von Informationen zur Ressourcenauslastung</a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Risikokosten]</td> 
   <td> <p>Die Summe der [!UICONTROL potenziellen Kosten] aller Risiken des Projekts unter Berücksichtigung ihrer Eintrittswahrscheinlichkeit. Dieser Betrag ist in den [!UICONTROL geplanten Kosten] des Projekts nicht enthalten.</p> <p>Die [!UICONTROL geplanten Risikokosten] eines Projekts werden nach folgender Formel berechnet:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portalprofil]</td> 
   <td>Eine von dem oder der Admin definierte Sammlung von Registerkarten und Abschnitten, die in [!DNL Workfront] angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portalabschnitt]</td> 
   <td>Eine Komponente einer Registerkarte in einem Dashboard oder auf einer Portalseite. Normalerweise ein einzelner Bericht, ein Diagramm, ein Kalender oder eine Liste wichtiger Informationen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portalregisterkarte]</td> 
   <td>Eine Registerkarte in einem Portal oder Dashboard, die bis zu drei Portalabschnitte enthält.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Eine Sammlung von Projekten mit einheitlichen Merkmalen. Diese Projekte konkurrieren normalerweise um dieselben Ressourcen, Budgets oder Zeitfenster. Sie können Portfolios in Programme aufteilen und die Projekte mit den Programmen verknüpfen, bevor sie einem Portfolio hinzugefügt werden.</p> <p>Weitere Informationen zu Portfolios finden Sie unter <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Grundlegendes zur Portfoliomethodik</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio-Management]</td> 
   <td>Ein Tätigkeitsbereich, der sich auf die Verwaltung einer Sammlung oder damit verbundener Programme und Projekte konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio-Optimizer]</td> 
   <td>Ein Tool von [!DNL Workfront] zur Unterstützung bei der Bewertung und Priorisierung von Projekten in einem Portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio-Besitzer]</td> 
   <td>Personen, die für die Priorisierung und das Budget für ein Portfolio verantwortlich sind.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potenzielle Risikokosten]</td> 
   <td>Dies ist ein Projektfeld, das Sie in Listen und Berichten finden können. Es enthält die potenziellen Kosten für die Risiken, die mit dem Projekt verbunden sind, falls sie auftreten sollten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnung potenzieller Risikokosten</a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Vorgänger]</td> 
   <td> <p>Eine Aufgabe, die vor dem Abschluss einer abhängigen Aufgabe abgeschlossen werden muss. Auch eine Aufgabe, die als [!UICONTROL Abhängigkeit] für eine andere Aufgabe gekennzeichnet ist. Vorgänger ermöglichen es der planenden Person, eine Sequenzabhängigkeitslogik festzulegen, z. B. um eine Aufgabe nach Abschluss einer anderen Aufgabe zu starten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Überblick über Aufgabenvorgänger</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primärfirma]</td> 
   <td>Das Unternehmen, zu dem der Benutzer bzw. die Benutzerin gehört, wie in den Benutzereinstellungen angegeben. Unternehmen können auch mit Projekten verknüpft werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primärer Kontakt]</td> 
   <td><p>Der [!UICONTROL primäre Kontakt] ist der Ersteller bzw. die Erstellerin eines Problems und wird automatisch von [!DNL Workfront] bestimmt, wenn die Person das Problem erstellt. Sie können dieses Feld manuell aktualisieren, wenn Sie über die Berechtigung „[!DNL Manage]“ für das Problem verfügen. Für ein Problem kann es nur einen primären Kontakt geben.</p> 
   <p>Wenn Sie den primären Kontakt ändern, haben die ursprünglich als Primärkontakt angegebenen Benutzenden weiterhin das Zugriffsrecht „[!UICONTROL Verwalten]“ für das Problem.</p>
   <p>Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird die als [!UICONTROL primärer Kontakt] des Problems angegebene Person zu „[!UICONTROL Konvertiertes Problem – Urheberin/Urheber]“ des Projekts oder der Aufgabe. Wenn der [!UICONTROL primäre Kontakt] des Problems nach der Konvertierung des Problems aktualisiert wurde, wird die zum Zeitpunkt der Konvertierung unter „[!UICONTROL Konvertiertes Problem – Urheberin/Urheber]“ genannte Person als [!UICONTROL primärer Kontakt] des Problems beibehalten. Siehe auch „[!UICONTROL Konvertiertes Problem – Urheberin/Urheber]“ in diesem Artikel.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priorität]</td> 
   <td>Ein Wert, der einer Aufgabe, einem Problem oder einem Projekt zugewiesen werden kann, um festzulegen, wie wichtig sie bzw. es ist. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privat]</td> 
   <td>In einer [!UICONTROL Notiz] oder einem [!UICONTROL Dokument] sorgt diese Option dafür, dass dieses Objekt für die meisten Betrachtenden ausgeblendet ist. Bei einer Anfrage-Warteschlange für private Hilfe können nur Benutzende im Projekt-Team über den Bereich „[!UICONTROL Anfragen]“ Probleme an diese Warteschlange (oder dieses Projekt) senden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profil]</td> 
   <td>Alle Informationen zu einem Benutzerkonto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Programm]</td> 
   <td> <p>Eine Untergruppe innerhalb eines Portfolios, in der ähnliche Projekte gruppiert werden können, um einen klar definierten Nutzen zu erzielen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programm-Management]</td> 
   <td>Management von projektübergreifenden Abhängigkeiten, Risiken, Problemen, Anforderungen und Lösungen, um das Programm fehlerfrei zu halten und den definierten Programmnutzen zu erzielen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programm-Inhaber]</td> 
   <td>Der bzw. die Verantwortliche, der bzw. die für die Überwachung und Organisation von Aktivitäten verantwortlich ist, um sicherzustellen, dass die Projektziele mit den Unternehmenszielen übereinstimmen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Fortschritt]</span> </td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Ziel]“ wird hier der Prozentsatz angezeigt, wie nahe ein strategisches Ziel dem Abschluss ist. Der Prozentsatz des Fortschritts wird als Zahl angezeigt. Informationen zu strategischen Zielen finden Sie auch unter „[!UICONTROL Ziel]“ in dieser Tabelle.</p> <p>Dieses Feld ist nur sichtbar, wenn Ihre Organisation [!DNL Workfront] Goals erworben hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Hinzufügen von Projekten zu Zielen in [!DNL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortschrittsstatus]</td> 
   <td> <p>In einem Projekt-, Aufgaben- und Zielbericht zeigt dieses Feld den Fortschrittsstatus von Projekten, Aufgaben oder strategischen Zielen an. Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Überblick über den Fortschrittsstatus eines Projekts</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Überblick über den Fortschrittsstatus einer Aufgabe</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Überblick über den Zielfortschritt und die Bedingung in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Der Bericht des Typs „[!UICONTROL Ziel]“ und der [!UICONTROL Fortschrittsstatus] für das Feld „[!DNL goals]“ sind nur dann sichtbar, wenn Ihre Organisation [!DNL Workfront Goals] erworben hat. Informationen zu strategischen Zielen in [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>“. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Projekt]</td> 
   <td> <p>Ein großer Arbeitsaufwand, der innerhalb eines bestimmten Zeitrahmens abgeschlossen werden muss und für den ein bestimmtes Budget und eine bestimmte Anzahl von Ressourcen eingesetzt werden muss. Damit es überschaubar wird, unterteilen Sie das Projekt in eine Reihe von Aufgaben. Das Abschließen aller Aufgaben führt zum Abschluss des Projekts. Informationen zur Planung eines Projekts finden Sie unter <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Planen eines Projekts – Überblick</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Stunden für Projekt-Arbeitsauftrag]</td> 
   <td> <p>In einem Bericht des Typs „[!UICONTROL Aufgabengebiet der Initiative]“ wird die Anzahl der [!UICONTROL geplanten Stunden] angezeigt, die einem Aufgabengebiet zugeordnet sind, das Aufgaben oder Problemen im Projekt zugewiesen wurde. Dieses Feld und der Berichtstyp „[!UICONTROL Aufgabengebiet der Initiative]“ werden in Ihrer Instanz von [!DNL Workfront] nur dann angezeigt, wenn Ihr Unternehmen eine Lizenz für den [!DNL Workfront Scenario Planner] erworben hat. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektdetails]</td> 
   <td>Die Details des aktuellen Status eines Projekts.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Projektkosten]</td> 
   <td> <p> Dies sind die [!UICONTROL budgetierten Kosten] eines Projekts, wie sie in Listen und Berichten angezeigt werden.</p><p>Siehe auch „[!UICONTROL Budgetierte Kosten]“ in diesem Artikel.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Projekt-Management]</td> 
   <td>Eine Reihe von Richtlinien, die die Schwellenwerte für die Projekterstellung, -kategorisierung und -benennung steuern.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Projekt-Overhead]</td> 
   <td>In einem Bericht des Typs „[!UICONTROL Stunde]“ ist dieses Feld für Finanzinformationen reserviert, die sich auf die Stunden beziehen, die mit dem Stundentyp „[!UICONTROL Projektzeit]“ erfasst wurden. Projekte können über eigene Abrechnungssätze verfügen. Wenn eine Stunde direkt für ein Projekt erfasst wird, werden diese Sätze in Berechnungen verwendet. Basierend auf den Projekteinstellungen können Projekte auch verschiedene Währungen haben und es kann eine Währungsumrechnung für diese Stunden geben. Das Objekt „[!UICONTROL Projekt-Overhead]“ ermöglicht es [!DNL Workfront], diese Informationen abzurufen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektbesitzer]</td> 
   <td>Die Person, die für die Verwaltung von Umfang, Timeline und Arbeitsaufträgen eines Projekts verantwortlich ist. Die standardmäßige genehmigende Person für Änderungsaufträge, finanzielle Änderungen und Arbeitsergebnisse.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektplanung]</td> 
   <td>Prozesse zum Entwickeln und Verwalten des Projektplans.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektsponsor]</td> 
   <td>Ein spezielles Profil für Verantwortliche, auf das sich alle Benutzenden beziehen sollten. In [!DNL Workfront] werden diese als [!UICONTROL Zugriffsebenen] bezeichnet</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt-Teams]</td> 
   <td> <p>Die einem Projekt zugewiesene Sammlung von Benutzenden oder Rollen</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Überblick über Projekt-Teams</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektnachverfolgung]</td> 
   <td>Die Daten, mit denen Status und Umfang eines Projekts gemessen werden</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projiziert]</td> 
   <td> <p>Ein geschätzter Zeitstempel, der angibt, wann die Arbeit abgeschlossen wird, basierend auf den geplanten Stunden und dem abgeschlossenen Prozentsatz einer Aufgabe, eines Problems oder Projekts.</p> <p>Dies bezieht sich auf Termine oder die [!UICONTROL Dauer] von Aufgaben, Problemen oder Projekten. Normalerweise kennzeichnet es Daten und Zeiträume, die dem Zyklus der Arbeitselemente eher entsprechen, nachdem einige Arbeiten bereits abgeschlossen wurden oder einige Zeit vergangen ist. </p> <p>Beispielsweise wird unter „[!UICONTROL Voraussichtliches Abschlussdatum]“ für eine Aufgabe das Datum angegeben, an dem [!DNL Workfront] den Abschluss einer Aufgabe voraussichtlich erwartet, basierend auf dem bisherigen Arbeitsaufwand, der Anzahl der zugewiesenen Personen und der seit dem Startdatum verstrichenen Zeit.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugfrist]</td> 
   <td> <p>In Berichten, die das Objekt „[!UICONTROL Dokumentversion]“ enthalten (z. B. ein Bericht des Typs „[!UICONTROL Dokumentversion]“ oder ein Bericht des Typs „[!UICONTROL Korrekturabzug-Genehmigung]“), zeigt dieses Feld den Wochentag, das Datum, die Tageszeit und das Jahr der Korrekturabzugfrist an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzug-Entscheidung]</td> 
   <td> <p>In Berichten, die das Objekt „[!UICONTROL Dokumentversion]“ enthalten (z. B. ein Bericht des Typs „[!UICONTROL Dokumentversion]“ oder ein Bericht des Typs „[!UICONTROL Korrekturabzug-Genehmigung]“), zeigt dieses Feld den Entscheidungsstatus des Korrekturabzugs an (ausstehend, Änderungen erforderlich oder genehmigt)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name des Korrekturabzugs]</td> 
   <td> <p>In Berichten, die das Objekt „[!UICONTROL Dokumentversion]“ enthalten (z. B. ein Bericht des Typs „[!UICONTROL Dokumentversion]“ oder ein Bericht des Typs „[!UICONTROL Korrekturabzug-Genehmigung]“), zeigt dieses Feld den Namen des Korrekturabzugs an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugseiten]</td> 
   <td> <p>In Berichten, die das Objekt „[!UICONTROL Dokumentversion]“ enthalten (z. B. ein Bericht des Typs „[!UICONTROL Dokumentversion]“ oder ein Bericht des Typs „[!UICONTROL Korrekturabzug-Genehmigung]“), zeigt dieses Feld die Anzahl der im Korrekturabzug enthaltenen Seiten an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugverlauf]</td> 
   <td> <p>In Berichten, die das Objekt „[!UICONTROL Dokumentversion]“ enthalten (z. B. ein Bericht des Typs „[!UICONTROL Dokumentversion]“ oder ein Bericht des Typs „[!UICONTROL Korrekturabzug-Genehmigung]“), zeigt dieses Feld den Fortschrittsstatus des Korrekturabzugs an ([!UICONTROL Gesendet], [!UICONTROL Geöffnet], [!UICONTROL Kommentiert], [!UICONTROL Entscheidung getroffen]).</p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Überblick über den Korrekturabzugverlauf</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Überblick über den Fortschritt und den Status eines Korrekturabzugs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Ein Überprüfungsprozess, bei dem ein oder mehrere Benutzende Inhalte kennzeichnen und kommentieren, die in einem Bild, einem Textdokument, einem Video oder interaktiven Web-Inhalten geändert werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Öffentlich]</td> 
   <td>In einer [!UICONTROL Notiz] oder einem [!UICONTROL Dokument] macht diese Option dieses Objekt anderen Benutzenden oder sogar Personen außerhalb von [!DNL Workfront] zugänglich. Für eine [!UICONTROL Hilfeanfrage-Warteschlange] bedeutet „[!UICONTROL Öffentlich]“, dass alle Benutzenden, die Probleme an ein Projekt senden können, Probleme über den Bereich „[!UICONTROL Anfragen]“ senden können.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualität]</td> 
   <td>Die Wahrnehmung der Arbeitsqualität innerhalb der Organisation.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlange]</td> 
   <td>Wird auch als Helpdesk-Warteschlange oder [!UICONTROL Hilfeanfrage-Warteschlange] bezeichnet. Dies ist ein Projekt, das im Bereich „[!UICONTROL Anfragen]“ veröffentlicht wurde, damit Benutzende Probleme an das Projekt senden können. Normalerweise werden Warteschlangen für bestimmte Themen wie [!UICONTROL Fehler], [!UICONTROL Projektanfragen] usw. erstellt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlangeneigenschaften]</td> 
   <td>Diese Einstellungen definieren Problemübermittlungsregeln für ein Projekt, das im Bereich „[!UICONTROL Anfragen]“ veröffentlicht wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlangen-Thema]</td> 
   <td> <p>Eine Eigenschaft in einer [!UICONTROL Hilfeanfrage-Warteschlange], mit der Benutzende, die ein Problem übermitteln, ein Thema auswählen können. Für Themen kann Folgendes gelten:</p> 
    <ul> 
     <li>Sie können mit einem Formular für benutzerdefinierte Daten verknüpft sein.</li> 
     <li>Sie können das Problem über den Routing-Regelsatz für das ausgewählte Thema automatisch einem Benutzer bzw. einer Benutzerin, einer Rolle oder einem Team zuweisen.</li> 
     <li>Sie können das Problem über den für das ausgewählte Thema festgelegten Routing-Regelsatz zu einem anderen Projekt oder einer anderen Warteschlange verschieben.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Erstellen von Warteschlangenthemen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rang]</td> 
   <td> <p>In einem Bericht zur [!UICONTROL Zugriffsebene] können Sie manuell einen [!UICONTROL Rang] der [!UICONTROL Zugriffsebene] angeben. Auf diese Weise können Sie als Admin in [!DNL Workfront] den mit den einzelnen Zugriffsebenen verbundenen Komplexitätsgrad visuell erkennen. Beispielsweise können Sie niedrigere Zahlen für komplexere Zugriffsebenen ([!UICONTROL Plan]-Ebene) und höhere Zahlen für weniger komplexe Zugriffsebenen ([!UICONTROL Anforderer]-Ebene) angeben. Sie können die standardmäßigen Zugriffsebenen nicht nach Rang ordnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bereit]</td> 
   <td> <p>Dieses Feld in einem Aufgabenbericht gibt an, ob eine [!UICONTROL Agile]-Aufgabe im Rückstand als „[!UICONTROL Bereit]“ gekennzeichnet wurde. Diese Markierung nur für [!UICONTROL Agile]-Aufgaben, bei denen es sich um Aufgaben handelt, die einem [!UICONTROL Agile]-Team zugewiesen sind. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Eintrag]</td> 
   <td> <p>In Workfront-Planung ist ein Eintrag eine eindeutige Instanz eines Eintragstyps.</p>
<p>Nachdem Sie einem Arbeitsbereich einen Eintragstyp hinzugefügt haben, können Sie damit beginnen, Einträge dieses Typs auf der Seite des Eintragstyps hinzuzufügen.</p>
<p>Beispiel: „Kampagne“ kann ein Eintragstyp sein und „Sommerkampagne für EMEA“ ist ein Eintrag des Eintragstyps „Kampagne“.</p>
<p>Weitere Informationen zum Erstellen von Einträgen finden Sie unter <a href="/help/quicksilver/planning/records/create-records.md">Erstellen von Einträgen</a>. </p> <p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Eintragstyp]</td> 
   <td> <p>Der Objekttyp von Workfront-Planung.</p>
<p>Anders als bei Workfront, wo die Objekttypen vordefiniert sind, können Sie in Workfront-Planung eigene Objekttypen erstellen. Objekttypen in Workfront-Planung werden als Eintragstypen bezeichnet.</p>
<p>In Workfront sind beispielsweise die Objekttypen „Programm“, „Portfolio“, „Projekt“, „Aufgabe“ oder „Problem“ bereits erstellt.</p>
<p>In Workfront-Planung können Sie beliebige Eintragstypen erstellen, die den Workflows Ihrer Organisation entsprechen. Später können Sie definieren, wie die Eintragstypen miteinander in Beziehung stehen oder Abhängigkeiten bilden.</p> Weitere Informationen zum Erstellen von Eintragstypen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-record-types.md">Erstellen von Eintragstypen</a>. </p> <p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Intervallfrequenz]</td> 
   <td> <p>Ein Feld, das im Feld „[!UICONTROL Aufgabendetails]“ oder „[!UICONTROL Aufgabe bearbeiten]“ eines übergeordneten Elements wiederkehrender Aufgaben angezeigt wird. Dies ist die Häufigkeit, mit der die Aufgaben in der Intervall vorkommen. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Erstellen wiederkehrender Aufgaben</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Referenznummer]</td> 
   <td> <p>Projekte, Aufgaben und Probleme werden beim Erstellen automatisch mit einer eindeutigen Referenznummer verknüpft. Sie können die [!UICONTROL Referenznummer] auf der Seite „[!UICONTROL Details]“ der Projekte, Aufgaben oder Probleme oder in einer Liste oder in einem Bericht einsehen. </p> <p><b>TIPP</b><p><br>Sie können Referenznummern verwenden, wenn zwei Elemente denselben Namen haben, da Referenznummern immer eindeutig sind. </p> <p>[!DNL Workfront] generiert automatisch fortlaufende Referenznummern auf Systemebene. Jedes Projekt, jede Aufgabe oder jedes Problem erhält die nächste verfügbare fortlaufende Nummer. <br></p> <p>Wenn beispielsweise Person A eine Aufgabe erstellt, weist [!DNL Workfront] der Aufgabe möglicherweise automatisch die Referenznummer 100 zu. Wenn Person B unmittelbar danach ein Problem erstellt, weist [!DNL Workfront] dem Problem die Referenznummer 101 zu. Referenznummern können nicht manuell bearbeitet werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ablehnungsproblem]</td> 
   <td>In einem Projekt- oder Aufgabenbericht ist dies das Problem, das erstellt wird, wenn die Genehmigung für das Projekt oder die Aufgabe abgelehnt wird. Informationen zu Ablehnungsproblemen finden Sie im Artikel <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>. </td> 
  </tr>

<tr>
  <td>Beziehungstypen</td>
  <td><p>Workfront-Objekte werden immer über einen der folgenden Beziehungstypen miteinander verbunden:</p>

<ul><li> <b>Eins-zu-viele</b>: In dieser Beziehung kann ein Objekt mit mehreren anderen Objekten unterschiedlichen Typs verbunden werden. Beispielsweise kann ein Projekt mehrere Aufgaben haben. Die Beziehung zwischen Projekt und Aufgaben ist eine Eins-zu-viele-Beziehung. Sie können diese Beziehung nicht in einem Bericht über die Standardschnittstelle anzeigen. Sie müssen Berichte im Textmodus verwenden, um Eins-zu-viele-Beziehungen anzuzeigen.</li>
  <li><b>Eins-zu-eins</b>: In dieser Beziehung kann ein Objekt nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise kann ein Projekt nur eine Gruppe aufweisen. Die Beziehung zwischen Projekt und Gruppe ist eine Eins-zu-eins-Beziehung. Sie können Eins-zu-eins-Beziehungen zwischen Objekten in einem Standardbericht anzeigen.</li>
  <li><b>Viele-zu-eins</b>: In dieser Beziehung können mehrere Objekte nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise können mehrere Aufgaben mit demselben Projekt verbunden werden. Die Beziehung zwischen Aufgaben und Projekt ist eine Viele-zu-eins-Beziehung. In einem Standardbericht können Sie Viele-zu-eins-Beziehungen zwischen Objekten anzeigen. </li>
  <li><b>Viele-zu-viele</b>: In dieser Beziehung können mehrere Objekte desselben Typs mit mehreren Objekten eines anderen Typs verbunden werden. Beispielsweise können mehrere Benutzende zu mehreren anderen Teams gehören und die Teams können zu mehreren Benutzenden gehören. Sie können diese Beziehung nicht in einem Bericht über die Standardschnittstelle anzeigen. Sie müssen die Berichte im Textmodus verwenden, um Viele-zu-viele-Beziehungen anzuzeigen. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Restrisikokosten]</td> 
   <td> <p>Ein Projektfeld, das die Differenz zwischen den [!UICONTROL geplanten Risikokosten] eines Projekts und der Summe aller [!UICONTROL tatsächlichen Kosten] aller Risiken im Projekt anzeigt. </p> <p>Die [!UICONTROL verbleibenden Risikokosten] für ein Projekt werden mithilfe der folgenden Formel berechnet:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Neuplanung]</td> 
   <td>Ändern der Termine eines Projekts zur Behebung oder Lösung von Problemen. Beispielsweise müsste ein Projekt, das mehrere Monate zurückgestellt wurde, neu geplant werden, um genaue Termine widerzuspiegeln. Hierbei handelt es sich um einen manuellen Vorgang, bei dem Sie entweder die Termine des Projekts oder die der Aufgaben anpassen. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bericht]</td> 
   <td>Ein Diagramm oder eine Tabelle mit Informationen zu einem bestimmten Objekt in [!DNL Workfront] und seinen zugehörigen Attributen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Anfrage]</td> 
   <td> <p>Eine Art von Problem, das in einer einzigen zentralisierten Warteschlange triagiert wird und nicht mit einem laufenden Arbeitsaufwand in Zusammenhang steht.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Anfrage-Warteschlange]</td> 
   <td>Der Rückstand an Problemen, der von einem Traffic- und Triage-Prozess verwaltet wird.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anfragegeschwindigkeit]</td> 
   <td>Gesamtarbeitszykluszeit für die Aufnahme und den Abschluss einer Anfrage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anfragende Person]</td> 
   <td>In der Regel ein Lizenztyp. Benutzende mit Lizenz für anfragende Personen können Anfragen für neue Arbeiten im System senden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reservierte Zeit]</td> 
   <td>Tage, die als persönliche Zeit einer Person angegeben werden, was bedeutet, dass die Person nicht für Arbeit zur Verfügung steht. Siehe „[!UICONTROL Arbeitsfreie Tage]“.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Problem zu verweisen, das das Problem löst. </p> <p>Informationen zum Anzeigen problemlösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen von Informationen zu lösbaren und problemlösenden Objekten in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Überblick über problemlösende und lösbare Objekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Projekt zu verweisen, das das Problem löst. </p> <p>Informationen zum Anzeigen problemlösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen von Informationen zu lösbaren und problemlösenden Objekten in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Überblick über problemlösende und lösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabe lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf die Aufgabe zu verweisen, die das Problem löst. </p> <p>Informationen zum Anzeigen problemlösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen von Informationen zu lösbaren und problemlösenden Objekten in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Überblick über problemlösende und lösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressource]</td> 
   <td>Benutzende oder Rollen, die in [!DNL Workfront] vorhanden und Projekten, Teams, Aufgaben und Problemen zugewiesen sind. Sie sind für den Abschluss der Arbeiten im Zusammenhang mit Projekten, Aufgaben oder Problemen verantwortlich. </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in  Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr>
  -->
  <tr> 
   <td>[!UICONTROL Ressourcen-Management]</td> 
   <td> <p>[!UICONTROL Ressourcen-Management] ist ein Tool-Set für Unternehmen, mit dem Sie die Nutzung Ihrer Ressourcen auf der Grundlage ihrer Verfügbarkeit genau vorhersagen können, sodass die erforderlichen Arbeiten termingerecht und im Budget abgeschlossen werden. </p> <p>Mit Tools für das Ressourcen-Management können Sie die langfristige Kapazität und den kurzfristigen Planungsbedarf für Ihre Ressourcen planen. </p> <p>Informationen zum Ressourcen-Management in [!DNL Workfront] finden Sie unter <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit dem Ressourcen-Management</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcen-Manager-IDs]</td> 
   <td><p>In einem Projektbericht können Sie diese Option beim Erstellen eines Filters verwenden, um einen bestimmten Ressourcen-Manager bzw. eine bestimmte Ressourcen-Managerin zu finden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcen-Manager]</td> 
   <td> <p>In einem Projektbericht oder einer Listenansicht ist dies ein Informationsfeld, das Benutzende anzeigt, die für die Durchführung von Ressourcen-Management-Aktivitäten für das Projekt vorgesehen sind.  Wenn Sie „[!UICONTROL Ressourcen-Manager]“ in einem Bericht verwenden, wird eine Liste der Ressourcen-Manager und Ressourcen-Managerinnen angezeigt, wobei die einzelnen Ressourcen-Manager und Ressourcen-Managerinnen des Projekts durch Kommas voneinander getrennt sind. Sie können bis zu 30 Ressourcen-Manager oder Ressourcen-Managerinnen für ein bestimmtes Projekt bestimmen.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Bestimmen des Ressourcen-Managements für ein Projekt oder eine Vorlage</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Ressourcenplaner für budgetierte Stunden] </td> 
   <td>Die budgetierten Stunden für das Projekt und die damit verbundenen Ressourcen im [!UICONTROL Ressourcenplaner]. Siehe auch „[!UICONTROL Budgetierte Stunden]“ in diesem Artikel. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Ressourcenplaner] </td> 
   <td>Ein fortschrittliches Tool in [!DNL Workfront], mit dem Sie Ressourcen projektübergreifend, für Aufgabengebiete oder für Benutzende anzeigen und verwalten können. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Überblick über den Ressourcenplaner</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenplaner – budgetierte Lohnkosten]</td> 
   <td> <p>Dies sind die Kosten, die mit den Stunden verknüpft sind, die mithilfe des Ressourcenplaners für die Aufgabengebiete eines Projekts budgetiert wurden. </p> <p>Siehe auch „Budgetierte Lohnkosten“ in diesem Artikel. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Ressourcen-Pools]</td> 
   <td> <p>Ressourcen-Pools sind Sammlungen von Benutzenden, die mit einem Projekt verknüpft werden können. Die Benutzenden im selben Ressourcen-Pool gehören normalerweise derselben Abteilung an, verfügen über ähnliche oder komplementäre Fähigkeiten oder werden aus demselben Budget finanziert. Sie können mehrere Ressourcen-Pools mit einem Projekt oder einer Person verknüpfen. Ein Ressourcen-Pool kann einem Projekt exklusiv zugewiesen oder von mehreren Projekten gemeinsam genutzt werden.</p> 
   <p>Weitere Informationen zu Ressourcen-Pools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Überblick über Ressourcen-Pools</a>.</p> 
   <p>In Projektberichten handelt es sich bei Ressourcen-Pools um alle Pools, die mit einem Projekt verknüpft sind. Dieses Objekt kann nicht in einer Gruppierung verwendet werden.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenauslastung]</td> 
   <td>Ein Bericht, der die Anzahl der in einem bestimmten Zeitraum verfügbaren Stunden und die für jede Person geplante Anzahl der Stunden anzeigt. Dies wird auch in die [!UICONTROL durchschnittlichen Stunden pro Tag] und einen Zuordnungsprozentsatz einberechnet.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Ergebnis]</td> 
   <td>In [!DNL Workfront Goals] ist ein Ergebnis ein Fortschrittsindikator für ein Ziel. Dabei kann es sich um eine Zahl, einen Prozentwert oder einen Währungsbetrag handeln, den Sie manuell aktualisieren. Es ist nicht möglich, Ergebnisse in einem Bericht anzuzeigen und über die [!DNL Workfront]-API darauf zuzugreifen. Informationen zu Aktivitäten finden Sie unter <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Umsatz]</td> 
   <td>Ein fakturierbarer Betrag für die Aufgabe oder das Projekt. Der Betrag kann stündlich, fest oder eine Kombination aus beidem sein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Umsatzart]</td> 
   <td>Die Umsatzart bestimmt, wie der Aufgabe Einnahmen zufließen. Einige Beispiele sind „[!UICONTROL Festgelegt pro Stunde]“, „[!UICONTROL Stundensatz nach Rolle]“ und „[!UICONTROL Stundensatz nach Rolle mit Begrenzung]“. Informationen zur Umsatznachverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Überblick über Abrechnung und Umsatz</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prüfer]</td> 
   <td>In der Regel ein Lizenztyp. Benutzende mit einer [!UICONTROL Prüfer]-Lizenz können Arbeitselemente im System überprüfen und genehmigen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risiko]</td> 
   <td> <p>Dies kann sich auf die folgenden Konzepte in [!DNL Workfront] beziehen:</p> 
    <ul> 
     <li> <p>Ein Feld in einem Projekt, das anzeigt, wie riskant ein Projekt sein kann. Sie können die Ausführung Ihrer Projekte nach der Risikostufe priorisieren. Projekte können die folgenden Risikostufen aufweisen:</p> <p>– [!UICONTROL Sehr niedrig]</p> <p>– [!UICONTROL Niedrig]</p> <p>– [!UICONTROL Mittel]</p> <p>– [!UICONTROL Hoch]</p> <p>– [!UICONTROL Sehr hoch]</p> <p>Die von Ihnen für ein Projekt angegebenen Risikostufen können nicht angepasst werden. </p> <p> Informationen zum Aktualisieren des Risikos eines Projekts finden Sie im Abschnitt „Projekteinstellungen“ des Artikels <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Bearbeiten von Projekten</a>. Sie können das Risikofeld eines Projekts in Berichten anzeigen. </p> </li> 
     <li> <p>Ein Ereignis, das während der Laufzeit eines Projekts auftreten kann und potenzielle Auswirkungen auf die Kosten, den Umfang oder den Zeitplan des Projekts angibt. Sie definieren potenzielle Risiken für ein Projekt und verknüpfen die Wahrscheinlichkeit ihres Auftretens oder die Kosten, während Sie den Business-Case des Projekts erstellen. Informationen zum Hinzufügen von Risiken zum Business-Case des Projekts finden Sie unter „Erstellen und Bearbeiten von Risiken für Projekte“. </p> <p>Sie können die im [!UICONTROL Business-Case] definierten Risiken nicht in Berichten anzeigen. Sie können nur verschiedene Arten von Risikokosten in Berichten und Listen anzeigen. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risikokosten]</td> 
   <td> <p>Die mit den Risiken eines Projekts verbundenen Kosten. Im Folgenden finden Sie Risikokosten im Zusammenhang mit Projekten, die Sie in Berichten anzeigen können:</p> 
    <ul> 
     <li> <p>[!UICONTROL Tatsächliche Kosten]: Ein Feld für ein Risiko, das die tatsächlichen Kosten für das eingetretene Risiko anzeigt. Zusätzlich zu Berichten und Listen können Sie es beim Bearbeiten oder Erstellen eines Risikos im Feld „[!UICONTROL Risiko bearbeiten]“ suchen. </p> <p>Informationen zu Projekt-, Aufgaben- oder Problemkosten finden Sie unter „[!UICONTROL Tatsächliche Kosten]“ in diesem Artikel. </p> </li> 
     <li> <p>[!UICONTROL Geplante Risikokosten]: Ein Feld im Projekt, das die Summe aller [!UICONTROL potenziellen Risikokosten] für das Projekt anzeigt. Siehe auch „[!UICONTROL Geplante Risikokosten]“ in diesem Artikel. </p> <p>Informationen zu potenziellen Risikokosten finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnen der potenziellen Risikokosten</a>. </p> </li> 
     <li> <p>[!UICONTROL Verbleibende Risikokosten]: Ein Feld im Projekt, das die Differenz zwischen der Summe der [!UICONTROL tatsächlichen Kosten] aller Risiken und den [!UICONTROL geplanten Risikokosten] anzeigt. Siehe auch „Verbleibende Risikokosten“ in diesem Artikel. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risiko-Management]</td> 
   <td>Prozesse zur Identifizierung, Minderung und Überwachung von Risiken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rolle]</td> 
   <td>Siehe „[!UICONTROL Aufgabengebiet]“ in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Automatisches Zuweisen oder Verschieben eines Problems, normalerweise aufgrund eines Warteschlangen-Themas oder als Standardroute (Routing-Regel) für die Warteschlange.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing-Regel]</td> 
   <td>Eine Einstellung für Projekte und Warteschlangen-Themen, mit der ein Problem automatisch einem Benutzer bzw. einer Benutzerin, einer Rolle oder einem Team zugewiesen oder in ein anderes Projekt oder Warteschlangenthema verschoben wird. Routing-Regeln werden im Allgemeinen mit Warteschlangen für Hilfeanfragen verwendet, um eingehende Probleme automatisch zuzuweisen.</td> 
  </tr> 
 </tbody> 
</table>

## S–U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gespeicherte Suche]</td> 
   <td>Eine Suche, für die die Suchkriterien gespeichert wurden. Gespeicherte Suchen erleichtern die erneute Ausführung derselben Suchvorgänge, ohne dass die Suchkriterien erneut eingegeben werden müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Szenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Ein Szenario besteht aus einer Reihe von Schritten (Modulen), die angeben, wie Daten zwischen Anwendungen/Diensten übertragen und umgewandelt werden sollen.</p> <p>Informationen zu Szenarien in [!DNL Workfront Fusion] finden Sie unter „Überblick über <a href="https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion]-Szenarien</a>“.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Szenario] (im [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Im [!DNL Scenario Planner] ist ein Szenario eine Kopie eines Plans. </p> <p>Der [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick über den [!DNL Scenario Planner]</a>. </p> <p>Informationen zum Erstellen von Szenarien finden Sie unter <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Erstellen und Vergleichen von Planszenarien im [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitplan]</td> 
   <td>Der wöchentliche Arbeitszeitplan, einschließlich Arbeitszeiten, kombiniert mit arbeitsfreien Tagen (z. B. Feiertage) und Ausnahmetagen (z. B. Samstag als Arbeitstag). Sie können Zeitpläne mit Projekten und Benutzenden verknüpfen.</td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Zeitplan-Leistungsindex (Schedule Performance Index, SPI)]</td> 
   <td><p>Der [!UICONTROL Zeitplan-Leistungsindex (Schedule Performance Index, SPI)] beschreibt die Beziehung zwischen dem geplanten Zeitplan und dem tatsächlichen Zeitplan. Adobe Workfront berechnet den SPI auf Projekt- und Aufgabenebene. Das Projekt-Management überprüft diese Metrik, um festzustellen, ob Aufgaben oder Projekte derzeit vor oder hinter dem Zeitplan liegen.</p>
  <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-spi.md">Berechnen des Zeitplan-Leistungsindex (Schedule Performance Index, SPI)</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitplanausnahme]</td> 
   <td>Wird auch als „[!UICONTROL Geänderte Schicht]“ bezeichnet. Geplante Tage im Gegensatz zu den regulären Wochenarbeitszeiten, gemäß der Definition im Zeitplan. Beispielsweise wäre ein Samstag, an dem gearbeitet werden soll, obwohl der Zeitplan so eingerichtet ist, dass nur von Montag bis Freitag gearbeitet wird, eine [!UICONTROL Zeitplanausnahme].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Bericht]</td> 
   <td> <p>Wenn Sie einen Bericht aus Berichten erstellen, können Sie Informationen zu den Zeitplänen des Berichts anzeigen, wenn der Bericht über das Feld „[!UICONTROL Geplanter Bericht]“ für die Bereitstellung eingeplant ist. Dieses Feld zeigt in einer Aufzählungsliste mehrere Werte an, einen für jeden Zeitplan jedes Berichts. Weitere Informationen zur Planung von Berichten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Überblick über den Berichtsversand</a>.</p> <p>Da dieses Feld mehrere Werte aufweist, kann es nicht in einer Gruppierung verwendet werden. Der Zugriff ist nur über einen Filter oder eine Ansicht möglich. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Umfangsänderung]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll], das, sofern es aktiv ist, bei jeder Änderung am Umfang eines Projekts oder einer Aufgabe eine Notiz erzeugt, z. B. wenn eine [!UICONTROL Dauer einer Aufgabe] oder die [!UICONTROL Vorgänger] geändert werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschnitt]</td> 
   <td>Ein Bereich auf dem Bildschirm mit einer eigenen Kopfzeile, der erstellt wurde, um die benutzerdefinierten Daten für Anzeigezwecke zu organisieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschnittsumbruch]</td> 
   <td>Eine Lücke oder ein Rahmen zwischen Abschnitten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sicherheit]</td> 
   <td>Die Einstellungen, die es einem Benutzer bzw. einer Benutzerin ermöglichen, mit bestimmten Objekten im System zu interagieren und nicht mit anderen. Siehe auch „[!UICONTROL Zugriffsebenen]“ in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Der Bereich, in dem Admins Systemkonfigurationen und -einstellungen einrichten können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schweregrad]</td> 
   <td> <p>Eine Angabe unter „[!UICONTROL Schweregrad]“ ist ein Hinweis darauf, wie wahrscheinlich es ist, dass ein Element die Fertigstellung der Arbeit beeinträchtigt. Beispielsweise kann ein Problem mit hohem [!UICONTROL Schweregrad] den Abschluss einer Aufgabe vollständig blockieren, aber ein Problem mit niedrigem [!UICONTROL Schweregrad] hat möglicherweise nur geringe Auswirkungen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref">Aktualisieren des Problemschweregrads</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schweregrade]</td> 
   <td>Siehe „[!UICONTROL Schweregrad]“ in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Freigabe]</td> 
   <td>Die Aktion, bei der es anderen Benutzenden erlaubt wird, ein bestimmtes Element in [!DNL Workfront] anzuzeigen oder zu bearbeiten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack-Datum]</td> 
   <td>In einer Aufgabenansicht oder einem Bericht handelt es sich beim [!UICONTROL Slack-Datum] um das genaue Datum, an dem sich eine Aufgabe definitiv auf das [!UICONTROL Abschlussdatum] des Projekts auswirken könnte. Informationen zum [!UICONTROL Slack-Datum] einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Überblick über das Slack-Datum der Aufgabe</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intelligente Arbeitsaufträge]</td> 
   <td> <p>Beim Zuweisen von Aufgaben oder Problemen an Benutzende gibt [!DNL Workfront] Empfehlungen ([!UICONTROL intelligente Arbeitsaufträge]) dazu, welche Benutzenden für die Durchführung der Arbeit am besten geeignet sind. Diese Empfehlungen beziehen sich auf die Zeit, die ihnen für die Fertigstellung zur Verfügung steht, und auf ihre Beziehung zum Projekt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Überblick über intelligente Arbeitsaufträge</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quelle]</td> 
   <td> <p>Gibt das übergeordnete Objekt eines anderen Objekts an. Beispiel: Bei einem an eine Aufgabe angefügten Dokument ist der Name der Aufgabe im Feld „[!UICONTROL Quelle]“ eines Berichts oder einer Ansicht zu einem [!UICONTROL Dokument] angegeben. Bei einem Problem, das unter einem Projekt erfasst ist, ist der Name des Projekts im Feld „[!UICONTROL Quelle]“ eines Problemberichts oder einer Ansicht angegeben. </p> 
   <p>Die folgenden Berichte enthalten die Spalte „Quelle“, in der Sie Informationen zum übergeordneten Objekt anzeigen können:</p>
  <ul><li>Berichte zu Problemen</li>
    <li>Berichte zu Stunden</li>
    <li>Berichte zu Dokumenten </li>
    </ul>
   <p>Wenn Benutzende keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, bleibt die Spalte „Quelle“ des Berichts leer, selbst wenn der Bericht so konfiguriert ist, dass er mit den Zugriffsrechten eines anderen Benutzers bzw. einer anderen Benutzerin angezeigt oder bereitgestellt wird. </p>
   <p> Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, empfehlen wir, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der der Name des übergeordneten Objekts angezeigt werden kann. </p>
    <p>Sie können beispielsweise eines der folgenden Elemente zu einem Bericht hinzufügen, in dem es die Spalte „Quelle“ gibt: </p>
    <ul><li>Die Spalten „Projektname“, „Aufgabenname“ oder „Problemname“ für ein Dokument oder einen Stundenbericht.</li>
    <li>Die Spalten „Projektname“ oder „Aufgabenname“ für einen Problembericht. </li> </ul>
    Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Ausführen und Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers oder einer anderen Benutzerin</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p>Das Datum, an dem die Arbeit an einem Element beginnen soll. In [!DNL Workfront] gibt es mehrere Starttermine: </p> 
    <ul> 
     <li>[!UICONTROL Geplant]</li> 
     <li>[!UICONTROL Tatsächlich]</li> 
     <li>[!UICONTROL Projiziert] </li> 
    </ul> <p>In einem [!UICONTROL Tarifbericht] ist dies das Datum, an dem ein neuer Abrechnungssatz für ein Aufgabengebiet auf Projektebene beginnt. Die mit dem Projekt verknüpften Stunden nach diesem Datum werden mit diesem Abrechnungssatz multipliziert, um den Projektumsatz zu berechnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Ein Indikator, der eine Position eines Arbeitselements im Arbeitsablauf oder eines strategischen Ziels signalisiert.</p> <p>Bei Projekten ist der [!UICONTROL Status] eine Einstellung des Projekts, die angibt, ob das Projekt einen der folgenden Status aufweist:</p> 
    <ul> 
     <li>[!UICONTROL Aktuell]</li> 
     <li>[!UICONTROL Zurückgestellt] </li> 
     <li>[!UICONTROL Abgeschlossen] </li> 
     <li>[!UICONTROL Eingestellt]</li> 
    </ul> <p>Weitere Informationen zum Projektstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Zugriff auf die Liste der Systemprojektstatus</a>.</p>
    <p>Bei Aufgaben ist der [!UICONTROL Status] eine Einstellung für die Aufgabe, der angibt, ob die Aufgabe einen der folgenden Status aufweist:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL Wird ausgeführt]</li> 
     <li>[!UICONTROL Abgeschlossen]</li> 
    </ul> <p>Weitere Informationen zum Aufgabenstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Zugriff auf die Liste der Systemaufgabenstatus</a></p> <p>Bei Problemen ist der [!UICONTROL Status] eine Einstellung zum Problem, die angibt, ob dieses Problem einen der folgenden Status aufweist:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL Wird ausgeführt]</li> 
     <li>[!UICONTROL Warten auf Feedback]</li> 
     <li>[!UICONTROL Zurückgestellt]</li> 
     <li>[!UICONTROL Gelöst]</li> 
     <li>[!UICONTROL Lässt sich nicht lösen]</li> 
     <li>[!UICONTROL Kann nicht duplizieren]</li> 
     <li>[!UICONTROL Abschluss bestätigt]</li> 
     <li>[!UICONTROL Erneut geöffnet]</li> 
    </ul> <p>Weitere Informationen zum Problemstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemproblemstatus</a>.</p> 
    <p>Bei strategischen Zielen ist der [!UICONTROL Status] eine Einstellung für das Ziel, die angibt, ob das Ziel einen der folgenden Status aufweist:</p> 
     <ul> 
      <li>[!UICONTROL Aktiv]</li> 
      <li>[!UICONTROL Entwurf]</li> 
      <li>[!UICONTROL Inaktiv]</li> 
      <li>[!UICONTROL Geschlossen]</li> 
     </ul> 
     <p>Weitere Informationen zu strategischen Zielen finden Sie auch unter „[!UICONTROL Ziel]“ oder „[!UICONTROL Ziele]“ in diesem Artikel. </p> 
     <p>Bei strategischen Zielen ist dieses Feld nur sichtbar, wenn Ihre Organisation [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter „Überblick über <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals]</a>“. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusänderung]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll]. Eine Notiz wird erzeugt, wenn ein Benutzer bzw. eine Benutzerin den Status des Projekts, der Aufgabe oder des Problems ändert.</td> 
  </tr> 
  <tr> 
   <td>Status-Symbole</td> 
   <td> <p>Sie können das integrierte Feld „[!UICONTROL Status-Symbole]“ als Spalte in Ihren Ansichten hinzufügen, um die Transparenz zu wichtigen Punkten Ihrer Objekte zu verbessern, z. B.:</p> 
    <ul> 
     <li>An ein Objekt sind Dokumente angefügt</li> 
     <li>Ein Objekt ist mit einem Genehmigungsprozess verknüpft</li> 
     <li>Einem Objekt sind zusätzliche Notizen zugeordnet</li> 
     <li>Kosten sind fakturierbar oder erstattungsfähig </li> 
     <li>Eine Aufgabe befindet sich in einem kritischen Pfad</li> 
     <li>Ein Benutzer bzw. eine Benutzerin gehört zu einem Unternehmen, einem Team oder befindet sich in einer anderen Zeitzone </li> 
    </ul> <p>Sie können das Feld „[!UICONTROL Status-Symbole]“ in den Ansichten der folgenden Objekte hinzufügen: </p> 
    <ul> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li> 
     <li>[!UICONTROL Vorlagen]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Benutzende]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Status-Symbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusaktualisierung]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht zeigt dieses Feld die neueste Statusaktualisierung an, die Objektbesitzer und -besitzerinnen im Bereich „[!UICONTROL Aktualisierungen]“ angegeben haben. Für Projekte bedeutet dies, dass Kommentare vom Projektbesitzer bzw. von der Projektbesitzerin abgegeben werden, und für Aufgaben und Probleme bedeutet dies, dass Kommentare von den zugewiesenen Personen abgegeben werden.</p> 
   <p> Kommentare, die beim Aktualisieren des Status eines Objekts erstellt werden, werden nicht in der Spalte [!UICONTROL Statusaktualisierung] angezeigt.</p> <p>Um die Status „[!UICONTROL Neu]“, „[!UICONTROL In Bearbeitung]“ und „[!UICONTROL Abgeschlossen]“ anzuzeigen, verwenden Sie die Spalte „[!UICONTROL Status]“.</p> <p>Weitere Informationen zum Status finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aktualisieren des Aufgabenstatus</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td>Siehe „[!UICONTROL Status]“ in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Ein Diagramm, das den Status von Storys (Aufgaben in der Agile-Methodik) und ihren Fortschritt hin zum Abschluss darstellt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story-Stunden]</td> 
   <td>Eine Metrik zum Messen der Schwierigkeit oder Komplexität einer Story. Agile-Teams können wählen, ob sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story-Punkte]</td> 
   <td>Eine Metrik zum Messen der Schwierigkeit oder Komplexität einer Story. Agile-Teams können wählen, ob sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategisch]</td> 
   <td>Langfristige Arbeit, die die Organisation oder die Funktionsweise der Organisation ändert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategische Ausrichtung]</td> 
   <td>Messen und Ausrichten von Unternehmenszielen über Portfolios und Programme hinweg.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Dieses Objekt wird bei Verwendung der Textmodus-Oberfläche in Berichtsspalten verwendet. </p>
   <p>Mit <code>[!UICONTROL stretch]</code> wird ermittelt, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. Die Breite der Benutzeroberfläche des Arbeitsbereichs beträgt für typische Benutzende etwa 850 Pixel. Das bedeutet, dass eine Ansicht mit vier Spalten (jeweils 150 Pixel) 600 von 850 Pixeln einnimmt. Es gibt 250 zusätzliche Pixel in der Benutzeroberfläche, die zu den Spalten hinzugefügt werden, für die ein Ausdehnungsprozentsatz angegeben ist. </p>
   <p>Die Ausdehnung einer Spalte wird erzwungen, wenn Sie die zusätzliche Code-Zeile <code>[!UICONTROL usewidths=true]</code> für mindestens eine der Spalten in der Ansicht verwenden. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Abonnentinnen und Abonnenten]</td> 
   <td> <p>Benutzende, die Projekte, Aufgaben oder Probleme abonnieren.</p> <p>Wenn Sie dieses Feld in einem Bericht verwenden, wird eine Liste mit Abonnierenden angezeigt, wobei die einzelnen Personen durch Kommas voneinander getrennt sind.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonnieren von Elementen in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übersichtsaufgabe]</td> 
   <td>Siehe „[!UICONTROL Übergeordnete Aufgabe]“ in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unteraufgabe]</td> 
   <td>Eine untergeordnete Aufgabe, die sich unter einer übergeordneten Aufgabe befindet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System-Governance]</td> 
   <td>Ein Satz von Richtlinien, der Änderungen und die Wartung eines Systems steuert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Systemintegration]</td> 
   <td>Der Vorgang der physischen oder funktionalen Verbindung verschiedener Computer-Systeme und Software-Anwendungen, um als ein koordiniertes Ganzes zu fungieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabe]</td> 
   <td> <p>Eine Aktivität, die als Schritt zum Erreichen eines endgültigen Ziels (Abschluss des Projekts) ausgeführt werden muss.</p>

<p>Aufgaben sind kleinere Arbeitseinheiten, die letztendlich ein Projekt abschließen, das eine größere Arbeitseinheit darstellt.</p>
   <p>Aufgaben können niemals unabhängig existieren. Sie sind immer Teil eines Projekts. </p>
   <p>Weitere Informationen zu Aufgaben finden Sie unter <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Überblick über Aufgaben</a>.</p> 
   <p>Informationen zum Erstellen von Aufgaben finden Sie unter <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Erstellen von Aufgaben in einem Projekt</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabenattribut]</td> 
   <td>Andere Felder oder Objekte, die mit einer Aufgabe verknüpft sind und bestimmte Details zu der Aufgabe angeben. Beispiele sind „[!UICONTROL Geplantes Abschlussdatum]“ und „[!UICONTROL Status]“.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabenbeschränkung]</td> 
   <td>Siehe „[!UICONTROL Einschränkungstyp]“ und „[!UICONTROL Einschränkungsdatum]“.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgaben-Management]</td> 
   <td>Ein Satz von Richtlinien, die die Schwellenwerte für die Erstellung, Zuweisung, Schließung und Sichtbarkeit von Aufgaben steuern.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabenbesitzer]</td> 
   <td>Das Team oder die Person, das bzw. die für die Schätzung des Aufwands und den Abschluss der Aufgabe verantwortlich ist</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Eine Sammlung von Benutzenden, die ähnliche Ziele oder Geschäftsziele verfolgen. Diese Benutzenden können gemeinsam einem Arbeitselement zugewiesen werden, indem das Team dem Arbeitselement zugewiesen wird.</p> <p>Weitere Informationen zu Teams finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Überblick über Teams</a>.</p> <p>Projekte können über ein [!UICONTROL Projekt-Team] verfügen, das alle Benutzenden oder Rollen enthält, die mit der Arbeit für das Projekt verknüpft sind.</p> <p>Weitere Informationen zu Projekt-Teams finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Überblick über Projekt-Teams</a></p> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Vorlage]</td> 
   <td> <p>Projektvorlagen sind allgemeine Entwürfe Ihrer am häufigsten wiederholten Projekte. Beim Erstellen einer Projektvorlage können Sie Aufgaben, Warteschlangenthemen und benutzerdefinierte Formulare definieren und Dokumente oder Genehmigungen anfügen, um Zeit zu sparen, wenn Sie ein neues Projekt erstellen müssen. </p> <p>Sie können Vorlagen an vorhandene Projekte anfügen oder sie zum Erstellen neuer Projekte verwenden. Alle in der Vorlage angegebenen Informationen werden in die Projekte übertragen, die damit erstellt werden. </p> <p>Weitere Informationen zu Vorlagen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Überblick über Projektvorlagen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorlagenaufgabe]</td> 
   <td>Eine Aufgabe, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, das mithilfe der Vorlage erstellt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Eine [!UICONTROL Notiz] und die zugehörige Sammlung der Antworten, die sich auf ein bestimmtes Thema beziehen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniaturansicht]</td> 
   <td> <p> In einer Liste oder einem Bericht zu einem [!UICONTROL Dokument] wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p> Wählen Sie <strong>[!UICONTROL Miniaturansicht]</strong> aus, um eine 33–66 Pixel breite Miniaturansicht im Bericht anzuzeigen. </p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch „[!UICONTROL Große Miniaturansicht]“ in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausfallzeit]</td> 
   <td>Sie können einen Bericht zur [!UICONTROL Ausfallzeit] erstellen, um anzuzeigen, wann Benutzende Ausfallzeit in ihrem Profil angegeben haben. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeittabelle]</td> 
   <td> <p>Eine Arbeitszeitkarte, mit der Benutzende die tatsächlichen Stunden eingeben können, die sie mit der Arbeit an Projekten, Aufgaben oder Problemen verbracht haben, oder die Stunden, die sie für andere Aktivitäten aufgewendet haben, die nicht mit der Arbeit zusammenhängen, z. B. Meetings oder Schulungen. Zusätzlich zur Eingabe der aufgewendeten Arbeitszeit können Sie mithilfe von Stundentypen auch angeben, ob es sich um arbeitsbezogene Zeit oder um Overhead-Zeit handelt, um Ihre Zeiteingaben zu definieren. Informationen zu Arbeitszeittabellen finden Sie unter <a href="../../../timesheets/timesheets/timesheets-overview.md">Überblick über Arbeitszeittabellen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeittabellenprofil]</td> 
   <td> <p>Ein [!UICONTROL Arbeitszeittabellenprofil] ist eine Vorlage, mit der [!DNL Workfront] automatisch Arbeitszeittabellen für die ihnen zugeordneten Benutzenden erstellt. </p> <p>Sie können eine Reihe von Einstellungen konfigurieren, die für jede Arbeitszeittabelle gelten, sobald diese erstellt wird. Einige dieser Einstellungen sind: Wie oft die Arbeitszeittabelle erstellt werden soll (wöchentlich, jede zweite Woche, zweimal im Monat oder monatlich), der Starttag der Arbeitszeittabelle, die genehmigenden Personen für Arbeitszeittabellen, die verfügbaren [!UICONTROL Stundentypen], die Benutzende aufgezeichneten Stunden zuordnen können.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID des obersten übergeordneten Elements] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und ihren Untergruppen in einer Liste oder einem Bericht ermitteln und filtern.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name des obersten übergeordneten Elements] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und ihren Untergruppen in einer [!UICONTROL Ansicht] für eine Liste oder einen Bericht ermitteln.</p> <p>Sie können dies auch über das Feld „[!UICONTROL ID des obersten übergeordneten Elements]“ durchführen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stunden gesamt]</td> 
   <td> <p>In einem [!UICONTROL Projektbericht] enthält dieses Feld die gerundete Summe aller aufgewendeten Projektstunden, die bei der letzten Berechnung der Projektfinanzen ermittelt wurden. [!UICONTROL Tatsächliche Stunden] spiegeln die genauen Stunden wider, die für das Projekt erfasst werden. In der Regel sollten die [!UICONTROL tatsächlichen Stunden] mit den [!UICONTROL Gesamtstunden] übereinstimmen. Wenn sich die [!UICONTROL Gesamtstunden] erheblich von der Angabe im Feld „[!UICONTROL Tatsächliche Stunden]“ unterscheiden, müssen Sie die Finanzen des Projekts neu berechnen.</p> <p>Weitere Informationen zur Neuberechnung der Projektfinanzen finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Neuberechnen der Projektfinanzen</a>.</p> <p>In der [!UICONTROL Standard]-Ansicht einer Arbeitszeittabelle bezieht sich dieses Feld auf die Gesamtstunden, die für Elemente für die in einer Arbeitszeittabelle angezeigten Datumsangaben erfasst wurden. Das Feld „[!UICONTROL Gesamtstunden]“ für Arbeitszeittabellen in dieser integrierten Ansicht verweist auf das Feld „[!UICONTROL hoursDuration]“, das den Unterschied zwischen dem Start- und dem Enddatum der Arbeitszeittabelle dynamisch in Stunden berechnet. Auf diese Weise wird die Spalte „[!UICONTROL Gesamtstunden]“ in Rot angezeigt, wenn der Benutzer bzw. die Benutzerin mehr Zeit erfasst, als Stunden im Zeitrahmen der Arbeitszeittabelle verfügbar sind. Weitere Informationen finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Anzeigen der Gesamtstunden in einer Arbeitszeittabelle</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking-Modus]</td> 
   <td> <p>Ein Attribut einer Aufgabe. Dadurch wird festgelegt, wie und wann die voraussichtlichen Timelines für eine Aufgabe aktualisiert werden. Beispiel:</p> 
    <ul> 
     <li>„[!UICONTROL Benutzer muss aktualisieren]“ erfordert, dass eine Aufgabe manuell aktualisiert wird. Andernfalls wird sie als „[!UICONTROL In Verzug]“ und dann als „[!UICONTROL Überfällig]“ gekennzeichnet.</li> 
     <li>Mit „[!UICONTROL Automatisch abschließen]“ wird eine Aufgabe automatisch abgeschlossen, wenn das Fälligkeitsdatum oder das [!UICONTROL geplante Abschlussdatum] verstrichen ist.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Überblick über den Tracking-Modus für Aufgaben</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Ein Ereignis, das ein Szenario startet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gefährdete Aufgabe]</td> 
   <td>Eine unvollständige Aufgabe mit der Bedingung „[!UICONTROL Überfällig]“, „[!UICONTROL In Verzug]“ oder „[!UICONTROL Gefährdet]“.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nicht zugewiesene Aufgabe]</td> 
   <td>Eine Aufgabe, die keinen Benutzenden, keiner Rolle und keinem Team zugewiesen ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktualisierungstyp]</td> 
   <td> <p>Eine Einstellung für ein Projekt, die bestimmt, wann die voraussichtliche Timeline des Projekts neu berechnet wird. Der [!UICONTROL Aktualisierungstyp] kann die folgenden Werte haben:</p> 
    <ul> 
     <li>[!UICONTROL Automatisch und bei Änderung]</li> 
     <li>[!UICONTROL Nur automatisch]</li> 
     <li>[!UICONTROL Nur manuell] </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps eines Projekts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzende]</td> 
   <td>Ein Konto, das in [!DNL Workfront] erstellt wurde, damit sich eine Person anmelden und mit dem System interagieren kann.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Benutzerdelegierung]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Sie über Folgendes informiert:</p> 
    <ul> 
     <li>Welche Benutzenden eine Aufgabe, ein Problem und Projektgenehmigungen delegiert haben</li> 
     <li>An welche Benutzenden Aufgaben, Probleme und Projektgenehmigungen delegiert wurden</li> 
     <li>Wann diese Delegierungen beginnen und enden</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Erstellen eines Berichts zur Benutzerdelegierung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzeroberfläche]</td> 
   <td>Alle visuellen und interaktiven Aspekte von [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzeroberflächeneinstellungen]</td> 
   <td>[!UICONTROL Setup der Benutzeroberfläche]. Admins in [!DNL Workfront] können diese Einstellungen ändern, um Aspekte der Benutzeroberfläche anzupassen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Einsatz]</td> 
   <td>Die Verfügbarkeit für einen Benutzer bzw. eine Benutzerin oder eine Rolle basierend auf dem zugewiesenen Zeitplan, der PTO und der aktuellen Arbeitslast.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzereinsatz]</td> 
   <td> <p>Eine Suche kombiniert mit einem Bericht, der zeigt, wie Benutzende (Ressourcen) zugeteilt oder überbelegt sind. Siehe „[!UICONTROL Ressourcenauslastung]“ in diesem Artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V–Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objektname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Geschwindigkeit]</td> 
   <td>Damit wird die Gesamtarbeitszykluszeit gemessen (wie lange es dauert, eine Arbeit zu erledigen) und wie häufig die Arbeit in der ursprünglich zugesagten Zeit erledigt wird (Verhältnis von Arbeit zu Zusage).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Ansicht]</td> 
   <td> <p>Ansichten beziehen sich auf ein Berichtselement, mit dem Sie die Spalten in einem Bericht oder in einer Liste von Objekten ändern können.</p> 
   <p> Der Begriff „Ansicht“ bezieht sich auch auf das Recht eines Benutzers bzw. einer Benutzerin, Informationen zu einem Objekt nur entsprechend seiner bzw. ihrer Zugriffsebene oder einer Berechtigungsstufe für die Freigabe dieses Objekts anzuzeigen.</p> 
   <p>In Workfront-Planung werden Einträge auf der Seite „Eintragstyp“ in einer der folgenden Arten von Ansichten angezeigt:</p>
   <ul><li>Tabelle</li>
   <li>Timeline</li>
   <li>Kalender</li></ul>
   <p>In Workfront-Planung enthalten Ansichten die Filter, Gruppierungen, Sortierungen und andere Einstellungen, die auf die Einträge auf dem Bildschirm angewendet wurden.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/views/manage-record-views.md">Verwalten von Eintragsansichten</a>.</p>   
   <p>Workfront-Planung benötigt eine zusätzliche Lizenz.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigebildsymbole]</td> 
   <td> <p> Dies ist dasselbe Feld wie „Status-Symbole“, es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL Dokumente] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Status-Symbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen im letzten Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen im letzten Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen im letzten Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen in diesem Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen in diesem Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen in diesem Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In einem Bericht wird bei Verwendung der Schnittstelle im [!UICONTROL Textmodus] die Code-Zeile verwendet, in der Sie die Breite jeder Spalte in Pixel angeben können. Workfront bietet eine empfohlene Breite für jedes Feld.
Je nach Typ des Feldes und Format können Sie jedoch Anpassungen vornehmen.
Sie müssen die zusätzliche Code-Zeile <code>[!UICONTROL usewidths=true]</code> verwenden, um die für die Spalte angegebene Breite zu erzwingen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht werden mithilfe der folgenden Anweisung im Textmodus die geplanten Stunden des Projekts, der Aufgabe oder des Problems angezeigt:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Überblick über die Textmodus-Syntax</a>. </p> 
   <p><b>TIPP</b> 
   <p>Wenn Sie in einem Problembericht eines der Felder unter „[!UICONTROL Geplante Stunden]“ hinzufügen, wird dem Bericht das Feld <code>work </code> hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeit]</td> 
   <td> <p>Einer der beiden primären Lizenztypen. Dieser Typ bietet geringeren Zugriff als „[!UICONTROL Plan]“, kann jedoch Aktualisierungen im System erstellen und vornehmen. Benutzende mit einer Arbeitslizenz haben mehr Möglichkeiten als Inhaber und Inhaberinnen von Lizenzen des Typs „[!UICONTROL Extern]“, „[!UICONTROL Prüfende Person]“ oder „[!UICONTROL Anfragende Person]“.</p> <p>Weitere Informationen finden Sie unter „Überblick über <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]-Lizenzen</a>“.</p> <p>„Arbeit“ kann sich auf die Anzahl der [!UICONTROL geplanten Stunden] für ein Projekt, eine Aufgabe oder ein Problem beziehen. Weitere Informationen finden Sie im Feld „[!UICONTROL work]“ in dieser Tabelle. </p> <p><b>TIPP</b></p> <p> Wenn Sie in einem Problembericht eines der Felder unter „[!UICONTROL Geplante Stunden]“ hinzufügen, wird dem Bericht das Feld <code>work </code>hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Struktur für Auffächerung des Arbeitsaufwands]</td> 
   <td>Eine hierarchische Struktur der Aufgaben, die vom Projekt-Team basierend auf der Beziehung zwischen übergeordneter und untergeordneter Ebene ausgeführt werden sollen.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsaufwand] </td> 
   <td> 
    <p>Das Projekt-Management kann dieses Feld anstelle von „[!UICONTROL Geplante Stunden]“ verwenden, um den für die Erfüllung einer Aufgabe erforderlichen Aufwand zu schätzen. Dieses Feld ist nur sichtbar, wenn die folgenden Bedingungen erfüllt sind:</p> 
     <ul> 
      <li> <p>Die Aufgabe hat den [!UICONTROL Typ „Einfache Dauer“]. </p> <p><b>TIPP</b></p> <p> Wenn Sie den [!UICONTROL Dauertyp] der Aufgabe auf einen anderen Typ aktualisieren, wird dieses Feld ausgeblendet. </p> </li> 
      <li>Das Projekt-Management hat die Option „[!UICONTROL Arbeitsaufwand verwenden]“ aktiviert, um die Berechnung für das Feld „[!UICONTROL Geplante Stunden]“ der Aufgabe im Projekt automatisch durchzuführen. </li> 
     </ul> 
     <p>Informationen zur Verwendung von „[!UICONTROL Arbeitsaufwand]“ anstelle von „[!UICONTROL Geplante Stunden]“ zur Schätzung des Aufgabenaufwands finden Sie unter <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Überblick über den Arbeitsaufwand</a>. </p> 
     <p>Dieses Feld kann in Aufgabenberichten und -listen angezeigt werden.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitselement]</td> 
   <td> <p>Dieses Feld bezieht sich auf Aufgaben oder Probleme in [!DNL Workfront]. </p> <p>Der Bericht zum [!UICONTROL Arbeitselement] zeigt Informationen zu Aufgaben und Problemen an. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – Mix]</td> 
   <td>Ein [!UICONTROL Arbeitsleistungsindikator] (Work Performance Indicator, WPI) für den Anteil der Arbeit, der für den Betrieb Ihres Unternehmens aufgewendet wird, im Vergleich zu dem Anteil, der für Veränderungen in Ihrem Unternehmen aufgewendet wird. Die Mix-API hilft Ihnen auf Organisationsebene zu verstehen, ob Ihre Strategie tatsächlich mit einer realen Arbeitszuteilung einhergeht.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – Ressource]</td> 
   <td>Eine Bestimmung einer Persona im System, die zum Erhalt von Arbeit oder zur Nachverfolgung der Zeit berechtigt ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – Rolle und Verantwortlichkeiten]</td> 
   <td>Hier werden die Inhaber und Inhaberinnen sowie die Verantwortlichen für die Verwaltung des Umfangs, der Ausführung und der Genehmigungen des angegebenen Problems, Projekts, Programms oder Portfolios oder der angegebenen Aufgabe definiert.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – SLA]</td> 
   <td>Eine quantifizierbare Metrik, auf die sich alle Verantwortlichen geeinigt haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – Stakeholder]</td> 
   <td>Eine Sammlung von Benutzenden mit einem begründeten Interesse an den Ergebnissen einer Arbeitsanfrage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeits-Management – Berührungspunkte]</td> 
   <td>Digitalisierte Aufzeichnungen über die Kommunikation zwischen den Verantwortlichen</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indikatoren für Arbeitsleistung] </td> 
   <td> <p>Mischungsverhältnis, Kapazität, Geschwindigkeit, Qualität und Interaktion.</p> <p>WPI ist ein gebräuchliches Akronym für [!UICONTROL Work Performance Indicator] (Indikator für Arbeitsleistung).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsverfahren]</td> 
   <td> <p>Die Methode, mit der Arbeit erhalten, priorisiert und ausgeführt wird. Die Art und Weise, wie Sie die Arbeit ausführen, wird in der Regel als „Arbeitsablauf“ oder „Projektplan“ bezeichnet (eine Liste mit Aufgaben mit Datumsangaben, Vorgängerbeziehungen usw.). </p> <p>Beispiele für ein Arbeitsverfahren können die Produktion eines einzelnen Werbemittels oder die Bereitstellung einer Kampagne mit mehreren Werbemitteln sein. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow-Vorlage]</td> 
   <td>Im Bericht zur [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld alle Workflow-Vorlagen an, die an einen Korrekturabzug angefügt sind. Wenn keine Vorlagen angefügt sind, ist die Spalte leer.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>

<p>Stellt den Prozentsatz der Zeit des Vollzeitäquivalenz (Full Time Equivalent; [!UICONTROL FTE]) dar, die Benutzende für die tatsächliche Arbeit, ohne Overhead, zur Verfügung haben. [!UICONTROL Arbeitszeit] muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.</p>
   </p>Der Standardwert des Feldes ist 1. Dies bedeutet, dass eine Person ihren gesamten [!UICONTROL FTE] für die tatsächliche, projektbezogene Arbeit aufwendet.  </p>
   <p>Anhand dieser Zahl berechnet das System die Verfügbarkeit der Person für die tatsächliche, projektbezogene Arbeit. </p>
   <p> Zeitplanausnahmen und Ausfallzeiten können sich auch auf die Benutzerkapazität auswirken. </p>
   <p>Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>
    <p>Workfront berechnet die Verfügbarkeit einer Person abhängig von den Voreinstellungen für das Ressourcen-Management im Bereich „[!UICONTROL Setup]“. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Konfigurieren von Voreinstellungen für das Ressourcen-Management</a>. </p> 
   <p>Sie können die [!UICONTROL Arbeitszeit] einer Person aktualisieren, wenn Sie die Person bearbeiten oder erstellen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Bearbeiten eines Benutzerprofils</a></p> 
   <b>TIPP</b> 
   <p>Legen Sie den Wert für die [!UICONTROL Arbeitszeit] auf 1 fest, um anzugeben, dass die Person für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>In der Workfront-Dokumentation wird dieser Begriff verwendet, um die Zeit zu beschreiben, die gemäß einem Zeitplan für die Arbeit zugeteilt ist.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht wird bei Verwendung der folgenden Anweisung im Textmodus die Anzahl der geplanten Stunden für das Projekt, die Aufgabe oder das Problem angezeigt, gefolgt vom Wort „Stunden“:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Überblick über die Textmodus-Syntax</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Arbeitsbereich] </td> 
   <td> <p>In Workfront-Planung ist ein Arbeitsbereich eine Sammlung von Eintragstypen, die den Betriebszyklus eines bestimmten Unternehmens definieren. Ein Arbeitsbereich ist der Arbeitsrahmen einer Organisationseinheit.</p>
   <p>Workfront-Planung benötigt eine zusätzliche Lizenz. </p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Erstellen von Arbeitsbereichen</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


