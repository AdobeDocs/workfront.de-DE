---
content-type: reference
navigation-topic: workfront-navigation
title: Glossar zur Terminologie von [!DNL Adobe Workfront] s
description: Das [!DNL Adobe Workfront] Glossar listet häufig verwendete Begriffe in der [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] Oberfläche, in Berichten auf oder versucht, die Bedeutung der in der [!DNL Workfront] Dokumentation definierten  [!DNL Workfront] Konzepte zu verstehen.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '20930'
ht-degree: 0%

---


# Glossar der Terminologie von [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Dieser Artikel sollte als Referenz verwendet werden, um die Begriffe zu verstehen, die in der [!DNL Adobe Workfront] -Anwendung, in der [!DNL Workfront] -Dokumentation oder im Allgemeinen in Bezug auf die Planung und Verwaltung von Arbeit auftreten können. Diese Informationen werden derzeit aktualisiert, sodass diese Tabelle möglicherweise nicht vollständig ist. Wir werden diesen Haftungsausschluss entfernen, wenn wir diese Informationen als erschöpfend betrachten.

Die folgende Tabelle enthält eine Liste häufig verwendeter Begriffe in Adobe Workfront:

## A - C

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
   <td>Ein Benutzerprofil, das bestimmt, wie ein Benutzer mit verschiedenen Objekten und Tools in Workfront interagieren kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>Eine unvollständige Aufgabe in einem aktuellen Projekt, die nicht daran gehindert wird, von einer Vorgängeraufgabe bearbeitet zu werden, und keine Aufgabenbeschränkung mit einem geplanten zukünftigen Startdatum hat. Mit anderen Worten, es kann heute bearbeitet werden.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Aktivität]</td> 
   <td>In [!DNL Workfront Goals] ist eine Aktivität eine Fortschrittsanzeige für ein Ziel. Es kann sich um eine Fortschrittsleiste handeln, die Sie manuell aktualisieren, oder um ein Projekt, das mit dem Ziel verknüpft ist. Sie können keine Aktivitäten in einem Bericht anzeigen und können nicht über die [!DNL Workfront] -API darauf zugreifen. Informationen zu Aktivitäten finden Sie unter <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront-Zielen</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Kosten]</td> 
   <td> <p>Bei Aufgaben und Problemen sind dies die Kosten im Zusammenhang mit den tatsächlichen Stunden, die protokolliert werden, in Bezug auf die Kosten pro Stunde der Ressource, die der Aufgabe oder dem Problem zugewiesen ist. Bei Projekten entspricht dies dem Gesamtbetrag aller [!UICONTROL Tatsächlichen Kosten] aus Aufgaben und Problemen im Zusammenhang mit dem Projekt. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten-Tracking</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Kosten]</td> 
   <td> <p>Die Summe der [!UICONTROL tatsächlichen Beträge] für alle Ausgaben, die für ein Projekt oder eine Aufgabe protokolliert werden.</p> <b>BEISPIEL </b>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und im Feld [!UICONTROL Tatsächlicher Betrag] den Betrag von 600,00 USD eingeben, belaufen sich die tatsächlichen Kosten für diese Aufgabe auf 600,00 USD. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel zur Berechnung der tatsächlichen Kosten von [!UICONTROL]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächliche Stunden]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht sind die tatsächlichen Stunden die Summe aller Stunden, die für das Projekt, die Aufgabe oder das Problem protokolliert wurden.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> Wenn Sie auf der Registerkarte [!UICONTROL Updates] für Aufgabe 1 auf "Log Time"klicken und 25 Stunden eingeben, beträgt die tatsächliche Stunde der Aufgabe 1 = 25 Stunden. </p> <p>[!DNL Workfront] berechnet [!UICONTROL Tatsächliche Stunden] für übergeordnete Aufgaben oder Projekte anhand der folgenden Formeln:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Arbeitskosten]</td> 
   <td> <p>Die tatsächlichen [!UICONTROL Kosten], die mit der in eine Aufgabe oder ein Projekt investierten Arbeitskraft verbunden sind. </p> <p>Für eine Aufgabe berechnet [!DNL Workfront] die tatsächlichen Arbeitskosten anhand der folgenden Formel:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Wenn die Aufgabe einen [!UICONTROL Kostentyp] von [!UICONTROL User Stündlich] aufweist, verwendet [!DNL Workfront] die Benutzerrate. Wenn die Aufgabe einen [!UICONTROL-Kostentyp] von [!UICONTROL Role Stündlich] aufweist, verwendet [!DNL Workfront] die Auftrags-Rollenrate zur Berechnung der tatsächlichen Arbeitskosten. </p> <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel zur Berechnung der [!UICONTROL Tatsächlichen Arbeitskosten]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten-Tracking</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn ein Benutzer beispielsweise 5 Stunden für eine Aufgabe mit einem [!UICONTROL Benutzer pro Stunde] [!UICONTROL Kostentyp] protokolliert und dessen Stundensatz 100 USD beträgt, beträgt die [!UICONTROL Tatsächliche Arbeitskosten] 500 USD.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächlicher Umsatz] </td> 
   <td> <p>Der [!UICONTROL Tatsächliche Umsatz] eines Projekts oder einer Aufgabe ist der Geldbetrag, der mit den [!UICONTROL tatsächlichen Stunden] des Projekts oder der Aufgabe verbunden ist. </p> <p>Informationen zum Verfolgen des Umsatzes in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächlicher Start]</td> 
   <td>Der Zeitstempel, zu dem ein Benutzer ein Objekt ändert, das bei der ihm zugewiesenen Arbeit in Bearbeitung ist.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile]-Methode</td> 
   <td>Eine Methodik, die auf der kollaborativen Entwicklung von Anforderungen und Lösungen mit funktionsübergreifenden Teams basiert. Sie fördert Flexibilität und Änderungen auf der Grundlage einer festen Zeitleiste.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Das unterscheidet sich von einem traditionellen Team, da sie ihre voraussichtliche Arbeit aus einem Rückstand nehmen und innerhalb einer bestimmten Zeit daran arbeiten, die als [!UICONTROL Iteration] bezeichnet wird.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alle meine Teams]</td> 
   <td> <p>Wenn dies in [!UICONTROL Filtern] referenziert wird, zeigt dieses Feld entweder Benutzer an, die zu einem der Teams gehören, zu denen der angemeldete Benutzer gehört, oder Arbeitselemente, die einem der Teams zugewiesen sind, zu denen der angemeldete Benutzer gehört. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der abhängig davon, wer sich anmeldet, unterschiedliche Informationen anzeigt, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuordnungsdatum]</td> 
   <td> <p>Dieses Feld finden Sie in den folgenden Berichtstypen:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Projekt] (Finanzdaten)</li> 
     <li>[!UICONTROL Budgetierte Stunde]</li> 
    </ul> <p>Für einen Bericht vom Typ<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Projekt (Finanzdaten)]: </p> 
    <ul> 
     <li>Erstellen Sie diesen Bericht, wenn Sie versuchen, <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> die [!UICONTROL Planen Stunden] zu verstehen, die Ihren Ressourcen zugewiesen sind.</li> 
     <li> <p>Das [!UICONTROL Zuweisungsdatum] ist der erste Tag (Sonntag) einer Woche, in dem die Zuordnung einer [!UICONTROL Auftragsrolle] zu einer Aufgabe beginnt. Eine Ressource ([!UICONTROL Job Role]) kann so viele [!UICONTROL Zuordnungsdaten] wie Wochen während der [!UICONTROL Dauer] der Aufgaben haben, denen sie zugewiesen ist. Wenn Aufgaben mehrere Monate umfassen, kann der erste Tag eines Monats auch zum [!UICONTROL Zuordnungsdatum] werden, wenn er unter die [!UICONTROL Dauer] der Aufgabe fällt.</p> <p>Sie können beispielsweise eine [!UICONTROL Auftragsrolle] einer Aufgabe zuweisen, die mehr als 3 Wochen dauert und 90 [!UICONTROL geplante Stunden] hat. Diese Stunden werden gleichmäßig über die Dauer der Aufgabe verteilt. Dadurch werden täglich 6 [!UICONTROL Planed Hours] zu Ihrer Auftragsrolle zugewiesen:</p> <p><em> [!UICONTROL Tägliche geplante Stunden] = [!UICONTROL Gesamtgeplante Stunden]/ Anzahl der [!UICONTROL Arbeitstage] während der [!UICONTROL Dauer] der Aufgabe </em> </p> <p>Daher gibt es während der [!UICONTROL Dauer] der Aufgabe drei [!UICONTROL Zuweisungsdaten], eines für jeden Sonntag jeder Woche, mit jeweils einer bestimmten Anzahl von [!UICONTROL geplanten Stunden].<br>Wenn die Aufgabe mitten in der letzten Woche eines Monats beginnt und zwei Wochen nach Beginn eines neuen Monats endet, hat die Aufgabe vier [!UICONTROL Zuordnungsdaten]: einen für jeden Sonntag jeder Woche während der [!UICONTROL Dauer] der Aufgabe und einen für den ersten Tag des neuen Monats.</p> <p>Um diese Informationen optimal zu nutzen, empfehlen wir, einen "<!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Project"(Finanzdaten)-Bericht zu erstellen und eine Matrixgruppierung für [!UICONTROL Allokationsdatum] hinzuzufügen und dann die Ergebnisse wöchentlich, monatlich, vierteljährlich oder jährlich für die genauesten Daten zu gruppieren.<br>Informationen zum Erstellen einer Matrixgruppierung finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Erstellen eines Matrix-Berichts</a>.</p> </li> 
    </ul> <p>Finanzinformationen werden nur dann in [!UICONTROL Project (Financial Data)]-Berichten ausgefüllt, wenn die damit verbundenen Daten weniger als 5 Jahre alt sind. Wenn beispielsweise im Januar 2015 einer Aufgabe eine Stellenrolle zugewiesen wurde und heute September 2021 ist, wird ein Finanzfeld wie das [!UICONTROL Zuweisungsdatum] für die Stellenrolle nicht im [!UICONTROL Projekt (Finanzdaten)]-Bericht ausgefüllt. </p> 
    <div> 
     <p>Für einen [!UICONTROL Budgeted Hour]-Bericht:</p> 
     <ul> 
      <li>Erstellen Sie diesen Bericht, wenn Sie versuchen, die [!UICONTROL Budgeted Hours] zu verstehen, die Ihren Ressourcen oder Ihren Projekten im Ressourcenplaner zugewiesen sind.</li> 
      <li> <p>Das [!UICONTROL Zuweisungsdatum] ist der erste Tag (ein Sonntag) der Woche, für den Sie die Stunden im [!UICONTROL Resource Planer] im Voraus geplant haben. </p> <p><b>TIPP</b></p> <p>Wenn sich eine Woche über zwei Monate erstreckt, werden im Bericht zwei Zeilen generiert: eine Zeile, die dem ersten Wochentag (Sonntag der ersten Woche, die im ersten Monat stattfindet) entspricht, und die zweite Zeile den ersten Tag des zweiten Monats. </p> <p>Wenn Sie z. B. für die Woche vom 30. Juni (Sonntag) bis 6. Juli (Samstag) 8 Stunden für einen Benutzer einplanen, zeigen die beiden Zeilen ein [!UICONTROL Zuordnungsdatum] vom 30. Juni und 1. Juli. </p> </p> <p>Weitere Informationen zu Budgetierungsressourcen in der [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen in der [!DNL Resource Planner], die die Ansichten [!UICONTROL Projekt] und [!UICONTROL Rolle] verwenden</a>.</p> <p>Informationen zum Erstellen eines [!UICONTROL Budgeted Hour]-Berichts finden Sie unter <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mitteilungen]</td> 
   <td> <p>Eine Möglichkeit, Informationen innerhalb des Systems an Benutzer zu kommunizieren. Diese Informationen stammen häufig von [!DNL Workfront] an den Administrator oder vom Administrator an den Benutzer. </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Mitteilungen senden</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App-Integration]</td> 
   <td>Eine App stellt in den meisten Fällen einen Connector zu einer Softwareanwendung dar, kann aber auch spezielle Funktionen darstellen, mit denen Daten bearbeitet werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigerentscheidung]</td> 
   <td> <p>Im [!UICONTROL Validierungsbericht] zeigt dieses Feld Entscheidungen zur Testversandvalidierung für nicht mehr aktive Testsendungen an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Phase des Genehmigers]</td> 
   <td>Im [!UICONTROL Bericht über die Validierung von Testsendungen] zeigt dieses Feld Informationen über den aktuellen Stand der Testsendungen an.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Validierung]</td> 
   <td> <p>Ein bestimmtes Arbeitselement, wie z. B. eine Aufgabe, ein Dokument oder ein Timesheet, kann vorschreiben, dass ein Supervisor oder ein anderer Benutzer das Arbeitselement abzeichnet. Dieser Prozess der Abmeldung wird als Genehmigung bezeichnet. </p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über den Genehmigungsprozess</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Validierungsdatum]</td> 
   <td>Im [!UICONTROL Validierungsbericht] zeigt dieses Feld das Datum an, an dem ein Testversand genehmigt wurde.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmiger]</td> 
   <td>Eine Benutzer- oder Auftragsrolle, die für ein bestimmtes Arbeitselement abzeichnen muss, oder der Benutzer, der Stundeneinträge in Timesheets genehmigt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisung zu]</td> 
   <td> <p>In einem [!UICONTROL Task- oder Problembericht] zeigt dieses Feld den Eigentümer der Aufgabe oder des Problems oder den Primären Verantwortlichen [!UICONTROL] an. Sie können auch nach diesem Feld filtern oder gruppieren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisung]</td> 
   <td>Ein Benutzer, eine Rolle oder ein Team, das einem Problem oder einer Aufgabe zugewiesen ist. Projekte, Portfolios oder Programme können nicht zugewiesen werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisung]</td> 
   <td> <p>In einem [!UICONTROL Task]- oder [!UICONTROL-Problem]-Bericht zeigt dieses Feld eine Liste aller Entitäten (Benutzer, Jobrollen, Teams) an, die der Aufgabe oder dem Problem zugewiesen sind. Sie können nach diesem Feld filtern, indem Sie die Felder [!UICONTROL Zuweisungsbenutzer] und [!UICONTROL Zuweisungsrollen] verwenden. Im Feld Team können Sie nach dem der Aufgabe oder dem Problem zugewiesenen Team filtern. Ein Bericht kann nicht nach diesem Feld gruppiert werden.</p> <p>Arbeitselemente, die im [!UICONTROL Papierkorb] platziert wurden, werden weiterhin in einigen Berichten angezeigt, die auf das [!UICONTROL Assignment]-Objekt verweisen, in dem ein [!DNL OR] -Filtermodifikator verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisungsrollen]</td> 
   <td>
   <p>In einem [!UICONTROL Task] - oder [!UICONTROL Problem] -Bericht werden in diesem Feld Informationen zu den den Aufgaben oder Problemen zugewiesenen Auftrags-Rollen angezeigt. In diesem Feld werden [!UICONTROL Primäre Eigentümer] sowie andere Aufgabenrollen angezeigt, die Aufgaben oder Problemen zugewiesen sind.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisungsstatus]</td> 
   <td> <p>In einem Zuweisungs-, Aufgaben- oder Problembericht zeigt der [!UICONTROL Zuweisungsstatus] an, ob die einem Arbeitselement zugewiesenen Benutzer auf die [!UICONTROL Work On It]- oder die [!UICONTROL Done]-Schaltfläche geklickt haben, um die Arbeit zu akzeptieren oder abzuschließen. Die folgenden [!UICONTROL Zuweisungsstatus] sind vorhanden:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: Der Benutzer wurde der Aufgabe oder dem Problem zugewiesen, aber er hat noch nicht auf die Schaltfläche [!UICONTROL Work On It] geklickt, um mit der Bearbeitung zu beginnen.</li> 
     <li><b>[!UICONTROL Working]</b>: Der Benutzer hat auf die Schaltfläche [!UICONTROL Work On It] geklickt und arbeitet derzeit an dem Element. </li> 
     <li><b>[!UICONTROL Fertig]</b>: Der Benutzer hat auf die Schaltfläche [!UICONTROL Fertig] geklickt und seine Arbeit an dem Element abgeschlossen. </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref"> [!UICONTROL Work On It] und [!UICONTROL Done] button overview</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisungsteams]</td> 
   <td>
   <p>In einem [!UICONTROL Task] - oder [!UICONTROL Problem] -Bericht werden in diesem Feld Informationen zu den Teams angezeigt, die den Aufgaben oder Problemen zugewiesen sind. Im Feld werden [!UICONTROL Primäre Eigentümer] sowie andere Teams angezeigt, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisung von Benutzern]</td> 
   <td>
   <p>In einem [!UICONTROL Task] - oder [!UICONTROL Problem] -Bericht werden in diesem Feld Informationen zu den Benutzern angezeigt, die den Aufgaben oder Problemen zugewiesen sind. In diesem Feld werden [!UICONTROL Primäre Eigentümer] sowie andere Benutzer angezeigt, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribut]</td> 
   <td>Ein Attribut ist eine Eigenschaft eines [!DNL Workfront] -Objekts.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auditbereich]</td> 
   <td> <p>Prüfungen sind Systemnachrichten, die eine in Workfront ausgeführte Aktion aufzeichnen. Die folgenden Audittypen werden aufgezeichnet:</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL Allgemein bearbeiten]</li> 
     <li>[!UICONTROL Statusänderung]</li> 
     <li>[!UICONTROL Hinweis]</li> 
     <li>[!UICONTROL Kombinierter Eintrag]</li> 
     <li>[!UICONTROL Fehlereintrag]</li> 
     <li>[!UICONTROL Statusänderung]</li> 
     <li>[!UICONTROL Abonnementänderung]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit-Protokoll]</td> 
   <td>Die Sammlung von Notizen, die automatisch von Ereignissen generiert werden, die durch aufgezeichnete Änderungen verfolgt werden ([!UICONTROL Audit-Bereiche]). Jede Notiz zeichnet auf, wer die Aktion durchgeführt hat, was er getan hat und wann er sie durchgeführt hat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatisch und bei Änderung]</td> 
   <td> <p>Einer der [!UICONTROL Projektaktualisierungstypen. Dadurch werden die geplanten und geplanten Zeitpläne des Projekts neu berechnet, wenn der nächtliche Neuberechnungsprozess ausgeführt wird und das Projekt oder die Aufgaben im Rahmen des Projekts aktualisiert werden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps für das Projekt </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Verfügbarkeit</p></td> 
   <td> <p>Dieser Begriff wird im Zusammenhang mit "Benutzerverfügbarkeit"oder "Ressourcenverfügbarkeit"verwendet und zeigt an, wie lange die Ressource (Benutzer- oder Arbeitsplatzrolle) zur Verfügung steht. </p> 
   <p>Workfront berechnet die Benutzerverfügbarkeit anhand verschiedener Felder und abhängig von den Einstellungen der Voreinstellungen für die Ressourcenverwaltung in Ihrem System. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>. </p>
   <p>Weitere Informationen zur Ressourcenverfügbarkeit finden Sie unter <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit der Ressourcenverwaltung</a></p>
   Alternativ wird auch "Kapazität"verwendet, um auf die Verfügbarkeit der Ressourcen zu verweisen. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatisch]</td> 
   <td> <p>Einer der [!UICONTROL Projektaktualisierungstypen. Dadurch werden die geplanten und geplanten Zeitpläne neu berechnet, wenn der nächtliche Neuberechnungsprozess ausgeführt wird.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps für das Projekt</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>"Business as usual" Arbeit, die dazu beiträgt, die alltäglichen primären Geschäftsziele zu erreichen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>Das Gebiet in einem agilen Umfeld, in dem neue Probleme beibehalten werden, bis sie zur Bearbeitung bereit sind.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Eine Datenquelle zur Messung von Iterationen in einer agilen Umgebung.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Rechnungskosten]</td> 
   <td> <p>Eine dem Kunden als abrechnungsfähig gekennzeichnete Ausgabe. Dies kann entweder eine geplante oder eine tatsächliche Ausgabe sein.</p> <p>Die Felder Geplante Abrechnungskosten und Tatsächliche Abrechnungskosten stehen Ihnen zur Verfügung, um sie Ansichten und Berichten hinzuzufügen. Sie werden nicht auf den Projekt- oder Aufgabendetailseiten angezeigt.</p>
   <p>Sie finden diese Felder in den folgenden Berichtstypen:</p>
   <ul>
   <li>Ausgangsbasis</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Markieren einer Ausgabe als abrechnungsfähig finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Verwalten von Projektausgaben</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Rechnungsdatensatz]</td> 
   <td> <p>Erfasst die abrechnungsfähigen Einnahmen, Stunden oder Ausgaben. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchführungssystem verwendet werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Erstellen von Rechnungsdatensätzen</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status des Rechnungsdatensatzes</td> 
   <td> <p>In einem Abrechnungsdatensatz- oder Stundenbericht zeigt der Status eines Abrechnungsdatensatzes an, ob der Abrechnungsdatensatz abgerechnet wurde oder nicht abgerechnet wurde. Sie können ein Projekt nicht löschen oder die mit einem abrechnungsfähigen Datensatz verknüpfte Zeit bearbeiten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Erstellen von Rechnungsdatensätzen</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Der Prozess der Anpassung von [!DNL Workfront], um der Oberfläche ein Erscheinungsbild zu verleihen, das Ihr Unternehmen mithilfe Ihrer Farben und Logos widerspiegelt.</p><p><strong>HINWEIS</strong><br>Wenn Ihr Unternehmen in [!DNL Adobe Experience Cloud] integriert wurde, ist das Branding nicht verfügbar.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Der Bereich oben auf der Seite, der die hierarchische Position des Benutzers in der Anwendung anzeigt.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Übersicht über Breadcrumbs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetstatus]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die dieses Feld anzeigen kann, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat und die nicht aktualisiert werden kann. </p> <p>In diesem Feld wird angezeigt, ob das Projekt dem [!UICONTROL Capacity Planner] hinzugefügt wurde und ob die Budgetberechnung dafür abgeschlossen wurde. Der [!UICONTROL Capacity Planner] wurde aus [!DNL Workfront] entfernt. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetiertes Abschlussdatum]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die in diesem Feld angezeigt werden, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden. </p>
   <p> Dieses Feld ist weiterhin in [!UICONTROL Projekt]-Berichten und -Listen sichtbar.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Kosten]</td>

<td> <p>Dies sind die Kosten, die mit den Haushaltsmitteln für ein Projekt verbunden sind. </p>
   <p>Das Feld wird in den folgenden Bereichen von [!DNL Workfront] unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL Budgetierte Kosten]</strong>: im Bedienfeld [!UICONTROL Zusammenfassung der Geschäftsszenarios]</li>
   <li><strong>[!UICONTROL Cost]</strong>: in den [!UICONTROL Utilization]-Bereichen, wenn Informationen nach [!UICONTROL Cost] angezeigt werden</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: in Listen und Berichten</li>
   </ul>   
    <p>Die [!UICONTROL Budgeted Cost] für das Projekt werden anhand der folgenden Formel berechnet:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Weitere Informationen zur Berechnung von [!UICONTROL Budgeted Cost] und zum Verständnis verschiedener Namen für dieses Konzept in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Berechnete Kosten für das Projekt berechnen</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgetierte Stunden]</td> 
   <td> <p>Die für die Ressourcen für die Arbeit, die sie für Projekte durchführen müssen, vorgesehenen Stunden. Dieses Feld bezieht sich auf die im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case] (oder im [!UICONTROL Resource Planner]) für das Projekt oder die Projektressourcen veranschlagten Stunden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Grundlegendes zu [!UICONTROL Budgeted Labour Cost] und [!UICONTROL Budgeted Hours] für Projekte</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Weitere Informationen zum Budgetieren von Benutzern in der [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen in der [!DNL Resource Planner], die die Ansichten [!UICONTROL Projekt] und [!UICONTROL Rolle] verwenden</a>. </p> 
    <p>Die im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case] oder des [!UICONTROL Resource Planner] geplanten Stunden werden in den folgenden Bereichen von [!DNL Workfront] und unter den folgenden Namen angezeigt:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Anzeigename: [!UICONTROL Budgeted Hours]</strong></td> 
        <td><strong>Gebiete von [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Resource Budgeting] Bereich des [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planer] angezeigt von [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgetierte Stunden]</td> 
        <td> <p>Ansicht des Nutzungsberichts [!UICONTROL Stunden]</p> <p>Weitere Informationen zum [!UICONTROL Utilization]-Bericht finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Überblick über den [!UICONTROL Resource Utilization]-Bericht</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Stunden]</td> 
        <td> <p>[!UICONTROL Budgetierte Stunde] Bericht</p><p>Das Objekt [!UICONTROL Budgeted Hour] im Bericht Budgeted Hour bezieht sich auf Informationen zu einem veralteten Tool zur Ressourcenverwaltung. Nur der "[!UICONTROL Bud. Das Feld Stunden]"in diesem Bericht bezieht sich auf die im [!UICONTROL Resource Planer] oder im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case] des Projekts veranschlagten Stunden. </p> <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerspezifischen Bericht erstellen</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planer - Budgetierte Stunden] </td> 
        <td> <p>In den folgenden Berichten enthalten:</p>
        <ul>
        <li>[!UICONTROL Projekt]
        <li>[!UICONTROL Projekt (Finanzdaten)]-Bericht
        <li>[!UICONTROL Task]
        <li>[!UICONTROL Problembericht]
        <li>[!UICONTROL Budgetierte Stunde] Bericht</li>
        </ul>
         <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerspezifischen Bericht erstellen</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Jede andere Erwähnung von [!UICONTROL Budgeted Hours] in [!DNL Adobe Workfront] bezieht sich auf die geplanten Stunden mit veralteten Funktionen, die aus Workfront entfernt wurden. Diese Felder sind schreibgeschützt und werden nicht mit aktuellen Informationen aktualisiert, wenn Sie die aktuellen Tools für die Ressourcenbudgetierung verwenden. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Arbeitskosten]</td> 
   <td> <p>Dies sind die Kosten, die mit den Stunden verbunden sind, die Sie als Ressourcen-Manager für Ihre Stellenrollen für die Arbeit, die sie an Projekten durchführen müssen, einplanen. </p> <p>Die [!UICONTROL Budgeted Labour Cost] in einem Projektbericht wird mit der folgenden Formel berechnet:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Dieses Feld kann sich auf Folgendes beziehen:</p> 
    <ul> 
     <li> <p>Arbeitskosten, die im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case] oder im [!UICONTROL Resource Planer] angezeigt werden und mit den Kosten der Stellenangebote eines Projekts verbunden sind. Weitere Informationen zur Berechnung der [!UICONTROL Budgeted Labour Cost] finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Budgetierte Arbeitskosten] und [!UICONTROL Budgetierte Arbeitsstunden] für Projekte</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Arbeitskosten, die im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case] angezeigt werden und die [!UICONTROL People Costs] widerspiegeln, die in einer mit dem Projekt verknüpften Initiative aus dem [!DNL Scenario Planner] geschätzt werden, wenn Sie den Szenario-Planer zum Budget Ihrer Projektressourcen verwenden. Weitere Informationen zu Initiativen finden Sie unter <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Übersicht über Initiativen im Szenario-Planer</a>. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Sie wird in den folgenden Bereichen von unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labour Cost]</strong>: im [!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: im [!UICONTROL Utilization]-Bericht [!UICONTROL Cost]-Ansicht
   <p>Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Informationen zur Ressourcenauslastung anzeigen </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in den Ansichten [!DNL Resource Planner] Projekt oder [!DNL Role] bei der Anzeige nach Kosten
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in den folgenden Berichten: 
   <ul>
    <li>[!UICONTROL Projekt]</li>
    <li>[!UICONTROL Projekt (Finanzdaten)]-Bericht</li>
    <li>[!UICONTROL Task]</li>
    <li>[!UICONTROL Problembericht]</li>
    <li>[!UICONTROL Budgetierte Stunde] Bericht</li> 
    </ul>
    <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerspezifischen Bericht erstellen</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgetiertes Startdatum]</td> 
  <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die in diesem Feld angezeigt werden, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden.</p>
  <p>Diese Bereiche wurden aus [!DNL Workfront] entfernt. </p> 
  <p>Das Feld ist weiterhin in [!UICONTROL Projekt]-Berichten und -Listen sichtbar.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Niederschlagsdiagramm]</td> 
   <td>Ein Liniendiagramm, das eine visuelle Darstellung abgeschlossener und verbleibender Arbeiten bereitstellt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Geschäftsfall]</td> 
   <td> <p>Ein Tool zur Bewertung, ob ein Projekt vom Status [!UICONTROL Idee] in den Status [!UICONTROL Planung] verschoben werden soll. Mit anderen Worten: Ein [!UICONTROL Geschäftsfall] hilft der Organisation zu entscheiden, ob es sich lohnt, das Projekt zu starten und abzuschließen oder nicht, insbesondere beim Vergleich von Projekten mit anderen in einem Portfolio.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Erstellen eines [!UICONTROL Geschäftsfalls] für ein Projekt </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Geschäftsfall - Budgetierte Stunden]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die in diesem Feld angezeigt werden, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden.</p> <p>Dieses Feld ist weiterhin in Projekt- und [!UICONTROL Aufgabe] Listen und Berichten sichtbar. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechnete Zuweisung]</td> 
   <td> <p>Eine der Aufgaben [!UICONTROL Dauer Typen] . Dies berechnet den Prozentsatz eines achtstündigen Arbeitstags, der dem der Aufgabe zugewiesenen Benutzer der Aufgabe zugewiesen wird, basierend auf der [!UICONTROL Dauer] der Aufgabe und der [!UICONTROL Arbeit erforderlich].</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Dauer] und [!UICONTROL Dauer Typ]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechnete Arbeit]</td> 
   <td> <p>Eine der Aufgaben [!UICONTROL Duration Types]. Dies berechnet die [!UICONTROL Arbeit erforderlich] für eine Aufgabe anhand der Prozentsätze [!UICONTROL Dauer] und [!UICONTROL Zuweisung] des Benutzers (die auf einem achtstündigen Arbeitstag basieren).</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Dauer] und [!UICONTROL Dauer Typ]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender]</td> 
   <td> <p>In Workfront ist ein Kalenderbericht ein dynamischer Bericht, in dem Benutzer das Datum und andere wichtige Details eines Ereignisses anzeigen können, einschließlich Fälligkeitsdatum, Arbeitsstatus und dem Benutzer, dem das Ereignis zugewiesen wurde.</p> <p> Weitere Informationen zu Kalenderberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Übersicht über Kalenderberichte</a>.</p>
   <p> In der Workfront-Planung ist eine Kalenderansicht eine Art Ansicht für einen Datensatztyp, der Datensätze in einem Kalender anzeigt. Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>Dieses Feld gibt an, ob eine Aufgabe bereit ist, mit der Arbeit zu beginnen. Wenn der Start bereit für die Bearbeitung des [!UICONTROL Can Start] Felds für die Aufgabe ist auf [!UICONTROL True] eingestellt. </p> <p>Weitere Informationen finden Sie in der Übersicht über die Aufgaben unter <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start]"</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Kapazität</p> </td> 
   <td> <p>Die verfügbare Zeit einer Ressource, in der sie für die Arbeit zugewiesen werden können. Siehe "Verfügbarkeit". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Kategorie]</p> </td> 
   <td> <p>Eine Kategorie ist ein benutzerdefiniertes Formular. Sie können Berichte für dieses Objekt erstellen und es auch in anderen Objektberichten anzeigen. Nicht alle Objekte können über ein benutzerdefiniertes Formular oder eine benutzerdefinierte Kategorie verfügen. Die folgenden Objekte können über ein benutzerdefiniertes Formular verfügen: <br></p> 
    <ul> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL Programm]</li> 
     <li>[!UICONTROL Benutzer]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kategoriename]</td> 
   <td> <p>Wenn der Ansicht der folgenden Objekte als Spalte hinzugefügt wird, wird eine Liste aller mit diesen Objekten verknüpften benutzerdefinierten Formulare angezeigt:</p> 
    <ul> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Problem]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Ausgaben]<br></li> 
     <li>[!UICONTROL Programm]<br></li> 
     <li>[!UICONTROL Benutzer]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Ein Praxisbereich, der sich auf die Definition, das Verständnis und die Anpassung der geplanten Arbeit an Änderungen in Umfang, Zeitplan, Kosten und Ressourcenfaktoren konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Reihenfolge ändern</td> 
   <td>Eine Art von Problem, das sich mit einem Projekt befasst, in dem eine beantragte Änderung des vereinbarten Anwendungsbereichs beschrieben wird.</td> 
  </tr> 
  <tr> 
   <td>Nur Änderung:</td> 
   <td>Eines der Projekte [!UICONTROL Aktualisierungstypen]. Es werden nur die Zeitpläne [!UICONTROL Project Projected] und [!UICONTROL Planned] aktualisiert, wenn Aktualisierungen an Aufgaben vorgenommen oder Änderungen an dem Projekt bzw. den Aufgaben vorgenommen werden.</td> 
  </tr> 
  <tr> 
   <td>Reihenfolge ändern</td> 
   <td> <p>Einer der [!UICONTROL Problemtypen], der normalerweise angibt, dass ein ungeplanter Arbeitsaufwand erforderlich ist, bevor das Projekt abgeschlossen werden kann.</p> <p>Weitere Informationen zu [!UICONTROL Problemtypen] finden Sie im Abschnitt "Standardausgabetypen"im Artikel <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Standardausgabetypen anpassen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Untergeordnete Aufgabe]</td> 
   <td>Eine Aufgabe, die eine [!UICONTROL Unteraufgabe] einer [!UICONTROL übergeordneten Aufgabe] ([!UICONTROL Zusammenfassungsaufgabe]) ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>Die Sammlung von [!UICONTROL Unteraufgaben] zu einer [!UICONTROL übergeordneten Aufgabe] ([!UICONTROL Zusammenfassungsaufgabe]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] und [!UICONTROL Training]</td> 
   <td>Lernmodule, Zertifizierungen, Standards oder eine Gemeinschaft der Praxis.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Ein Kommunikationstool für Benutzer, mit dem sie Erwartungen an Aufgabenlieferungen setzen können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Veröffentlichungsdatum]</td> 
   <td>Ein Kommunikationstool für Benutzer, um Erwartungen in Bezug auf Aufgabenlieferungen zu setzen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] und [!UICONTROL Reporting]</td> 
   <td>Standards zur Überprüfung der Ausnahmen und des Zustands eines Projekts, Programms oder Portfolios</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Eine [!UICONTROL Firma] ist eine Organisationseinheit in [!DNL Workfront]. </p> 
   <p> Sie können einen Benutzer oder ein Projekt mit einem Unternehmen verknüpfen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Unternehmen erstellen und bearbeiten</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussdatum]</td> 
   <td> <p>Das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem abgeschlossen sein soll. Es gibt mehrere Arten von [!UICONTROL Abschlussdaten] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Tatsächliches Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Überblick über das Projekt [!UICONTROL Tatsächliches Abschlussdatum] </a>.</li> 
     <li>[!UICONTROL Geplantes Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Festlegen des geplanten Abschlussdatums für das Projekt [!UICONTROL]</a> und <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Überblick über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]</a>.</li> 
     <li>[!UICONTROL Projektiertes Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Überblick über das geplante Abschlussdatum von [!UICONTROL] für Projekte, Aufgaben und Probleme</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussdatum]</td> 
   <td>Der Tag, relativ zum Beginn der [!UICONTROL Vorlage], an dem eine [!UICONTROL Vorlagenaufgabe] oder eine [!UICONTROL Vorlage] abgeschlossen sein soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussmodus]</td> 
   <td> <p>Dies zeigt an, wie ein Projekt als [!UICONTROL Complete] markiert wird. Er kann zwei Werte haben:</p> 
    <ul> 
     <li>[!UICONTROL Handbuch]: Benutzer müssen den Projektstatus in [!UICONTROL Complete] ändern.</li> 
     <li>[!UICONTROL Automatisch]: Der Projektstatus ändert sich automatisch in [!UICONTROL Abgeschlossen], wenn alle Aufgaben im Projekt zu 100 % abgeschlossen sind und alle Probleme geschlossen sind.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bedingung]</td> 
   <td> <p>Dies ist eine visuelle Darstellung des Fortschritts einer Aufgabe, eines Problems oder eines Projekts.</p> <p>Bei Projekten kann die Bedingung vom Projekteigentümer manuell festgelegt werden oder automatisch durch [!DNL Workfront] festgelegt werden, basierend auf dem Fortschrittsstatus des Projekts. </p> <p>Die möglichen Werte für die Projektbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL on Target]</li> 
     <li>[!UICONTROL Risiko]</li> 
     <li>[!UICONTROL in Schwierigkeiten]</li> 
    </ul> <p>Weitere Informationen zu Projektbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Überblick über [!UICONTROL Projektbedingungen] und [!UICONTROL Bedingungstyp]</a>.</p>
     <p>Sie können Aufgaben- und Problembedingungen mit einer Zahl verknüpfen, die in Berichten angezeigt werden kann. In den folgenden Listen werden die Standardnamen und Zahlen für Aufgaben- und Problembedingungen angezeigt. Ihr Systemadministrator kann die Namen der Bedingungen aktualisieren und neue Bedingungen mit unterschiedlichen Zahlen hinzufügen. Nachdem eine Zahl mit einer Bedingung verknüpft wurde, kann sie nicht mehr bearbeitet werden.  </p> 
     <p>Bei Aufgaben wird die Bedingung vom Aufgabenbesitzer manuell festgelegt. Die möglichen Werte für die Aufgabenbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL Gehe reibungslos] (0)<br></li> 
     <li> [!UICONTROL Einige Bedenken] (1)<br></li> 
     <li>[!UICONTROL Wichtige Hindernisse] (2)</li> 
    </ul> <p>Weitere Informationen zu Aufgabenbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisieren der [!UICONTROL-Bedingung] für Aufgaben und Probleme</a>.</p> <p>Bei Problemen wird die Bedingung manuell vom Eigentümer des Problems festgelegt. Die möglichen Werte für die Problembedingung sind:<br></p> 
    <ul> 
     <li>[!UICONTROL Gehe reibungslos] (0)<br></li> 
     <li>[!UICONTROL Einige Bedenken] (1)<br></li> 
     <li>[!UICONTROL Wichtige Hindernisse] (2)</li> 
    </ul> 
   <p><b>NOTIZ</b></p>
    <p>Wenn das Feld [!UICONTROL Bedingung] in [!UICONTROL Journal Entry]-Berichten nachverfolgt wird, zeigen die Werte [!UICONTROL New] und [!UICONTROL Old Number Values] die mit der Bedingung verknüpfte Zahl anstelle ihres Namens an. Wenn eine Bedingung ursprünglich nicht für eine Aufgabe oder ein Problem definiert wurde und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den [!UICONTROL Old Number Value] des Felds [!UICONTROL Condition] als -2.147.483.648 an. Siehe auch "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]"und "[!UICONTROL Journal Entry]"in diesem Artikel. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bedingungsaktualisierung]</td> 
   <td> <p>In diesem Feld wird der aktuelle Zustand von Aufgaben, Projekten oder Problemen angezeigt. Diese Option zeigt die neuesten Updates, die die Eigentümer von Aufgaben, Projekten oder Problemen im Feld [!UICONTROL Aktualisierungsstatus] bereitgestellt haben, sowie die neue Bedingung an.</p> <p>Kommentare zu Bedingungsaktualisierungen werden nicht in der Spalte [!UICONTROL Bedingungsaktualisierung] angezeigt, sondern nur die Hauptaktualisierung.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected record types]</td> 
   <td> <p>In der Workfront-Planung können Sie eine Verbindung zwischen einem der folgenden Elemente erstellen: </p>
   <ul>
   <li>Zwei Datensatztypen</li>
   <li>Datensatz und Workfront-Objekttyp</li>
   <li>Datensatz-Typ und Adobe Experience Manager-Asset</li></ul>
   <p>Durch das Verbinden von Datensatztypen können Sie Informationen aus einem Datensatz oder Objekttyp in einem anderen Datensatztyp anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Übersicht über Connected Record Types</a>  </p>
  <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected records]</td> 
   <td> <p>Wenn Sie in der Workfront-Planung zwei Datensatztypen miteinander verbinden, können Sie zwei einzelne Datensätze dieser Typen miteinander verbinden.  </p>
   <p>Durch das Verbinden von Datensätzen können Sie Informationen aus einem Datensatz oder einem Objekt aus einer anderen Anwendung in einem anderen Datensatz anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Übersicht über Connected records</a>. </p>

<p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Verbindungen]</td> 
   <td> <p>In der Workfront-Planung beziehen sich Verbindungen auf verbundene Datensatztypen oder verbundene Datensätze. Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Beschränkungsdatum]</td> 
   <td> <p>Wenn Sie eine [!UICONTROL Task Constraint] verwenden, die an ein bestimmtes Datum gebunden ist, z. B. [!UICONTROL Must Start On], wird dieses spezifische Datum zum [!UICONTROL Constraint Date] der Aufgabe.</p> <p>Mit den folgenden Aufgabenbegrenzungen wird das Feld [!UICONTROL Constraint Date] aktualisiert:</p> 
    <ul> 
     <li>[!UICONTROL Muss am]</li> 
     <li>[!UICONTROL Muss abgeschlossen sein]</li> 
     <li>[!UICONTROL Start nicht später als]</li> 
     <li>[!UICONTROL Start nicht früher als]</li> 
    </ul> <p><b>TIPP</b></p>   
     <ul> 
      <li> <p>Eine Aufgabe mit einer [!UICONTROL Einschränkung] von [!UICONTROL Feste Datumswerte] hat kein [!UICONTROL Beschränkungsdatum]. </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] ist nur in einem Bericht oder einer benutzerdefinierten Ansicht sichtbar.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Wenn Sie eine Aufgabenbegrenzung in einer Vorlagenaufgabe verwenden, die an einen bestimmten Tag gebunden ist, z. B. Muss am beginnen, wird dieser bestimmte Tag zum Beschränkungstag der Vorlagenaufgabe.</p> <p>Mit den folgenden Aufgabenbegrenzungen wird das Feld [!UICONTROL Constraint Day] aktualisiert:</p> 
    <ul> 
     <li>[!UICONTROL Muss am]</li> 
     <li>[!UICONTROL Muss abgeschlossen sein]</li> 
     <li>[!UICONTROL Start nicht später als]</li> 
     <li>[!UICONTROL Start nicht früher als]</li> 
    </ul> <p><b>TIPP</b></p> <p>  [!UICONTROL Constraint Day] ist nur in einem Bericht oder einer benutzerdefinierten Ansicht sichtbar. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Begrenzungstyp]</td> 
   <td> <p>Die Planungstendenz einer Aufgabe. [!UICONTROL Planen Sie beispielsweise so bald wie möglich], dass eine Aufgabe so bald wie möglich beginnt und [!UICONTROL Später als beenden] eine Aufgabe so planen wird, dass sie bis zum [!UICONTROL Begrenzungsdatum] beendet wird und nicht später.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kontextmenü]</td> 
   <td>Ein Menü auf der linken Bildschirmseite, in dem die Elemente geändert werden, um sie mit dem aktiven Inhalt zu korrelieren. Wenn ein Benutzer beispielsweise ein Projekt anzeigt, zeigt das [!UICONTROL Kontextmenü] Links zu projektbezogenen Informationen und Tools an.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Ein Feld in einem Projekt- oder Aufgabenbericht, das Informationen über den Benutzer anzeigt, der der [!UICONTROL Primäre Kontakt] eines Problems ist, wenn das Problem in ein Projekt oder eine Aufgabe konvertiert wird. Das Feld wird auch im Abschnitt [!UICONTROL Projektdetails] angezeigt, in dem der Name des [!UICONTROL Primären Kontakts] des konvertierten Problems angezeigt wird. Siehe auch "[!UICONTROL Primärer Kontakt]"in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Der Geldbetrag, den Sie beim Abschluss eines Projekts, einer Aufgabe oder eines Problems ausgeben müssen. </p> <p>Sie können verschiedene Arten von Kosten für Arbeit, Ausgaben und Risiken im Zusammenhang mit dem Projekt nachverfolgen. Informationen zu Nachverfolgungskosten in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Kosten verfolgen</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kostentyp]</td> 
   <td>Für eine Aufgabe bestimmt der [!UICONTROL Kostentyp], wie die Aufgabe Kosten anfällt. Einige Beispiele sind [!UICONTROL Fest Stündlich], [!UICONTROL Benutzer Stündlich] und [!UICONTROL Benutzer Stündlich plus Fest]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektübergreifende Abhängigkeiten]</td> 
   <td> <p>Eine Aufgabe eines Projekts hängt von einer Aufgabe eines anderen Projekts ab.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Erstellen projektübergreifender Vorgänger</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefinierte Daten]</td> 
   <td> <p>Daten, die für eine Organisation eindeutig sind. Unternehmen können die Anwendung [!DNL Workfront] anpassen, indem sie benutzerdefinierte Formulare und benutzerdefinierte Felder erstellen. Diese benutzerdefinierten Informationen können die Berichterstellung für KPIs, die Prüfung und den Nachfragemix fördern. </p> <p>[!UICONTROL Benutzerdefinierte Daten] können mit folgenden Elementen verknüpft werden:</p> 
    <ul> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Benutzer]</li> 
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
   <td>[!UICONTROL Benutzerdefinierter Datentyp]</td> 
   <td>Die Option, um anzugeben, ob ein [!UICONTROL Benutzerdefinierte Daten]-Feld als Text, Datum, Zahl oder Währung in der Datenbank gespeichert wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierter Anzeigetyp]</td> 
   <td>Der Feldanzeigetyp eines benutzerdefinierten Felds. Beispiele sind [!UICONTROL Dropdown], [!UICONTROL Textfeld], [!UICONTROL Textbereich], [!UICONTROL Optionsfelder] usw.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefiniertes Feld]</td> 
   <td>Bei benutzerdefinierten Daten, die es dem Benutzer ermöglichen, aus mehreren Optionen auszuwählen, handelt es sich um die Werte, aus denen der Benutzer auswählen kann. Benutzerdefinierte Optionen sind nur in [!UICONTROL Dropdown], [!UICONTROL Dropdown für mehrere Auswahlen], [!UICONTROL Optionsfelder] und [!UICONTROL Kontrollkästchen] gültig.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Bei Verwendung eines benutzerdefinierten Anzeigetyps mit benutzerdefinierten Optionen ist dies der Text der Benutzeroberfläche, der im Dropdown-Menü, in den Kontrollkästchen oder im Optionsfeld für diese benutzerdefinierte Option angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierter Wert]</td> 
   <td>Bei Verwendung eines benutzerdefinierten Felds mit benutzerdefinierten Optionen ist dies der Wert, der für eine bestimmte Option in der Datenbank gespeichert wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierte Ansicht]</td> 
   <td>Eine Definition der Datenfelder oder Spalten, die für jedes Objekt in einer Liste angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Eine Organisation, die eine Instanz von Workfront verwendet.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

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
   <td> <p> Sie können dieses Feld zu einem Bericht oder einer Ansicht des Berichtsobjekts hinzufügen, um die Dashboards anzuzeigen, in denen der Bericht in einer Liste aufgeführt ist. </p> <p> Mit diesem Feld können Sie auch nach Berichten filtern, die in einem bestimmten Dashboard aufgeführt sind. </p> <p> Weitere Informationen zum Einbeziehen von Dashboard-Informationen in Berichtobjektberichte finden Sie im Abschnitt "Grundlegendes zu den Berichten in Dashboards"im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Zugriff auf und Organisieren von Berichten</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datentyp]</td> 
   <td>Siehe [!UICONTROL Benutzerdefinierter Datentyp].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tage verspätet]</td> 
   <td> <p>In diesem Feld wird ein Datumsunterschied zwischen [!UICONTROL Geplanter Start] und [!UICONTROL Today] angezeigt, wenn das [!UICONTROL Tatsächliche Abschlussdatum] fehlt.</p> <p>Zeigt außerdem einen Datumsunterschied zwischen [!UICONTROL Tatsächlicher Abschluss] und [!UICONTROL geplanter Abschluss] an, wenn ein [!UICONTROL tatsächlicher Abschlussdatum] vorhanden ist.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Standardzeitplan]</td> 
   <td> <p>Anpassbare Standard-Arbeitszeiten, die Benutzern und Projekten in einer Organisation zugewiesen werden können. </p> <p>Mit Zeitplänen werden die geplanten, Start- und Enddaten von Aufgaben berechnet, die Benutzern zugewiesen werden.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Zustellbar]</td> 
   <td>Quantitative Güter oder Dienstleistungen, die nach Abschluss eines Projekts erbracht werden müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Bewertung und Priorisierung der Aufnahmeprozesse.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Hauptziele]</td> 
   <td>Ziele, die sich auf eine bestimmte Abteilung beziehen und sich auf die Verbesserung der operativen Metriken innerhalb der Abteilung konzentrieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abhängigkeit]</td> 
   <td>Die Verknüpfung zwischen zwei Aufgaben, bei denen eine Aufgabe den Status vor der anderen ändern muss, kann ebenfalls den Status ändern.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abhängigkeitstyp]</td> 
   <td> <p>Die Art der Planungsbeziehung zwischen einer Aufgabe und ihren Vorgängern. Ein Beispiel ist [!UICONTROL Finish-Start]. Dies erfordert, dass die erste Aufgabe abgeschlossen sein muss, bevor die zweite Aufgabe gestartet werden kann.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Übersicht über Aufgabenabhängigkeitstypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Jede Datei, die mit einem Objekt in [!DNL Workfront] verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokumentversion]</td> 
   <td> <p>Jedes Mal, wenn dasselbe Dokument in dasselbe Objekt hochgeladen wird, wird ihm eine Versionsnummer zugewiesen. Benutzer können mehrere Optionen für eine frühere Version eines Dokuments anzeigen und ändern.</p> <p>Weitere Informationen finden Sie unter <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Dokumentversionen verwalten</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe oder ein Problem abgeschlossen werden soll. Das Fälligkeitsdatum einer Aufgabe oder eines Problems ist dasselbe Datum wie das geplante Abschlussdatum.</p>
    <p>Die Aufgabe und das Problem Fälligkeitsdatum sind in den Aufgaben- und Problemlisten und Berichten sichtbar.</p> 
    <p>Siehe auch Geplantes Abschlussdatum in dieser Tabelle. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer]</td> 
   <td> <p>Das Zeitfenster, das für den Abschluss eines Aufgabenproblems oder Projekts zugewiesen wird (bestimmt durch die Anzahl der Tage zwischen dem geplanten Start von [!UICONTROL und dem geplanten Abschluss).</p> 
    <ul> 
     <li>Bei Aufgaben ist die Dauer ein editierbares Feld, wenn die Dauer der Aufgabe nicht einfach ist. Wenn der Aufgabentyp einfach ist oder die Aufgabenbegrenzung feste Datumswerte ist, wird die Dauer von Workfront berechnet.</li> 
     <li>Bei Problemen ist die Dauer immer ein bearbeitbares Feld und sollte eine Schätzung einer Anzahl von Tagen darstellen, für die das Problem behoben werden muss.</li> 
     <li>Bei Projekten ist die Dauer eine von [!DNL Workfront] vorgenommene Berechnung und stellt den Unterschied in Tagen zwischen dem geplanten Beginn der frühesten Aufgabe und dem geplanten [!UICONTROL Abschluss] der letzten Aufgabe im Projekt dar.</li> 
    </ul> <p>Weitere Informationen zum Unterschied zwischen [!UICONTROL Dauer] und [!UICONTROL Geplante Dauer] für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Unterschied zwischen [!UICONTROL Geplante Dauer] und [!UICONTROL Dauer] für Aufgaben</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer in Minuten]</td> 
   <td>In diesem Feld werden dieselben Informationen wie im Feld [!UICONTROL Dauer] in Minuten statt in Tagen angezeigt. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Dauer pro Vorfall]</td> 
   <td> <p>Dies wird in den Feldern [!UICONTROL Task Details] und [!UICONTROL Aufgabe bearbeiten] eines übergeordneten Elements wiederkehrender Aufgaben angezeigt. Es zeigt die Dauer jeder wiederkehrenden Aufgabe an. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Erstellen wiederkehrender Aufgaben</a>. </p> <p> <span>Die in einzelnen wiederkehrenden Aufgaben geänderten Zeiträume zeigen nicht den in diesem Feld angegebenen Wert an.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Ein Aufgabenfeld, das anzeigt, wie die zum Abschließen der Aufgabe erforderliche Arbeit den Bevollmächtigten über die Dauer der Aufgabe hinweg zugewiesen wird. Es stellt die Beziehung zwischen der [!UICONTROL Dauer] der Aufgabe, der [!UICONTROL Arbeit erforderlich] und der Zeitdauer (oder [!UICONTROL Zuordnung]) dar, die die zugewiesenen Ressourcen für die Aufgabe ausgeben sollten, um sie abzuschließen. </p> <p>Dieses Feld wird auf der Registerkarte [!UICONTROL Details] einer Aufgabe angezeigt. </p> <p>Für den Aufgabentyp stehen folgende Optionen zur Verfügung:</p> 
    <ul> 
     <li>[!UICONTROL Berechnete Zuweisung]</li> 
     <li>[!UICONTROL Berechnete Arbeit]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Dauer] und [!UICONTROL Dauer Typ]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>Die Einheit, die verwendet wird, um die Zeit in einer Stromsuche zu messen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>Die Beziehung zwischen der Anzahl der Benutzer und der Dauer, die die Aufgabe abschließen muss. Wenn Sie weitere Benutzer hinzufügen, verringert sich die für den Abschluss der Aufgabe geplante Gesamtdauer, die Dauer der Aufgabe bleibt jedoch gleich. Wenn beispielsweise eine Aufgabe ein Barrel Erdnüsse schüttelt, wird durch das Hinzufügen von mehr Personen die geplante Zeit verkürzt, aber die Dauer in Personentagen bleibt gleich.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vergangene Zeit]</td> 
   <td> <p>[!UICONTROL Vergangene Zeit] ist eine Zeiteinheit für die [!UICONTROL Dauer] einer Aufgabe. Dies ist die Zeit zwischen dem geplanten [!UICONTROL Startdatum] und dem geplanten [!UICONTROL Abschlussdatum] einer Aufgabe, die Feiertage, Wochenenden und eine Verspätung umfasst. Mit anderen Worten, vergangene Zeit ist der Durchgang von Kalendertagen. </p> <p>[!DNL Workfront] unterstützt die folgenden verstrichenen Zeiteinheiten für die Aufgabendauer:</p> 
    <ul> 
     <li> <p>[!UICONTROL Vergangene Minuten]</p> </li> 
     <li> <p>[!UICONTROL Vergangene Stunden]</p> </li> 
     <li> <p>[!UICONTROL Vergangene Tage]</p> </li> 
     <li> <p>Vergangene Wochen]</p> </li> 
     <li> <p>[!UICONTROL Vergangene Monate]</p> </li> 
    </ul> <p>Weitere Informationen zur Aufgabendauer, einschließlich der verstrichenen Zeit, finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Dauer] und [!UICONTROL Dauer Typ]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> In einem [!UICONTROL Rate] -Bericht ist dies das Datum, an dem ein neuer Abrechnungskurs für eine Stellenrolle auf Projektebene endet. Die dem Projekt zugeordneten Stunden, die vor diesem Datum liegen, werden mit diesem Abrechnungskurs multipliziert, um den Umsatz für das Projekt zu berechnen. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Einsatz]</td> 
   <td>Der [!UICONTROL Work Performance Indicator] (WPI), der anzeigt, wann das Engagement und der Glaube an die Aufgabe, das Projekt, das Team oder die Organisation abnimmt. Dies zeigt, dass Sie handeln müssen, um diesen Glauben und diese Verpflichtung wiederzubeleben. WPIs würden anhand der einfachen Fragen gemessen: "Haben Sie verstanden, was von Ihnen erwartet wurde? Hat die Arbeit, die Ihnen zugewiesen wurde, etwas für die Organisation bewirkt? Habt ihr großartige Arbeit geleistet?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Unternehmensziele]</td> 
   <td>Funktionsübergreifende Ziele, die zur Metrik der Unternehmensziele beitragen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Jede Änderung an einem Projekt oder einer Aufgabe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Automatisierte Aufgaben, die auftreten, wenn Ereignisse stattfinden. Ein häufiges Beispiel ist eine automatisierte E-Mail-Benachrichtigung.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignisbenachrichtigung]</td> 
   <td>E-Mail, die von einem Ereignishandler generiert wird.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td>Arbeitslose Kosten für Aufgaben oder Projekte.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>Normalerweise handelt es sich hierbei um einen Lizenztyp oder einen Benutzer mit einer solchen Lizenz. Ein Benutzer mit einem solchen Lizenztyp kann nur Informationen im System überprüfen. Sie können sich nicht aktiv an der Arbeit beteiligen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Lizenzübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externes System]</td> 
   <td>Alle Dienste oder Software, die außerhalb des vorgesehenen Datensatzsystems gespeichert und verwaltet werden.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Jedes Workfront-Objekt oder die mit ihm verknüpften Informationen, wie es in der Datenbank angezeigt wird. </p>
   <p>Beispielsweise sind "project", "user", "hour" sowohl Workfront-Objekte als auch -Felder. "Name", "Status", "Eigentümer", "Startdatum"sind Workfront-Felder, die mit den oben genannten Objekten verknüpft sind. </p>

<p>Beim Verweis auf Objekte können die Begriffe "Objekte"und "Felder"austauschbar verwendet werden.</p>
   <p>Im Berichtsbereich beziehen sich die "Felder"auf die Objekte oder Informationen über das Objekt, das Sie im Bericht erfassen möchten.</p>

<p><b>NOTIZ</b></p>

<p>Bei der Berichterstellung für mehr Text beziehen sich Felder auf die Objekte oder deren Informationen, wie sie in der Datenbank angezeigt werden.</p>
   <p>Manchmal unterscheidet sich der in der Benutzeroberfläche angezeigte Name vom Namen des Felds in der Datenbank. Beispielsweise ist "issue"der Name des Objekts in der Workfront-Benutzeroberfläche, "opTask"ist jedoch der Name des Objekts (oder des Felds) in der Workfront-Datenbank. </p> 
   <p> Es ist wichtig, das Feld so zu verwenden, wie es in der Datenbank angezeigt wird, wenn Sie einen Textmodusbericht, eine Ansicht, einen Filter oder eine Gruppierung erstellen oder wenn Sie ein berechnetes Feld erstellen.</p>

<p>Weitere Informationen finden Sie unter <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> und <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Textmodus - Übersicht</a>.</p>

<p>Standardmäßig enthält Workfront eine Reihe von Feldern, die beide Objekte und ihre Informationen definieren. Sie können auch benutzerdefinierte Felder erstellen, um Objekte zu definieren, jedoch keine benutzerdefinierten Objekte erstellen.</p>

<p>In der Workfront-Planung können Sie benutzerdefinierte Felder für alle Datensatztypen erstellen. Workfront-Datensatztypen verfügen über eine sehr begrenzte Anzahl von Feldern. Sie müssen alle Felder von Grund auf neu erstellen und sie mit Datensatztypen verknüpfen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/fields/fields-overview.md">Feldübersicht</a>. </p> <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Einer der Hauptbausteine eines Berichts oder eines Listenelements, das bestimmt, welche Informationen auf dem Bildschirm angezeigt werden. Weitere Informationen zu Berichterstellungselementen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> <p>Der Filter bestimmt die Ergebnisse, die in einem Bericht oder in einer Liste mit einem [!DNL Workfront] -Bedienfeld angezeigt werden, z. B. Projekte, Aufgaben oder Probleme.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Prozess zum Verwalten von Arbeits-, Ausgaben- und Umsatzdaten in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Feste Kosten]</td> 
   <td>Sie können einen festen Kostenbetrag für ein Projekt definieren. Dies ist Teil der [!UICONTROL Plankosten] des Projekts, die den Geldbetrag darstellen, den Sie zum Abschluss des Projekts benötigen. Informationen zu Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten-Tracking</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fester Umsatz]</td> 
   <td>Sie können einen festen Umsatzbetrag für ein Projekt definieren. Dies ist Teil des [!UICONTROL Planen Umsatzes] des Projekts, der den Geldbetrag darstellt, den Sie erhalten könnten, wenn Sie das Projekt abschließen. Informationen zum Umsatz finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Dies ist dasselbe Feld wie [!UICONTROL Status Icons], es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL Vorlagen] </li> 
     <li> [!UICONTROL Ausgaben] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner]</td> 
   <td>Ordner dienen zum Organisieren von Dokumenten oder Berichten, die mit einem Objekt verknüpft sind.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Vollzeitäquivalent)</td> 
   <td>Dies ist das Vollzeitäquivalent, das angibt, wie viel Zeit eine Ressource für die Arbeit zur Verfügung steht. 
   Das Feld [!UICONTROL FTE] wird in den folgenden Bereichen angezeigt: 
  <ul>
   <li> Benutzerprofil beim Bearbeiten oder Erstellen des Benutzers </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Szenario-Planer] (erfordert zusätzliche Lizenz für den Workfront-Szenario-Planer) </li>
   <li> Benutzerlisten und Berichte </li> </ul>

<p>Die [!UICONTROL FTE] muss eine Dezimalzahl von bis zu 1 sein und darf nicht 0 sein. </p>
   <p> Eine [!UICONTROL FTE] von 1 (die Standardeinstellung für das [!UICONTROL FTE]-Feld eines Benutzers, wie in seinem Profil definiert) bedeutet, dass eine Ressource (Benutzer oder Rolle) die gesamte Anzahl von Stunden ausführt, basierend auf dem Zeitplan, der die Verfügbarkeit berechnet. </p>
   <p>Ihr Workfront-Administrator entscheidet, welcher Zeitplan zur Bestimmung der Benutzerverfügbarkeit verwendet werden soll.  </p>
   <ul>
   <li> Wenn der [!UICONTROL Standardzeitplan] verwendet wird, verwendet Workfront die [!UICONTROL FTE] des in seinem Profil gefundenen Benutzers, um die Verfügbarkeit zu berechnen. </li>
   <li> Wenn der Benutzerzeitplan verwendet wird, verwendet Workfront die Zeitdauer des Benutzers, den [!UICONTROL Arbeitszeitwert] und die Stunden des [!UICONTROL Standardzeitplans], um die [!UICONTROL FTE] des Benutzers zu berechnen. </li> </ul>

<p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.  </p>
   <p>Weitere Informationen zum Erstellen von Zeitplänen in [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>

<p><b>NOTIZ</b></p>
   <p>Für alle Berechnungen im [!UICONTROL Szenario-Planer] verwendet Workfront den folgenden Wert: 1 [!UICONTROL FTE] = 8 Stunden.</p>
   <p>Weitere Informationen finden Sie unter <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Erste Schritte mit dem [!UICONTROL Szenario-Planer]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

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
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Eine visuelle Zeitleiste des Projekts datiert in einer Kalenderansicht basierend auf den geplanten oder geplanten Daten, da die Aufgaben des Projekts derzeit geplant sind.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ziel]</td> 
   <td><p>In [!DNL Workfront] gibt es zwei Konzepte für Ziele: </p> 
    <ul> 
     <li> <p><b>Projektziele</b>: Eine Reihe von Geschäftszielen, die von den relevanten Interessengruppen eines Projekts vereinbart wurden. Projektziele sind Teil des Business Case eines Projekts. </p> <p>Projektziele können nicht in Listen oder Berichten angezeigt werden, Sie können aber über die API darauf zugreifen. </p> <p>Weitere Informationen zu den Projektzielen von Business Case finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Ziele für Geschäftsfälle erstellen </a>. </p> </li> 
     <li> <p><b>Strategische Ziele</b>: Ein strategisches Ziel ist ein Ziel, das Sie zur Planung Ihrer Arbeitsstrategie für einen bestimmten Zeitraum erstellen. Sie können diese Arten von Zielen mit [!DNL Workfront Goals] erstellen. Ihre Organisation muss eine zusätzliche Lizenz erwerben und Sie müssen Zugriff auf diese Funktion haben, um strategische Ziele erreichen zu können. [!DNL Workfront Goals] sind nur mit einer zusätzlichen Lizenz verfügbar.</p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] Übersicht </a>. </p> 
     <p>Sie können strategische Ziele in einem Ziel oder Projektbericht anzeigen und über die API darauf zugreifen. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Zielhierarchie]</td> 
   <td> <p>In den Berichten [!UICONTROL Ziel] und [!UICONTROL Projekt] ist dies ein Erfassungsfeld, das die Ziele in der Hierarchie anzeigt, zu denen ein strategisches Ziel gehört, wenn es an anderen Zielen ausgerichtet ist. Die Ziele werden durch ein System-Trennzeichen voneinander getrennt. </p> <p>Nur die übergeordneten Elemente des Ziels und des Ziels werden in diesem Feld angezeigt. Untergeordnete Ziele werden nicht angezeigt. </p> <p>Informationen zum Ausrichten von Zielen in [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Übersicht über die Zielausrichtung in [!DNL Workfront Goals]</a>. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] Übersicht </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ziel-Erfolgsbewertung]</td> 
   <td> In einem [!UICONTROL Projektbericht] verwies dieses Feld auf Projektziele im Zusammenhang mit dem [!UICONTROL Business] Case. Derzeit ist dieses Feld veraltet und mit keiner Funktion verknüpft.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziele] </td> 
   <td> <p>In einem [!UICONTROL Projekt]-Bericht ist dies ein Erfassungsfeld, das alle strategischen Ziele anzeigt, die mit einem Projekt verbunden sind. Die Ziele werden durch Kommas getrennt.</p> <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] Übersicht</a>. Weitere Informationen zu strategischen Zielen und Projektzielen in [!DNL Workfront] finden Sie unter "[!UICONTROL Ziel]"in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Schnittstellenvoreinstellungen]</td> 
   <td>Einstellungen der Benutzeroberfläche, die alle Benutzer betreffen. [!UICONTROL Globale Schnittstellenvoreinstellungen] können über die [!UICONTROL Benutzeroberflächenvoreinstellungen] überschrieben werden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Eine Sammlung von Benutzern (möglicherweise aus derselben Abteilung oder Geschäftseinheit), die Zugriff auf dieselben Objekte haben. Zusätzlich zu den Benutzern können Gruppen mit Portfolios, Programmen, Projekten,<span> Projektvorlagen,</span> Unternehmen, Teams, Zeitplänen, Layoutvorlagen und Timesheet-Profilen verknüpft werden.</p> <p>Sie können auch Berechtigungen für Objekte nach Gruppe gewähren. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> <p>In einer Liste oder einem Bericht mit Objekten eines der folgenden Typen können Sie im Feld [!UICONTROL Group] auflisten, welche Objekte dieses Typs einer bestimmten Gruppe zugeordnet sind: Benutzer, Portfolio, Programm, Projekt, <span>Projektvorlage</span>, Unternehmen, Team, Zeitplan, Layoutvorlage oder Timesheet-Profil.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gruppenadministrator]</td> 
   <td> <p>Benutzer, die die Objekte, Zugriffe und Benutzer bestimmter Benutzergruppen verwalten.</p> <p> In einem [!UICONTROL Group] -Bericht werden in diesem Feld die Namen der Benutzer angezeigt, die in der Gruppe als [!UICONTROL Gruppenadministratoren] bezeichnet wurden. Weitere Informationen zu Gruppenadministratoren finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gruppe mit Administratorzugriff]</td> 
   <td> <p> In einem [!UICONTROL Layout Template]-, [!UICONTROL Timesheet Profile]- oder [!UICONTROL Schedule report] zeigt dieses Feld die Gruppen an, deren Gruppenadministratoren Zugriff auf die Änderung der Vorlage haben. Sie können diesen Bericht auch nach diesem Feld filtern. </p> <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gruppierung]</td> 
   <td> <p>Ein Berichterstellungselement, mit dem Informationen in einer Liste nach einem gemeinsamen Kriterium kategorisiert werden.</p> <p>Weitere Informationen finden Sie im Abschnitt "[!UICONTROL Gruppings]"im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übermittlungsdatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe zur Arbeit verfügbar wird. Das [!UICONTROL Übermittlungsdatum] ist eine Berechnung und kann nicht manuell festgelegt werden. <br>Weitere Informationen zum [!UICONTROL Übergabedatum] finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Ein alternativer Name zur Beschreibung des Bereichs [!UICONTROL Requests] von [!DNL Workfront]. Im Bereich [!UICONTROL Requests] können Sie Support-Tickets, Projektanfragen, Helpdesk-Tickets usw. verarbeiten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inhaber]</td> 
   <td>In einem [!UICONTROL Stunden] Bericht ist der [!UICONTROL Inhaber] der Benutzer, dem die Stunden zugeordnet werden. Dies unterscheidet sich von dem Benutzer, der die Zeit tatsächlich protokolliert. Diese beiden Entitäten können manchmal zwei verschiedene Benutzer sein. <br>Weitere Informationen zur Protokollierungszeit für einen anderen Benutzer finden Sie im Artikel <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Protokollzeit</a>.</td> 
  </tr>

<tr> 
   <td>Stundenstatus</td> 
   <td> <p>Ein von Workfront für die tatsächlichen Zeiten festgelegtes Attribut, das Benutzer für Aufgaben, Probleme oder Projekte protokollieren. </p>

Stündeinträge können in Workfront einen der folgenden Status aufweisen:
<ul>
   <li><b>Gesendet</b>: Die Stunden wurden bei einem Projekt, einer Aufgabe oder einem Problem protokolliert. Sie sind entweder Teil eines Rechnungsdatensatzes oder noch nicht zu einem Rechnungsdatensatz hinzugefügt.</li>
   <li><b>Genehmigt</b>: Die Stunden wurden protokolliert und vom Projekteigentümer genehmigt. Sie sind entweder Teil eines Rechnungsdatensatzes oder noch nicht zu einem Rechnungsdatensatz hinzugefügt.</li> 
   <li><b>Nicht genehmigt</b>: Die Stunden wurden vom Projekteigentümer protokolliert und abgelehnt. Sie sind entweder Teil eines Rechnungsdatensatzes oder noch nicht zu einem Rechnungsdatensatz hinzugefügt.</li>
   <li><b>Abgerechnet</b>: Die Stunden wurden protokolliert, zu einem Abrechnungsdatensatz hinzugefügt und der Status des Abrechnungsdatensatzes wurde als Abgerechnet markiert. Sie mussten nicht vom Projekteigentümer genehmigt werden.</li>
   <li><b>Abgerechnet und genehmigt</b>: Die Stunden wurden protokolliert, vom Projekteigentümer genehmigt und der Status des Abrechnungsdatensatzes wurde als Abgerechnet markiert.</li>
   </ul>

<p>Wenn Stunden Teil eines Abrechnungsdatensatzes sind, zeigt der Status Stunde an, ob die Stunden genehmigt wurden oder ob der Abrechnungsdatensatz, zu dem sie gehören, in Rechnung gestellt wurde. Der Stundenstatus eines Stundeneintrags wird nur in einer Stundenliste oder einem Bericht angezeigt. </p>

<p>Weitere Informationen zum Hinzufügen von Stunden zu Rechnungsdatensätzen finden Sie im Abschnitt "Hinzufügen von Stunden zu Rechnungsdatensätzen"im Artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Erstellen von Rechnungsdatensätzen</a>.</p>

<p>Weitere Informationen zum Genehmigen der Zeit für Projekte finden Sie unter <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Genehmigung der Zeit für ein Projekt erforderlich</a>.</p>

<p><b>TIPP</b></p>

<p>Allgemeine Stunden, die nicht direkt bei Arbeitselementen protokolliert werden, zeigen keinen Stundenstatus an. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Stündentyp]</td> 
   <td> <p>Ein Attribut, das für die tatsächlichen Stunden festgelegt werden kann, die Benutzer für Aufgaben, Probleme oder Projekte protokollieren. Dies ist auch ein Attribut für die protokollierten Stunden, die nicht direkt mit der Arbeit verbunden sind, wie [!UICONTROL Urlaub] und [!UICONTROL Time Off].</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Verwalten von Stundentypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Die ID ist ein alphanumerischer Indikator, der mit jedem Objekt in [!DNL Workfront] verknüpft ist. Sie identifiziert jedes Objekt in der [!DNL Workfront]-Datenbank eindeutig. Sie können die ID eines beliebigen Objekts in einem Bericht oder in einer Liste für jedes Objekt anzeigen. </p> <p><b>TIPP</b></p>   <p>Sie können die ID auch in der URL der Objektseite anzeigen. Beispielsweise könnte die Kennung eines Projekts etwa wie die in der folgenden URL angegebene Zahl aussehen, wenn Sie auf die Seite [!UICONTROL Projektdetails] zugreifen:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individuelle Ziele]</td> 
   <td>Einzelne Ziele, die zur Metrik der Teamziele beitragen, aber nicht mit der persönlichen oder beruflichen Entwicklung in Zusammenhang stehen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Vererbter Zugriff]</td> 
   <td>Freigabefunktion, die den Zugriff auf die Übertragung von einem Objekt auf ein anderes ermöglicht. Beispielsweise der in Programm- und Portfoliodatensätzen definierte Erbzugriff des Projektnutzers.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>In der [!DNL Workfront Scenario Planner] können Sie einen Plan in mehrere Initiativen unterteilen, um die Verwaltung des Plans zu vereinfachen. <span>Sie können einen [!UICONTROL Initiative]-Bericht erstellen und auf [!UICONTROL Initiative]-Informationen in einem [!UICONTROL Project]-Bericht zugreifen.</span></p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick [!DNL Scenario Planner]</a>. </p> <p>Der Bericht [!DNL Initiative] ist in Ihrer [!DNL Workfront] -Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat. Sie können nicht über die API auf [!UICONTROL Initiativen] zugreifen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>Der Berichtstyp [!UICONTROL Initiative Job Role] zeigt Informationen zu den Stellenrollen an, die mit einer Planinitiative in der [!DNL Workfront Scenario Planner]</span> verknüpft sind. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Scenario Planner]</a>. </p> <p><span>Dieser Berichtstyp ist in Ihrer [!DNL Workfront] -Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> In einem [!UICONTROL Initiative Job Role]-Bericht wird die Anzahl der Stunden angezeigt, die einer Stellenrolle in einer Initiative zugeordnet sind.</span> </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Scenario Planner]</a>. </p> <p>Dieses Feld und der Berichtstyp [!UICONTROL Initiative Job Role] sind in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>In einem [!UICONTROL Initiative Job Role] -Bericht wird die Anzahl der spezifischen Arbeitsplatzrollen angezeigt, die mit einer Initiative verbunden sind.</p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Scenario Planner]</a>. </p> <p>Dieses Feld und der Berichtstyp [!UICONTROL Initiative Job Role] sind in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative - Letztes Veröffentlichungsdatum]</td> 
   <td> <p>In einem Feld in einem [!UICONTROL Initiative]-, [!UICONTROL Initiative Job Role]- und [!UICONTROL Project]-Bericht wird das Datum angezeigt, an dem eine Planinitiative zuletzt in einem Projekt veröffentlicht wurde. Sie können Initiativen veröffentlichen, um Projekte zu erstellen oder Projekte zu aktualisieren, die mit den Initiativen in Verbindung stehen.</p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Scenario Planner]</a>. </p> <p><span>Informationen zu Veröffentlichungsinitiativen finden Sie unter </span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publish-Szenarien zum Erstellen und Aktualisieren von Projekten in der [!DNL Workfront Scenario Planner]</a>. Dieses Feld ist in Ihrer [!DNL Workfront] -Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>Eine Suche, die während des Ausfüllens eines Formulars durchgeführt wird, um mögliche Einträge für ein bestimmtes Feld zu finden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface-Einrichtung]</td> 
   <td>Der Bereich der Anwendung, der die Definition benutzerdefinierter Ansichten, Filter, Gruppierungen, Listen-Steuerelemente usw. ermöglicht.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Ist Unternehmensziel]</p></td> 
   <td> <p>In [!DNL goal reports] wird für jedes strategische Ziel der Wert "[!UICONTROL True]/ [!UICONTROL False]"angezeigt, um anzugeben, ob Ihr Unternehmen dem Ziel als Eigentümer zugewiesen ist. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] Übersicht </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problem]</td> 
   <td> <p>Ein ungeplantes Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Es wird für die weitere Berücksichtigung des Arbeitsaufwands getestet und bewertet</p> <p>Ein [!UICONTROL Problem] kann auch eine [!UICONTROL Help Desk]-Anfrage sein. [!UICONTROL Änderungsaufträge], [!UICONTROL Anforderungen] und [!UICONTROL Fehler] sind ebenfalls [!UICONTROL Probleme].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problemverwaltung]</td> 
   <td> <p>Der Prozess und die Regeln für die Definition der Ausgabetypen und des Routing-, Test- oder Traffic-Prozesses für jeden Typ.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Projekteigentümer]</td> 
   <td>Das Team oder die Benutzer, die für das Testen und Abschließen eines Problems verantwortlich sind.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Ein Zeitraum, in dem ein Team einen vordefinierten Satz von Lieferzielen erzeugt.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

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
   <td>[!UICONTROL Auftragsrolle]</td> 
   <td> <p>Dient zur Identifizierung der täglichen Arbeitsfunktionen und -aufgaben eines Benutzers. Den Arbeitselementen können Vorgangsrollen zugewiesen werden, um die erforderlichen Kenntnisse für den Abschluss eines Arbeitsprozesses zu identifizieren, ohne ihn einem bestimmten Benutzer zuzuweisen. </p> <p>Ein Benutzer kann mehrere Rollen haben. Beispiele sind Graphic Designer oder Consultant.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journaleintrag]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Informationen über Systemaktualisierungen für getrackte Felder angibt, die im Bereich [!UICONTROL Updates] von Projekten, Aufgaben, Problemen und anderen Objekten angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Bericht über den [!UICONTROL Updates]-Bereich</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>In einem [!UICONTROL Task] Report oder [!UICONTROL Issue] Report zeigt das Feld [!UICONTROL Kanban Flag] den Flaggenstatus an, der auf dem [!UICONTROL Kanban Board] festgelegt ist. Mögliche Werte sind [!UICONTROL On Track], [!UICONTROL Ready to Pull] und [!UICONTROL Is Blocked].</p> <p>Weitere Informationen zum Festlegen des Flaggenstatus für Meldungen im [!UICONTROL Kanban Story Board] finden Sie unter  den Artikel <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Verwenden Sie Flags auf Geschichten auf der [!UICONTROL Kanban-Pinnwand]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Ein messbarer Wert, der zeigt, wie effektiv ein Unternehmen wichtige Geschäftsziele erreicht.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Die Zeit, die vergehen muss, nachdem das geplante [!UICONTROL Abschlussdatum] der Vorgängeraufgabe verstrichen ist, bis die abhängige Aufgabe beginnen kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>Die Methode zur Berechnung der [!UICONTROL Lag]. Er kann:</p> 
    <ul> 
     <li>[!UICONTROL Tage] (Arbeitstage)</li> 
     <li>[!UICONTROL Kalendertage] (Feiertage ignorieren)</li> 
     <li>[!UICONTROL Prozent]</li> 
     <li>[!UICONTROL Wochentag]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Übersicht über Lag-Typen</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Große Miniaturansicht]</td> 
   <td> <p> In einer [!UICONTROL Dokument]-Liste oder einem Bericht wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p>Wählen Sie <strong>[!UICONTROL Große Miniaturansicht]</strong> aus, um eine 400 Pixel breite Miniaturansicht im Bericht anzuzeigen.</p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch "[!UICONTROL Thumbnail]"in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte 10 Viewer]</td> 
   <td> <p>In einer Berichtsliste werden in diesem Feld die Namen von bis zu 10 Benutzern angezeigt, die den Bericht zuletzt angesehen haben.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte Bedingungshinweise]</td> 
   <td> <p>In diesem Feld wird die zuletzt vom Eigentümer des Objekts in ein Objekt eingegebene Aktualisierung angezeigt. Dies ist die letzte Aktivität oder Interaktion des Eigentümers für ein Objekt.</p> <p>Die Spalte "[!DNL Last Condition Note]" ist leer, wenn der Text der Notiz der letzten Anmerkung eines Objekts gelöscht wurde. Wenn eine neue Anmerkung auf dem Objekt eingegeben wird, wird sie zur letzten Anmerkung und wird erneut in der Spalte angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letztes Aktualisierungsdatum der Finanzverwaltung]</td> 
   <td>In einem [!UICONTROL Projekt] -Bericht wird in diesem Feld das Datum und der Zeitpunkt der letzten Berechnung und Aktualisierung der Projektfinanzierungen erfasst. Informationen zu den Projektfinanzen finden Sie unter <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Übersicht über die Projektfinanzen</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzter Hinweis]</td> 
   <td> <p>In diesem Feld wird die zuletzt von einem Benutzer in einem Objekt eingegebene Aktualisierung angezeigt. Dies ist die neueste Aktivität oder Interaktion für ein Objekt.</p> <p>Die Spalte [!UICONTROL Letzte Anmerkung] ist leer, wenn der Text der letzten Anmerkung eines Objekts gelöscht wurde. Wenn eine neue Anmerkung auf dem Objekt eingegeben wird, wird sie zur letzten Anmerkung und wird erneut in der Spalte angezeigt.</p>
   <p>Wenn dieses Feld zu einem [!UICONTROL Task]-Bericht hinzugefügt wird, werden alle Aktualisierungen an untergeordneten Objekten (z. B. Problemen, Unteraufgaben, Dokumenten usw.) beibehalten. — der Aufgabe nicht in dieser Spalte angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuletzt angezeigt von]</td> 
   <td> <p>In einer Berichtsliste zeigt dieses Feld Informationen über den Benutzer an, der den Bericht zuletzt angesehen hat.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letztes Ansichtsdatum]</td> 
   <td> <p>In einer Berichtsliste zeigt dieses Feld das Datum an, an dem der Bericht zuletzt angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout-Vorlage]</td> 
   <td>Wird vom Systemadministrator oder Gruppenadministrator definiert, um die Registerkarten und Berichte zu identifizieren, die im Arbeitsbereich eines bestimmten Benutzers angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layouttyp]</td> 
   <td>In Verbindung mit [!UICONTROL benutzerdefinierten Ansichten] gibt der [!UICONTROL Layouttyp] den Typ der benutzerdefinierten Ansicht an. Derzeit ist nur Liste verfügbar. In Zukunft wird möglicherweise [!UICONTROL Detail] (die [!UICONTROL Detail]-Ansicht eines Objekts) verfügbar sein.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Lizenztyp]</td> 
   <td>Die Art der Lizenz, die einer [!UICONTROL Zugriffsstufe] zugewiesen wurde. Es handelt sich entweder um [!UICONTROL Full User], [!UICONTROL Limited User] oder [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>In einer [!UICONTROL Group]-Ansicht oder einem Bericht zeigt dieses Feld die maximale Anzahl von [!UICONTROL Plan]-Lizenzen an, die Benutzern zugewiesen werden können, die die jeweilige Gruppe als [!UICONTROL Home Group] bezeichnet haben.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>In einer [!UICONTROL Group]-Ansicht oder einem Bericht zeigt dieses Feld die maximale Anzahl von [!UICONTROL Work]-Lizenzen an, die Benutzern zugewiesen werden können, deren [!UICONTROL Home Group] die entsprechende Gruppe ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eingeschränkter Benutzer]</td> 
   <td>Ein Lizenztyp, der die Erstellung eines [!DNL Access Level] -Felds ermöglicht, das schreibgeschützte Berechtigungen enthält, mit der Möglichkeit, Probleme zu senden, Notizen einzugeben und Dokumente hochzuladen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Listenelemente]</td> 
   <td> <p>Ein Teil der [!UICONTROL Interface-Einrichtung], der die Verknüpfung benutzerdefinierter Filter, Ansichten und Gruppierungen mit einzelnen Benutzern oder global mit allen Benutzern ermöglicht.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Suchfelder]</td> 
   <td> <p>Wenn Sie in der Workfront-Planung die Verbindung zwischen zwei Datensatztypen hergestellt und einzelne Datensätze miteinander verknüpft haben, können Sie auf die Felder der verknüpften Datensätze in dem Datensatz verweisen, aus dem Sie eine Verbindung herstellen.</p>
   <p>Wenn Sie beispielsweise einen Campaign-Datensatz mit einem Workfront-Projektobjekttyp verbinden, können Sie das Feld Budget der verbundenen Projekte in den Kampagnensätzen anzeigen. Das Feld Budget-Projekt ist ein Suchfeld aus Projekten in einer Kampagne.</p> <p>Die Werte der Suchfelder werden automatisch in die Datensätze eingefügt, aus denen sie verbunden sind.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Übersicht über Connected records</a>.</p>
   <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

## M - O

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
   <td>[!UICONTROL Manual]</td> 
   <td> <p>Eines der [!UICONTROL Projekt]-Aktualisierungstypen. Mit dieser Einstellung können die Zeitpläne [!UICONTROL Project Projected] und [!UICONTROL Planned] nur aktualisiert werden, wenn auf "[!UICONTROL Neuberechnete Zeitpläne]"geklickt wird. Auf diese Weise eingerichtete Projekte werden während der nächtlichen Neuberechnung und bei der Aktualisierung des Projekts bzw. der Aufgaben im Projekt ignoriert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Projekts [!UICONTROL Aktualisierungstyp] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Dies bezieht sich auf den derzeit angemeldeten Benutzer. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der abhängig davon, wer sich anmeldet, unterschiedliche Informationen anzeigt, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die dieses Feld anzeigen kann, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat und die nicht aktualisiert werden kann. </p> <p>In früheren Versionen von [!DNL Workfront] konnten Sie dieses Feld beim Erstellen oder Bearbeiten einer Auftragsrolle aktualisieren. Es wurde die Gesamtzahl der Benutzer angezeigt, die mit einer Rolle in jedem Projekt verknüpft werden können. Der Wert null ist für eine unbegrenzte Anzahl von Benutzern zulässig, die für ein Projekt zugewiesen werden können. </p>Das Feld ist weiterhin in einigen Berichten und Listen sichtbar, die angezeigten Informationen können jedoch nicht aktualisiert werden. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Eine Markierung, die Sie mit einer Aufgabe verknüpfen können, um anzugeben, dass beim Abschluss der Aufgabe ein wichtiger Punkt im Projekt erreicht wurde. Im Allgemeinen können Sie Meilensteine verwenden, um ein bedeutendes Ereignis anzuzeigen, z. B. den Abschluss einer Phase des Projekts oder eine Reihe kritischer Aktivitäten. [!UICONTROL Milestones] sind normalerweise mit übergeordneten Aufgaben verknüpft. Sie müssen die Meilensteine erstellen, bevor Sie sie an Aufgaben anhängen können. Weitere Informationen zu Meilensteinen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Meilensteinpfad erstellen</a> und <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Meilensteine mit Aufgaben verknüpfen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Eine Sammlung von [!UICONTROL Meilensteinen]. [!UICONTROL Milestone Paths] werden in Projekten verwendet, um Projekte mit bestimmten [!UICONTROL Milestones] von Projekten mit unterschiedlichen [!UICONTROL Milestones] zu unterscheiden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Eine Aufgabe, die zur Angabe eines zu messenden meldefähigen Ereignisses gekennzeichnet ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Modul]</td> 
   <td>Ein einzelner Schritt innerhalb eines Szenarios in [!DNL Workfront Fusion] , der eine Funktion basierend auf der zugehörigen App ausführt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meine Primäre Rolle</td> 
   <td> <p>Wenn dies in Filtern referenziert wird, zeigt dies entweder Benutzer an, die dieselbe [!UICONTROL Primäre Rolle] wie der angemeldete Benutzer haben, oder Arbeitselemente, die der [!UICONTROL Primären Rolle] des angemeldeten Benutzers zugewiesen sind.</p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der abhängig davon, wer sich anmeldet, unterschiedliche Informationen anzeigt, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Wenn dies in Filtern referenziert wird, zeigt dieses Feld entweder Benutzer an, die zum [!UICONTROL Home Team] des angemeldeten Benutzers gehören, oder Arbeitselemente, die dem [!UICONTROL Home Team] des angemeldeten Benutzers zugewiesen sind. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der abhängig davon, wer sich anmeldet, unterschiedliche Informationen anzeigt, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Namenskonvention]</td> 
   <td>Ein organisationsweiter Regelsatz, der Daten verwendet, um Namen von Projekten, Aufgaben und Lieferzielen zu erstellen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Eine Integration, die keine manuelle Kodierung oder API-Konfiguration erfordert. Wird auch als vordefinierte Integration bezeichnet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigationsmenü]</td> 
   <td>Das obere mittlere Bedienfeld der Anwendung, das Links zu den Hauptbereichen von [!UICONTROL Workfront] enthält.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Zahlenwert]</td> 
   <td>In einem [!UICONTROL Journal Entry] -Bericht wird der aktualisierte Wert eines Felds angezeigt, das den [!UICONTROL Old Number Value] ersetzt.
   Weitere Informationen finden Sie unter "[!UICONTROL Old Number Value]"in diesem Artikel.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Nicht in Rechnung gestellte Kosten]</td> 
   <td> <p>Eine Ausgabe, die nicht als dem Kunden abrechenbar markiert ist. Dies kann entweder eine geplante oder eine tatsächliche Ausgabe sein.</p> <p>Die Felder "Geplante nicht abrechnungsfähige Kosten"und "Tatsächliche nicht abrechnungsfähige Kosten"stehen Ihnen zur Verfügung, um sie Ansichten und Berichten hinzuzufügen. Sie werden nicht auf den Projekt- oder Aufgabendetailseiten angezeigt.</p>
   <p>Sie finden diese Felder in den folgenden Berichtstypen:</p>
   <ul>
   <li>Ausgangsbasis</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Markieren einer Ausgabe als abrechnungsfähig finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Verwalten von Projektausgaben</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Nichtarbeitstag]</td> 
   <td>Ein Tag, der nicht dem Abschluss von Zuweisungen zugeordnet wird. Dies ist normalerweise ein Urlaubstag, ein Feiertag oder ein Wochenende. Der Begriff wird im API-Explorer angezeigt. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hinweis]</td> 
   <td>Ein Kommentar oder eine Aktualisierung für ein [!DNL Workfront] -Objekt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hinweistext]</td> 
   <td> <p>Dadurch wird der Text eines Updates angezeigt, das von einem Benutzer für ein beliebiges Objekt eingegeben wurde. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anzahl verknüpfter Ziele]</td> 
   <td> <p>In einem [!UICONTROL Projekt]-Bericht ist dies die Anzahl der strategischen Ziele, die mit dem Projekt verbunden sind. Informationen zum Verknüpfen von Projekten mit strategischen Zielen finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Projekte zu Zielen hinzufügen in [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Weitere Informationen zu strategischen Zielen finden Sie in diesem Artikel auch unter "[!UICONTROL Ziel]".</p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Projekte zu Zielen hinzufügen in [!UICONTROL Adobe Workfront-Zielen]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objekt]</td> 
   <td> <p>Die Informationen, die Sie in [!DNL Adobe Workfront] anzeigen, werden durch Objekte dargestellt, die in der [!DNL Workfront] -Datenbank gespeichert sind. Die Objekte sind das, was die Informationen in Workfront antreibt. Beispiele für Objekte:</p> 
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
     <li>[!UICONTROL Benutzer]</li> 
     <li>[!UICONTROL Unternehmen]</li> 
     <li>[!UICONTROL Benutzerdefinierte Formulare]</li>
     <li>[!UICONTROL Benutzerdefinierte Felder]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Abrechnungsraten]</li> 
     <li>[!UICONTROL Vorlagen]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li>

<p><b>NOTIZ</b></p>
  <p>Dies ist keine umfassende Liste. </p>

</ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Grundlegendes zu Objekten in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objekttypen]</td> 
   <td>Wenn Sie einen Bericht oder eine Liste erstellen, der bzw. die alle Ihre benutzerdefinierten Formulare enthält, können Sie dieses Feld als Ansicht oder Filter verwenden, um zu sehen, welche Objekttypen mit den einzelnen Formularen verknüpft sind. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>In einem [!UICONTROL Journal Entry] -Bericht wird der ursprüngliche Wert eines Felds angezeigt, bevor es aktualisiert wurde. Sobald der Wert eines Felds aktualisiert wurde, wird er als [!UICONTROL Neuer Zahlenwert] in einem [!UICONTROL Journal Entry]-Bericht angezeigt. Weitere Informationen finden Sie auch unter "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Nur bei Änderung]</td> 
   <td> <p>Einer der [!UICONTROL Projektaktualisierungstypen. Wenn diese Option ausgewählt ist, werden die Zeitpläne [!UICONTROL Project Projected] und [!UICONTROL Planned] nur aktualisiert, wenn das Projekt oder eine Aufgabe innerhalb des Projekts aktualisiert oder geändert wird. Das Projekt wird nicht jede Nacht aktualisiert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps für das Projekt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>Der Name für [!UICONTROL Problem] in der [!DNL Workfront] -Datenbank, der in Textmodusberichten oder berechneten benutzerdefinierten Daten verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Ein Problem oder eine Aufgabe, die nicht abgeschlossen ist, aber bearbeitet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Kurz für Organisationsdiagramm. Dies ist ein Diagramm, das die Hierarchie einer Organisation anzeigt. Sie befindet sich auch auf der Registerkarte auf dem Detailbildschirm [!UICONTROL User] , auf dem die [!UICONTROL User]-Beziehungen [!UICONTROL Company] und [!UICONTROL Reporting] angezeigt und festgelegt werden können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organisatorische Einrichtung]</td> 
   <td>Dadurch werden [!UICONTROL Unternehmen], [!UICONTROL Gruppen] und [!UICONTROL Sicherheitsprofile] für Ihr Unternehmen definiert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Andere Gruppen]</td> 
   <td> <p>In einem Bericht oder einer Ansicht, in dem Benutzer aufgeführt sind, zeigt dieses Feld alle Gruppen an, denen jeder Benutzer angehört. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Währung überschreiben]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Job Role] -Bericht ist dies die Währung, die mit einer Auftragsrolle verknüpft ist. Es handelt sich um eine Überschreibung der [!UICONTROL Basiswährung], wie sie im [!UICONTROL Setup]-Bereich vom [!DNL Workfront] -Administrator festgelegt wurde. </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Währungsabrechnung/Stunde überschreiben]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Job Role] -Bericht ist dies die Abrechnungsrate pro Stunde der Auftragsrolle unter Verwendung der ausgewählten [!UICONTROL Override Currency] der Auftragsrolle.</p> 
     <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Währungskosten/ Stunde überschreiben]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Job Role] -Bericht ist dies die Kosten pro Stunde für die Rolle "Job"unter Verwendung der ausgewählten [!UICONTROL Override Currency] der Rolle "Job". </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Inhaber]</td> 
   <td>Der Benutzer, der für das Ausfüllen des angegebenen Objekts verantwortlich ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Inhaber Type]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Ziel] -Bericht zeigt dies den Typ des Eigentümers an, der einem strategischen Ziel zugewiesen ist. Im Folgenden finden Sie die Zieleigentümertypen:</p> 
     <ul> 
      <li> <p>[!UICONTROL Benutzer]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>In diesem Feld wird kein Wert angezeigt, wenn der Zieleigentümer Ihre Organisation ist. </p> 
     <p>Dies erfordert eine zusätzliche Lizenz. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] Übersicht</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

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
   <td>Parameter [!UICONTROL]</td> 
   <td> <p>Ein [!UICONTROL Parameter] ist ein benutzerdefiniertes Feld. Sie können einen Bericht für alle Parameter oder benutzerdefinierte Felder in Ihrem System erstellen. </p> </td> 
  </tr> 
  <tr> 
   <td>Übergeordnetes Element von [!UICONTROL]</td> 
   <td>In einem Bericht zeigt dieses Feld Informationen zum übergeordneten Objekt an. In einem [!UICONTROL Problem]-Bericht können beispielsweise Informationen über die Aufgabe oder das Projekt angezeigt werden, unter der das Problem protokolliert wird. In einem Aufgabenbericht können Informationen über die direkt übergeordnete Aufgabe oder über das Projekt angezeigt werden. Weitere Informationen darüber, welche Objekte möglicherweise übergeordnete Elemente in [!DNL Workfront] haben, finden Sie im Abschnitt "Interdependency and hierarchy of object"im Artikel <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in [!DNL Adobe Workfront]</a> verstehen. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnete Ebene]</td> 
   <td>Die Zeit, die zwischen dem Start der [!UICONTROL übergeordneten Aufgabe] und dem Start der [!UICONTROL Unteraufgabe] verstreichen muss.</td> 
  </tr> 
  <tr> 
   <td>Übergeordnete Aufgabe von [!UICONTROL]</td> 
   <td>Wird auch als [!UICONTROL Zusammenfassungsaufgabe] bezeichnet. Dies ist eine Aufgabe mit Unteraufgaben (auch [!UICONTROL Children Tasks] genannt). Die [!UICONTROL Dauer], die [!UICONTROL Arbeit erforderlich] und die [!UICONTROL Prozent Abschluss] der übergeordneten Aufgabe werden aus den Unteraufgaben berechnet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Teilzeitressourcen]</td> 
   <td>Ein lizenzierter Benutzer, der weniger Kapazität hat als der im System definierte Standardzeitplan.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prozentsatz abgeschlossen]</td> 
   <td> <p>Ein Projekt-, Aufgaben- oder Problemfeld, das anzeigt, welcher Prozentsatz der mit der Aufgabe, dem Projekt oder dem Problem verbundenen Arbeit abgeschlossen ist.</p> <p>Sie können dieses Feld für Probleme und Arbeitsaufgaben manuell aktualisieren. </p> <p>Bei Projekten und übergeordneten Aufgaben handelt es sich bei diesem Feld um eine Datenaggregation aus allen Arbeitsaufgaben, die Sie nicht manuell aktualisieren können. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Übersicht über das Projekt [!UICONTROL Prozentualer Abschluss]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechtigung]</td> 
   <td> <p>Rechte, die einem Benutzer für ein Objekt gewährt werden, normalerweise gegeben, damit er die Arbeit an dem Element abschließen oder das Element anzeigen kann. Sie können Berechtigungen gewähren für:</p> 
    <ul> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Berichte]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Ansichten]</li> 
     <li>[!UICONTROL Filter]</li> 
     <li>[!UICONTROL Gruppierungen]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Überblick über die Freigabe von Berechtigungen für Objekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Dies ist ein vollständiger Lizenztyp im System [!DNL Workfront]. Benutzer müssen über diese Funktion verfügen, um auf alle Funktionen in [!DNL Workfront] zugreifen zu können.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Lizenzübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (in der [!DNL Scenario Planner])</td> 
   <td> <p>Ein Plan ist das Hauptobjekt bei der Arbeit mit dem Szenario-Planer [!DNL Workfront] . Sie können die Strategie für die kurz- und langfristige Zukunft Ihres Unternehmens skizzieren und jedes Ergebnis auf hoher Ebene identifizieren und es dem [!DNL Workfront]-Szenario-Planer als Plan hinzufügen. </p> <p>Sie können keine [!DNL Scenario Planner]-Pläne in einem Bericht anzeigen und nicht über die [!DNL Workfront]-API darauf zugreifen. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplant]</td> 
   <td> <p>Der Zeitrahmen, in dem planmäßig etwas geschehen soll. Wenn Sie in [!DNL Workfront] Projekte, Aufgaben oder Probleme erstellen, legen Sie die geplanten Start- und Enddaten sowie den geplanten Zeitrahmen fest, in dem sie auftreten. Diese Werte repräsentieren Ihre ursprüngliche Absicht oder Schätzung, wie lange ein Artikel benötigen sollte, um abgeschlossen zu werden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Vorteil]</td> 
   <td>Dies ist ein manueller Eintrag für den Projekt-Manager, um abzuschätzen, ob der Abschluss eines Projekts der Organisation einen finanziellen Nutzen bringen würde. Die Angabe dieses Werts kann Teil der Erstellung eines [!UICONTROL Geschäftsfalls] für das Projekt sein. Sie müssen über [!UICONTROL Manager] -Berechtigungen für das Projekt verfügen, um diesen Wert zu aktualisieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Geplante Haushaltsstunden]</td> 
   <td> <p>In einem [!UICONTROL Budgeted Hour]-Bericht wird die Anzahl der für Projekte geplanten Stunden oder [!UICONTROL Job Roles] im [!UICONTROL Resource Planer] angezeigt. </p> <p>Informationen zu Budgetierungsprojekten oder Rollen im [!UICONTROL Resource Planer] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen im [!UICONTROL Resource Planer], der [!UICONTROL Project] und [!UICONTROL Role] Ansichten verwendet</a>. Weitere Informationen zum Bericht [!UICONTROL Budgeted Hours] finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>Sie können das geplante [!UICONTROL Abschlussdatum] einer Aufgabe, eines Projekts oder einer Ausgabe manuell auf ein Datum Ihrer Wahl festlegen. Wenn Sie das geplante Abschlussdatum nicht festlegen, wird es von [!DNL Workfront] automatisch festgelegt. Wenn dies automatisch festgelegt wird, lautet das geplante Abschlussdatum [!UICONTROL]: [!UICONTROL Geplantes Startdatum] + [!UICONTROL Dauer].</p> <p>Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Überblick über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Legen Sie das Projekt fest [!UICONTROL Geplantes Abschlussdatum]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Kosten]</td> 
   <td> <p>Gesamtsumme der [!UICONTROL Planten Arbeitskosten] und der [!UICONTROL Planeten Kosten] des Projekts. Dies umfasst nicht die geplanten [!UICONTROL Risikokosten] für das Projekt.  </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Geplante Datumsausrichtung]</td> 
   <td> <p>Dies ist ein automatischer Indikator, mit dem Workfront Projekte, Aufgaben und Probleme zuweist, um anzuzeigen, wann ein Element in Bezug auf das geplante Abschlussdatum abgeschlossen wird. </p>
   <p>Die folgenden Werte sind für den Indikator Geplante Datumsausrichtung möglich: </p>
<ul>
<li>Wird zum geplanten Abschlussdatum fertiggestellt</li>
<li>Wird vor dem geplanten Abschlussdatum fertiggestellt</li>
<li>Wird nach dem geplanten Abschlussdatum fertiggestellt</li></ul>
<p>Die geplante Datumsausrichtung ist in Projekt-, Aufgaben- und Problemlisten und Berichten sichtbar. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Dauer]</td> 
   <td> <p>[!UICONTROL Geplante Dauer] einer Aufgabe entspricht in der Regel der [!UICONTROL Dauer] der Aufgabe. Er stellt den Unterschied in Tagen zwischen dem geplanten [!UICONTROL Start] und dem geplanten [!UICONTROL Abschlussdatum] der Aufgabe dar. </p> <p>Wenn die Aufgabe einen [!UICONTROL Duration]-Typ von [!UICONTROL Effort Driven] aufweist, kann die geplante [!UICONTROL Dauer] von der [!UICONTROL Dauer] der Aufgabe abweichen, je nachdem, wie viele Ressourcen Sie der Aufgabe zuweisen. </p> <p>Wenn beispielsweise eine Aufgabe mit einer [!UICONTROL Dauer] vom Typ [!UICONTROL Effort Driven] eine [!UICONTROL Dauer] von 3 Tagen hat und Sie der Aufgabe eine Ressource mit einem vollen Zeitplan zuweisen, beträgt die geplante Dauer [!UICONTROL] ebenfalls 3 Tage. Wenn Sie derselben Aufgabe drei Ressourcen mit einem vollen Zeitplan zuweisen, bleibt die [!UICONTROL Dauer] 3 Tage, die [!UICONTROL geplante Dauer] wird jedoch 1 Tag. Die geplante [!UICONTROL Dauer] ändert auch die [!UICONTROL geplanten Start]- und [!UICONTROL geplanten Fertigstellungsdaten der Aufgabe, um die neue [!UICONTROL geplante Dauer] widerzuspiegeln. Daher ist auch die Timeline des Projekts betroffen. </p> <p>Weitere Informationen zum Unterschied zwischen [!UICONTROL Dauer] und [!UICONTROL Geplante Dauer] für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Unterschied zwischen [!UICONTROL Geplante Dauer] und [!UICONTROL Dauer] für Aufgaben</a>.</p> <p>Projekte und Probleme haben keine [!UICONTROL geplante Dauer]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Dauer in Minuten]</td> 
   <td> <p>Die [!UICONTROL geplante Dauer eines Projekts oder eines Problems ist die [!UICONTROL Dauer] des Projekts oder der Ausgabe in Minuten. </p> <p>Aufgaben verfügen nicht über das Feld [!UICONTROL Geplante Dauer-Minuten] . </p> <p>[!UICONTROL Vorlagenaufgaben] verfügen über ein Feld mit der geplanten Dauer von Minuten , in dem die [!UICONTROL geplante Dauer] der Aufgabe in Minuten angezeigt wird. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Kosten]</td> 
   <td> <p>Die Summe der geplanten [!UICONTROL Beträge] für alle Ausgaben, die für ein Projekt oder eine Aufgabe protokolliert werden.</p> <p><b>BEISPIEL</b></p>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und im Feld [!UICONTROL Geplanter Betrag] den Betrag von 600,00 USD eingeben, belaufen sich die geplanten [!UICONTROL Kosten] für diese Aufgabe auf 600,00 USD. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel zur Berechnung der geplanten [!UICONTROL Kosten]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Stunden]</td> 
   <td> <p>Dieses Feld wird in den [!UICONTROL Projekten], [!UICONTROL Aufgaben] angezeigt und enthält Bereiche, Berichte für Projekte, Aufgaben oder Probleme sowie Ressourcen-Management-Tools wie den [!UICONTROL Resource Planer], [!UICONTROL Workload Balancer] und den [!UICONTROL Utilization]-Bericht. </p> <p>Er zeigt die Anzahl der Stunden an, die der Projektinhaber schätzt, dass die einzelnen Aufgaben oder Probleme abgeschlossen sein sollten. Bei Projekten handelt es sich in der Regel um eine Zusammenfassung der [!UICONTROL geplanten Stunden] aus den Aufgaben im Rahmen des Projekts. </p> <p>Im Feld [!UICONTROL Geplante Stunden] werden möglicherweise unterschiedliche Informationen angezeigt, je nachdem, von wo aus Sie sie anzeigen. Informationen zu geplanten Stunden finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Übersicht über geplante Stunden</a>.</p> <p>Geplante Stunden werden in Minuten in der Datenbank [!DNL Workfront] gespeichert. Stellen Sie beim Schreiben von Berechnungen mit diesem Feld sicher, dass die Stunden als Minuten angezeigt werden.<br></p> <p>Standardmäßig werden geplante Stunden gleichmäßig auf alle Tage innerhalb der Dauer eines Arbeitselements und auch auf alle Ressourcen verteilt, die der Aufgabe zugewiesen sind. Benutzer können die tägliche Anzahl geplanter Stunden für ein Arbeitselement oder die einzelnen geplanten Stunden für jeden Bevollmächtigten aktualisieren.</p> <p>Die Aktualisierung dieses Felds unterscheidet sich bei Projekten, Aufgaben und Problemen: </p> 
    <ul> 
     <li> <p>Bei Problemen können Sie dieses Feld manuell aktualisieren. Die geplanten Problemzeiten werden nicht zu den geplanten Projektzeiten hinzugefügt. </p> <p><b>TIPP</b></p> <p>In einem Problembericht wird eines der Felder [!UICONTROL Geplante Stunden] durch das Feld [!UICONTROL Arbeit] ersetzt. Im Feld wird die Anzahl der geplanten Stunden zum Problem angezeigt. Weitere Informationen finden Sie in den Feldern "Arbeit" oder "[!UICONTROL Arbeit]" in dieser Tabelle. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Für Aufgaben können Sie dieses Feld manuell aktualisieren, wenn der [!UICONTROL Durationstyp] der Aufgabe die [!UICONTROL berechnete Zuweisung] oder [!UICONTROL Einfach] ist. Dieses Feld wird durch [!DNL Workfront] berechnet, wenn der [!UICONTROL Dauer-Typ] der Aufgabe [!UICONTROL Berechnete Arbeit] oder [!UICONTROL Aufwand gesteuert] lautet.<br>Weitere Informationen zu [!UICONTROL Task Duration] finden Sie im Artikel <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Dauer] und [!UICONTROL Dauer Typ]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Für Projekte berechnet [!DNL Workfront] die geplanten Stunden, indem alle geplanten Stunden aus allen Aufgaben des Projekts hinzugefügt werden. </p> </li> 
    </ul> <p><b>TIPP</b></p> <p>Sie können [!UICONTROL Planed Hours] auch in [!UICONTROL Projekt]-, [!UICONTROL Aufgabe]- oder [!UICONTROL Probleme]-Berichten anzeigen, indem Sie den Textmodus verwenden und auf zusätzliche Felder verweisen. Weitere Informationen finden Sie in den Feldern "<code>work</code>", "[!UICONTROL Work]"und "<code>workRequiredExpression</code>" in dieser Tabelle. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Arbeitskosten]</td> 
   <td> 
    <p>Bei einer Aufgabe die Stundenrate des Benutzers oder der Rolle multipliziert mit der Anzahl der Stunden, die dem Benutzer oder der Rolle zugewiesen sind.</p> <p>Bei einem Projekt handelt es sich um die Gesamtsumme aller [!UICONTROL Planeten Arbeitskosten] aller Aufgaben.</p> <p>Ob die Rate des Benutzers oder der Rolle verwendet wird, hängt vom Kostentyp ab, der für die jeweilige Aufgabe ausgewählt ist. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Kosten-Tracking</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Umsatz]</td> 
   <td> <p>Aufgaben und Projekte können einen Wert für [!UICONTROL Geplanter Umsatz] in [!DNL Workfront] anzeigen. [!UICONTROL Geplanter Umsatz] bezeichnet den Geldbetrag, der mit den [!UICONTROL Planeten Stunden] der Aufgaben im Rahmen des Projekts verbunden ist. Bei Projekten kann er auch den [!UICONTROL festen Umsatz] des Projekts umfassen. </p> <p>Bei Aufgaben ist dies der Umsatz, der mit den geplanten [!UICONTROL Stunden] von Aufgaben verbunden ist. Die geplanten Stunden aus allen Aufgaben werden in die geplanten Stunden des Projekts einfließen, um zur Berechnung des Projekts beizutragen [!UICONTROL Geplante Stunden]. </p> 
   <p>[!DNL Workfront] berechnet den geplanten Umsatz von [!UICONTROL für Aufgaben und Projekte anhand der folgenden Formeln:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Das Projekt [!UICONTROL Geplanter Umsatz], das im Bereich [!UICONTROL Projektdetails] und in Projektberichten angezeigt wird, unterscheidet sich von dem geplanten Umsatz, der im [!UICONTROL Utilization]-Bericht angezeigt wird. </p> <p>Der geplante Umsatz [!UICONTROL] im Bereich [!UICONTROL Projektdetails] spiegelt den Umsatz der Aufgabe sowie den feststehenden Umsatz des Projekts wider. Der geplante Umsatz von [!UICONTROL] im [!UICONTROL Utilization Report] zeigt [!UICONTROL Planter Umsatz] an, der nur mit den Aufgaben im Projekt verbunden ist. </p> 
     <p><b>BEISPIEL</b></p>  
      <p>Wenn das Projekt eine Aufgabe mit 10 Stunden umfasst, die einem Berater mit 20 US-Dollar-Stundensatz zugewiesen ist und das Projekt einen Umsatz von 100 US-Dollar aufweist, zeigt der [!UICONTROL Utilization]-Bericht 200 US-Dollar für [!UICONTROL Geplanter Umsatz] (den [!UICONTROL geplanten Umsatz], der den Stunden der Aufgabe zugeordnet ist). Im Abschnitt [!UICONTROL Projektdetails] werden 300 USD (der geplante [!UICONTROL Umsatz] aus der Aufgabe und der feste Umsatz für das Projekt) angezeigt. </p> 
    <p>Informationen zum Verfolgen des Umsatzes in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Übersicht über Abrechnung und Umsatz</a>. </p> 
    <p>Weitere Informationen zu [!UICONTROL Planen Umsatz]-Berechnungen im [!UICONTROL Utilization Report] finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Anzeigen von Informationen zur Ressourcenauslastung </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Risikokosten]</td> 
   <td> <p>Gesamtsumme der [!UICONTROL Potenziellen Kosten] aller Risiken, die sich auf die Projektefaktorierung auswirken und deren Wahrscheinlichkeit, dass sie auftreten. Dieser Betrag ist nicht in den geplanten [!UICONTROL Kosten] des Projekts enthalten.</p> <p>Die [!UICONTROL Planeten Risikokosten] eines Projekts werden nach folgender Formel berechnet:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal-Profil]</td> 
   <td>Eine vom Administrator definierte Sammlung von Registerkarten und Abschnitten, die in "[!DNL Workfront]"angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal-Abschnitt]</td> 
   <td>Eine Komponente einer Registerkarte auf einer Dashboard- oder Portalseite. Normalerweise ein einzelner Bericht, ein Diagramm, einen Kalender oder eine Liste mit Schlüsselinformationen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal-Registerkarte]</td> 
   <td>Eine Registerkarte in einem Portal oder Dashboard, die bis zu drei Portalabschnitte enthält.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Eine Sammlung von Projekten mit einheitlichen Merkmalen. Diese Projekte konkurrieren normalerweise um dieselben Ressourcen, Budgets oder Zeitnischen. Sie können Portfolios in Programme unterteilen und sie mit den Programmen verknüpfen, bevor sie einem Portfolio hinzugefügt werden.</p> <p>Weitere Informationen zu Portfolios finden Sie unter <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Übersicht über das Portfolio in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Ein Praxisbereich, der sich auf die Verwaltung einer Sammlung oder verwandter Programme und Projektbemühungen konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Ein [!DNL Workfront]-Tool, das die Bewertung und Priorisierung von Projekten innerhalb eines Portfolios unterstützt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>Der Verantwortliche für die Priorisierung und den Haushalt eines Portfolios.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potenzielle Risikokosten]</td> 
   <td>Dies ist ein Projektfeld, das Sie in Listen und Berichten finden können. Er zeigt die potenziellen Kosten für die mit dem Projekt verbundenen Risiken, falls sie auftreten sollten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnen der potenziellen Risikokosten </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Vorgänger]</td> 
   <td> <p>Eine Aufgabe, die vor dem Abschluss einer abhängigen Aufgabe abgeschlossen werden muss. Auch eine Aufgabe, die als [!UICONTROL Abhängigkeit] für eine andere Aufgabe markiert ist. Vorläufer ermöglichen es dem Planer, eine Sequenzabhängigkeitslogik festzulegen, z. B. eine Aufgabe zu starten, nachdem eine andere Aufgabe abgeschlossen wurde.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Übersicht über Aufgabenverfasser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primär Company]</td> 
   <td>Das Unternehmen, zu dem der Benutzer gehört, wie in seinen Benutzereinstellungen angegeben. Unternehmen können auch mit Projekten verbunden werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primärer Kontakt]</td> 
   <td><p>Der Primäre Kontakt [!UICONTROL] ist der Ersteller eines Problems und wird automatisch durch [!DNL Workfront] gekennzeichnet, wenn der Benutzer das Problem erstellt. Sie können dieses Feld manuell aktualisieren, wenn Sie [!DNL Manage] -Berechtigungen für das Problem haben. Ein Problem kann nur einen Primären Kontakt haben.</p> 
   <p>Wenn Sie den Primären Kontakt ändern, hat der ursprünglich als Hauptkontakt bestimmte Benutzer weiterhin [!UICONTROL Manager] Zugriff auf das Problem.</p>
   <p>Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird der als [!UICONTROL Primärer Kontakt] des Problems bezeichnete Benutzer zum [!UICONTROL Converted Issue Originator] des Projekts oder der Aufgabe. Wenn der [!UICONTROL Primäre Kontakt] des Problems aktualisiert wird, nachdem das Problem konvertiert wurde, wird der [!UICONTROL Converted Issue Originator] zum Zeitpunkt der Konvertierung als [!UICONTROL Primärer Kontakt] des Problems beibehalten. Siehe auch "[!UICONTROL Converted Issue Originator]"in diesem Artikel.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Ein Wert, der einer Aufgabe, einem Problem oder einem Projekt zugewiesen werden kann, um zu bestimmen, wie wichtig dieser Wert ist. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Bei einem [!UICONTROL Hinweis] oder [!UICONTROL Dokument] wird dieses Objekt durch diese Option für die meisten Betrachter ausgeblendet. Für eine Warteschlange mit privaten Hilfeanfragen können nur Benutzer des Projektteams Probleme über den Bereich [!UICONTROL Anforderungen] an diese Warteschlange (oder dieses Projekt) senden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profil]</td> 
   <td>Alle Informationen zu einem Benutzerkonto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Programm]</td> 
   <td> <p>Teilmenge innerhalb eines Portfolios, in der ähnliche Projekte gruppiert werden können, um einen klar definierten Nutzen zu erzielen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programm-Management]</td> 
   <td>Verwaltung projektübergreifender Abhängigkeiten, Risiken, Probleme, Anforderungen und Lösungen, um das Programm gesund zu halten und den definierten Programmnutzen zu erzielen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programmeigentümer]</td> 
   <td>Der Verantwortliche für die Überwachung und Organisation der Aktivitäten, um sicherzustellen, dass die Projektziele mit den Unternehmenszielen übereinstimmen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Fortschritt]</span> </td> 
   <td> <p>In einem [!UICONTROL Ziel] -Bericht wird der prozentuale Anteil der Fertigstellung eines strategischen Ziels angezeigt. Der Fortschritt in Prozent wird als Zahl angezeigt. Weitere Informationen zu strategischen Zielen finden Sie in dieser Tabelle auch unter "[!UICONTROL Ziel]".</p> <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront] Ziele erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Projekte zu Zielen hinzufügen in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortschrittsstatus]</td> 
   <td> <p>In einem Projekt-, Aufgaben- und Zielbericht zeigt dieses Feld den Fortschrittsstatus von Projekten, Aufgaben oder strategischen Zielen an. Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Überblick über den Projektfortschrittsstatus</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Übersicht über den Aufgabenfortschrittsstatus</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Überblick über den Fortschritt und die Bedingung des Ziels in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Der Bericht [!UICONTROL Ziel] und das Feld [!UICONTROL Fortschrittsstatus] für [!DNL goals] sind nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zu strategischen Zielen in [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] Übersicht</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Projekt]</td> 
   <td> <p>Eine große Menge an Arbeit, die innerhalb eines bestimmten Zeitrahmens abgeschlossen werden muss und ein bestimmtes Budget und eine bestimmte Anzahl von Ressourcen verwenden muss. Um das Projekt verwaltbar zu machen, unterteilen Sie es in eine Reihe von Aufgaben. Wenn Sie alle Aufgaben ausführen, ist das Projekt abgeschlossen. Weitere Informationen zur Planung eines Projekts finden Sie unter <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Projektübersicht planen</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektzuweisung geplant Stunden]</td> 
   <td> <p>In einem [!UICONTROL Initiative Job Role] -Bericht wird die Anzahl der geplanten [!UICONTROL Stunden] angezeigt, die mit einer Auftrags-Rolle verknüpft sind, die Aufgaben oder Problemen im Projekt zugewiesen ist. Dieses Feld und der Berichtstyp [!UICONTROL Initiative Job Role] werden nur dann in Ihrer [!DNL Workfront] -Instanz angezeigt, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektdetails]</td> 
   <td>Die Details zum aktuellen Status eines Projekts.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt - Budgetierte Kosten]</td> 
   <td> <p> Dies sind die [!UICONTROL Budgeted Cost] eines Projekts, wie sie in Listen und Berichten angezeigt werden.</p><p>Siehe auch "[!UICONTROL Budgeted Cost]"in diesem Artikel.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Projektmanagement]</td> 
   <td>Eine Reihe von Richtlinien, die die Schwellenwerte für die Erstellung, Kategorisierung und Benennung von Projekten festlegen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Projektaufwand]</td> 
   <td>In einem [!UICONTROL Stunden] Bericht ist dieses Feld für Finanzinformationen reserviert, die mit den Stunden verknüpft sind, die mit dem Stundentyp [!UICONTROL Project Time] protokolliert wurden. Projekte können über eigene Abrechnungsraten verfügen. Wenn eine Stunde direkt in einem Projekt protokolliert wird, werden diese Beträge in Berechnungen verwendet. Basierend auf den Projekteinstellungen können Projekte auch unterschiedliche Währungen aufweisen und es kann eine Währungsumrechnung für diese Stunden geben. Das [!UICONTROL Project Overhead]-Objekt ermöglicht es [!DNL Workfront], diese Informationen abzurufen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektinhaber]</td> 
   <td>Der Benutzer, der für die Verwaltung des Umfangs, der Zeitleiste und der Zuweisungen eines Projekts verantwortlich ist. Der standardmäßige Genehmiger für Änderungsaufträge, Finanzänderungen und Lieferziele.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektplanung]</td> 
   <td>Prozesse zur Entwicklung und Pflege des Projektplans.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektsponsor]</td> 
   <td>Ein bestimmtes Profil von Interessenträgern, auf das sich jeder Ihrer Benutzer beziehen sollte. In [!DNL Workfront] werden diese als [!UICONTROL Zugriffsebenen] bezeichnet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektteams]</td> 
   <td> <p>Die Sammlung von Benutzern oder Rollen, die einem Projekt zugewiesen sind</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Übersicht über das Projektteam</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt-Tracking]</td> 
   <td>Die Daten, mit denen der Zustand und Umfang eines Projekts gemessen wird</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekted]</td> 
   <td> <p>Eine Schätzung des Zeitstempels für den Abschluss der Arbeit basierend auf den geplanten Stunden und dem prozentualen Abschluss einer Aufgabe, eines Problems oder eines Projekts.</p> <p>Dies bezieht sich auf Daten oder die [!UICONTROL Dauer] von Aufgaben, Problemen oder Projekten. In der Regel werden Daten und Dauern bestimmt, die für das Leben der Arbeitselemente besser zutreffen, nachdem einige Arbeiten bereits abgeschlossen oder einige Zeit vergangen sind. </p> <p>Beispielsweise ist das [!UICONTROL Projektionsdatum] einer Aufgabe das Datum, an dem [!DNL Workfront] schätzt, dass die Aufgabe abgeschlossen wird, basierend darauf, wie viel Arbeit bisher daran geleistet wurde, wie viele Personen ihr zugewiesen sind und wie viel Zeit seit dem Startdatum vergangen ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-Frist]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. den Bericht [!UICONTROL Document Version] und den Bericht [!UICONTROL Proof Approval] ), zeigt dieses Feld den Wochentag, das Datum, die Uhrzeit und das Jahr der Testversand-Deadline an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testentscheidung]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. den Bericht [!UICONTROL Document Version]  und [!UICONTROL Bericht zur Bestätigung des Testversands]), zeigt dieses Feld den Entscheidungsstatus des Testversands an (ausstehend, erforderliche oder genehmigte Änderungen).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testname]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. den Bericht [!UICONTROL Document Version] und den Bericht [!UICONTROL Proof Approval] ), wird in diesem Feld der Name des Testversands angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testseiten]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. den Bericht [!UICONTROL Document Version] und den Bericht [!UICONTROL Proof Approval] ), zeigt dieses Feld die Anzahl der im Testversand enthaltenen Seiten an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. den Bericht [!UICONTROL Document Version] und den Bericht [!UICONTROL Proof Approval]), wird der Fortschrittsstatus des Testversands angezeigt ([!UICONTROL Gesendet], [!UICONTROL Geöffnet], [!UICONTROL Kommentar], [!UICONTROL Decision Made]).</p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Übersicht über den Fortschritt des Testversands</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Übersicht über den Fortschritt des Testversands und den Status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand]</td> 
   <td>Ein Überprüfungsprozess, bei dem ein oder mehrere Benutzer Inhalte markieren und kommentieren, die in einem Bild, einem Textdokument, einem Video oder interaktiven Webinhalt geändert werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>In einem [!UICONTROL Hinweis] oder [!UICONTROL Dokument] ermöglicht diese Option anderen Benutzern oder sogar Personen von außerhalb von [!DNL Workfront] den Zugriff auf dieses Objekt. Für eine [!UICONTROL Help Request Queue] bedeutet [!UICONTROL Public], dass alle Benutzer, die Probleme an ein Projekt senden können, Probleme über den Bereich [!UICONTROL Requests] senden können.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualität]</td> 
   <td>Die Wahrnehmung der Arbeitsqualität innerhalb der Organisation.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Auch als Help Desk Queue oder [!UICONTROL Help Request Queue] bezeichnet. Dies ist ein Projekt, das im Bereich [!UICONTROL Anforderungen] veröffentlicht wurde, damit Benutzer Probleme senden können. In der Regel werden Warteschlangen für bestimmte Themen erstellt, z. B. [!UICONTROL Bugs], [!UICONTROL Projektanforderungen] usw.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Diese Einstellungen definieren die Regeln zur Übermittlung von Problemen für ein Projekt, das im Bereich [!UICONTROL Anforderungen] veröffentlicht wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlangenthema]</td> 
   <td> <p>Eine Eigenschaft in einer [!UICONTROL Help Request Queue], mit der Benutzer, die ein Problem senden, ein Thema auswählen können. Themen können:</p> 
    <ul> 
     <li>Mit einem benutzerdefinierten Datenformular verknüpfen.</li> 
     <li>Weisen Sie das Problem automatisch einem Benutzer, einer Rolle oder einem Team über den Routing-Regelsatz im ausgewählten Thema zu.</li> 
     <li>Verschieben Sie das Problem in ein anderes Projekt oder eine andere Warteschlange durch den Routing-Regelsatz für das ausgewählte Thema.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Themen für Warteschlangen erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In einem [!UICONTROL Access Level] Bericht können Sie manuell einen [!UICONTROL Rang] der [!UICONTROL Zugriffsstufe] angeben. Dies hilft Ihnen als [!DNL Workfront] -Administrator dabei, die Komplexität der einzelnen Zugriffsebenen visuell zu identifizieren. Sie können beispielsweise niedrigere Zahlen für komplexere ([!UICONTROL Plan]-Zugriffsebenen und höhere Zahlen für weniger komplexe ([!UICONTROL Antragsteller]-Zugriffsebenen) angeben. Die standardmäßigen Zugriffsebenen können nicht eingestuft werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bereit]</td> 
   <td> <p>Dieses Feld in einem Aufgabenbericht gibt an, ob eine [!UICONTROL Agile] Aufgabe im Backlog als [!UICONTROL Bereit] markiert wurde. Diese Markierung gilt nur für [!UICONTROL Agile]-Aufgaben, bei denen es sich um Aufgaben handelt, die einem [!UICONTROL Agile]-Team zugewiesen sind. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Datensatz]</td> 
   <td> <p>In der Workfront-Planung ist ein Datensatz eine eindeutige Instanz eines Datensatztyps.</p>
<p>Nachdem Sie einem Arbeitsbereich einen Datensatztyp hinzugefügt haben, können Sie damit beginnen, Datensätze dieses Typs auf der Seite des Datensatztyps hinzuzufügen.</p>
<p>Beispielsweise kann "Campaign"ein Datensatztyp sein und "Summer Campaign for EMEA"ist ein Datensatz vom Typ "Campaign-Datensatz".</p>
<p>Informationen zum Erstellen von Datensätzen finden Sie unter <a href="/help/quicksilver/planning/records/create-records.md">Erstellen von Datensätzen</a>. </p> <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Der Objekttyp von Workfront Planning.</p>
<p>Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in der Workfront-Planung eigene Objekttypen erstellen. Workfront-Planungs-Objekttypen werden als Datensatztypen bezeichnet.</p>
<p>Beispielsweise sind in Workfront die Objektarten "Programm", "Portfolio", "Projekt", "Aufgabe"oder "Problem"bereits erstellt.</p>
<p>In der Workfront-Planung können Sie beliebige Datensatztypen erstellen, die den Workflows Ihres Unternehmens entsprechen. Später können Sie definieren, wie sich die Datensatztypen untereinander oder mit Formularabhängigkeiten verhalten.</p> Informationen zum Erstellen von Datensatztypen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-record-types.md">Erstellen von Datensatztypen</a>. </p> <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Häufigkeit der Wiederholungen]</td> 
   <td> <p>Ein Feld, das in den [!UICONTROL Aufgabendetails] oder im Feld [!UICONTROL Aufgabe bearbeiten] eines übergeordneten Elements wiederkehrender Aufgaben angezeigt wird. Die Häufigkeit, mit der die Aufgaben in der Wiederholung auftreten. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Erstellen wiederkehrender Aufgaben</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Referenznummer]</td> 
   <td> <p>Projekte, Aufgaben und Probleme werden bei ihrer Erstellung automatisch mit einer eindeutigen Referenznummer verknüpft. Sie können die [!UICONTROL Referenznummer] auf der [!UICONTROL Detailseite] von Projekten, Aufgaben oder Problemen oder in einer Liste oder einem Bericht anzeigen. </p> <p><b>TIPP</b><p><br>Sie können Referenznummern verschieben, wenn zwei Elemente denselben Namen haben, da Referenznummern immer eindeutig sind. </p> <p>[!DNL Workfront] generiert automatisch sequenzielle Referenznummern auf Systemebene. Jedes Projekt, jede Aufgabe oder jedes Problem erhält die nächste verfügbare Zahl in der Sequenz. <br></p> <p>Wenn beispielsweise Benutzer A eine Aufgabe erstellt, weist [!DNL Workfront] der Aufgabe möglicherweise automatisch die Referenznummer 100 zu. Wenn Benutzer B direkt danach ein Problem erstellt, weist [!DNL Workfront] das Problem der Referenznummer 101 zu. Referenznummern können nicht manuell bearbeitet werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zurückweisungsproblem]</td> 
   <td>In einem Projekt oder einem Aufgabenbericht ist dies das Problem, das erstellt wird, wenn die Genehmigung für das Projekt oder die Aufgabe abgelehnt wird. Informationen zu Zurückweisungsproblemen finden Sie im Artikel <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>. </td> 
  </tr>

<tr>
  <td>Beziehungstypen</td>
  <td><p>Workfront-Objekte sind immer miteinander über einen der folgenden Beziehungstypen verbunden:</p>

<ul><li> <b>1:n</b>: In dieser Beziehung kann ein Objekt mit mehreren anderen Objekten unterschiedlicher Typen verbunden werden. Beispielsweise kann ein Projekt mehrere Aufgaben haben. Die Beziehung zwischen Projekt und Aufgaben ist eine Beziehung zu vielen. Sie können diese Beziehung nicht in einem Bericht anzeigen, der die Standardoberfläche verwendet. Sie müssen die Textmodusberichte verwenden, um eine oder mehrere Beziehungen anzuzeigen.</li>
  <li><b>Eins zu eins</b>: In dieser Beziehung kann ein Objekt nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise kann ein Projekt nur eine Gruppe haben. Die Beziehung zwischen Projekt und Gruppe besteht aus einer Eins-zu-Eins-Beziehung. Sie können in einem Standardbericht eine bis eine Beziehung zwischen Objekten anzeigen.</li>
  <li><b>Viele zu eins</b>: In dieser Beziehung können mehrere Objekte nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise können mehrere Aufgaben mit demselben Projekt verbunden werden. Die Beziehung zwischen Aufgaben und Projekt ist eine Beziehung zwischen vielen und einer. Sie können in einem Standardbericht viele bis eine Beziehung zwischen Objekten anzeigen. </li>
  <li><b>Viele zu viele</b>: In dieser Beziehung können mehrere Objekte desselben Typs mit mehreren Objekten eines anderen Typs verbunden werden. Beispielsweise können mehrere Benutzer mehreren anderen Teams angehören und die Teams mehreren Benutzern angehören. Sie können diese Beziehung nicht in einem Bericht anzeigen, der die Standardoberfläche verwendet. Sie müssen die Textmodusberichte verwenden, um viele bis viele Beziehungen anzuzeigen. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Verbleibende Risikokosten]</td> 
   <td> <p>Ein Projektfeld, das die Differenz zwischen den [!UICONTROL Planeten Risikokosten] eines Projekts und den Gesamtkosten aller [!UICONTROL Tatsächlichen Kosten] für alle Risiken des Projekts anzeigt. </p> <p>Die [!UICONTROL Verbleibende Risikokosten] für ein Projekt werden anhand der folgenden Formel berechnet:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Neuplanung]</td> 
   <td>Änderung der Daten eines Projekts zur Behebung oder Behebung von Problemen. Beispielsweise müsste ein Projekt, das mehrere Monate auf Eis gelegt ist, neu geplant werden, um genaue Daten widerzuspiegeln. Dies ist ein manueller Vorgang zur Anpassung der Daten des Projekts oder der Aufgaben. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bericht]</td> 
   <td>Ein Diagramm oder eine Tabelle mit Informationen zu einem bestimmten [!DNL Workfront] -Objekt und den zugehörigen Attributen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Anfrage]</td> 
   <td> <p>Ein Problem, das in einer zentralen Warteschlange getestet wird und nicht mit einem laufenden Arbeitsaufwand in Zusammenhang steht.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Anforderungswarteschlange]</td> 
   <td>Der Rückstand bei Problemen, die durch einen Traffic- und Testprozess verwaltet werden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anforderungsgeschwindigkeit]</td> 
   <td>Gesamtarbeitszyklusdauer für Aufnahme und Durchführung einer Anforderung.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Antragsteller]</td> 
   <td>Normalerweise ein Lizenztyp. Ein Benutzer mit einer Requester-Lizenz kann Anfragen für neue Arbeiten im System einreichen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reservierte Zeit]</td> 
   <td>Tage, die in der persönlichen Zeit eines Benutzers angegeben sind und angeben, dass der Benutzer nicht zur Arbeit verfügbar sein wird. Siehe "[!UICONTROL Nichtarbeitstage]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Problem zu verweisen, das das Problem behebt. </p> <p>Informationen zum Anzeigen aufgelöster Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Auflösbare und aufgelöste Objektinformationen in einem Bericht anzeigen</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auflösungsprojekt]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Projekt zu verweisen, das das Problem behebt. </p> <p>Informationen zum Anzeigen aufgelöster Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Auflösbare und aufgelöste Objektinformationen in einem Bericht anzeigen</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabe auflösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf die Aufgabe zu verweisen, die das Problem behebt. </p> <p>Informationen zum Anzeigen aufgelöster Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Auflösbare und aufgelöste Objektinformationen in einem Bericht anzeigen</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Benutzer oder Rollen, die in [!DNL Workfront] vorhanden sind und den Projektteams, Aufgaben und Problemen zugewiesen sind. Sie sind für die Fertigstellung der Arbeiten im Zusammenhang mit Projekten, Aufgaben oder Problemen verantwortlich. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] ist ein Satz von Tools für Unternehmen, mit denen Sie die Nutzung Ihrer Ressourcen auf der Grundlage ihrer Verfügbarkeit genau vorhersagen können, sodass die zu leistenden Arbeiten rechtzeitig und im Budget abgeschlossen werden. </p> <p>Mit Ressourcen-Management-Tools können Sie langfristige Kapazitäten und kurzfristige Planungsanforderungen für Ihre Ressourcen planen. </p> <p>Informationen zur Ressourcenverwaltung in [!DNL Workfront] finden Sie unter <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit der Ressourcenverwaltung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>In einem Projektbericht können Sie diese Option bei der Erstellung eines Filters verwenden, um einen bestimmten Ressourcen-Manager zu finden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager]</td> 
   <td> <p>In einem Projektbericht oder einer Listenansicht ist dies ein Informationsfeld, in dem Benutzer angezeigt werden, die zur Durchführung von Ressourcenverwaltungsaktivitäten für das Projekt bestimmt sind.  Wenn Sie "[!UICONTROL Resource Manager]"in einem Bericht verwenden, wird eine Liste der Ressourcen-Manager angezeigt, wobei jeder Ressourcen-Manager im Projekt durch ein Komma getrennt ist. Sie können bis zu 30 Ressourcen-Manager für ein bestimmtes Projekt bestimmen.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Ressourcen-Manager für ein Projekt oder eine Vorlage bestimmen </a> .</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planer - Budgetierte Stunden] </td> 
   <td>Die für das Projekt vorgesehenen Stunden und die mit ihm verknüpften Ressourcen im [!UICONTROL Resource Planer]. Siehe auch "[!UICONTROL Budgeted Hours]"in diesem Artikel. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Ein erweitertes [!DNL Workfront] -Tool, mit dem Sie Ressourcen über Projekte, Aufgabenrollen oder Benutzer hinweg anzeigen und verwalten können. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Ressourcenplaner - Übersicht</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenplaner - Budgetierte Arbeitskosten]</td> 
   <td> <p>Dies sind die Kosten, die mit den Stunden verbunden sind, die für die Rolle von Projektaufträgen im Ressourcenplaner veranschlagt sind. </p> <p>Siehe auch "Budgetierte Arbeitskosten"in diesem Artikel. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Ressourcen]</td> 
   <td> <p>Ressourcenpools sind Sammlungen von Benutzern, die mit einem Projekt verknüpft werden können. Die Benutzer im selben Ressourcen-Pool gehören in der Regel zur gleichen Abteilung, verfügen über ähnliche oder komplementäre Fähigkeiten oder werden aus demselben Budget finanziert. Sie können einem Projekt oder einem Benutzer mehrere Ressourcen-Pools zuweisen. Ein Ressourcenpool kann ausschließlich einem Projekt zugewiesen oder von mehreren Projekten gemeinsam genutzt werden.</p> 
   <p>Weitere Informationen zu Ressourcen-Pools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Überblick über Ressourcen-Pools </a>.</p> 
   <p>In Projektberichten zeigen die Ressourcen-Pools alle mit einem Projekt verknüpften Pools an. Dieses Objekt kann nicht in einer Gruppierung verwendet werden.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenauslastung]</td> 
   <td>Ein Bericht, der die Anzahl der Stunden anzeigt, die in einem bestimmten Zeitraum verfügbar sind, sowie die Anzahl der Stunden, die für jeden Benutzer im Bericht geplant sind. Dies wird auch in [!UICONTROL Durchschnittliche Stunden pro Tag] und einem Zuordnungsprozentsatz berechnet.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Ergebnis]</td> 
   <td>In [!DNL Workfront Goals] ist ein Ergebnis ein Fortschrittsanzeigen für ein Ziel. Dabei kann es sich um eine Zahl, einen Prozentwert oder einen Währungsbetrag handeln, den Sie manuell aktualisieren. Ergebnisse in einem Bericht können nicht angezeigt werden und Sie können nicht über die [!DNL Workfront] -API darauf zugreifen. Informationen zu Aktivitäten finden Sie unter <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront-Zielen</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Umsatz]</td> 
   <td>Ein abrechnungsfähiger Betrag für die Aufgabe oder das Projekt. Der Betrag kann stündlich, fest oder eine Kombination aus beidem sein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Umsatz]</td> 
   <td>Der Umsatztyp bestimmt, wie die Aufgabe Umsatz erbringt. Beispiele sind [!UICONTROL Fixed Stündlich], [!UICONTROL Role Stündlich] und [!UICONTROL Role Stündlich w/Cap]. Informationen zum Verfolgen des Umsatzes in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Normalerweise ein Lizenztyp. Ein Benutzer mit einer [!UICONTROL Reviewer]-Lizenz kann Arbeitselemente im System überprüfen und genehmigen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risiko]</td> 
   <td> <p>Dies kann sich auf die folgenden Konzepte in [!DNL Workfront] beziehen:</p> 
    <ul> 
     <li> <p>Ein Feld in einem Projekt, das angibt, wie riskant ein Projekt sein kann. Sie können die Ausführung Ihrer Projekte je nach Risikograd priorisieren. Projekte können die folgenden Risiken aufweisen:</p> <p>- [!UICONTROL Sehr niedrig]</p> <p>- [!UICONTROL Niedrig]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL Hoch]</p> <p>- [!UICONTROL Sehr hoch]</p> <p>Die Risikostufen, die Sie für ein Projekt angeben, können nicht angepasst werden. </p> <p> Informationen zum Aktualisieren des Projektrisikos finden Sie im Abschnitt "Projekteinstellungen"des Artikels <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>. Sie können das Risikofeld eines Projekts in Berichten anzeigen. </p> </li> 
     <li> <p>Ein Ereignis, das während der Laufzeit eines Projekts eintreten kann, das eine potenzielle Auswirkung auf Kosten, Umfang oder Zeitplan des Projekts feststellt. Sie definieren potenzielle Risiken für ein Projekt und verknüpfen eine Wahrscheinlichkeit, dass sie auftreten, oder eine Kosten, während Sie den Geschäftsszenario des Projekts erstellen. Informationen zum Hinzufügen von Risiken zum Geschäftsfall des Projekts finden Sie unter "Risiken für Projekte erstellen und bearbeiten". </p> <p>Sie können keine im [!UICONTROL Geschäftsfall] definierten Risiken in Berichten anzeigen. Sie können nur verschiedene Arten von Risikokosten in Berichten und Listen anzeigen. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risikokosten]</td> 
   <td> <p>Die mit den Risiken eines Projekts verbundenen Kosten. Im Folgenden finden Sie die Risikokosten im Zusammenhang mit Projekten, die Sie in Berichten anzeigen können:</p> 
    <ul> 
     <li> <p>[!UICONTROL Tatsächliche Kosten]: ein Feld für ein Risiko, das die tatsächlichen Kosten für das eingetretene Risiko anzeigt. Zusätzlich zu Berichten und Listen können Sie sie beim Bearbeiten oder Erstellen eines Risikos im Feld [!UICONTROL Risiko bearbeiten] suchen. </p> <p>Informationen zu Projekt-, Aufgaben- oder Problemkosten finden Sie in diesem Artikel unter "[!UICONTROL Tatsächliche Kosten]". </p> </li> 
     <li> <p>[!UICONTROL Geplante Risikokosten]: ein Feld im Projekt, in dem alle [!UICONTROL Potenziellen Risikokosten] für das Projekt ausgewiesen sind. Siehe auch "[!UICONTROL Planed Risk Cost]"in diesem Artikel. </p> <p>Weitere Informationen zu potenziellen Risikokosten finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnen der potenziellen Risikokosten </a>. </p> </li> 
     <li> <p>[!UICONTROL Verbleibende Risikokosten]: ein Feld im Projekt, in dem die Differenz zwischen den gesamten tatsächlichen [!UICONTROL Kosten] aller Risiken und den geplanten [!UICONTROL Risikokosten] angezeigt wird. Siehe auch "Verbleibende Risikokosten"in diesem Artikel. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risikomanagement]</td> 
   <td>Prozesse zur Ermittlung, Minderung und Überwachung von Risiken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rolle]</td> 
   <td>Siehe "[!UICONTROL Job Role]"in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Automatisches Zuweisen oder Verschieben eines Problems, normalerweise aufgrund eines Warteschlangenthemas oder als Standardroute (Routing-Regel) für die Warteschlange.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing-Regel]</td> 
   <td>Eine Einstellung für Projekte und Warteschlangenthemen, mit der einem Benutzer, einer Rolle oder einem Team automatisch ein Problem zugewiesen wird oder das Problem in ein anderes Projekt oder Warteschlangenthema verschoben wird. Routing-Regeln werden in der Regel mit Hilfeanfragewarteschlangen verwendet, um eingehende Probleme automatisch zuzuweisen.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

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
   <td>[!UICONTROL gespeicherte Suche]</td> 
   <td>Eine Suche, deren Suchkriterien gespeichert wurden. Gespeicherte Suchvorgänge erleichtern die wiederholte Ausführung der Suchkriterien, ohne die Suchkriterien erneut eingeben zu müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Szenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Ein Szenario besteht aus einer Reihe von Schritten (Modulen), die angeben, wie Daten zwischen Apps/Diensten übertragen und transformiert werden sollen.</p> <p>Informationen zu Szenarien in [!DNL Workfront Fusion] finden Sie unter <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] szenario - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Szenario] (im [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Im [!DNL Scenario Planner] ist ein Szenario eine Kopie eines Plans. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Überblick [!DNL Scenario Planner]</a>. </p> <p>Informationen zum Erstellen von Szenarien finden Sie unter <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Erstellen und Vergleichen von Planszenarien in der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitplan]</td> 
   <td>Der wöchentliche Arbeitsplan, einschließlich der Arbeitszeiten, kombiniert mit den Tagen ohne Urlaub (z. B. Feiertage) und den Ausnahmetagen (z. B. Samstagarbeitstag). Sie können Zeitpläne mit Projekten und Benutzern verknüpfen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planausnahme]</td> 
   <td>Wird auch als [!UICONTROL Modified Shift] bezeichnet. Im Gegensatz zu den im Zeitplan festgelegten regulären wöchentlichen Arbeitszeiten geplante Tage. So wäre beispielsweise ein Samstag, der für die Arbeit vorgesehen ist, wenn der Zeitplan nur Montag bis Freitag für die Arbeit eingerichtet ist, eine [!UICONTROL geplante Freistellung].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Terminierter Bericht]</td> 
   <td> <p>Wenn Sie einen Bericht mit Berichten erstellen, können Sie Informationen zu den Zeitplänen des Berichts anzeigen, wenn die Bereitstellung des Berichts über das Feld [!UICONTROL Terminierter Bericht] geplant ist. Dieses Feld zeigt mehrere Werte, einen für jeden Zeitplan eines jeden Berichts, in einer Liste mit Aufzählungszeichen an. Weitere Informationen zum Planen von Berichten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Übersicht über die Berichtbereitstellung</a>.</p> <p>Da dieses Feld mehrere Werte anzeigt, kann es nicht in einer Gruppierung verwendet werden. Sie können nur in einem Filter oder einer Ansicht darauf zugreifen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll], das, falls aktiv, bei jeder Änderung des Umfangs eines Projekts oder einer Aufgabe einen Hinweis generiert, z. B. wenn eine [!UICONTROL Task Duration] oder die [!UICONTROL Predecessors] geändert werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschnitt]</td> 
   <td>Ein Bildschirmbereich mit einer eigenen Kopfzeile, der erstellt wurde, um die benutzerdefinierten Daten für Anzeigezwecke zu organisieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschnittsumbruch]</td> 
   <td>Eine Lücke oder Grenze zwischen Abschnitten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sicherheit]</td> 
   <td>Die Einstellungen, mit denen ein Benutzer mit bestimmten Objekten im System und nicht mit anderen interagieren kann. Siehe auch "[!UICONTROL Access Levels]"in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Der Bereich, in dem Administratoren Systemkonfigurationen und Voreinstellungen einrichten können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schweregrad]</td> 
   <td> <p>Der [!UICONTROL Schweregrad] ist ein Hinweis darauf, wie wahrscheinlich ein Artikel die Fertigstellung der Arbeit beeinflussen wird. Beispielsweise kann ein Problem mit hoher [!UICONTROL Prioritätsstufe] den Abschluss einer Aufgabe vollständig blockieren, aber ein Problem mit geringer [!UICONTROL Prioritätsstufe] kann nur kosmetisch sein.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Schweregrad des Problems aktualisieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schwerpunkte]</td> 
   <td>Siehe "[!UICONTROL Severity]"in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Die Aktion, mit der anderen Benutzern die Anzeige oder Bearbeitung eines bestimmten Elements in [!DNL Workfront] ermöglicht wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>In einer Aufgabenansicht oder einem Bericht zeigt das [!UICONTROL Slack Date] das genaue Datum an, an dem eine Aufgabe definitiv das [!UICONTROL Abschlussdatum] des Projekts beeinflussen könnte. Informationen zum [!UICONTROL Slack Date] einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Task Slack Date - Übersicht</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assets]</td> 
   <td> <p>Beim Zuweisen von Aufgaben oder Problemen an Benutzer gibt [!DNL Workfront] Empfehlungen ([!UICONTROL Smart Assignments]) dazu, wer die besten Benutzer die Arbeit abschließen sollten, basierend auf der Zeit, die ihnen zur Verfügung steht, um sie abzuschließen, und ihrer Beziehung zum Projekt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Übersicht über Smart-Zuweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Gibt das übergeordnete Objekt eines anderen Objekts an. Beispielsweise hat ein Dokument, das einer Aufgabe angehängt ist, den Namen der Aufgabe im Feld [!UICONTROL Source] eines [!UICONTROL Document] Berichts oder einer Ansicht. Ein in einem Projekt protokolliertes Problem hat den Namen des Projekts im Feld [!UICONTROL Source] eines Problemberichts oder einer Ansicht. </p> 
   <p>Die folgenden Berichte zeigen eine Source-Spalte an, in der Sie Informationen zum übergeordneten Objekt anzeigen können:</p>
  <ul><li>Problemberichte</li>
    <li>Stündliche Berichte</li>
    <li>Dokumentberichte </li>
    </ul>
   <p>Wenn Benutzer keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, wird die Source-Spalte des Berichts leer angezeigt, selbst wenn der Bericht für die Anzeige oder Bereitstellung mit den Zugriffsrechten eines anderen Benutzers konfiguriert ist. </p>
   <p> Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, wird empfohlen, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der der Name des übergeordneten Objekts angezeigt werden kann. </p>
    <p>Sie können beispielsweise Folgendes zu einem Bericht mit einer Source-Spalte hinzufügen: </p>
    <ul><li>Die Spalten "Projektname", "Aufgabenname"oder "Problemname"in einem Dokument- oder Stundenbericht.</li>
    <li>Die Spalten "Projektname"oder "Aufgabenname"für einen Problembericht. </li> </ul>
    Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Ausführen und Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p>Das Datum, an dem die Arbeit an einem Element auf den Beginn gesetzt ist. Es gibt mehrere Startdaten in [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Geplant]</li> 
     <li>[!UICONTROL realisiert]</li> 
     <li>[!UICONTROL Projekted] </li> 
    </ul> <p>In einem [!UICONTROL Ratenbericht] ist dies das Datum, an dem eine neue Abrechnungsrate für eine Stellenrolle auf Projektebene beginnt. Die mit dem Projekt verknüpften Stunden, die nach diesem Datum liegen, werden mit dieser Abrechnungsrate multipliziert, um den Umsatz für das Projekt zu berechnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Ein Indikator, mit dem eine Workflow-Position eines Arbeitselements oder eines strategischen Ziels signalisiert wird.</p> <p>Bei Projekten ist der [!UICONTROL Status] eine Einstellung im Projekt, die angibt, ob das Projekt:</p> 
    <ul> 
     <li>[!UICONTROL Aktuell]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Abgeschlossen] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Weitere Informationen zum Status eines Projekts finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Zugriff auf die Liste der Systemprojektstatus</a>.</p>
    <p>Bei Aufgaben ist der [!UICONTROL Status] eine Einstellung für die Aufgabe, die angibt, ob die Aufgabe:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL In Bearbeitung</li> 
     <li>[!UICONTROL Abgeschlossen]</li> 
    </ul> <p>Weitere Informationen zum Aufgabenstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Zugriff auf die Liste der Systemaufgabenstatus</a></p> <p>Bei Problemen ist der [!UICONTROL Status] eine Einstellung für das Problem, die angibt, ob dieses Problem:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL In Bearbeitung</li> 
     <li>[!UICONTROL WarteFeedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL aufgelöst]</li> 
     <li>[!UICONTROL wird nicht auflösen]</li> 
     <li>[!UICONTROL Kann nicht duplizieren]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Neu geöffnet]</li> 
    </ul> <p>Weitere Informationen zum Status von Problemen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemfehlerstatus</a>.</p> 
    <p>Bei strategischen Zielen ist der [!UICONTROL Status] eine Einstellung für das Ziel, die angibt, ob das Ziel:</p> 
     <ul> 
      <li>[!UICONTROL Aktiv]</li> 
      <li>[!UICONTROL Entwurf]</li> 
      <li>[!UICONTROL Inaktiv]</li> 
      <li>[!UICONTROL geschlossen]</li> 
     </ul> 
     <p>Weitere Informationen zu strategischen Zielen finden Sie in diesem Artikel auch unter "[!UICONTROL Ziel]"oder "[!UICONTROL Ziele]". </p> 
     <p>Für strategische Ziele ist dieses Feld nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mit [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] Übersicht</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusänderung]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll]. Ein Hinweis wird generiert, wenn ein Benutzer den Status des Projekts, der Aufgabe oder des Problems ändert.</td> 
  </tr> 
  <tr> 
   <td>Status-Symbole</td> 
   <td> <p>Sie können das integrierte [!UICONTROL Status Icons]-Feld als Spalte in Ihren Ansichten hinzufügen, um die Sichtbarkeit in Schlüsselpunkten zu Ihren Objekten zu verbessern, z. B.:</p> 
    <ul> 
     <li>Ein Objekt hat angehängte Dokumente</li> 
     <li>Ein Objekt ist einem Genehmigungsprozess zugeordnet</li> 
     <li>Ein Objekt hat zusätzliche Notizen zugeordnet</li> 
     <li>Eine Ausgabe ist abrechenbar oder rückzahlbar </li> 
     <li>Eine Aufgabe befindet sich auf einem kritischen Pfad</li> 
     <li>Ein Benutzer gehört zu einem Unternehmen, einem Team oder befindet sich in einer anderen Zeitzone. </li> 
    </ul> <p>Sie können das Feld [!UICONTROL Status Icons] in den Ansichten der folgenden Objekte hinzufügen: </p> 
    <ul> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Projekte]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li> 
     <li>[!UICONTROL Vorlagen]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL Dokumente]</li> 
     <li>[!UICONTROL Benutzer]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusaktualisierung]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht zeigt dieses Feld die aktuellste Statusaktualisierung an, die Objekteigentümer im Bereich '[!UICONTROL Updates]' vorgenommen haben. Für Projekte bedeutet dies, dass Kommentare des Projekteigentümers und für Aufgaben und Probleme, dass Kommentare der Bevollmächtigten bedeutet.</p> 
   <p> Kommentare, die bei der Aktualisierung des Status eines Objekts abgegeben wurden, werden nicht in der Spalte [!UICONTROL Status Update] angezeigt.</p> <p>Verwenden Sie die Spalte [!UICONTROL Status] , um den Status '[!UICONTROL In Process]' und '[!UICONTROL Complete]' anzuzeigen.</p> <p>Weitere Informationen zu den Status finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Status der Aufgabe aktualisieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td>Siehe "[!UICONTROL Status]"in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Ein Diagramm, das den Status von Geschichten (Aufgaben in der agilen Methodik) und deren Fortschritt in Richtung Fertigstellung darstellt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Eine Metrik zur Messung der Schwierigkeit oder Komplexität einer Meldung. Agile Teams können wählen, ob Sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Eine Metrik zur Messung der Schwierigkeit oder Komplexität einer Meldung. Agile Teams können wählen, ob Sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Langzeitarbeit, die die Organisation ändert oder die Funktionsweise der Organisation ändert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategische Ausrichtung]</td> 
   <td>Messen und Ausrichten von Unternehmenszielen über Portfolios und Programme hinweg.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Dies wird in Berichtsspalten bei der Verwendung der Textmodus -Benutzeroberfläche verwendet. </p>
   <p>Mit dem <code>[!UICONTROL stretch]</code> wird ermittelt, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. Die Breite der Benutzeroberfläche des Arbeitsbereichs für einen typischen Benutzer beträgt etwa 850 Pixel. Das bedeutet, wenn Sie eine Ansicht mit vier
   Spalten (jeweils 150 Pixel), die Ihre Ansicht 600 von 850 Pixel umfasst. Die Benutzeroberfläche enthält 250 zusätzliche Pixel, die zu den Spalten hinzugefügt werden, für die ein gestreckter Prozentsatz bereitgestellt wird. </p>
   <p>Der Abschnitt einer Spalte wird erzwungen, wenn Sie die zusätzliche Codezeile verwenden: <code>[!UICONTROL usewidths=true]</code> für mindestens eine der Spalten in der Ansicht. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Abonnenten]</td> 
   <td> <p>Benutzer, die Projekte, Aufgaben oder Probleme abonnieren.</p> <p>Wenn Sie dieses Feld in einem Bericht verwenden, wird eine Liste mit Abonnenten angezeigt, wobei jeder Abonnent durch ein Komma getrennt ist.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Elemente in [!DNL Adobe Workfront]</a> abonnieren .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zusammenfassungsaufgabe]</td> 
   <td>Siehe "Übergeordnete Aufgabe[!UICONTROL]"in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unteraufgabe]</td> 
   <td>Eine untergeordnete Aufgabe, die sich unter einer übergeordneten Aufgabe befindet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Eine Reihe von Richtlinien, die Änderungen und die Wartung eines Systems regeln.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Systemintegration]</td> 
   <td>Die Zusammenführung verschiedener Computersysteme und Softwareanwendungen physisch oder funktional, um als koordiniertes Ganzes zu agieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Eine Aktivität, die als Schritt zur Erreichung eines endgültigen Ziels durchgeführt werden muss (Abschluss des Projekts).</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Aufgabenübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task-Attribut]</td> 
   <td>Andere Felder oder Objekte, die mit einer Aufgabe verknüpft sind, und geben bestimmte Details zur Aufgabe an. Einige Beispiele sind [!UICONTROL Planes Abschlussdatum] und [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Siehe "[!UICONTROL Constraint Type]"und "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Eine Reihe von Richtlinien, die die Schwellenwerte für die Erstellung, Zuweisung, Schließung und Sichtbarkeit von Aufgaben bestimmen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>Das für die Schätzung des Aufwands und den Abschluss der Aufgabe verantwortliche Team oder Benutzer</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Eine Sammlung von Benutzern, die ähnliche Ziele oder Geschäftsziele verfolgen. Diese Benutzer können einem Arbeitselement gemeinsam zugewiesen werden, indem das Team dem Arbeitselement zugewiesen wird.</p> <p>Weitere Informationen zu Teams finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Übersicht über Teams</a>.</p> <p>Projekte können über ein [!UICONTROL Projektteam] verfügen, das alle Benutzer oder Rollen enthält, die mit der Arbeit an dem Projekt verknüpft sind.</p> <p>Weitere Informationen zu Projekt-Teams finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Übersicht über das Projektteam</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Vorlage]</td> 
   <td> <p>Projektvorlagen sind allgemeine Entwürfe der wiederholbaren Projekte. Sie können beim Erstellen einer Projektvorlage Aufgaben, Warteschlangenthemen, benutzerdefinierte Formulare, Dokumente anhängen oder Genehmigungen definieren, um Zeit zu sparen, wenn Sie ein neues Projekt erstellen müssen. </p> <p>Sie können Vorlagen an bestehende Projekte anhängen oder sie zum Erstellen neuer Projekte verwenden. Alle in der Vorlage angegebenen Informationen werden an die mit der Vorlage erstellten Projekte übermittelt. </p> <p>Weitere Informationen zu Vorlagen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Übersicht über Projektvorlagen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorlagenaufgabe]</td> 
   <td>Eine Aufgabe, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, das mithilfe der Vorlage erstellt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Eine [!UICONTROL Notiz] und deren Sammlung von Antworten, die sich auf ein bestimmtes Thema beziehen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniaturansicht]</td> 
   <td> <p> In einer [!UICONTROL Dokument]-Liste oder einem Bericht wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p> Wählen Sie <strong>[!UICONTROL Miniatur]</strong> aus.  , um eine 33-66 Pixel breite Miniaturansicht im Bericht anzuzeigen. </p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch "[!UICONTROL Large Thumbnail]"in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Sie können einen [!UICONTROL Time Off]-Bericht erstellen, um zu sehen, wann Benutzer in ihrem Profil eine Zeitüberschreitung angegeben haben. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Eine Zeitkarte, mit der Benutzer tatsächliche Arbeitszeiten eingeben können, die sie mit Projekten, Aufgaben oder Problemen verbracht haben, oder Stunden, die sie für andere Aktivitäten verbracht haben, die nicht mit der Arbeit in Zusammenhang stehen, wie z. B. Meetings oder Schulungen. Zusätzlich zur Eingabe der Arbeitszeit können Sie auch angeben, ob die Arbeitszeit mit der Arbeitszeit verbunden ist oder ob sie mit einer Arbeitszeit verbunden ist, indem Sie Ihre Zeiteinträge mit den Stundentypen definieren. Weitere Informationen zu Timesheets finden Sie unter <a href="../../../timesheets/timesheets/timesheets-overview.md">Timesheets - Übersicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet-Profil]</td> 
   <td> <p>Ein [!UICONTROL Timesheet-Profil] ist eine Vorlage, die [!DNL Workfront] verwendet, um automatisch Timesheets für die ihnen zugeordneten Benutzer zu erstellen. </p> <p>Es besteht die Möglichkeit, für jedes erstellte Datenblatt eine Reihe von Einstellungen zu konfigurieren. Einige dieser Einstellungen sind: wie oft das Timesheet erstellt werden soll (wöchentlich, jede zweite Woche, zweimal im Monat oder monatlich), der Starttag des Zeitplans, die Zeitblatt-Genehmiger, die verfügbaren [!UICONTROL Stunden-Typen], die Benutzer mit aufgezeichneten Stunden verknüpfen können.</p> </td> 
  </tr> 
  <tr > 
   <td>Übergeordnete [!UICONTROL ID] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und deren Untergruppen in einer Liste oder einem Bericht identifizieren und filtern.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordneter Name] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und ihren Untergruppen in einer [!UICONTROL Ansicht] für eine Liste oder einen Bericht identifizieren.</p> <p>Sie können dies auch über das Feld [!UICONTROL Top Parent ID] tun.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gesamtstunden]</td> 
   <td> <p>In einem [!UICONTROL Projektbericht] zeigt dieses Feld die gerundete Summe aller Stunden im Projekt an, bei der die Projektfinanzierung zuletzt berechnet wurde. [!UICONTROL Actual Hours] spiegeln die genauen Stunden wider, die für das Projekt angemeldet sind. Normalerweise sollten die [!UICONTROL tatsächlichen Stunden] mit den [!UICONTROL Gesamtstunden] übereinstimmen. Wenn sich die [!UICONTROL Gesamtstunden] erheblich vom Feld [!UICONTROL Tatsächliche Stunden] unterscheidet, müssen Sie die Projektfinanzierungen neu berechnen.</p> <p>Weitere Informationen zur Neuberechnung der Projektfinanzen finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Neuberechnung der Projektfinanzen vornehmen</a>.</p> <p>In einer Timesheet [!UICONTROL Standard]-Ansicht bezieht sich dieses Feld auf die Gesamtanzahl der Stunden, die für die in einem Zeitblatt angezeigten Daten für die Elemente protokolliert wurden. Das Feld [!UICONTROL Total Hours] für Timesheets in dieser integrierten Ansicht verweist auf das Feld "[!UICONTROL hoursDuration]", das die Differenz in Stunden zwischen dem Start- und dem Enddatum des Zeitblatts dynamisch berechnet. Dies wird verwendet, um die Spalte [!UICONTROL Total Hours] in Rot anzuzeigen, wenn der Benutzer mehr Zeit als die verfügbaren Stunden im Zeitrahmen des Zeitblatts angibt. Weitere Informationen finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Gesamtstunden auf dem Timesheet anzeigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking-Modus]</td> 
   <td> <p>Ein Attribut einer Aufgabe. Dadurch wird festgelegt, wie und wann die vorgeschlagenen Zeitpläne für eine Aufgabe aktualisiert werden. Beispiel:</p> 
    <ul> 
     <li>[!UICONTROL Benutzer muss aktualisieren] erfordert, dass eine Aufgabe manuell aktualisiert wird. Andernfalls wird es [!UICONTROL Hinter dem Zeitplan] und dann zu [!UICONTROL Late].</li> 
     <li>[!UICONTROL Automatischer Abschluss] schließt automatisch eine Aufgabe ab, wenn das Fälligkeitsdatum (oder das geplante Abschlussdatum) überschritten wurde.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Übersicht über den Task Tracking Mode</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Ein Ereignis, das ein Szenario startet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fehleraufgabe]</td> 
   <td>Eine unvollständige Aufgabe mit der Bedingung [!UICONTROL Late], [!UICONTROL Behind Schedule] oder [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nicht zugewiesene Aufgabe]</td> 
   <td>Eine Aufgabe, die keinem Benutzer, einer Rolle oder einem Team zugewiesen ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktualisierungstyp]</td> 
   <td> <p>Eine Einstellung für ein Projekt, die bestimmt, wann die geplante Zeitleiste des Projekts neu berechnet wird. Der [!UICONTROL Aktualisierungstyp] kann die folgenden Werte aufweisen:</p> 
    <ul> 
     <li>[!UICONTROL Automatisch und bei Änderung]</li> 
     <li>[!UICONTROL Automatisch]</li> 
     <li>[!UICONTROL Manual] </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Aktualisierungstyps für das Projekt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzer]</td> 
   <td>Ein in [!DNL Workfront] erstelltes Konto, über das sich eine Person anmelden und mit dem System interagieren kann.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Benutzerdelegierung]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Ihnen Folgendes mitteilt:</p> 
    <ul> 
     <li>Welche Benutzer haben Aufgaben-, Problem- und Projektgenehmigungen delegiert?</li> 
     <li>Welche Benutzer wurden mit Aufgaben-, Problem- und Projektgenehmigungen beauftragt?</li> 
     <li>Wann diese Delegationen beginnen und enden</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Bericht "Benutzerdelegierung erstellen"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzeroberfläche]</td> 
   <td>Alle visuellen und interaktiven Aspekte der [!DNL Workfront]-Anwendung.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzeroberflächeneinstellungen]</td> 
   <td>[!UICONTROL Benutzeroberflächeneinstellungen]. [!DNL Workfront] -Administratoren können diese Einstellungen ändern, um Aspekte der Benutzeroberfläche anzupassen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Nutzung]</td> 
   <td>Die Verfügbarkeit eines Benutzers oder einer Rolle basierend auf dem zugewiesenen Zeitplan, der PTO und der aktuellen Arbeitslast.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerauslastung]</td> 
   <td> <p>Eine Suche in Kombination mit einem Bericht, der anzeigt, wie Benutzer (Ressourcen) zugewiesen oder übergeordnet werden. Siehe "[!UICONTROL Resource Utilization]"in diesem Artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

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
   <td>[!UICONTROL Velocity]</td> 
   <td>Ein Maß für die Gesamtdauer des Arbeitszyklus (wie lange es dauert, ein Arbeitsstück abzuschließen) und wie häufig die Arbeit in der ursprünglich vorgesehenen Zeit ausgeführt wird (Verhältnis zwischen Arbeit und Auftrag).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Ansicht]</td> 
   <td> <p>Ansichten beziehen sich auf ein Berichterstellungselement, mit dem Sie die Spalten eines Berichts oder einer Objektliste ändern können.</p> 
   <p> Ansicht bezieht sich auch auf das Recht eines Benutzers, Informationen nur zu einem Objekt anzuzeigen, je nach Zugriffsstufe oder Berechtigungsfreigabe.</p> 
   <p>In der Workfront-Planung werden Datensätze auf der Datensatztypseite in einem der folgenden Ansichtstypen angezeigt:</p>
   <ul><li>Tabelle</li>
   <li>Timeline</li>
   <li>Kalender</li></ul>
   <p>In der Workfront-Planung umfassen Ansichten die Filter, Gruppierungen, Sortierung und andere Einstellungen, die auf die Datensätze auf dem Bildschirm angewendet werden.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/views/manage-record-views.md">Verwalten von Datensatzansichten</a>.</p>   
   <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Symbole anzeigen]</td> 
   <td> <p> Dies ist dasselbe Feld wie Statussymbole, es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL Dokumente] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten im letzten Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten im letzten Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Nutzung von Berichten anzeigen</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten letztes Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten in diesem Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten in diesem Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Nutzung von Berichten anzeigen</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ansichten in diesem Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtlisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Nutzung von Berichten anzeigen</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> Wenn Sie in einem Bericht die Benutzeroberfläche des [!UICONTROL Textmodus] verwenden, ist dies die Codezeile, in der Sie die Breite jeder Spalte in Pixel angeben können. Workfront bietet für jedes Feld eine empfohlene Breite.
Je nach Art des Felds und Formats können Sie jedoch Anpassungen vornehmen.
Sie müssen die zusätzliche Codezeile <code>[!UICONTROL usewidths=true]</code> verwenden, um die für die Spalte angegebene Breite zu erzwingen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht werden unter Verwendung der folgenden Anweisung im Textmodus die geplanten Stunden des Projekts, der Aufgabe oder des Problems angezeigt:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Syntax des Textmodus</a>. </p> 
   <p><b>TIP</b> 
   <p>Wenn Sie in einen Problembericht eines der Felder [!UICONTROL Geplante Stunden] einfügen, wird das Feld <code>work </code>zum Bericht hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Einer der beiden primären Lizenztypen. Dies hat weniger Zugriff als [!UICONTROL Plan], kann jedoch im System Aktualisierungen erstellen und vornehmen. Ein Benutzer mit einer Work-Lizenz verfügt über mehr Fähigkeiten als ein [!UICONTROL External]-, [!UICONTROL Reviewer]- oder [!UICONTROL Antragsteller]-Lizenzinhaber.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Lizenzübersicht</a>.</p> <p>Die Arbeit kann sich auf die Anzahl der geplanten [!UICONTROL Stunden] für ein Projekt, eine Aufgabe oder ein Problem beziehen. Weitere Informationen finden Sie im Feld "[!UICONTROL work]"in dieser Tabelle. </p> <p><b>TIPP</b></p> <p> Wenn Sie in einen Problembericht eines der Felder [!UICONTROL Geplante Stunden] einfügen, wird das Feld <code>work </code>zum Bericht hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Struktur der Arbeitsaufschlüsselung]</td> 
   <td>Eine hierarchische Struktur der vom Projektteam auszuführenden Aufgaben basierend auf der übergeordneten/untergeordneten Beziehung.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsaufwand] </td> 
   <td> 
    <p>Ein Projektmanager kann beschließen, dieses Feld anstelle von [!UICONTROL Geplante Stunden] zu verwenden, um den für die Erfüllung einer Aufgabe erforderlichen Aufwand abzuschätzen. Dieses Feld ist nur sichtbar, wenn die folgenden Bedingungen erfüllt sind:</p> 
     <ul> 
      <li> <p>Die Aufgabe hat einen [!UICONTROL einfachen Dauertyp]. </p> <p><b>TIPP</b></p> <p> Wenn Sie die Aufgabe [!UICONTROL Duration Type] auf einen anderen Typ aktualisieren, wird dieses Feld ausgeblendet. </p> </li> 
      <li>Der Projektmanager hat das Feld [!UICONTROL Arbeitsaufwand verwenden] aktiviert, um die [!UICONTROL geplante Arbeitszeit] automatisch für das Projekt zu berechnen. </li> 
     </ul> 
     <p>Informationen zur Verwendung von [!UICONTROL Work Effort] anstelle von [!UICONTROL Planeten Stunden] zur Schätzung des Aufgabenaufwands finden Sie unter <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>. </p> 
     <p>Sie können dieses Feld in Aufgabenberichten und -listen anzeigen.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitselement]</td> 
   <td> <p>Dieses Feld bezieht sich entweder auf Aufgaben oder Probleme in [!DNL Workfront]. </p> <p>Der Bericht [!UICONTROL Arbeitselement] enthält Informationen zu Aufgaben und Problemen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Mix]</td> 
   <td>Ein [!UICONTROL Work Performance Indicator] (WPI) des Anteils der Arbeit, die für die Ausführung Ihres Unternehmens zugewiesen wurde, im Vergleich zu einer Änderung Ihres Unternehmens. Die Mix-WPI hilft Ihnen, auf organisatorischer Ebene zu verstehen, ob für Ihre Strategie eine echte Arbeitszuordnung angewendet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Benennung einer Person im System, die für die Aufnahme einer Arbeits- oder Verfolgungszeit berechtigt ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rolle und Zuständigkeiten des Arbeitsmanagements]</td> 
   <td>Definition der Eigentümer und Interessengruppen für die Verwaltung des Umfangs, der Ausführung und der Genehmigungen der festgelegten Ausgabe, Aufgabe, des Projekts, Programms oder Portfolios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management SLA]</td> 
   <td>Eine quantifizierbare Metrik, auf die sich alle Beteiligten geeinigt haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stakeholder im Arbeitsmanagement]</td> 
   <td>Eine Sammlung von Benutzern, die ein eigenes Interesse an den Ergebnissen einer Arbeitsanfrage haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Touchpoints im Arbeitsmanagement]</td> 
   <td>Digitalisierte Aufzeichnungen der Kommunikation zwischen den Akteuren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Leistungsindikatoren] </td> 
   <td> <p>Mischen Sie Verhältnis, Kapazität, Geschwindigkeit, Qualität und Interaktion.</p> <p>WPI ist ein gängiges Akronym für [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsprozess]</td> 
   <td> <p>Die Methode, bei der Arbeiten empfangen, priorisiert und ausgeführt werden. Die Ausführung der Arbeit wird in der Regel als "Workflow"oder "Projektplan"bezeichnet (eine Liste von Aufgaben mit Datumsangaben, Vorgängerbeziehungen usw.). </p> <p>Beispiele für einen Arbeitsprozess sind die Produktion eines einzelnen Assets oder die Bereitstellung einer Kampagne mit mehreren Assets. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow-Vorlage]</td> 
   <td>Im Bericht [!UICONTROL Validierung des Testversands] werden in diesem Feld alle an einen Testversand angehängten Workflow-Vorlagen angezeigt. Wenn keine Vorlagen angehängt sind, ist die Spalte leer.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>

<p>Stellt den Prozentsatz der Vollzeitäquivalenzzeit ([!UICONTROL FTE]) dar, der dem Benutzer für die tatsächliche Arbeit zur Verfügung steht, ohne den Mehraufwand. Die [!UICONTROL Arbeitszeit] muss eine Dezimalzahl von bis zu 1 sein, und sie darf nicht 0 sein. Eine Verfügbarkeit von 20 % für tatsächliche Arbeit wäre beispielsweise 0,2.</p>
   </p>Der Standardwert des Felds ist 1, was bedeutet, dass ein Benutzer seine gesamte [!UICONTROL FTE] für tatsächliche, projektbezogene Arbeit ausgibt.  </p>
   <p>Das System verwendet diese Zahl, um die Verfügbarkeit des Benutzers für tatsächliche, projektbezogene Arbeiten zu berechnen. </p>
   <p> Eine Planung von Ausnahmen und Zeitüberschreitungen kann sich auch auf die Benutzerkapazität auswirken. </p>
   <p>Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>
    <p>Workfront berechnet die Verfügbarkeit eines Benutzers entsprechend den Voreinstellungen für die Ressourcenverwaltung im [!UICONTROL Setup]-Bereich. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>. </p> 
   <p>Sie können die [!UICONTROL Arbeitszeit] eines Benutzers aktualisieren, wenn Sie den Benutzer bearbeiten oder erstellen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Profil eines Benutzers bearbeiten</a></p> 
   <b>TIP</b> 
   <p>Setzen Sie den Wert [!UICONTROL Arbeitszeit] auf 1, um anzugeben, dass der Benutzer für projektbezogene Arbeit in seiner gesamten Vollzeitäquivalenz verfügbar ist.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>In der Workfront-Dokumentation wird dieser Begriff verwendet, um die Arbeitszeit gemäß einem Zeitplan zu beschreiben.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht zeigt die Verwendung der folgenden Anweisung im Textmodus die Anzahl der geplanten Stunden des Projekts, der Aufgabe oder des Problems an, gefolgt vom Wort "Stunden":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Syntax des Textmodus</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>In der Workfront-Planung ist ein Arbeitsbereich eine Sammlung von Datensatztypen, die den Lebenszyklus einer bestimmten Organisation definieren. Ein Arbeitsbereich ist der Arbeitsbereich einer Organisationseinheit.</p>
   <p>Für die Planung von Workfront ist eine zusätzliche Lizenz erforderlich. </p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Erstellen von Arbeitsbereichen</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


