---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossar der  [!DNL Adobe Workfront] '
description: Das  [!DNL Adobe Workfront] -Glossar listet häufig verwendete Begriffe in  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] -Oberfläche, Berichte oder Sie versuchen, die Bedeutung von  [!DNL Workfront]  in der  [!DNL Workfront] -Dokumentation definierten Konzepten zu verstehen.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '20931'
ht-degree: 0%

---


# Glossar [!DNL Adobe Workfront] Terminologie

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Dieser Artikel sollte als Referenz verwendet werden, um die Begriffe zu verstehen, auf die Sie in der [!DNL Adobe Workfront] Anwendung, in der [!DNL Workfront]-Dokumentation oder im Allgemeinen bei der Planung und Verwaltung von Arbeit stoßen können. Diese Informationen werden derzeit aktualisiert, sodass diese Tabelle möglicherweise nicht vollständig ist. Wir werden diesen Haftungsausschluss entfernen, wenn wir diese Informationen für erschöpfend halten.

In der folgenden Tabelle finden Sie eine Liste häufig verwendeter Begriffe in Adobe Workfront:

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
   <td>Ein Benutzerprofil, das bestimmt, wie Benutzende mit verschiedenen Objekten und Tools in Workfront interagieren können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktive Aufgabe]</td> 
   <td>Eine unvollständige Aufgabe in einem aktuellen Projekt, die nicht durch eine Vorgängeraufgabe daran gehindert wird, bearbeitet zu werden, und die keine Aufgabenbeschränkung mit einem geplanten Startdatum für die Zukunft hat. Mit anderen Worten, man kann heute daran arbeiten.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL-Aktivität]</td> 
   <td>In [!DNL Workfront Goals] ist eine Aktivität eine Fortschrittsindikatorfunktion für ein Ziel. Dabei kann es sich um eine Fortschrittsleiste handeln, die Sie manuell aktualisieren, oder um ein Projekt, das mit dem Ziel verknüpft ist. Sie können keine Aktivitäten in einem Bericht anzeigen und nicht über die [!DNL Workfront] API darauf zugreifen. Informationen zu Aktivitäten finden Sie unter <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Erste Schritte mit Ergebnissen und Aktivitäten in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Istkosten]</td> 
   <td> <p>Bei Vorgängen und Problemen sind dies die Kosten, die mit den tatsächlich protokollierten Stunden verknüpft sind, und zwar im Verhältnis zum Stundensatz der Ressource, die der Aufgabe oder dem Problem zugewiesen wurde. Bei Projekten entspricht dies der Summe aller [!UICONTROL Istkosten] aus Aufgaben und Problemen des Projekts. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächliche Ausgabenkosten]</td> 
   <td> <p>Die Summe der [!UICONTROL Ist-Beträge] für alle Ausgaben, die für ein Projekt oder eine Aufgabe protokolliert wurden.</p> <b>BEISPIEL </b>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und 600,00 $ in das Feld [!UICONTROL Istbetrag] eingeben, beträgt die [!UICONTROL Istkosten] für diese Aufgabe 600,00 $. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um [!UICONTROL Tatsächliche Ausgabenkosten] zu berechnen:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächliche Stunden]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht sind [!UICONTROL Actual Hours] die Summe aller für das Projekt, die Aufgabe oder das Problem protokollierten Stunden.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span> Wenn Sie auf der Registerkarte [!UICONTROL Updates] für Aufgabe 1 auf „Zeit protokollieren“ klicken und 25 Stunden eingeben, sind die tatsächlichen Stunden von Aufgabe 1 = 25 Stunden. </p> <p>[!DNL Workfront] Berechnet [!UICONTROL Tatsächliche Stunden] für übergeordnete Aufgaben oder Projekte anhand der folgenden Formeln:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ist-Lohnkosten]</td> 
   <td> <p>Die [!UICONTROL Istkosten], die mit den in eine Aufgabe oder ein Projekt investierten Arbeitskräften verbunden sind. </p> <p>Für eine Aufgabe berechnet [!DNL Workfront] die [!UICONTROL Ist-Lohnkosten] anhand der folgenden Formel:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Wenn die Aufgabe einen [!UICONTROL Kostentyp] von [!UICONTROL Benutzer Stündlich] hat, verwendet [!DNL Workfront] den Benutzersatz. Wenn die Aufgabe einen [!UICONTROL Kostentyp] von [!UICONTROL Role Hourly] hat, berechnet [!DNL Workfront] die tatsächlichen [!UICONTROL Ist-Lohnkosten] anhand des Tarifs für Aufgabengebiete. </p> <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um die [!UICONTROL Ist-Lohnkosten] zu berechnen:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten </a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn ein Benutzer beispielsweise 5 Stunden für eine Aufgabe mit dem Kostentyp [!UICONTROL Benutzer Hourly] [!UICONTROL] protokolliert und ihr Stundensatz 100 $ beträgt, beträgt die tatsächliche Arbeitskosten von [!UICONTROL] 500 $.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tatsächlicher Umsatz] </td> 
   <td> <p>Der [!UICONTROL Tatsächlicher Umsatz] eines Projekts oder einer Aufgabe ist der Geldbetrag, der mit den [!UICONTROL Tatsächliche Stunden] des Projekts oder der Aufgabe verknüpft ist. </p> <p>Informationen zur Umsatzverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tatsächlicher Start]</td> 
   <td>Der Zeitstempel, wann ein Benutzer ein Objekt ändert, das gerade an ihm zugewiesenen Arbeiten durchgeführt wird.</td> 
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
   <td>Eine Art von Methodik, die auf der gemeinsamen Entwicklung von Anforderungen und Lösungen mit funktionsübergreifenden Teams basiert. Es fördert Flexibilität und Veränderungen auf der Grundlage eines festen Zeitplans.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Unterscheidet sich von einem herkömmlichen Team, da es seine voraussichtliche Arbeit aus einem Rückstand nimmt und innerhalb eines bestimmten Zeitraums daran arbeitet, der als [!UICONTROL Iteration] bezeichnet wird.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alle meine Teams]</td> 
   <td> <p>Wenn in [!UICONTROL filters] darauf verwiesen wird, zeigt dieses Feld entweder Benutzer an, die zu einem der Teams gehören, denen der angemeldete Benutzer angehört, oder Arbeitselemente, die einem der Teams zugewiesen sind, denen der angemeldete Benutzer angehört. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuordnungsdatum]</td> 
   <td> <p>Dieses Feld finden Sie in den folgenden Berichtstypen:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL-Projekt] (Finanzdaten)</li> 
     <li>[!UICONTROL Budgetierte Stunde]</li> 
    </ul> <p>Für einen <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)]-Bericht: </p> 
    <ul> 
     <li>Erstellen Sie diesen Bericht, wenn Sie versuchen zu verstehen, <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> wie viele [!UICONTROL Planned Hours] Ihren Ressourcen zugewiesen sind.</li> 
     <li> <p>Das [!UICONTROL Zuordnungsdatum] ist der erste Tag (Sonntag) einer Woche, in der die Zuordnung eines [!UICONTROL Aufgabengebiets] zu einer Aufgabe beginnt. Eine Ressource ([!UICONTROL Aufgabengebiet]) kann so viele [!UICONTROL Zuordnungsdaten] haben, wie sie Wochen während der [!UICONTROL Dauer] der Aufgaben hat, denen sie zugewiesen ist. Wenn Aufgaben sich über mehrere Monate erstrecken, kann der erste Tag eines Monats auch zu einem [!UICONTROL Zuteilungsdatum] werden, wenn er in die [!UICONTROL Dauer] der Aufgabe fällt.</p> <p>Sie können beispielsweise ein [!UICONTROL Aufgabengebiet] einer Aufgabe zuweisen, die sich über 3 Wochen erstreckt und 90 [!UICONTROL Geplante Stunden] hat. Diese Stunden werden während der Aufgabendauer gleichmäßig verteilt, sodass Sie Ihrem Aufgabengebiet täglich 6 [!UICONTROL Geplante Stunden] zuweisen:</p> <p><em> [!UICONTROL Tägliche geplante Stunden] = [!UICONTROL Gesamte geplante Stunden]/ Anzahl der [!UICONTROL Arbeitstage] während der [!UICONTROL-Dauer] des </em> </p> <p>Infolgedessen gibt es drei [!UICONTROL Zuteilungstermine], einen für jeden Sonntag jeder Woche während der [!UICONTROL Duration] der Aufgabe, wobei jeder eine bestimmte Anzahl von [!UICONTROL Geplante Stunden] zugeordnet ist.<br>Wenn die Aufgabe Mitte der letzten Woche eines Monats beginnt und zwei Wochen nach dem Beginn eines neuen Monats endet, hat die Aufgabe vier [!UICONTROL Zuteilungstermine]: einen für jeden Sonntag jeder Woche während der [!UICONTROL Duration] der Aufgabe und einen für den ersten Tag des neuen Monats.</p> <p>Um diese Informationen optimal zu nutzen, empfehlen wir, einen <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Projektbericht (Finanzdaten) zu erstellen und eine Matrixgruppierung für [!UICONTROL Zuteilungsdatum] hinzuzufügen. Anschließend werden die Ergebnisse wöchentlich, monatlich, vierteljährlich oder jährlich gruppiert, um die genauesten Daten zu erhalten.<br>Informationen zum Erstellen einer Matrixgruppierung finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Erstellen eines Matrixberichts</a>.</p> </li> 
    </ul> <p>Finanzinformationen werden nur dann in [!UICONTROL Project (Financial Data)]-Berichte eingefügt, wenn die damit verbundenen Daten weniger als 5 Jahre alt sind. Wenn beispielsweise einer Aufgabe im Januar 2015 ein Aufgabengebiet zugewiesen wurde und heute September 2021 ist, wird ein Finanzfeld wie das [!UICONTROL Zuordnungsdatum] für das Aufgabengebiet nicht im Bericht [!UICONTROL Project (Financial Data)] angezeigt. </p> 
    <div> 
     <p>Für einen Bericht zu [!UICONTROL Budgetierte Stunde]:</p> 
     <ul> 
      <li>Erstellen Sie diesen Bericht, wenn Sie versuchen, die Menge an [!UICONTROL Budgetierte Stunden] zu verstehen, die Ihren Ressourcen oder Ihren Projekten im Ressourcenplaner zugewiesen ist.</li> 
      <li> <p>Das [!UICONTROL Zuordnungsdatum] ist der erste Tag (ein Sonntag) der Woche, für die Sie die Stunden im [!UICONTROL Ressourcenplaner] budgetiert haben. </p> <p><b>TIPP</b></p> <p>Wenn sich eine Woche über zwei Monate erstreckt, werden zwei Zeilen im Bericht generiert: eine Zeile, die dem ersten Wochentag entspricht (Sonntag der ersten Woche, die im ersten Monat liegt), und die zweite Zeile zeigt den ersten Tag des zweiten Monats an. </p> <p>Wenn Sie beispielsweise 8 Stunden für einen Benutzer für die Woche vom 30. Juni (Sonntag) bis zum 6. Juli (Samstag) budgetieren, zeigen die beiden Zeilen ein [!UICONTROL Zuordnungsdatum] vom 30. Juni und 1. Juli an. </p> </p> <p>Informationen zur Budgetierung von Ressourcen im [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen im [!DNL Resource Planner] mithilfe der Ansichten [!UICONTROL Project] und [!UICONTROL Role</a>.</p> <p>Informationen zum Erstellen eines Berichts zur [!UICONTROL Budgetierte Stunde] finden Sie unter <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ankündigungen]</td> 
   <td> <p>Eine Möglichkeit, Benutzerinformationen innerhalb des Systems zu kommunizieren. Diese Informationen stammen oft vom [!DNL Workfront] an den Administrator oder vom Administrator an den Benutzer. </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Ankündigungen senden</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App-Integration]</td> 
   <td>Eine App stellt meist einen Connector zu einer Software-Anwendung dar, kann aber auch spezielle Funktionen zur Bearbeitung von Daten darstellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Genehmigerentscheidung]</td> 
   <td> <p>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld Korrekturabzugsgenehmigungsentscheidungen für Korrekturabzüge an, die nicht mehr aktiv sind.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmiger-Phase]</td> 
   <td>Im [!UICONTROL Korrekturabzugs-Genehmigungs-Bericht] zeigt dieses Feld Informationen zu einem aktuellen Korrekturabzugsschritt an.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Genehmigung]</td> 
   <td> <p>Für ein bestimmtes Arbeitselement, z. B. eine Aufgabe, ein Dokument oder eine Arbeitszeittabelle, kann es erforderlich sein, dass ein Verantwortlicher oder ein anderer Benutzer das Arbeitselement abzeichnet. Dieser Prozess der Abzeichnung wird als Genehmigung bezeichnet. </p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über den Genehmigungsprozess</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Genehmigungsdatum]</td> 
   <td>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld das Datum an, an dem ein Korrekturabzug genehmigt wurde.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL genehmigende Person]</td> 
   <td>Ein Benutzer oder Aufgabengebiet, der bzw. das für ein bestimmtes Arbeitselement abzeichnen muss oder Stundeneinträge in Arbeitszeittabellen genehmigt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL zugewiesen zu]</td> 
   <td> <p>In einem [!UICONTROL Aufgabe oder Problem]-Bericht zeigt dieses Feld den Verantwortlichen der Aufgabe oder des Problems oder den [!UICONTROL Primärer Verantwortlicher] an. Sie können auch nach diesem Feld filtern oder gruppieren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Zuweisung]</td> 
   <td>Ein Benutzer, ein Aufgabengebiet oder ein Team, das bzw. das einem Problem oder einer Aufgabe zugewiesen ist. Projekte, Portfolios oder Programme dürfen keine Zuweisungen haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Zuweisungen]</td> 
   <td> <p>In einem [!UICONTROL Aufgabe]- oder [!UICONTROL Problem]-Bericht zeigt dieses Feld eine Liste aller Entitäten (Benutzer, Aufgabengebiete, Teams) an, die der Aufgabe oder dem Problem zugewiesen sind. Sie können nach diesem Feld filtern, indem Sie die Felder [!UICONTROL Assignment Users] und [!UICONTROL Assignment Roles] verwenden. Sie können über das Feld Team nach dem Team filtern, das der Aufgabe oder dem Problem zugewiesen wurde. Sie können einen Bericht nicht nach diesem Feld gruppieren.</p> <p>Arbeitselemente, die in den [!UICONTROL Papierkorb] gelegt wurden, werden weiterhin in einigen Berichten angezeigt, die auf das [!UICONTROL Zuweisungsobjekt] verweisen, in dem ein [!DNL OR] verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisungsrollen]</td> 
   <td>
   <p>In einem [!UICONTROL Aufgabe]- oder [!UICONTROL Problem]-Bericht zeigt dieses Feld Informationen zu den den Aufgaben oder Problemen zugewiesenen Aufgabengebieten an. In diesem Feld werden [!UICONTROL Primäre Verantwortliche] sowie andere Aufgabengebiete angezeigt, die Aufgaben oder Problemen zugewiesen sind.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuweisungsstatus]</td> 
   <td> <p>In einem Zuweisungs-, Aufgaben- oder Problembericht zeigt der [!UICONTROL Zuweisungsstatus] an, ob die einem Arbeitselement zugewiesenen Benutzer zum Annehmen oder Abschließen der Arbeit auf die Schaltfläche [!UICONTROL Work On It] oder [!UICONTROL Done] geklickt haben. Die folgenden [!UICONTROL Zuweisungsstatus] sind vorhanden:</p> 
    <ul> 
     <li><b>[!UICONTROL angefordert]</b>: Der/die Benutzende wurde der Aufgabe oder dem Problem zugewiesen, hat jedoch noch nicht auf die Schaltfläche [!UICONTROL Bearbeiten] geklickt, um mit der Bearbeitung zu beginnen.</li> 
     <li><b>[!UICONTROL Working]</b>: Der Benutzer hat auf die Schaltfläche [!UICONTROL Work On It] geklickt und arbeitet derzeit an dem Element. </li> 
     <li><b>[!UICONTROL Done]</b>: Der Benutzer hat auf die Schaltfläche [!UICONTROL Done] geklickt und seine Arbeit am Element abgeschlossen. </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Bearbeiten] und [!UICONTROL Fertig] Schaltfläche Übersicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftragsteams]</td> 
   <td>
   <p>In einem [!UICONTROL task]- oder [!UICONTROL issue]-Bericht zeigt dieses Feld Informationen zu den Teams an, die den Aufgaben oder Problemen zugewiesen wurden. Das Feld zeigt [!UICONTROL Primäre Verantwortliche] sowie andere Teams an, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitsauftrag - Benutzer]</td> 
   <td>
   <p>In einem [!UICONTROL Aufgabe]- oder [!UICONTROL Problem]-Bericht zeigt dieses Feld Informationen zu den Benutzern an, die den Aufgaben oder Problemen zugewiesen wurden. In diesem Feld werden [!UICONTROL Primäre Eigentümer] sowie andere Benutzende angezeigt, die Aufgaben oder Problemen zugewiesen sind. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Attribut]</td> 
   <td>Ein Attribut ist eine Eigenschaft eines [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auditbereich]</td> 
   <td> <p>Audits sind Systemmeldungen, die eine Aktion aufzeichnen, die in Workfront stattfand. Die folgenden Audittypen werden aufgezeichnet:</p> 
    <ul> 
     <li>[!UICONTROL Umfangsänderung]</li> 
     <li>[!UICONTROL Anlagenaktion]</li> 
     <li>[!UICONTROL Allgemeine Bearbeitung]</li> 
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
   <td>Die Sammlung von Notizen, die automatisch von Ereignissen generiert werden, die durch die aufgezeichneten Änderungen ([!UICONTROL Audit Areas]) verfolgt werden. In jeder Notiz wird aufgezeichnet, wer die Aktion ausgeführt hat, was sie getan hat und wann sie sie ausgeführt hat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatisch und bei Änderung]</td> 
   <td> <p>Einer der [!UICONTROL Project Update]-Typen. Dadurch werden die erwarteten und geplanten Zeitleisten des Projekts neu berechnet, wenn der Prozess der nächtlichen Neuberechnung ausgeführt wird und wenn am Projekt oder an den Aufgaben innerhalb des Projekts Aktualisierungen vorgenommen werden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswahl des Projektaktualisierungstyps </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Verfügbarkeit</p></td> 
   <td> <p>Dieser Begriff wird in Bezug auf „Benutzerverfügbarkeit“ oder „Ressourcenverfügbarkeit“ verwendet und veranschaulicht die Zeitdauer, während der die Ressource (Benutzer oder Aufgabengebiet) für die Arbeit verfügbar ist. </p> 
   <p>Workfront berechnet die Benutzerverfügbarkeit anhand mehrerer Felder und abhängig von den Einstellungen in den Einstellungen für die Ressourcenverwaltung in Ihrem System. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>. </p>
   <p>Weitere Informationen zur Ressourcenverfügbarkeit finden Sie unter <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit der Ressourcenverwaltung</a></p>
   Alternativ wird auch „Kapazität“ verwendet, um auf die Verfügbarkeit von Ressourcen zu verweisen. 
   </td> 
  </tr>

<tr> 
   <td>[!Nur UICONTROL automatisch]</td> 
   <td> <p>Einer der [!UICONTROL Project Update]-Typen. Dadurch werden die prognostizierten und geplanten Zeitleisten bei der nächtlichen Neuberechnung neu berechnet.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswahl des Projektaktualisierungstyps</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Ein „Business as usual“ ist eine Arbeit, die dazu beiträgt, die alltäglichen primären Geschäftsziele zu erreichen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>Der Bereich in einer agilen Umgebung, in dem neue Probleme aufbewahrt werden, bis sie bereit sind, bearbeitet zu werden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Eine Datenquelle, an der Iterationen in einer agilen Umgebung gemessen werden.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Verrechenbare Kosten]</td> 
   <td> <p>Eine Ausgabe, die für den Kunden als fakturierbar gekennzeichnet ist. Dies kann entweder eine geplante Ausgabe oder eine tatsächliche Ausgabe sein.</p> <p>Die Felder Geplante abrechenbare Kosten und Tatsächliche abrechenbare Kosten können zu Ansichten und Berichten hinzugefügt werden. Sie werden nicht auf den Seiten mit den Projekt- oder Aufgabendetails angezeigt.</p>
   <p>Diese Felder finden Sie in den folgenden Berichtstypen:</p>
   <ul>
   <li>Ausgangsbasis</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Kennzeichnen einer Ausgabe als fakturierbar finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Projektausgaben verwalten</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Rechnungsnachweis]</td> 
   <td> <p>Erfasst die Einnahmen, Stunden oder Ausgaben, die in Rechnung gestellt werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchhaltungssystem verwendet werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Rechnungsnachweise erstellen</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status des Rechnungsnachweises</td> 
   <td> <p>In einem Rechnungsnachweis oder Stundenbericht gibt der Status eines Rechnungsnachweises an, ob der Rechnungsnachweis in Rechnung gestellt wurde oder nicht. Sie können kein Projekt löschen oder die mit einem Rechnungsnachweis verknüpfte Zeit bearbeiten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Rechnungsnachweise erstellen</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Der Prozess der Anpassung von [!DNL Workfront], um der Oberfläche ein Erscheinungsbild zu geben, das Ihrem Unternehmen entspricht, indem Sie Ihre Farben und Logos verwenden.</p><p><strong>HINWEIS</strong><br>Wenn Ihre Organisation in [!DNL Adobe Experience Cloud] integriert wurde, ist kein Branding verfügbar.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Der Bereich oben auf der Seite, der die hierarchische Position anzeigt, an der sich der Benutzer in der Anwendung befindet.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Weitere Informationen finden Sie unter <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Breadcrumbs - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetstatus]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die dieses Feld möglicherweise anzeigt, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat und das Feld kann nicht aktualisiert werden. </p> <p>Dieses Feld zeigt an, ob das Projekt dem [!UICONTROL Kapazitätsplaner] hinzugefügt wurde und ob die Budgetberechnung dafür abgeschlossen wurde. Der [!UICONTROL Capacity Planner] wurde aus [!DNL Workfront] entfernt. </p> 
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
   <td> <p>Dies ist ein veraltetes Feld. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden. </p>
   <p> Dieses Feld ist weiterhin in [!UICONTROL project]-Berichten und -Listen sichtbar.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgetierte Kosten]</td>

<td> <p>Dies sind die Kosten für die Budgetierung von Ressourcen für ein Projekt. </p>
   <p>Das Feld wird in den folgenden [!DNL Workfront] unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL Budgetierte Kosten]</strong>: im Bedienfeld [!UICONTROL Business Case-Zusammenfassung]</li>
   <li><strong>[!UICONTROL Kosten]</strong>: in den Bereichen [!UICONTROL Auslastung], wenn Sie Informationen nach [!UICONTROL Kosten] anzeigen</li>
   <li><strong>[!UICONTROL Projekt budgetierte Kosten]</strong>: in Listen und Berichten</li>
   </ul>   
    <p>Die [!UICONTROL Budgetierte Kosten] für das Projekt werden anhand der folgenden Formel berechnet:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Weitere Informationen zur Berechnung der [!UICONTROL Budgetierten Kosten] und verschiedene Namen für dieses Konzept in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Berechnen der budgetierten Projektkosten</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgetierte Stunden]</td> 
   <td> <p>Die budgetierten Stunden der Ressourcen für die Arbeit, die sie an Projekten durchführen müssen. Dieses Feld bezieht sich auf die budgetierten Stunden im Bereich [!UICONTROL Resource Budgeting] des [!UICONTROL Business Case] (oder im [!UICONTROL Resource Planner]) für das Projekt oder die Projektressourcen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Grundlegendes zu [!UICONTROL Budgetierte Lohnkosten] und [!UICONTROL Budgetierte Stunden] für Projekte</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Informationen zur Budgetierung von Benutzern in der [!DNL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen in der [!DNL Resource Planner] mithilfe der Ansichten [!UICONTROL Project] und [!UICONTROL Role</a>. </p> 
    <p>Die budgetierten Stunden im Bereich [!UICONTROL Resource Budgeting] des [!UICONTROL Business Case] oder des [!UICONTROL Resource Planner] werden in den folgenden [!DNL Workfront] und unter den folgenden Namen angezeigt:</p> 
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
        <td>[!UICONTROL Resource Budgeting]-Bereich des [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] angezeigt von [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgetierte Stunden]</td> 
        <td> <p>Ansicht „Auslastungsbericht [!UICONTROL Hours]"</p> <p>Weitere Informationen zum Bericht zur [!UICONTROL-Nutzung] finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Übersicht über den Bericht zur [!UICONTROL-Ressourcenauslastung</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BUD. Stunden]</td> 
        <td> <p>Bericht zu [!UICONTROL Budgetierte Stunde]</p><p>Das Objekt [!UICONTROL Budgetierte Stunde] im Bericht Budgetierte Stunde bezieht sich auf Informationen zu einem veralteten Ressourcenverwaltungstool. Nur der "[!UICONTROL BUD. Stunden]" in diesem Bericht bezieht sich auf die budgetierten Stunden im Bereich [!UICONTROL Resource Planner] oder [!UICONTROL Resource Budgeting] des [!UICONTROL Business Case] des Projekts. </p> <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ressourcenplaner - budgetierte Stunden] </td> 
        <td> <p>In den folgenden Berichten enthalten:</p>
        <ul>
        <li>[!UICONTROL Project]-Bericht
        <li>Bericht zu [!UICONTROL Project (Finanzdaten)]
        <li>Bericht zu [!UICONTROL Task]
        <li>[!UICONTROL Problem] Bericht
        <li>Bericht zu [!UICONTROL Budgetierte Stunde]</li>
        </ul>
         <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Jede andere Erwähnung von [!UICONTROL Budgetierte Stunden] in [!DNL Adobe Workfront] bezieht sich auf Stunden, die mit veralteten Funktionen budgetiert wurden, die aus Workfront entfernt wurden. Diese Felder sind schreibgeschützt und werden nicht mit aktuellen Informationen aktualisiert, wenn Sie die aktuellen Tools für die Ressourcenbudgetierung verwenden. </p>
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
   <td>[!UICONTROL budgetierte Lohnkosten]</td> 
   <td> <p>Dies sind die Kosten im Zusammenhang mit den Stunden, die Sie als Ressourcenmanager für Ihre Aufgabengebiete für die Arbeit budgetieren, die sie in Projekten erledigen müssen. </p> <p>Die [!UICONTROL budgetierten Lohnkosten] in einem Projektbericht werden nach folgender Formel berechnet:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Dieses Feld kann sich auf Folgendes beziehen:</p> 
    <ul> 
     <li> <p>Arbeitskosten, die im Bereich [!UICONTROL Resource Budgeting] des [!UICONTROL Business Case] oder im [!UICONTROL Resource Planner] angezeigt werden und mit den Kosten für Aufgabengebiete in einem Projekt verknüpft sind. Informationen zur Berechnung der [!UICONTROL Budgetierte Lohnkosten] finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Budgetierte Lohnkosten verstehen] und [!UICONTROL Budgetierte Stunden] für Projekte</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Im Bereich [!UICONTROL Ressourcenbudgetierung] des [!UICONTROL Business Case] werden Arbeitskosten angezeigt, die die geschätzten [!UICONTROL Personalkosten] in einer mit dem Projekt verknüpften Initiative aus dem [!DNL Scenario Planner] widerspiegeln, wenn Sie den Szenarienplaner zur Budgetierung Ihrer Projektressourcen verwenden. Informationen zu Initiativen finden Sie unter <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Initiativen - Übersicht im Szenario-Planer</a>. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Die [!DNL Scenario Planner] - Übersicht</a>. </p> </li> 
     <p>Er wird in den folgenden Bereichen von unter den folgenden Namen angezeigt:</p>
   <ul>
   <li><strong>[!UICONTROL budgetierte Lohnkosten]</strong>: im Bereich [!UICONTROL Resource Budgeting] des [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgetierte Kosten]</strong>: in der Ansicht [!UICONTROL Auslastungsbericht] [!UICONTROL Kosten]
   <p>Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Informationen zur Ressourcenauslastung anzeigen</a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in der [!DNL Resource Planner] Projekt- oder [!DNL Role]-Ansicht bei Anzeige nach Kosten
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in den folgenden Berichten: 
   <ul>
    <li>[!UICONTROL Project]-Bericht</li>
    <li>Bericht zu [!UICONTROL Project (Finanzdaten)]</li>
    <li>Bericht zu [!UICONTROL Task]</li>
    <li>[!UICONTROL Problem] Bericht</li>
    <li>Bericht zu [!UICONTROL Budgetierte Stunde]</li> 
    </ul>
    <p>Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Erstellen eines benutzerdefinierten Berichts</a>.</p>
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
   <td>[!UICONTROL Budgetierter Anfangstermin]</td> 
  <td> <p>Dies ist ein veraltetes Feld. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden.</p>
  <p>Diese Bereiche wurden aus [!DNL Workfront] entfernt. </p> 
  <p>Das Feld ist weiterhin in [!UICONTROL project]-Berichten und -Listen sichtbar.</p>
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
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Ein Tool, mit dem ausgewertet wird, ob ein Projekt vom Status [!UICONTROL IDEA] zum Status [!UICONTROL Planning] weitergeleitet werden soll. Mit anderen Worten: Ein [!UICONTROL Business Case] hilft dem Unternehmen bei der Entscheidung, ob es sich lohnt, das Projekt zu starten und abzuschließen oder nicht, insbesondere beim Vergleich von Projekten mit anderen in einem Portfolio.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Erstellen eines [!UICONTROL Business Case] für einen </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgetierte Geschäftsfall-Stunden]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle in diesem Feld angezeigten Informationen beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat. Dieses Feld kann nicht aktualisiert werden.</p> <p>Dieses Feld ist weiterhin in den Projektlisten und Berichten von [!UICONTROL task] sichtbar. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechnete Zuweisung]</td> 
   <td> <p>Einer der [!UICONTROL Duration Types] der Aufgabe. Dieser berechnet den Prozentsatz eines 8-Stunden-Arbeitstags, den der Benutzer der Aufgabe zugewiesen bekommt, basierend auf der [!UICONTROL Duration] der Aufgabe und der [!UICONTROL Work Required].</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Duration] und [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Berechnete Arbeit]</td> 
   <td> <p>Einer der [!UICONTROL Duration Types]-Aufgaben. Dadurch wird die [!UICONTROL Arbeit erforderlich] für eine Aufgabe unter Berücksichtigung der [!UICONTROL Dauer] und der [!UICONTROL Zuweisung] Prozentsätze des Benutzers (die auf einem 8-Stunden-Arbeitstag basieren) berechnet.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Duration] und [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Kalender]</td> 
   <td> <p>In Workfront ist ein Kalenderbericht ein dynamischer Bericht, in dem Benutzende das Datum und andere wichtige Details eines Ereignisses anzeigen können, einschließlich des Fälligkeitsdatums, des Arbeitsstatus und des Benutzers, dem das Ereignis zugewiesen ist.</p> <p> Weitere Informationen zu Kalenderberichten finden Sie unter <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Übersicht über Kalenderberichte</a>.</p>
   <p> In Workfront Planning ist eine Kalenderansicht eine Art von Ansicht für einen Datensatztyp, der Datensätze in einem Kalender anzeigt. Sie benötigen eine zusätzliche Lizenz, um auf Workfront Planning zugreifen zu können. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL kann starten]</td> 
   <td> <p>Dieses Feld gibt an, ob eine Aufgabe bereit für die Bearbeitung ist. Wenn der Start bereit ist, am Feld [!UICONTROL Can Start] der Aufgabe zu arbeiten, wird auf [!UICONTROL True] gesetzt. </p> <p>Weitere Informationen zu Aufgaben finden Sie unter <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start]"</a>.</p> 
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
   <td> <p>Die verfügbare Zeit einer Ressource, zu der sie der Arbeit zugeordnet werden kann. Siehe „Verfügbarkeit“. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Kategorie]</p> </td> 
   <td> <p>Eine Kategorie ist ein benutzerdefiniertes Formular. Sie können Berichte für dieses Objekt erstellen und sie auch in anderen Objektberichten anzeigen. Nicht alle Objekte können ein benutzerdefiniertes Formular oder eine benutzerdefinierte Kategorie haben. Die folgenden Objekte können ein benutzerdefiniertes Formular haben: <br></p> 
    <ul> 
     <li>[!UICONTROL-Projekt]</li> 
     <li>[!UICONTROL Aufgabe]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL-Portfolio]</li> 
     <li>[!UICONTROL-Dokument]</li> 
     <li>[!UICONTROL Ausgabe]</li> 
     <li>[!UICONTROL-Programm]</li> 
     <li>[!UICONTROL-Benutzer]</li> 
     <li>[!UICONTROL Firma]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kategoriename]</td> 
   <td> <p>Wenn sie als Spalte zur Ansicht eines der folgenden Objekte hinzugefügt wird, wird eine Liste aller benutzerdefinierten Formulare angezeigt, die mit diesen Objekten verknüpft sind:</p> 
    <ul> 
     <li>[!UICONTROL-Projekt]</li> 
     <li>[!UICONTROL Aufgabe]<br></li> 
     <li>[!UICONTROL Problem]<br></li> 
     <li>[!UICONTROL-Portfolio]<br></li> 
     <li>[!UICONTROL-Dokument]<br></li> 
     <li>[!UICONTROL Ausgabe]<br></li> 
     <li>[!UICONTROL-Programm]<br></li> 
     <li>[!UICONTROL-Benutzer]<br></li> 
     <li>[!UICONTROL Firma]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Änderungsverwaltung]</td> 
   <td>Ein Praxisbereich, der sich auf die Definition, das Verständnis und die Anpassung geplanter Arbeiten an Änderungen in Bezug auf Umfang, Zeitplan, Kosten und Ressourcenfaktoren konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Änderungsanforderung]</td> 
   <td>Eine Art von Problem, das gegen ein Projekt aufgeworfen wurde und eine angeforderte Änderung am vereinbarten Umfang skizziert.</td> 
  </tr> 
  <tr> 
   <td>[!Nur UICONTROL ändern]</td> 
   <td>Einer der [!UICONTROL Update Types] des Projekts. Es werden nur die Zeitleisten [!UICONTROL Project Projected] und [!UICONTROL Planned] aktualisiert, wenn Aktualisierungen an Aufgaben vorgenommen oder Änderungen am Projekt oder an Aufgaben durchgeführt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Änderungsanforderung]</td> 
   <td> <p>Einer der [!UICONTROL Problem] Typen, der normalerweise angibt, dass vor dem Abschluss des Projekts ungeplanter Arbeitsaufwand erforderlich ist.</p> <p>Weitere Informationen zu [!UICONTROL Problem]-Typen finden Sie im Abschnitt „Standardproblemtypen“ im Artikel "<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref"> von Standardproblemtypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Untergeordnete Aufgabe]</td> 
   <td>Eine Aufgabe, die eine [!UICONTROL Subtask] einer [!UICONTROL Parent Task] ([!UICONTROL Summary Task]) ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Untergeordnete Elemente]</td> 
   <td>Die Auflistung von [!UICONTROL Subtasks] in eine [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] und [!UICONTROL Training]</td> 
   <td>Lernmodule, Zertifizierungen, Standards oder eine Community of Practice.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL COMMIT]</td> 
   <td>Ein Kommunikationstool für Benutzer, mit dem sie Erwartungen an die zu erbringenden Aufgaben definieren können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit-Datum]</td> 
   <td>Ein Kommunikationswerkzeug für Benutzerinnen und Benutzer, um Erwartungen an Aufgabenleistungen zu setzen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommunikation] und [!UICONTROL Reporting]</td> 
   <td>Standards zur Überprüfung der Ausnahmen und des Zustands eines Projekts, Programms oder Portfolios</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Firma]</td> 
   <td> <p>Eine [!UICONTROL Company] ist eine Organisationseinheit in [!DNL Workfront]. </p> 
   <p> Sie können einen Benutzer oder ein Projekt mit einer Firma verknüpfen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Firmen erstellen und bearbeiten</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussdatum]</td> 
   <td> <p>Das Datum, an dem ein Projekt, eine Aufgabe oder ein Problem abgeschlossen sein soll. Es gibt mehrere Typen von [!UICONTROL Abschlussdaten] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Tatsächliches Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Übersicht über das Projekt [!UICONTROL Tatsächliches Abschlussdatum] </a>.</li> 
     <li>[!UICONTROL Geplantes Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref"> des Projekts [!UICONTROL Geplantes Abschlussdatum]</a> und <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Überblick über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]</a>.</li> 
     <li>[!UICONTROL Voraussichtliches Abschlussdatum]. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Übersicht über das geplante Abschlussdatum von [!UICONTROL] für Projekte, Aufgaben und Probleme</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschlussdatum]</td> 
   <td>Der Tag, relativ zum Beginn der [!UICONTROL Template], an dem eine [!UICONTROL Template Task] oder eine [!UICONTROL Template] abgeschlossen sein soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fertigstellungsmodus]</td> 
   <td> <p>Dies gibt an, wie ein Projekt als [!UICONTROL Abgeschlossen] markiert wird. Sie kann zwei Werte haben:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: Ein Benutzer muss den Projektstatus in [!UICONTROL Complete] ändern.</li> 
     <li>[!UICONTROL Automatisch]: Der Projektstatus ändert sich automatisch in [!UICONTROL Abgeschlossen], wenn alle Aufgaben im Projekt zu 100 % abgeschlossen sind und alle Probleme geschlossen sind.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Bedingung]</td> 
   <td> <p>Dies ist eine visuelle Darstellung des Fortschritts einer Aufgabe, eines Problems oder Projekts.</p> <p>Bei Projekten kann die Bedingung vom Projekteigentümer manuell festgelegt werden oder automatisch von [!DNL Workfront] auf der Grundlage des Fortschrittsstatus des Projekts festgelegt werden. </p> <p>Die möglichen Werte für die Projektbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL on Target]</li> 
     <li>[!UICONTROL Gefährdet]</li> 
     <li>[!UICONTROL in Schwierigkeiten]</li> 
    </ul> <p>Weitere Informationen zu Projektbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Projektbedingung] und den [!UICONTROL Bedingungstyp]</a>.</p>
     <p>Sie können Aufgaben- und Problembedingungen mit einer Zahl verknüpfen, die in Berichten angezeigt werden kann. In den folgenden Listen werden die Standardnamen und -nummern für Aufgaben- und Problembedingungen angezeigt. Ihre bzw. Ihr Systemadmin kann die Namen der Bedingungen aktualisieren und neue Bedingungen mit unterschiedlichen Nummern hinzufügen. Nachdem eine Zahl mit einer Bedingung verknüpft wurde, kann sie nicht mehr bearbeitet werden.  </p> 
     <p>Für Aufgaben wird die Bedingung vom Aufgabenbesitzer manuell festgelegt. Die möglichen Werte für die Aufgabenbedingung sind:</p> 
    <ul> 
     <li>[!UICONTROL läuft reibungslos] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Hauptsperren] (2)</li> 
    </ul> <p>Weitere Informationen zu Aufgabenbedingungen finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisieren der [!UICONTROL-Bedingung] für Aufgaben und Probleme</a>.</p> <p>Bei Problemen wird die Bedingung manuell vom Problembesitzer festgelegt. Die möglichen Werte für die Problembedingung sind:<br></p> 
    <ul> 
     <li>[!UICONTROL läuft reibungslos] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Hauptsperren] (2)</li> 
    </ul> 
   <p><b>NOTIZ</b></p>
    <p>Wenn das Feld [!UICONTROL Bedingung] in [!UICONTROL Tagebucheintrag]-Berichten verfolgt wird, zeigen die [!UICONTROL Neu] und [!UICONTROL Alte Zahlenwerte] die mit der Bedingung verknüpfte Zahl anstelle ihres Namens an. Wenn eine Bedingung ursprünglich für eine Aufgabe oder ein Problem nicht definiert ist und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den [!UICONTROL Alter Zahlenwert] des Felds [!UICONTROL Bedingung] als -2,147,483,648 an. Siehe auch "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]" und "[!UICONTROL Journal Entry]" in diesem Artikel. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bedingungsaktualisierung]</td> 
   <td> <p>In diesem Feld wird der aktuelle Status von Aufgaben, Projekten oder Problemen angezeigt. Diese Option zeigt die neuesten Aktualisierungen, die die Verantwortlichen für Aufgaben, Projekte oder Probleme im Feld [!UICONTROL Aktualisierungsstatus] bereitgestellt haben, zusammen mit der neuen Bedingung an.</p> <p>Kommentare zu Bedingungsaktualisierungen werden nicht in der Spalte [!UICONTROL Condition Update] angezeigt, sondern nur die Hauptaktualisierung.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected record types]</td> 
   <td> <p>In Workfront Planning können Sie eine Verbindung zwischen folgenden Elementen erstellen: </p>
   <ul>
   <li>Zwei Datensatztypen</li>
   <li>Einen Datensatztyp und einen Workfront-Objekttyp</li>
   <li>Datensatztyp und Adobe Experience Manager-Asset</li></ul>
   <p>Durch das Verbinden von Datensatztypen können Sie Informationen von einem Datensatz oder Objekttyp zu einem anderen Datensatztyp anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Übersicht über verbundene Datensatztypen</a>  </p>
  <p>Workfront Planning benötigt eine zusätzliche Lizenz. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected records]</td> 
   <td> <p>In Workfront Planning können Sie nach dem Verbinden von zwei Datensatztypen zwei einzelne Datensätze dieser Typen miteinander verbinden.  </p>
   <p>Durch das Verbinden von Datensätzen können Sie Informationen aus einem Datensatz oder Objekt aus einer anderen Anwendung in einem anderen Datensatz anzeigen.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Übersicht über verbundene Datensätze</a>. </p>

<p>Workfront Planning benötigt eine zusätzliche Lizenz. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL-Verbindungen]</td> 
   <td> <p>In Workfront Planning können Verbindungen auf verbundene Datensatztypen oder verbundene Datensätze verweisen. Workfront Planning benötigt eine zusätzliche Lizenz.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Einschränkungsdatum]</td> 
   <td> <p>Wenn Sie eine [!UICONTROL Aufgabenbeschränkung] verwenden, die mit einem bestimmten Datum verknüpft ist, z. B. [!UICONTROL Muss beginnen am], wird dieses bestimmte Datum zum [!UICONTROL Einschränkungsdatum] der Aufgabe.</p> <p>Die folgenden Aufgabenbeschränkungen aktualisieren das Feld [!UICONTROL Einschränkungsdatum]:</p> 
    <ul> 
     <li>[!UICONTROL muss beginnen am]</li> 
     <li>[!UICONTROL muss beendet werden am]</li> 
     <li>[!UICONTROL Start Spätestens]</li> 
     <li>[!UICONTROL Start nicht früher als]</li> 
    </ul> <p><b>TIPP</b></p>   
     <ul> 
      <li> <p>Eine Aufgabe mit einer [!UICONTROL-Beschränkung] von [!UICONTROL Feste Daten] hat kein [!UICONTROL-Einschränkungsdatum]. </p> </li> 
      <li> <p> [!UICONTROL Einschränkungsdatum] kann nur in einem Bericht oder in einer angepassten Ansicht angezeigt werden.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einschränkungstag]</td> 
   <td> <p>Wenn Sie eine Aufgabenbeschränkung in einer Vorlagenaufgabe verwenden, die an einen bestimmten Tag gebunden ist, z. B. „Start am“, wird dieser Tag zum Einschränkungstag der Vorlagenaufgabe.</p> <p>Die folgenden Aufgabenbeschränkungen aktualisieren das Feld [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL muss beginnen am]</li> 
     <li>[!UICONTROL muss beendet werden am]</li> 
     <li>[!UICONTROL Start Spätestens]</li> 
     <li>[!UICONTROL Start nicht früher als]</li> 
    </ul> <p><b>TIPP</b></p> <p>  [!UICONTROL Constraint Day] kann nur in einem Bericht oder in einer benutzerdefinierten Ansicht angezeigt werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einschränkungstyp]</td> 
   <td> <p>Die Planungsneigung einer Aufgabe. Beispielsweise plant [!UICONTROL Sofort as possible], dass eine Aufgabe so bald wie möglich beginnt, und [!UICONTROL Finish Später nicht später] plant, dass eine Aufgabe bis zum [!UICONTROL Constraint Date] und nicht später abgeschlossen sein soll.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Aufgabenbeschränkung] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kontextmenü]</td> 
   <td>Ein Menü links im Bildschirm, in dem sich die Elemente ändern, sodass sie mit dem aktiven Inhalt korrelieren. Wenn ein Benutzer beispielsweise ein Projekt anzeigt, zeigt das [!UICONTROL Kontextmenü] Links zu projektbezogenen Informationen und Tools an.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Ein Feld in einem Projekt- oder Aufgabenbericht, das Informationen zu dem Benutzer anzeigt, der der [!UICONTROL Primär Contact] für ein Problem ist, wenn das Problem in ein Projekt oder eine Aufgabe konvertiert wird. Das Feld wird auch im Abschnitt [!UICONTROL Projektdetails] angezeigt, wo es den Namen des [!UICONTROL Primär Contact] des konvertierten Problems anzeigt. Siehe auch "[!UICONTROL Primär Contact]" in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Kosten]</td> 
   <td> <p>Der Geldbetrag, den Sie beim Abschluss eines Projekts, einer Aufgabe oder eines Problems ausgeben müssen. </p> <p>Sie können verschiedene Arten von Kosten für Arbeit, Ausgaben und Risiken im Zusammenhang mit dem Projekt verfolgen. Informationen zur Kostennachverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Kosten nachverfolgen</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kostentyp]</td> 
   <td>Für eine Aufgabe bestimmt der [!UICONTROL Kostentyp], wie der Aufgabe Kosten entstehen. Einige Beispiele sind [!UICONTROL Fester Wert pro Stunde], [!UICONTROL Benutzer pro Stunde] und [!UICONTROL Benutzer pro Stunde plus Fester Wert]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL projektübergreifende Abhängigkeiten]</td> 
   <td> <p>Eine Aufgabe eines Projekts ist von einer Aufgabe aus einem anderen Projekt abhängig.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Erstellen von projektübergreifenden Vorgängern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefinierte Daten]</td> 
   <td> <p>Daten, die für eine Organisation eindeutig sind. Unternehmen können das [!DNL Workfront]-Programm anpassen, indem sie benutzerdefinierte Formulare und Felder erstellen. Diese benutzerdefinierten Informationen können die Berichterstellung für KPIs, Auditing und Demand Mix fördern. </p> <p>[!UICONTROL Benutzerdefinierte Daten] kann verknüpft werden mit:</p> 
    <ul> 
     <li>[!UICONTROL-Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Benutzer]</li> 
     <li>[!UICONTROL Firmen]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL-Dokumente]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Iterationen]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierter Datentyp]</td> 
   <td>Die Option, um anzugeben, ob ein [!UICONTROL Custom Data]-Feld in der Datenbank als Text, Datum, Zahl oder Währung gespeichert wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierter Anzeigetyp]</td> 
   <td>Der Anzeigetyp des Felds eines benutzerdefinierten Felds. Beispiele sind [!UICONTROL Dropdown], [!UICONTROL Textfeld], [!UICONTROL Textbereich], [!UICONTROL Optionsfelder] usw.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefiniertes Feld]</td> 
   <td>Bei benutzerdefinierten Daten, mit denen Benutzende aus mehreren Optionen auswählen können, sind dies die Werte, aus denen Benutzende auswählen können. Benutzerdefinierte Optionen sind nur für die Kontrollkästchen [!UICONTROL Dropdown], [!UICONTROL Mehrfachauswahl-Dropdown], [!UICONTROL Optionsfelder] und [!UICONTROL] gültig.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerdefinierte Formularbeschriftung]</td> 
   <td>Bei Verwendung eines benutzerdefinierten Anzeigetyps mit benutzerdefinierten Optionen ist dies der Text der Benutzeroberfläche, der im Dropdown-Menü, in den Kontrollkästchen oder den Optionsfeldern für diese benutzerdefinierte Option angezeigt wird.</td> 
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
   <td>[!UICONTROL Kunde]</td> 
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
   <td> <p> Sie können dieses Feld einem Bericht oder einer Ansicht des Berichtsobjekts hinzufügen, um die Dashboards anzuzeigen, in denen der Bericht in einer Liste aufgeführt ist. </p> <p> Sie können dieses Feld auch verwenden, um nach Berichten zu filtern, die in einem bestimmten Dashboard aufgeführt sind. </p> <p> Weitere Informationen zum Einschließen von Dashboard-Informationen in Berichte zu Berichtsobjekten finden Sie im Abschnitt „Verstehen, welche Berichte in Dashboards aufgelistet sind“ im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Zugreifen auf und Organisieren von Berichten</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datentyp]</td> 
   <td>Siehe "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verspätungstage]</td> 
   <td> <p>Dieses Feld zeigt eine Datumsdifferenz zwischen [!UICONTROL Geplanter Start] und [!UICONTROL Today] an, wenn das [!UICONTROL Tatsächliches Abschlussdatum] fehlt.</p> <p>Zeigt auch eine Datumsdifferenz zwischen dem tatsächlichen Abschluss von [!UICONTROL] und dem geplanten Abschluss von [!UICONTROL] an, wenn ein tatsächliches Abschlussdatum von [!UICONTROL] vorhanden ist.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Standardzeitplan]</td> 
   <td> <p>Anpassbare Standardarbeitszeiten, die Benutzern und Projekten in einer Organisation zugewiesen werden können. </p> <p>Zeitpläne werden verwendet, um die geplanten Termine, das Start- und das Abschlussdatum von Aufgaben zu berechnen, die Benutzern zugewiesen werden.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Leistung]</td> 
   <td>Quantifizierbare Waren oder Dienstleistungen, die nach Abschluss eines Projekts bereitgestellt werden müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Bewertung und Priorisierung der Aufnahmeprozesse.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Abteilungsziele]</td> 
   <td>Eindeutige Ziele für eine bestimmte Abteilung, die sich auf die Verbesserung der Betriebsmetriken innerhalb der Abteilung konzentrieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Abhängigkeit]</td> 
   <td>Die Verknüpfung zwischen zwei Aufgaben, für die eine Aufgabe den Status ändern muss, bevor die andere Aufgabe den Status ändern kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abhängigkeitstyp]</td> 
   <td> <p>Der Typ der Planungsbeziehung zwischen einer Aufgabe und ihren Vorgängern. Ein Beispiel ist [!UICONTROL Beenden-Start]. Dies setzt voraus, dass die erste Aufgabe beendet wird, bevor die zweite Aufgabe beginnen kann.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Übersicht über Aufgabenabhängigkeitstypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Dokument]</td> 
   <td>Jede Datei, die an ein Objekt in [!DNL Workfront] angehängt ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokumentversion]</td> 
   <td> <p>Jedes Mal, wenn dasselbe Dokument in dasselbe Objekt hochgeladen wird, wird ihm eine Versionsnummer zugewiesen. Benutzer können mehrere Optionen für eine frühere Version eines Dokuments anzeigen und ändern.</p> <p>Weitere Informationen finden Sie unter <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Dokumentversionen verwalten</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Fälligkeitsdatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe oder ein Problem abgeschlossen sein soll. Das Fälligkeitsdatum einer Aufgabe oder eines Problems entspricht dem geplanten Abschlussdatum.</p>
    <p>Das Fälligkeitsdatum von Aufgaben und Problemen ist in Aufgaben- und Problemlisten und Berichten sichtbar.</p> 
    <p>Siehe auch Geplantes Abschlussdatum in dieser Tabelle. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer]</td> 
   <td> <p>Das Zeitfenster, das für den Abschluss einer Aufgabe, eines Problems oder Projekts zugewiesen wurde (bestimmt durch die Anzahl der Tage zwischen dem geplanten Start von [!UICONTROL] und dem geplanten Abschluss).</p> 
    <ul> 
     <li>Bei Aufgaben ist die Dauer ein bearbeitbares Feld, wenn der Dauertyp der Aufgabe nicht „Einfach“ ist. Wenn der Dauertyp der Aufgabe „Einfach“ ist oder die Aufgabenbeschränkung „Feste Daten“ ist, ist die Dauer eine von Workfront durchgeführte Berechnung.</li> 
     <li>Bei Problemen ist die Dauer immer ein bearbeitbares Feld und sollte eine Schätzung der Anzahl der Tage darstellen, an denen das Problem gelöst werden muss.</li> 
     <li>Bei Projekten ist die Dauer eine von [!DNL Workfront] durchgeführte Berechnung und stellt die Differenz in Tagen zwischen dem geplanten Beginn der frühesten Aufgabe und dem geplanten Abschluss der letzten Aufgabe im Projekt [!UICONTROL Geplant] dar.</li> 
    </ul> <p>Weitere Informationen zum Unterschied zwischen der [!UICONTROL-Dauer] und der [!UICONTROL-geplanten Dauer] für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Unterschied zwischen der [!UICONTROL-geplanten Dauer] und der [!UICONTROL-Dauer] für Aufgaben</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Dauer in Minuten]</td> 
   <td>Dieses Feld zeigt dieselben Informationen wie das Feld [!UICONTROL Dauer] in Minuten anstelle von Tagen an. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Dauer pro Intervall]</td> 
   <td> <p>Wird in den Feldern [!UICONTROL Aufgabendetails] und [!UICONTROL Aufgabe bearbeiten] eines übergeordneten Elements wiederkehrender Aufgaben angezeigt. Angezeigt wird die Dauer jeder wiederkehrenden Aufgabe. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> <p> <span>In einzelnen wiederkehrenden Aufgaben geänderte Dauer zeigt nicht den in diesem Feld angegebenen Wert an.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Dauertyp]</td> 
   <td> <p>Ein Aufgabenfeld, das angibt, wie die für die Erfüllung der Aufgabe erforderliche Arbeit den Beauftragten über die Aufgabendauer hinweg zugewiesen wird. Es stellt die Beziehung zwischen der [!UICONTROL Duration] der Aufgabe, der [!UICONTROL Work Required] und der Zeit oder der [!UICONTROL Allocation] dar, die die zugewiesenen Ressourcen für die Aufgabe aufwenden sollen, um sie abzuschließen. </p> <p>Dieses Feld wird auf der Registerkarte [!UICONTROL Details] einer Aufgabe angezeigt. </p> <p>Die Optionen für den Dauertyp einer Aufgabe sind:</p> 
    <ul> 
     <li>[!UICONTROL Berechnete Zuweisung]</li> 
     <li>[!UICONTROL Berechnete Arbeit]</li> 
     <li>[!UICONTROL Leistungsgesteuert]</li> 
     <li>[!UICONTROL Einfach]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Duration] und [!UICONTROL Duration Type]</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Dauereinheit]</td> 
   <td>Die Einheit, die zur Zeitmessung in einem Power Search-Tool verwendet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Leistungsgesteuert]</td> 
   <td>Die Beziehung zwischen der Anzahl der Benutzerinnen und Benutzer und der Zeit, die die Aufgabe benötigt. Je mehr Benutzer Sie hinzufügen, desto kürzer wird die für den Abschluss der Aufgabe geplante Gesamtzeit. Die Dauer der Aufgabe bleibt jedoch gleich. Wenn eine Aufgabe beispielsweise ein Fass Erdnüsse bombardiert, verringert sich durch das Hinzufügen weiterer Personen die geplante Zeit, aber die Dauer in Tagen bleibt gleich.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verstrichene Zeit]</td> 
   <td> <p>[!UICONTROL Verstrichene Zeit] ist eine Zeiteinheit für die [!UICONTROL-Dauer] einer Aufgabe. Dies ist die Zeit zwischen dem [!UICONTROL Geplantes Startdatum] und dem [!UICONTROL Geplantes Abschlussdatum] einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen. </p> <p>[!DNL Workfront] Unterstützt die folgenden Zeiteinheiten für die Aufgabendauer:</p> 
    <ul> 
     <li> <p>[!UICONTROL Verstrichene Minuten]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Stunden]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Tage]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Wochen]</p> </li> 
     <li> <p>[!UICONTROL Verstrichene Monate]</p> </li> 
    </ul> <p>Weitere Informationen zur Aufgabendauer, einschließlich der verstrichenen Zeit, finden Sie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer [!UICONTROL] und den [!UICONTROL-Dauertyp]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> In einem [!UICONTROL Rate]-Bericht ist dies das Datum, an dem ein neuer Abrechnungssatz für ein Aufgabengebiet auf Projektebene endet. Die mit dem Projekt verknüpften Stunden vor diesem Datum werden mit diesem Abrechnungssatz multipliziert, um den Projektumsatz zu berechnen. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL-Interaktion]</td> 
   <td>Der [!UICONTROL Work Performance Indicator] (WPI), der angibt, wann das Engagement und die Überzeugung in der Aufgabe, dem Projekt, dem Team oder der Organisation abnehmen. Dies zeigt, dass Sie handeln müssen, um diese Überzeugung und dieses Engagement wiederzubeleben. Der WPI wird anhand der einfachen Frage gemessen: „Haben Sie verstanden, was von Ihnen erwartet wurde? Hat die Ihnen zugewiesene Arbeit einen Unterschied für die Organisation gemacht? Habt ihr großartige Arbeit geleistet?“</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Unternehmensziele]</td> 
   <td>Funktionsübergreifende Ziele, die zur Metrik der Unternehmensziele beitragen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ereignis]</td> 
   <td>Jede Änderung in einem Projekt oder einer Aufgabe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignishandler]</td> 
   <td>Automatisierte Aufgaben, die bei Ereignissen auftreten. Ein gängiges Beispiel ist eine automatisierte E-Mail-Benachrichtigung.</td> 
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
   <td>[!UICONTROL extern]</td> 
   <td> <p>In der Regel handelt es sich um einen Lizenztyp oder einen Benutzer mit einer solchen Lizenz. Ein Benutzer mit einem solchen Lizenztyp kann nur Informationen im System überprüfen. Sie können nicht aktiv an der Arbeit teilnehmen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Externes System]</td> 
   <td>Alle Dienste oder Software, die außerhalb des vorgesehenen Aufzeichnungsverfahrens gespeichert und verwaltet werden.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL-Feld]</td> 
   <td><p>alle Workfront-Objekte oder die damit verbundenen Informationen, wie sie in der Datenbank angezeigt werden. </p>
   <p>Beispielsweise sind „Projekt“, „Benutzer“, „Stunde“ sowohl Workfront-Objekte als auch Felder. „Name“, „Status“, „Eigentümer“, „Startdatum“ sind Workfront-Felder, die mit den oben genannten Objekten verknüpft sind. </p>

<p>Bei der Bezugnahme auf Objekte können die Begriffe „Objekte“ und „Felder“ synonym verwendet werden.</p>
   <p>Im Umfang des Reportings beziehen sich die „Felder“ auf die Objekte oder die Informationen über das Objekt, die Sie im Bericht erfassen möchten.</p>

<p><b>NOTIZ</b></p>

<p>Bei der textbezogenen Berichterstellung beziehen sich Felder auf die Objekte oder deren Informationen, wie sie in der Datenbank angezeigt werden.</p>
   <p>Manchmal unterscheidet sich der Name, den Sie in der Benutzeroberfläche sehen, vom Namen des Felds in der Datenbank. Beispielsweise ist „Problem“ der Name des Objekts in der Workfront-Benutzeroberfläche, aber „opTask“ ist der Name des Objekts (oder des Felds) in der Workfront-Datenbank. </p> 
   <p> Es ist wichtig, das Feld so zu verwenden, wie es in der Datenbank angezeigt wird, wenn ein Textmodusbericht, eine Ansicht, ein Filter oder eine Gruppierung geschrieben oder ein berechnetes Feld erstellt wird.</p>

<p>Weitere Informationen finden Sie unter <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> und <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Textmodus - Übersicht</a>.</p>

<p>Standardmäßig enthält Workfront eine Reihe von Feldern, die sowohl Objekte als auch deren Informationen definieren. Sie können auch benutzerdefinierte Felder zum Definieren von Objekten erstellen, jedoch keine benutzerdefinierten Objekte.</p>

<p>In Workfront Planning können Sie benutzerdefinierte Felder für alle Datensatztypen erstellen. Workfront-Datensatztypen verfügen nur über eine sehr begrenzte Anzahl von Feldern. Sie müssen alle Felder von Grund auf neu erstellen und sie Datensatztypen zuordnen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/fields/fields-overview.md">Feldübersicht</a>. </p> <p>Workfront Planning benötigt eine zusätzliche Lizenz. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL filter]</td> 
   <td> <p>Einer der Hauptbausteine eines Berichts oder eines Listenelements, der bzw. das definiert, welche Informationen auf dem Bildschirm angezeigt werden. Weitere Informationen zu Berichtselementen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichtselemente: Filter, Ansichten und Gruppierungen</a>.</p> <p>Der Filter bestimmt die Ergebnisse, die in einem Bericht oder in einer Liste eines [!DNL Workfront] Bedienfelds angezeigt werden, z. B. Projekte, Aufgaben oder Probleme.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Prozess zum Verwalten von Arbeitskosten-, Ausgaben- und Umsatzdaten in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixkosten]</td> 
   <td>Sie können einen festen Kostenbetrag für ein Projekt definieren. Dies ist Teil der [!UICONTROL Geplanten Kosten] des Projekts, die den Betrag darstellen, den Sie zum Abschließen des Projekts benötigen. Informationen zu den Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fester Umsatz]</td> 
   <td>Sie können einen festen Umsatzbetrag für ein Projekt definieren. Dies ist Teil des [!UICONTROL Geplanter Umsatz] des Projekts, der dem Geldbetrag entspricht, den Sie möglicherweise erhalten, wenn Sie das Projekt abschließen. Informationen zu Einnahmen finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Dies ist dasselbe Feld wie [!UICONTROL Status Icons], es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL-Vorlagen] </li> 
     <li> [!UICONTROL Ausgaben] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner]</td> 
   <td>Mit Ordnern können Sie Dokumente oder Berichte organisieren, die mit einem Objekt verknüpft sind.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Vollzeitäquivalent)</td> 
   <td>Dies ist die Vollzeitäquivalenz, die die Zeitdauer angibt, während der eine Ressource für Arbeit verfügbar ist. 
   Das Feld [!UICONTROL FTE] wird in den folgenden Bereichen angezeigt: 
  <ul>
   <li> Benutzerprofil beim Bearbeiten oder Erstellen des Benutzers </li>
   <li> [!UICONTROL Ressourcenplaner] </li>
   <li> [!UICONTROL Scenario Planner] (erfordert zusätzliche Lizenz für den Workfront Scenario Planner) </li>
   <li> Benutzerlisten und Berichte </li> </ul>

<p>Der [!UICONTROL FTE] muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. </p>
   <p> Ein [!UICONTROL FTE] von 1 (der Standard für das Feld [!UICONTROL FTE] eines Benutzers, wie in seinem Profil definiert) bedeutet, dass eine Ressource (Benutzer oder Funktion) die gesamte Anzahl von Stunden arbeitet, basierend auf dem Zeitplan, der ihre Verfügbarkeit berechnet. </p>
   <p>Ihr Workfront-Administrator entscheidet, welcher Zeitplan zur Bestimmung der Benutzerverfügbarkeit verwendet werden soll.  </p>
   <ul>
   <li> Wenn der [!UICONTROL Standard Schedule] verwendet wird, verwendet Workfront den [!UICONTROL FTE] des Benutzers, der in seinem Profil gefunden wurde, um die Verfügbarkeit zu berechnen. </li>
   <li> Wenn der Zeitplan des Benutzers verwendet wird, verwendet Workfront den Urlaubstag des Benutzers, den Wert von [!UICONTROL Work Time] und die Stunden von [!UICONTROL Default Schedule], um den [!UICONTROL FTE] des Benutzers zu berechnen. </li> </ul>

<p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.  </p>
   <p>Weitere Informationen zum Erstellen von Zeitplänen in [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>

<p><b>NOTIZ</b></p>
   <p>Für alle Berechnungen im [!UICONTROL Scenario Planner] verwendet Workfront den folgenden Wert: 1 [!UICONTROL FTE] = 8 Stunden.</p>
   <p>Weitere Informationen finden Sie unter <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Erste Schritte mit dem [!UICONTROL Scenario Planner]</a>. </p>
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
   <td>[!UICONTROL Gantt-Diagramm]</td> 
   <td> <p>Eine visuelle Zeitleiste der Projekttermine in einer Kalenderansicht, die auf den geplanten oder projizierten Terminen basiert, da die Aufgaben des Projekts derzeit geplant sind.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ziel]</td> 
   <td><p>In [!DNL Workfront] gibt es zwei Konzepte von Zielen: </p> 
    <ul> 
     <li> <p><b>Projektziele</b> Eine Reihe von Geschäftszielen, die von den relevanten Stakeholdern eines Projekts vereinbart wurden. Projektziele sind Teil des Business Case eines Projekts. </p> <p>Sie können Projektziele nicht in Listen oder Berichten anzeigen, aber Sie können über die API darauf zugreifen. </p> <p>Informationen zu Business Case-Projektzielen finden Sie unter <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Erstellen von Business Case-Zielen </a>. </p> </li> 
     <li> <p><b>Strategische Ziele</b> Ein strategisches Ziel ist ein Ziel, das Sie erstellen, um Ihre Arbeitsstrategie für einen bestimmten Zeitraum zu planen. Sie können diese Arten von Zielen mithilfe von [!DNL Workfront Goals] erstellen. Ihr Unternehmen muss eine zusätzliche Lizenz erwerben und Sie müssen Zugriff auf diese Funktion haben, um strategische Ziele erstellen zu können. [!DNL Workfront Goals] sind nur mit einer zusätzlichen Lizenz verfügbar.</p> 
     <p>Weitere Informationen finden Sie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] Übersicht </a>. </p> 
     <p>Sie können strategische Ziele in einem Ziel- oder Projektbericht anzeigen und über die API darauf zugreifen. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Zielhierarchie]</td> 
   <td> <p>In [!UICONTROL Goal]- und [!UICONTROL Project]-Berichten ist dies ein Sammlungsfeld, das die Ziele in der Hierarchie anzeigt, zu der ein strategisches Ziel gehört, wenn es an anderen Zielen ausgerichtet wird. Die Ziele werden durch ein ▸ Trennzeichen getrennt. </p> <p>In diesem Feld werden nur die übergeordneten Elemente des Ziels und des Ziels angezeigt. Untergeordnete Ziele werden nicht angezeigt. </p> <p>Informationen zum Ausrichten von Zielen in [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Übersicht über die Zielausrichtung in [!DNL Workfront Goals]</a>. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] - Übersicht </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ziel Erfolgsbewertung]</td> 
   <td> In einem [!UICONTROL Project-Bericht] wird dieses Feld verwendet, um auf die Ziele auf Projektebene zu verweisen, die mit dem [!UICONTROL Business]-Fall verknüpft sind. Derzeit ist dies ein veraltetes Feld, das mit keiner Funktion verknüpft ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziele] </td> 
   <td> <p>In einem [!UICONTROL Project]-Bericht ist dies ein Sammlungsfeld, das alle strategischen Ziele anzeigt, die mit einem Projekt verbunden sind. Die Ziele werden durch Kommas getrennt.</p> <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] - Übersicht</a>. Weitere Informationen zu strategischen Zielen und Projektzielen in [!DNL Workfront] finden Sie unter "[!UICONTROL Goal]" in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Globale Schnittstelleneinstellungen]</td> 
   <td>Einstellungen der Benutzeroberfläche, die sich auf alle Benutzer auswirken. [!UICONTROL Globale Schnittstelleneinstellungen] können durch die [!UICONTROL Benutzeroberflächeneinstellungen] überschrieben werden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL-Gruppe]</td> 
   <td> <p>Eine Sammlung von Benutzern (möglicherweise aus derselben Abteilung oder Geschäftseinheit), die Zugriff auf dieselben Objekte haben. Zusätzlich zu den Benutzern können Gruppen mit Portfolios, Programmen, Projekten, <span> Projektvorlagen, </span> Unternehmen, Teams, Zeitplänen, Layout-Vorlagen und Arbeitszeittabellen-Profilen verknüpft werden.</p> <p>Sie können auch Berechtigungen für Objekte nach Gruppe erteilen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppen - Übersicht</a>.</p> <p>In einer Liste oder einem Bericht von Objekten eines der folgenden Typen können Sie mithilfe des Felds [!UICONTROL Group] auflisten, welche Objekte dieses Typs einer bestimmten Gruppe zugeordnet sind: Benutzer, Portfolio, Programm, Projekt, <span>Projektvorlage</span>, Firma, Team, Zeitplan, Layoutvorlage oder Arbeitszeittabellenprofil.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gruppenadministrator]</td> 
   <td> <p>Benutzer, die die Objekte, den Zugriff und die Benutzer bestimmter Benutzergruppen verwalten.</p> <p> In einem [!UICONTROL Group]-Bericht zeigt dieses Feld die Namen der Benutzer an, die in der Gruppe als [!UICONTROL Group Administrators] angegeben sind. Weitere Informationen zu Gruppenadministratoren finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Gruppe mit Administratorzugriff]</td> 
   <td> <p> In einem [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] oder [!UICONTROL Schedule Report] zeigt dieses Feld die Gruppen an, deren Gruppenadministratoren Zugriff haben, um die Vorlage zu ändern. Sie können diesen Bericht auch nach diesem Feld filtern. </p> <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL-Gruppierung]</td> 
   <td> <p>Ein Berichterstellungselement, mit dem Informationen in einer Liste anhand eines gemeinsamen Kriteriums kategorisiert werden.</p> <p>Weitere Informationen finden Sie im Abschnitt "[!UICONTROL Gruppierungen]" im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergabedatum]</td> 
   <td> <p>Das Datum, an dem eine Aufgabe für die Arbeit verfügbar wird. Das [!UICONTROL Übergabedatum] ist eine Berechnung und kann nicht manuell festgelegt werden. <br>Weitere Informationen zum [!UICONTROL Übergabedatum] finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Aufgabübergabedatum] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Helpdesk]</td> 
   <td>Ein alternativer Name zur Beschreibung des Bereichs [!UICONTROL Requests] von [!DNL Workfront]. Im Bereich [!UICONTROL Requests] können Sie Support-Tickets, Projektanfragen, Helpdesk-Tickets usw. verarbeiten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inhaber]</td> 
   <td>In einem [!UICONTROL Hour]-Bericht ist der [!UICONTROL Owner] der Benutzer, dem die Stunden zugeordnet sind. Dies unterscheidet sich von dem Benutzer, der die Zeit tatsächlich protokolliert. Diese beiden Entitäten können manchmal zwei verschiedene Benutzer sein. <br>Weitere Informationen zur Protokollierung der Zeit für einen anderen Benutzer finden Sie im Artikel <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Zeit protokollieren</a>.</td> 
  </tr>

<tr> 
   <td>Stundenstatus</td> 
   <td> <p>Ein Attribut, das von Workfront für die tatsächlichen Stunden festgelegt wird, die Benutzende für Aufgaben, Probleme oder Projekte protokollieren. </p>

Stundeneinträge können einen der folgenden Status in Workfront aufweisen:
<ul>
   <li><b>Eingereicht</b>: Die Stunden wurden für ein Projekt, eine Aufgabe oder ein Problem protokolliert. Sie sind entweder Teil eines Rechnungsnachweises oder noch nicht zu einem Rechnungsnachweis hinzugefügt.</li>
   <li><b>Genehmigt</b>: Die Stunden wurden protokolliert und vom Projektbesitzer genehmigt. Sie sind entweder Teil eines Rechnungsnachweises oder noch nicht zu einem Rechnungsnachweis hinzugefügt.</li> 
   <li><b>Nicht genehmigt</b>: Die Stunden wurden vom Projektbesitzer protokolliert und abgelehnt. Sie sind entweder Teil eines Rechnungsnachweises oder noch nicht zu einem Rechnungsnachweis hinzugefügt.</li>
   <li><b>Abgerechnet</b>: Die Stunden wurden protokolliert und einem Rechnungsnachweis hinzugefügt, und der Status des Rechnungsnachweises wurde als „In Rechnung gestellt“ markiert. Sie mussten nicht vom Projektbesitzer genehmigt werden.</li>
   <li><b>In Rechnung gestellt und genehmigt</b>: Die Stunden wurden protokolliert und vom Projektbesitzer genehmigt, und der Status des Abrechnungs-Datensatzes wurde als In Rechnung gestellt markiert.</li>
   </ul>

<p>Wenn Stunden Teil eines Rechnungsnachweises sind, gibt der Stundenstatus an, ob die Stunden genehmigt wurden oder ob der Rechnungsnachweis, zu dem sie gehören, in Rechnung gestellt wurde. Der Stundenstatus eines Stundeneintrags ist nur in einer Stundenliste oder einem Bericht sichtbar. </p>

<p>Weitere Informationen zum Hinzufügen von Stunden zu Rechnungsnachweisen finden Sie im Abschnitt „Hinzufügen von Stunden zu Rechnungsnachweisen“ im Artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Erstellen von Rechnungsnachweisen</a>.</p>

<p>Weitere Informationen zur Genehmigung der Zeit für Projekte finden Sie unter <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Zeit für die Genehmigung eines Projekts benötigen</a>.</p>

<p><b>TIPP</b></p>

<p>Allgemeine Stunden, die nicht direkt in Arbeitselementen protokolliert werden, zeigen keinen Stundenstatus an. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Stundentyp]</td> 
   <td> <p>Ein Attribut, das für die tatsächlichen Stunden festgelegt werden kann, die Benutzer für Aufgaben, Probleme oder Projekte protokollieren. Dies ist auch ein Attribut für die protokollierten Stunden, die nicht direkt mit der Arbeit verknüpft sind, z. B. [!UICONTROL Urlaub] und [!UICONTROL Urlaub].</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Verwalten von Stundentypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Die ID ist ein alphanumerischer Indikator, der mit jedem Objekt in [!DNL Workfront] verknüpft ist. Jedes Objekt in der [!DNL Workfront]-Datenbank wird eindeutig identifiziert. Sie können die ID eines beliebigen Objekts in einem Bericht oder eine Liste für jedes Objekt anzeigen. </p> <p><b>TIPP</b></p>   <p>Sie können die ID auch in der URL der -Objektseite anzeigen. Wenn Sie beispielsweise auf die Seite [!UICONTROL Projektdetails] zugreifen, könnte die ID eines Projekts in etwa wie die in der folgenden URL beschriebene Zahl aussehen:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Einzelziele]</td> 
   <td>Einzelne Ziele, die zu den Metriken der Teamziele beitragen, aber nicht mit der persönlichen oder beruflichen Entwicklung zusammenhängen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL geerbter Zugriff]</td> 
   <td>Freigabefunktion, mit der der Zugriff von einem Objekt zu einem anderen übertragen werden kann. Beispielsweise erbt der Zugriff des Projektbenutzers, der in Programm- und Portfoliodatensätzen definiert ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>Im [!DNL Workfront Scenario Planner] können Sie einen Plan in mehrere Initiativen unterteilen, um die Verwaltung des Plans zu vereinfachen. <span>Sie können einen [!UICONTROL Initiative]-Bericht erstellen und auf [!UICONTROL Initiative]-Informationen in einem [!UICONTROL Project]-Bericht zugreifen.</span></p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p>Der [!DNL Initiative]-Bericht ist in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner]-Lizenz erworben hat. Sie können nicht über die API auf [!UICONTROL Initiatives] zugreifen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Aufgabengebiet der <span>[!UICONTROL Initiative]</span> </td> 
   <td> <p><span>Der Berichtstyp [!UICONTROL Initiative Aufgabengebiet] zeigt Informationen zu den Aufgabengebieten an, die einer Planinitiative im [!DNL Workfront Scenario Planner] zugeordnet sind.</span> </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p><span>Dieser Berichtstyp ist in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner]-Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Aufgabengebietsstunden]</span> </td> 
   <td> <p><span> In einem Bericht mit dem Aufgabengebiet der [!UICONTROL Initiative] wird die Anzahl der Stunden angezeigt, die mit einem Aufgabengebiet in einer Initiative verknüpft sind.</span> </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p>Dieses Feld und der Berichtstyp [!UICONTROL Initiative Aufgabengebiet] sind in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Aufgabengebiet-Anzahl]</td> 
   <td> <p>In einem Bericht mit dem Aufgabengebiet der [!UICONTROL Initiative] wird die Anzahl der spezifischen Aufgabengebiete angezeigt, die einer Initiative zugeordnet sind.</p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p>Dieses Feld und der Berichtstyp [!UICONTROL Initiative Aufgabengebiet] sind in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Datum der letzten Veröffentlichung]</td> 
   <td> <p>Ein Feld in einem [!UICONTROL Initiative]-, [!UICONTROL Initiative Job Role]- und [!UICONTROL Project]-Bericht, das das Datum anzeigt, an dem eine Planinitiative zuletzt in einem Projekt veröffentlicht wurde. Sie können Initiativen veröffentlichen, um Projekte zu erstellen oder Projekte zu aktualisieren, die mit den Initiativen verknüpft sind.</p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p><span>Informationen zu Veröffentlichungsinitiativen finden Sie unter</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publish-Szenarien zum Erstellen und Aktualisieren von Projekten im [!DNL Workfront Scenario Planner]</a>. Dieses Feld ist in Ihrer [!DNL Workfront]-Instanz nur sichtbar, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner]-Lizenz erworben hat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline-Suche]</td> 
   <td>Eine Suche, die beim Ausfüllen eines Formulars durchgeführt wird, um mögliche Einträge für ein bestimmtes Feld zu finden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schnittstelleneinrichtung]</td> 
   <td>Der Bereich der Anwendung, in dem Sie benutzerdefinierte Ansichten, Filter, Gruppierungen, Listensteuerelemente usw. definieren können.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL ist Unternehmensziel]</p></td> 
   <td> <p>In [!DNL goal reports] wird für jedes strategische Ziel ein Wert "[!UICONTROL True]/ [!UICONTROL False]" angezeigt, um anzugeben, ob Ihre Organisation dem Ziel als Eigentümer zugewiesen ist. </p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] - Übersicht </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problem]</td> 
   <td> <p>Ein ungeplantes Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Er wird für weitere Überlegungen zum Arbeitsaufwand getriagiert und ausgewertet</p> <p>Ein [!UICONTROL Problem] kann auch eine [!UICONTROL Helpdesk]-Anfrage sein. [!UICONTROL-Änderungsanforderungen], [!UICONTROL-Anfragen] und [!UICONTROL-Fehler] sind ebenfalls [!UICONTROL-Probleme].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problem Management]</td> 
   <td> <p>Der Prozess und die Regeln für die Definition von Problemtypen und den Routing-, Triage- oder Traffic-Prozess, der mit jedem Typ verknüpft ist.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problembesitzer]</td> 
   <td>Das oder die Team(s), das oder die für das Auslösen und Abschließen eines Problems verantwortlich ist bzw. sind.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Ein Zeitraum, in dem ein Team eine vordefinierte Reihe von Leistungen erbringt.</td> 
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
   <td>[!UICONTROL Aufgabengebiet]</td> 
   <td> <p>Wird verwendet, um die alltäglichen Aufgabenbereiche und Aufgaben eines Benutzers zu identifizieren. Aufgabengebiete können Arbeitselementen zugewiesen werden, um die für den Abschluss eines Arbeitsprozesses erforderlichen Fertigkeiten zu ermitteln, ohne sie einem bestimmten Benutzer zuzuweisen. </p> <p>Ein Benutzer kann über mehrere Rollen verfügen. Beispiele sind Graphic Designer oder Consultant.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Tagebucheintrag]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Informationen zu Systemaktualisierungen für verfolgte Felder bereitstellt, die im Bereich [!UICONTROL-Aktualisierungen] von Projekten, Aufgaben, Problemen und anderen Objekten angezeigt werden.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Bericht zum Bereich [!UICONTROL-Updates</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban-Flag]</td> 
   <td> <p>In einem [!UICONTROL Aufgabe]- oder [!UICONTROL Problem]-Bericht zeigt das Feld [!UICONTROL Kanban Flag] den Flag-Status an, der für die Story auf dem [!UICONTROL Kanban Board] festgelegt ist. Mögliche Werte sind [!UICONTROL On Track], [!UICONTROL Ready to Pull] und [!UICONTROL Is Blocked].</p> <p>Weitere Informationen zum Festlegen des Flag-Status für Storys im [!UICONTROL Kanban Story Board] finden Sie unter  Der Artikel <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Verwenden von Flags auf Storys auf dem [!UICONTROL Kanban-Board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPIs</td> 
   <td>Ein messbarer Wert, der zeigt, wie effektiv ein Unternehmen wichtige Geschäftsziele erreicht.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Verzögerung]</td> 
   <td>Die Zeit, die nach Ablauf des [!UICONTROL Geplantes Abschlussdatum] der Vorgängeraufgabe vergehen muss, bis die abhängige Aufgabe beginnen kann.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>Die Methode zur Berechnung der [!UICONTROL Lag]-Eigenschaft. Es kann sein:</p> 
    <ul> 
     <li>[!UICONTROL Tage] (Arbeitstage)</li> 
     <li>[!UICONTROL Kalendertage] (Feiertage ignorieren)</li> 
     <li>[!UICONTROL Prozent]</li> 
     <li>[!UICONTROL Wochentag]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Übersicht über Verzögerungstypen</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Große Miniaturansicht]</td> 
   <td> <p> In einer [!UICONTROL Document]-Liste oder einem Bericht wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p>Wählen Sie <strong>[!UICONTROL Große Miniaturansicht]</strong> aus, um eine 400 Pixel breite Miniaturansicht im Bericht anzuzeigen.</p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch "[!UICONTROL Thumbnail]" in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte 10 Betrachter]</td> 
   <td> <p>In einer Berichtsliste zeigt dieses Feld die Namen von bis zu 10 Benutzern an, die den Bericht zuletzt angezeigt haben.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzte Bedingung Hinweis]</td> 
   <td> <p>Dieses Feld zeigt die letzte Aktualisierung an, die der Eigentümer des Objekts für ein Objekt eingegeben hat. Dies ist die letzte Aktivität oder Interaktion des Eigentümers mit einem Objekt.</p> <p>Die Spalte [!DNL Last Condition Note] ist leer, wenn der Notiztext der letzten Anmerkung eines Objekts gelöscht wurde. Wenn eine neue Anmerkung in das Objekt eingegeben wird, wird sie zur letzten Anmerkung und wird erneut in der Spalte angezeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datum der letzten Finanzaktualisierung]</td> 
   <td>In einem [!UICONTROL project]-Bericht erfasst dieses Feld das Datum und die Uhrzeit, zu der die Projektfinanzen zuletzt berechnet und aktualisiert wurden. Informationen zu den Projektfinanzen finden Sie unter <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Übersicht über die </a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Letzter Hinweis]</td> 
   <td> <p>Dieses Feld zeigt die letzte Aktualisierung an, die ein Benutzer für ein Objekt eingegeben hat. Dies ist die neueste Aktivität oder Interaktion mit einem Objekt.</p> <p>Die Spalte [!UICONTROL Last Note] ist leer, wenn der Text der letzten Anmerkung eines Objekts gelöscht wurde. Wenn eine neue Anmerkung in das Objekt eingegeben wird, wird sie zur letzten Anmerkung und wird erneut in der Spalte angezeigt.</p>
   <p>Wenn dieses Feld zu einem [!UICONTROL Task]-Bericht hinzugefügt wird, werden alle Aktualisierungen an untergeordneten Objekten, wie Probleme, Unteraufgaben, Dokumente usw., beibehalten. — der Aufgabe werden nicht in dieser Spalte angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zuletzt angezeigt von]</td> 
   <td> <p>In einer Berichtsliste zeigt dieses Feld Informationen zu dem Benutzer an, der den Bericht zuletzt angezeigt hat.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datum der letzten Anzeige]</td> 
   <td> <p>In einer Berichtsliste zeigt dieses Feld das Datum an, an dem der Bericht zuletzt angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout-Vorlage]</td> 
   <td>Wird vom Systemadministrator oder Gruppenadministrator definiert, um die Registerkarten und Berichte zu identifizieren, die im Arbeitsbereich eines bestimmten Benutzers angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layouttyp]</td> 
   <td>In Verbindung mit [!UICONTROL Custom Views] gibt der [!UICONTROL Layout Type] den Typ der [!UICONTROL Custom View] an. Derzeit ist nur eine Liste verfügbar. In Zukunft könnte [!UICONTROL Detail] (die [!UICONTROL Detail]-Ansicht eines Objekts) verfügbar werden.</td> 
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
   <td>Der einer [!UICONTROL Zugriffsebene] zugewiesene Lizenztyp. Entweder [!UICONTROL Full User], [!UICONTROL Eingeschränkter Benutzer] oder [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lizenzlimit-Plan]</td> 
   <td> <p>In einer Ansicht oder einem Bericht mit [!UICONTROL Group] zeigt dieses Feld die maximale Anzahl von [!UICONTROL Plan] Lizenzen an, die Benutzern zugewiesen werden können, deren jeweilige Gruppe als ihre [!UICONTROL Home Group] angegeben ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lizenzlimit Arbeit]</td> 
   <td> <p>In einer Ansicht oder einem Bericht mit [!UICONTROL Group] zeigt dieses Feld die maximale Anzahl von [!UICONTROL Work]-Lizenzen an, die Benutzern zugewiesen werden können, deren jeweilige Gruppe als ihre [!UICONTROL Home Group] angegeben ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eingeschränkter Benutzer]</td> 
   <td>Ein Lizenztyp, der die Erstellung eines [!DNL Access Level] ermöglicht, das schreibgeschützte Berechtigungen enthält, mit der Möglichkeit, Probleme zu senden, Notizen einzugeben und Dokumente hochzuladen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Listensteuerelemente]</td> 
   <td> <p>Ein Teil von [!UICONTROL Interface Setup], der die Verknüpfung benutzerdefinierter Filter, Ansichten und Gruppierungen mit einzelnen Benutzern oder global mit allen Benutzern ermöglicht.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Lookup fields]</td> 
   <td> <p>Nachdem Sie in Workfront Planning die Verbindung zwischen zwei Datensatztypen hergestellt haben und einzelne Datensätze miteinander verknüpft haben, können Sie die Felder der verknüpften Datensätze auf dem Datensatz referenzieren, von dem aus Sie eine Verbindung herstellen.</p>
   <p>Wenn Sie beispielsweise einen Campaign-Datensatztyp mit einem Workfront-Projektobjekttyp verbinden, können Sie das Budgetfeld der verbundenen Projekte in den Kampagnendatensätzen anzeigen. Das Feld Budget-Projekt ist ein Suchfeld aus Projekten in einer Kampagne.</p> <p>Die Werte der Suchfelder werden automatisch mit den Datensätzen ausgefüllt, mit denen sie verbunden sind.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/records/connected-records-overview.md">Übersicht über verbundene Datensätze</a>.</p>
   <p>Workfront Planning benötigt eine zusätzliche Lizenz.</p>
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
   <td>[!Nur UICONTROL Manuell]</td> 
   <td> <p>Einer der [!UICONTROL Update Types] eines [!UICONTROL-Projekts]. Diese Einstellung ermöglicht es, dass [!UICONTROL Project Projected]- und [!UICONTROL Planned]-Timelines nur aktualisiert werden, wenn "[!UICONTROL Recalcalculated Timelines]" angeklickt wird. Auf diese Weise eingerichtete Projekte werden bei der nächtlichen Neuberechnung und beim Aktualisieren des Projekts bzw. der Aufgaben im Projekt ignoriert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswählen des Projekts [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ME]</td> 
   <td> <p>Dies bezieht sich auf den aktuell angemeldeten Benutzer. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max. Benutzer]</td> 
   <td> <p>Dies ist ein veraltetes Feld. Alle Informationen, die dieses Feld möglicherweise anzeigt, beziehen sich auf eine Funktion, die [!DNL Workfront] entfernt hat und das Feld kann nicht aktualisiert werden. </p> <p>In früheren Versionen von [!DNL Workfront] konnten Sie dieses Feld aktualisieren, wenn Sie ein Aufgabengebiet erstellen oder bearbeiten. Es wurde die Gesamtzahl der Benutzer angezeigt, die in jedem Projekt einer Rolle zugeordnet werden können. Der Wert Null ermöglicht eine unbegrenzte Anzahl von Benutzern, die einem Projekt zugewiesen werden können. </p>Das Feld ist weiterhin in einigen Berichten und Listen sichtbar, aber die angezeigten Informationen können nicht aktualisiert werden. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Eine Markierung, die Sie mit einer Aufgabe verknüpfen können, um anzugeben, dass nach Abschluss der Aufgabe ein Schlüsselpunkt im Projekt erreicht wurde. Im Allgemeinen können Sie Meilensteine verwenden, um ein bedeutendes Ereignis anzuzeigen, z. B. den Abschluss einer Projektphase oder eine Reihe wichtiger Aktivitäten. [!UICONTROL Milestones] sind normalerweise mit übergeordneten Aufgaben verknüpft. Sie müssen die Meilensteine erstellen, bevor Sie sie Aufgaben zuordnen können. Weitere Informationen zu Meilensteinen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Erstellen eines Meilensteinpfads</a> und <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Zuordnen von Meilensteinen zu Aufgaben</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Meilensteinpfad]</td> 
   <td>Eine Sammlung von [!UICONTROL Milestones]. [!UICONTROL Meilensteinpfade] werden für Projekte verwendet, um Projekte mit bestimmten Typen von [!UICONTROL Meilensteinen] von Projekten mit einem anderen Satz [!UICONTROL Meilensteine] zu unterscheiden.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Meilensteinaufgabe]</td> 
   <td>Eine Aufgabe, die gekennzeichnet ist, um ein zu messendes berichtspflichtiges Ereignis anzugeben.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL-Modul]</td> 
   <td>Ein einzelner Schritt innerhalb eines Szenarios in [!DNL Workfront Fusion], das je nach zugeordneter App bestimmte Funktionen ausführt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Meine Primäre Rolle]</td> 
   <td> <p>Wenn dies in Filtern referenziert wird, zeigt dies entweder Benutzende an, die dieselbe [!UICONTROL Primär Role] wie der angemeldete Benutzende haben, oder Arbeitselemente, die der [!UICONTROL Primär Role] des angemeldeten Benutzenden zugewiesen sind.</p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Mein Home-Team]</td> 
   <td> <p>Wenn dies in Filtern referenziert wird, zeigt dieses Feld entweder Benutzer an, die zum [!UICONTROL Home Team] des angemeldeten Benutzers gehören, oder Arbeitselemente, die dem [!UICONTROL Home Team] des angemeldeten Benutzers zugewiesen sind. </p> <p>Es wird empfohlen, dieses Feld in einem Filter zu verwenden, um Berichte bei der Freigabe für andere Benutzer allgemeiner zu gestalten. Auf diese Weise können Sie nur einen Bericht erstellen, der unterschiedliche Informationen anzeigt, je nachdem, wer sich anmeldet, um ihn anzuzeigen, da die Informationen immer für den angemeldeten Benutzer angepasst werden. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL-Namenskonvention]</td> 
   <td>Ein organisationsweiter Regelsatz, der Daten zur Erstellung von Namen von Projekten, Aufgaben und Ergebnissen verwendet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Eine Integration, die keine manuelle Codierung oder API-Konfiguration erfordert. Wird auch als vorkonfigurierte Integration bezeichnet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigationsmenü]</td> 
   <td>Das Bedienfeld in der oberen Mitte der Anwendung, das Links zu den Hauptbereichen von [!UICONTROL Workfront] enthält.</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Zahlenwert]</td> 
   <td>In einem [!UICONTROL Tagebucheintrag]-Bericht wird der aktualisierte Wert eines Felds angezeigt, das den [!UICONTROL Alter Zahlenwert] ersetzt.
   Weitere Informationen finden Sie unter "[!UICONTROL Alter Zahlenwert]" in diesem Artikel.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Nicht fakturierbare Kosten]</td> 
   <td> <p>Eine Ausgabe, die für den Kunden nicht als fakturierbar markiert ist. Dies kann entweder eine geplante Ausgabe oder eine tatsächliche Ausgabe sein.</p> <p>Die Felder Geplante nicht fakturierbare Kosten und Tatsächliche nicht fakturierbare Kosten stehen Ihnen zur Verfügung, um sie Ansichten und Berichten hinzuzufügen. Sie werden nicht auf den Seiten mit den Projekt- oder Aufgabendetails angezeigt.</p>
   <p>Diese Felder finden Sie in den folgenden Berichtstypen:</p>
   <ul>
   <li>Ausgangsbasis</li>
   <li>Vorlage</li>
   <li>Projekt (Finanzdaten)</li>
   </ul>
   <p>Weitere Informationen zum Kennzeichnen einer Ausgabe als fakturierbar finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Projektausgaben verwalten</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL arbeitsfreier Tag]</td> 
   <td>Ein Tag, der nicht für den Abschluss von Zuweisungen zugewiesen ist. Dies ist normalerweise ein Urlaubstag, Urlaub oder Wochenende. Der Begriff wird im API-Explorer angezeigt. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hinweis]</td> 
   <td>Ein Kommentar oder eine Aktualisierung zu einem [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notizentext]</td> 
   <td> <p>Dadurch wird der Text einer Aktualisierung angezeigt, die von einem Benutzer für ein beliebiges Objekt eingegeben wurde. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anzahl der verknüpften Ziele]</td> 
   <td> <p>In einem [!UICONTROL Project]-Bericht ist dies die Anzahl der strategischen Ziele, die mit dem Projekt verbunden sind. Informationen zum Verknüpfen von Projekten mit strategischen Zielen finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Hinzufügen von Projekten zu Zielen in [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Informationen zu strategischen Zielen finden Sie auch unter "[!UICONTROL Goal]" in diesem Artikel.</p> 
   <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Hinzufügen von Projekten zu Zielen in [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Objekt]</td> 
   <td> <p>Die in [!DNL Adobe Workfront] angezeigten Informationen werden durch Objekte dargestellt, die in der [!DNL Workfront] Datenbank gespeichert sind. Die Objekte sind es, die die Informationen in Workfront steuern. Beispiele für -Objekte:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL-Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL-Dokumente]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Berichte]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Benutzer]</li> 
     <li>[!UICONTROL Firmen]</li> 
     <li>[!UICONTROL Benutzerdefinierte Formulare]</li>
     <li>[!UICONTROL Benutzerdefinierte Felder]</li>  
     <li>[!UICONTROL Stunden]</li> 
     <li>[!UICONTROL Abrechnungssätze]</li> 
     <li>[!UICONTROL-Vorlagen]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li>

<p><b>NOTIZ</b></p>
  <p>Dies ist keine umfassende Liste. </p>

</ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Objekttypen]</td> 
   <td>Wenn Sie einen Bericht oder eine Liste mit allen Ihren benutzerdefinierten Formularen erstellen, können Sie dieses Feld als Ansicht oder Filter verwenden, um zu sehen, welche Objekttypen mit jedem Formular verknüpft sind. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Alter Zahlenwert]</td> 
   <td>In einem [!UICONTROL Tagebucheintrag]-Bericht wird der ursprüngliche Wert eines Feldes vor seiner Aktualisierung angezeigt. Nachdem der Wert eines Felds aktualisiert wurde, wird es als [!UICONTROL Neuer Zahlenwert] in einem [!UICONTROL Tagebucheintrag]-Bericht angezeigt. Weitere Informationen finden Sie auch unter "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL nur bei Änderung]</td> 
   <td> <p>Einer der [!UICONTROL Project Update]-Typen. Wenn diese Option ausgewählt ist, werden die Zeitleisten [!UICONTROL Project Projected] und [!UICONTROL Planned] nur aktualisiert, wenn eine Aktualisierung oder Änderung am Projekt oder an einer Aufgabe innerhalb des Projekts vorgenommen wird. Das Projekt wird nicht jede Nacht aktualisiert.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswahl des Projektaktualisierungstyps </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabe]</td> 
   <td> <p>Der Name für [!UICONTROL Problem] in der [!DNL Workfront]-Datenbank, der in Textmodusberichten oder berechneten benutzerdefinierten Daten verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Öffnen]</td> 
   <td>Ein Problem oder eine Aufgabe, das bzw. die noch nicht abgeschlossen ist, aber bearbeitet wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigramm]</td> 
   <td>Abkürzung für Organigramm. Dies ist ein Diagramm, das die Hierarchie einer Organisation zeigt. Auf der Registerkarte auf dem Detailbildschirm [!UICONTROL Benutzer] werden auch die [!UICONTROL Company]- und [!UICONTROL Reporting]-Beziehungen des [!UICONTROL Benutzers] angezeigt und können festgelegt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organisations-Setup]</td> 
   <td>Dadurch werden [!UICONTROL Firmen], [!UICONTROL Gruppen] und [!UICONTROL Sicherheitsprofile] für Ihre Organisation definiert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Andere Gruppen]</td> 
   <td> <p>In einem Bericht oder einer Ansicht, der bzw. die Benutzer auflistet, zeigt dieses Feld alle Gruppen an, in denen jeder Benutzer Mitglied ist. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Währung überschreiben]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Aufgabengebiet]-Bericht ist dies die Währung, die mit einem Aufgabengebiet verknüpft ist. Dies ist eine Überschreibung der [!UICONTROL Basiswährung], wie sie vom [!DNL Workfront] im Bereich [!UICONTROL Setup] festgelegt wurde. </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Überschreiben Währung Abrechnung/Stunde]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Aufgabengebiet]-Bericht ist dies der Abrechnungssatz pro Stunde des Aufgabengebiets, das die ausgewählte [!UICONTROL Überschreibungswährung] des Aufgabengebiets verwendet.</p> 
     <p> Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Währungskosten/ Stunde überschreiben]</span> </td> 
   <td> 
    <div> 
     <p>In einem Bericht zu [!UICONTROL Aufgabengebiet] ist dies der Stundensatz des Aufgabengebiets unter Verwendung der ausgewählten [!UICONTROL Überschreibungswährung] des Aufgabengebiets. </p> 
     <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Inhaber]</td> 
   <td>Der Benutzer, der für die Fertigstellung des angegebenen Objekts verantwortlich ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Besitzertyp]</span> </td> 
   <td> 
    <div> 
     <p>In einem [!UICONTROL Goal]-Bericht wird der Besitzertyp angezeigt, der einem strategischen Ziel zugewiesen ist. Im Folgenden finden Sie die Typen von Zieleigentümern:</p> 
     <ul> 
      <li> <p>[!UICONTROL-Benutzer]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL-Gruppe]</p> </li> 
     </ul> 
     <p>In diesem Feld wird kein Wert angezeigt, wenn der Zielinhaber Ihr Unternehmen ist. </p> 
     <p>Dies erfordert eine zusätzliche Lizenz. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] - Übersicht</a>. </p> 
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
   <td>[!UICONTROL-Parameter]</td> 
   <td> <p>Ein [!UICONTROL-Parameter] ist ein benutzerdefiniertes Feld. Sie können einen Bericht für alle Parameter oder benutzerdefinierten Felder in Ihrem System erstellen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>In einem Bericht zeigt dieses Feld Informationen zum übergeordneten Element des -Objekts an. Beispielsweise kann in einem [!UICONTROL issue]-Bericht Informationen zu der Aufgabe oder dem Projekt angezeigt werden, unter der bzw. dem das Problem protokolliert ist. In einem Aufgabenbericht kann er Informationen zur direkt übergeordneten Aufgabe oder zum Projekt enthalten. Weitere Informationen dazu, welche Objekte in [!DNL Workfront] übergeordnete Elemente haben könnten, finden Sie im Abschnitt „Interdependenz und Hierarchie von Objekten“ im Artikel "<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref"> von Objekten in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnete Verzögerung]</td> 
   <td>Die Zeit, die zwischen dem Start der [!UICONTROL Parent Task] und dem Start der [!UICONTROL Subtask] vergehen muss.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnete Aufgabe]</td> 
   <td>Wird auch als [!UICONTROL Summary Task] bezeichnet. Dies ist eine Aufgabe mit Unteraufgaben (auch als [!UICONTROL Untergeordnete Aufgaben] bezeichnet). Die [!UICONTROL Duration], [!UICONTROL Work Required] und [!UICONTROL Percent Complete] der übergeordneten Aufgabe werden aus den Teilaufgaben berechnet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Teilzeitressourcen]</td> 
   <td>Ein lizenzierter Benutzer, der über weniger Kapazität verfügt als der im System definierte Standardzeitplan.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Prozent abgeschlossen]</td> 
   <td> <p>Ein Projekt, eine Aufgabe oder ein Problem, das bzw. das anzeigt, welcher Prozentsatz der mit der Aufgabe, dem Projekt oder dem Problem verbundenen Arbeit abgeschlossen ist.</p> <p>Sie können dieses Feld für Probleme und Arbeitsaufgaben manuell aktualisieren. </p> <p>Für Projekte und übergeordnete Aufgaben ist dieses Feld eine Zusammenfassung aller laufenden Aufgaben. Sie können es nicht manuell aktualisieren. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Projektübersicht [!UICONTROL Percent Complete</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Berechtigung]</td> 
   <td> <p>Rechte, die einem Benutzer für ein Objekt gewährt werden, normalerweise gewährt, damit er Arbeiten am Element abschließen oder das Element anzeigen kann. Berechtigungen können erteilt werden für:</p> 
    <ul> 
     <li>[!UICONTROL-Projekte]</li> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programme]</li> 
     <li>[!UICONTROL Berichte]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL-Dokumente]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL-Ansichten]</li> 
     <li>[!UICONTROL Filter]</li> 
     <li>[!UICONTROL Gruppierungen]</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über Freigabeberechtigungen für Objekte</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Plan]</td> 
   <td> <p>Dies ist ein vollständiger Lizenztyp im [!DNL Workfront]. Diese Berechtigung ist für den Zugriff auf alle Funktionen in [!DNL Workfront] erforderlich.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (im [!DNL Scenario Planner])</td> 
   <td> <p>Ein Plan ist das Hauptobjekt bei der Arbeit mit dem [!DNL Workfront]. Sie können die Strategie für die kurz- und langfristige Zukunft Ihres Unternehmens skizzieren, jedes Ergebnis auf hoher Ebene identifizieren und es als Plan zum [!DNL Workfront]-Szenario-Planer hinzufügen. </p> <p>Sie können [!DNL Scenario Planner] Pläne nicht in einem Bericht anzeigen und Sie können nicht über die [!DNL Workfront]-API darauf zugreifen. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Scenario Planner] - Übersicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL geplant]</td> 
   <td> <p>Der Zeitrahmen, in dem etwas eingetreten ist. Beim Erstellen von Projekten, Aufgaben oder Problemen in [!DNL Workfront] legen Sie die geplanten Start- und Enddaten sowie den geplanten Zeitrahmen fest, in dem sie auftreten. Diese Werte stellen Ihre ursprüngliche Absicht oder Schätzung dar, wie lange ein Element dauern sollte, um abgeschlossen zu werden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Nutzen]</td> 
   <td>Dies ist eine manuelle Eingabe für den Projekt-Manager, um zu schätzen, ob die Fertigstellung eines Projekts der Organisation einen finanziellen Vorteil bringen würde. Die Angabe dieses Werts kann Teil der Erstellung eines [!UICONTROL Business Case] für das Projekt sein. Sie müssen über [!UICONTROL Manage]-Berechtigungen für das Projekt verfügen, um diesen Wert zu aktualisieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Geplante budgetierte Stunden]</td> 
   <td> <p>In einem Bericht zu [!UICONTROL Budgetierte Stunde] wird die Anzahl der budgetierten Stunden für Projekte oder [!UICONTROL Aufgabengebiete] im [!UICONTROL Ressourcenplaner] angezeigt. </p> <p>Informationen zur Budgetierung von Projekten oder Funktionen im [!UICONTROL Resource Planner] finden Sie im Artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budgetressourcen im [!UICONTROL Resource Planner] unter Verwendung der Ansichten [!UICONTROL Project] und [!UICONTROL Role</a>. Informationen zum Bericht [!UICONTROL Budgetierte Stunden] finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Bericht: Budgetierte Stunde</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplantes Abschlussdatum]</td> 
   <td> <p>Sie können das geplante Abschlussdatum (!UICONTROL) einer Aufgabe, eines Projekts oder eines Problems manuell auf ein Datum Ihrer Wahl setzen. Wenn Sie das geplante Abschlussdatum [!UICONTROL] nicht festlegen, legt [!DNL Workfront] es automatisch fest. Bei automatischer Festlegung lautet das [!UICONTROL Geplantes Abschlussdatum]: [!UICONTROL Geplantes Startdatum] + [!UICONTROL Dauer]</p> <p>Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über die Aufgabe [!UICONTROL Geplantes Abschlussdatum]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Legen Sie das Projekt fest [!UICONTROL Geplantes Abschlussdatum]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Kosten]</td> 
   <td> <p>Summe der [!UICONTROL Geplanten Lohnkosten] und der [!UICONTROL Geplanten Ausgaben] des Projekts. Dies umfasst nicht die [!UICONTROL Geplante Risikokosten] für das Projekt.  </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Ausrichtung am geplanten Datum]</td> 
   <td> <p>Hierbei handelt es sich um einen automatischen Indikator, mit dem Workfront Projekte, Aufgaben und Probleme zuweist, um anzuzeigen, wann ein Element in Bezug auf das geplante Abschlussdatum abgeschlossen wird. </p>
   <p>Im Folgenden finden Sie mögliche Werte für den Indikator für die Ausrichtung am geplanten Datum: </p>
<ul>
<li>Wird zum geplanten Abschlussdatum fertiggestellt</li>
<li>Wird vor dem geplanten Abschlussdatum fertiggestellt</li>
<li>Wird nach dem geplanten Abschlussdatum fertiggestellt</li></ul>
<p>Die Ausrichtung am geplanten Datum ist in Projekt-, Aufgaben- und Problemlisten und Berichten sichtbar. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL geplante Dauer]</td> 
   <td> <p>Die geplante Dauer einer Aufgabe [!UICONTROL] ist normalerweise mit der [!UICONTROL-Dauer] der Aufgabe identisch. Sie stellt die Differenz in Tagen zwischen dem [!UICONTROL Geplanter Start] und dem [!UICONTROL Geplante Abschlussdatum] der Aufgabe dar. </p> <p>Wenn die Aufgabe einen [!UICONTROL Duration]-Typ von [!UICONTROL Effort Driven] hat, kann die [!UICONTROL Planned Duration] von der [!UICONTROL Duration] der Aufgabe abweichen, je nachdem, wie viele Ressourcen Sie der Aufgabe zuweisen. </p> <p>Wenn beispielsweise eine Aufgabe mit dem [!UICONTROL Duration]-Typ [!UICONTROL Effort Driven] eine [!UICONTROL Duration] von 3 Tagen hat und Sie der Aufgabe eine Ressource mit einem Vollzeitplan zuweisen, beträgt die [!UICONTROL Planned Duration] ebenfalls 3 Tage. Wenn Sie derselben Aufgabe drei Ressourcen mit einem Vollzeitplan zuweisen, bleibt die [!UICONTROL Duration] 3 Tage, aber die [!UICONTROL Planned Duration] wird zu 1 Tag. Die geplante Dauer von [!UICONTROL] ändert auch die Daten von [!UICONTROL Geplanter Start] und [!UICONTROL Geplanter Abschluss] der Aufgabe, um die neue geplante Dauer von [!UICONTROL] widerzuspiegeln. Daher ist auch die Zeitleiste des Projekts betroffen. </p> <p>Weitere Informationen zum Unterschied zwischen der [!UICONTROL-Dauer] und der [!UICONTROL-geplanten Dauer] für Aufgaben finden Sie im Artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Unterschied zwischen der [!UICONTROL-geplanten Dauer] und der [!UICONTROL-Dauer] für Aufgaben</a>.</p> <p>Projekte und Probleme haben keine [!UICONTROL geplante Dauer]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Dauer in Minuten]</td> 
   <td> <p>Die [!UICONTROL Geplante Dauer in Minuten] eines Projekts oder Problems entspricht der [!UICONTROL Dauer] des Projekts oder Problems in Minuten. </p> <p>Aufgaben haben kein Feld [!UICONTROL Geplante Dauer in Minuten]. </p> <p>[!UICONTROL Vorlagenaufgaben] haben ein Feld [!UICONTROL Geplante Dauer in Minuten], das die [!UICONTROL Geplante Dauer] der Aufgabe in Minuten anzeigt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Ausgaben]</td> 
   <td> <p>Die Summe der [!UICONTROL Geplanten Beträge] für alle Ausgaben, die für ein Projekt oder eine Aufgabe protokolliert wurden.</p> <p><b>BEISPIEL</b></p>
   <p>Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und 600,00 $ in das Feld [!UICONTROL Geplanter Betrag] eingeben, beträgt die [!UICONTROL Geplante Ausgabenkosten] für diese Aufgabe 600,00 $. </p> 
   <p>Für ein Projekt verwendet [!DNL Workfront] die folgende Formel, um [!UICONTROL Geplante Ausgaben] zu berechnen:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Stunden]</td> 
   <td> <p>Dieses Feld wird in den [!UICONTROL-Projekten], [!UICONTROL-Aufgaben] und Problembereichen, Berichten für Projekte, Aufgaben oder Probleme und Ressourcenverwaltungs-Tools wie dem [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] und dem [!UICONTROL Utilisation]-Bericht angezeigt. </p> <p>Darin wird die Anzahl der Stunden angezeigt, die nach Schätzungen des Projektbesitzers jede Aufgabe oder jedes Problem bis zur Fertigstellung dauern sollte. Bei Projekten handelt es sich im Allgemeinen um eine Zusammenfassung der [!UICONTROL Geplante Stunden] aus den Aufgaben im Projekt. </p> <p>Das Feld [!UICONTROL Geplante Stunden] zeigt möglicherweise unterschiedliche Informationen an, je nachdem, von wo aus sie angezeigt werden. Informationen zu den geplanten Stunden finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Übersicht über die geplanten Stunden</a>.</p> <p>Geplante Stunden werden in Minuten in der [!DNL Workfront]-Datenbank gespeichert. Berücksichtigen Sie beim Schreiben von Berechnungen mit diesem Feld, dass die Stunden als Minuten angezeigt werden.<br></p> <p>Standardmäßig werden die geplanten Stunden gleichmäßig auf alle Tage innerhalb der Dauer eines Arbeitselements und auch gleichmäßig auf alle Ressourcen verteilt, die der Aufgabe zugewiesen sind. Benutzer können die tägliche Anzahl der geplanten Stunden für ein Arbeitselement oder die individuellen geplanten Stunden für jeden Zugewiesenen aktualisieren.</p> <p>Die Aktualisierung dieses Feldes unterscheidet sich bei Projekten, Aufgaben und Problemen: </p> 
    <ul> 
     <li> <p>Bei Problemen können Sie dieses Feld manuell aktualisieren. Die geplanten Stunden für das Problem werden nicht zu den geplanten Stunden des Projekts hinzugefügt. </p> <p><b>TIPP</b></p> <p>In einem Problembericht wird eines der Felder [!UICONTROL Geplante Stunden] durch das Feld [!UICONTROL Arbeit] ersetzt. Das Feld zeigt die Anzahl der für das Problem geplanten Stunden an. Weitere Informationen finden Sie in den Feldern „Arbeit“ oder "[!UICONTROL Arbeit]" in dieser Tabelle. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Für Aufgaben können Sie dieses Feld manuell aktualisieren, wenn der [!UICONTROL Duration Type] der Aufgabe [!UICONTROL Calculated Assignment] oder [!UICONTROL Simple] ist. Dieses Feld wird von [!DNL Workfront] berechnet, wenn der [!UICONTROL Duration Type] der Aufgabe [!UICONTROL Calculated Work] oder [!UICONTROL Effort Driven] ist.<br>Informationen zur [!UICONTROL Aufgabendauer] finden Sie im Artikel <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die [!UICONTROL Aufgabendauer] und [!UICONTROL Dauertyp]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Bei Projekten berechnet [!DNL Workfront] die geplanten Stunden, indem alle geplanten Stunden aus allen Aufgaben im Projekt hinzugefügt werden. </p> </li> 
    </ul> <p><b>TIPP</b></p> <p>Sie können [!UICONTROL Geplante Stunden] in [!UICONTROL project]-, [!UICONTROL task]- oder [!UICONTROL issues]-Berichten auch mithilfe des Textmodus anzeigen und auf zusätzliche Felder verweisen. Weitere Informationen finden Sie in den Feldern "<code>work</code>", "[!UICONTROL Work]" und "<code>workRequiredExpression</code>" in dieser Tabelle. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Lohnkosten]</td> 
   <td> 
    <p>Für eine Aufgabe der Stundensatz des Benutzers oder der Funktion multipliziert mit der Anzahl der Stunden, die dem Benutzer oder der Funktion zugewiesen wurden.</p> <p>Bei einem Projekt entspricht dies der Summe aller [!UICONTROL Geplante Lohnkosten] aller Aufgaben.</p> <p>Ob der Satz des Benutzers oder der Funktion verwendet wird, hängt vom Kostentyp ab, der für die jeweilige Aufgabe ausgewählt wurde. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md">Kosten </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Umsatz]</td> 
   <td> <p>Aufgaben und Projekte können einen Wert für den [!UICONTROL Geplanter Umsatz] in [!DNL Workfront] anzeigen. [!UICONTROL Geplanter Umsatz] stellt den Geldbetrag dar, der mit den [!UICONTROL Geplante Stunden] der Aufgaben im Projekt verbunden ist. Bei Projekten kann sie auch den [!UICONTROL Festeinnahmen] des Projekts enthalten. </p> <p>Bei Aufgaben ist dies der Umsatz, der mit den [!UICONTROL Geplante Stunden] von Aufgaben verbunden ist. Die geplanten Stunden aller Aufgaben summieren sich auf die geplanten Stunden des Projekts, um zur Berechnung der geplanten Stunden des Projekts beizutragen [!UICONTROL]. </p> 
   <p>[!DNL Workfront] Berechnet [!UICONTROL Geplanter Umsatz] für Aufgaben und Projekte nach folgenden Formeln:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Das Projekt [!UICONTROL Geplanter Umsatz], das im Bereich [!UICONTROL Projektdetails] und in Projektberichten angezeigt wird, unterscheidet sich von den geplanten Einnahmen, die im Bericht [!UICONTROL Auslastung] angezeigt werden. </p> <p>Die [!UICONTROL Geplante Einnahmen] im Bereich [!UICONTROL Projektdetails] spiegeln die Aufgabeneinnahmen sowie die Festeinnahmen des Projekts wider. Der [!UICONTROL Geplanter Umsatz] im [!UICONTROL Auslastungsbericht] zeigt [!UICONTROL Geplanter Umsatz] an, der nur den Aufgaben im Projekt zugeordnet ist. </p> 
     <p><b>BEISPIEL</b></p>  
      <p>Wenn das Projekt 1 Aufgabe mit 10 Stunden hat, einem Berater mit einem Stundensatz von 20 $ zugewiesen ist und das Projekt 100 $ [!UICONTROL Fester Umsatz] hat, zeigt der Bericht zur [!UICONTROL-Nutzung] 200 $ für den [!UICONTROL Geplanter Umsatz] an (der [!UICONTROL Geplante Umsatz], der den Stunden für die Aufgabe zugeordnet ist). Der Abschnitt [!UICONTROL Projektdetails] zeigt 300 $ (den [!UICONTROL Geplanten Umsatz] aus der Aufgabe und den Festeinnahmen für das Projekt) an. </p> 
    <p>Informationen zur Umsatzverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Übersicht über Abrechnung und Umsatz</a>. </p> 
    <p>Weitere Informationen zu den Berechnungen des [!UICONTROL Geplanter Umsatz] im [!UICONTROL Auslastungsbericht] finden Sie unter <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Ressourcenauslastungsinformationen anzeigen</a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplante Risikokosten]</td> 
   <td> <p>Die Summe der [!UICONTROL Potenzialkosten] aller Risiken des Projekts unter Berücksichtigung ihrer Eintrittswahrscheinlichkeit. Dieser Betrag ist nicht in den [!UICONTROL Geplante Kosten] des Projekts enthalten.</p> <p>Die [!UICONTROL Geplante Risikokosten] eines Projekts werden nach folgender Formel berechnet:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portalprofil]</td> 
   <td>Eine vom Administrator definierte Sammlung von Registerkarten und Abschnitten, die in [!DNL Workfront] angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal-Abschnitt]</td> 
   <td>Eine Komponente einer Registerkarte auf einem Dashboard oder einer Portalseite. Normalerweise ein einzelner Bericht, ein Diagramm, ein Kalender oder eine Liste wichtiger Informationen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal-Registerkarte]</td> 
   <td>Eine Registerkarte in einem Portal oder Dashboard, die bis zu drei Portalabschnitte enthält.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL-Portfolio]</td> 
   <td> <p>Eine Sammlung von Projekten mit einheitlichen Merkmalen. Diese Projekte konkurrieren normalerweise um dieselben Ressourcen, Budgets oder Zeitfenster. Sie können Portfolios in Programme unterteilen und die Projekte mit den Programmen verknüpfen, bevor sie einem Portfolio hinzugefügt werden.</p> <p>Weitere Informationen zu Portfolios finden Sie unter Übersicht über das <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Ein Praxisbereich, der sich auf die Verwaltung einer Sammlung oder verwandter Programme und Projektmaßnahmen konzentriert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Ein [!DNL Workfront] Tool zur Unterstützung bei der Bewertung und Priorisierung von Projekten innerhalb eines Portfolios.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>Der Stakeholder, der für die Priorisierung und das Budget für ein Portfolio verantwortlich ist.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potenzielle Risikokosten]</td> 
   <td>Dies ist ein Projektfeld, das Sie in Listen und Berichten finden können. Es zeigt die potenziellen Kosten für die Risiken, die mit dem Projekt verbunden sind, falls sie auftreten sollten. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnung potenzieller Risikokosten - </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Vorgänger]</td> 
   <td> <p>Eine Aufgabe, die vor dem Abschluss einer abhängigen Aufgabe abgeschlossen werden muss. Auch eine Aufgabe, die als [!UICONTROL Dependency] für eine andere Aufgabe markiert ist. Vorgänger ermöglichen es dem Planer, eine Sequenzabhängigkeitslogik festzulegen, z. B. um eine Aufgabe nach Abschluss einer anderen Aufgabe zu starten.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Übersicht über Aufgabenvorgänger</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primäre Firma]</td> 
   <td>Das Unternehmen, zu dem der Benutzer gehört, wie in den Benutzereinstellungen angegeben. Firmen können auch mit Projekten verknüpft werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primärer Kontakt]</td> 
   <td><p>Der [!UICONTROL Primär Contact] ist der Ersteller eines Problems und wird automatisch von [!DNL Workfront] bestimmt, wenn die Person das Problem erstellt. Sie können dieses Feld manuell aktualisieren, wenn Sie über [!DNL Manage] für das Problem verfügen. Ein Problem kann nur einen Primären Kontakt haben.</p> 
   <p>Wenn Sie den Primären Kontakt ändern, hat der ursprünglich als Primärkontakt angegebene Benutzer weiterhin [!UICONTROL Manage] Zugriff auf das Problem.</p>
   <p>Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird der als [!UICONTROL Primär Contact] des Problems angegebene Benutzer zum [!UICONTROL Converted Issue Originator] des Projekts oder der Aufgabe. Wenn der [!UICONTROL Primär Contact] des Problems nach der Konvertierung des Problems aktualisiert wird, wird der [!UICONTROL Converted Issue Originator] zum Zeitpunkt der Konvertierung als der [!UICONTROL Primär Contact] des Problems beibehalten. Siehe auch "[!UICONTROL Converted Issue Originator]" in diesem Artikel.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL-Priorität]</td> 
   <td>Ein Wert, der einer Aufgabe, einem Problem oder einem Projekt zugewiesen werden kann, um festzulegen, wie wichtig er ist. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privat]</td> 
   <td>In einem [!UICONTROL Hinweis] oder [!UICONTROL Dokument] macht diese Option dieses Objekt für die meisten Betrachter ausgeblendet. Bei einer Warteschlange für private Hilfeanfragen können nur Benutzer des Projektteams Probleme an diese Warteschlange (oder dieses Projekt) über den Bereich [!UICONTROL Anfragen] senden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Profil]</td> 
   <td>Alle Informationen zu einem Benutzerkonto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL-Programm]</td> 
   <td> <p>Eine Untergruppe innerhalb eines Portfolios, in der ähnliche Projekte gruppiert werden können, um einen klar definierten Nutzen zu erzielen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programmverwaltung]</td> 
   <td>Management von projektübergreifenden Abhängigkeiten, Risiken, Problemen, Anforderungen und Lösungen, um das Programm gesund zu halten und den definierten Programmnutzen zu erzielen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Programmbesitzer]</td> 
   <td>Der Stakeholder, der für die Überwachung und Organisation von Aktivitäten verantwortlich ist, um sicherzustellen, dass die Projektziele mit den Unternehmenszielen übereinstimmen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL progress]</span> </td> 
   <td> <p>In einem [!UICONTROL Goal]-Bericht wird hier der Prozentsatz angezeigt, wie nahe ein strategisches Ziel dem Abschluss ist. Der Prozentsatz des Fortschritts wird als Zahl angezeigt. Informationen zu strategischen Zielen finden Sie auch unter "[!UICONTROL Goal]" in dieser Tabelle.</p> <p>Dieses Feld ist nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront] Ziele gekauft hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Hinzufügen von Projekten zu Zielen in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verlaufsstatus]</td> 
   <td> <p>In einem Projekt-, Aufgaben- und Zielbericht zeigt dieses Feld den Fortschrittsstatus von Projekten, Aufgaben oder strategischen Zielen an. Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Übersicht über den Projektfortschritt</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Übersicht über den Aufgabenstatus</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Übersicht über den Zielfortschritt und den Zustand in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Der Bericht [!UICONTROL Goal] und der Bericht [!UICONTROL Progress Status] für [!DNL goals] Feld sind nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zu strategischen Zielen in [!DNL Workfront Goals] finden Sie in <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] Übersicht</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL-Projekt]</td> 
   <td> <p>Ein großer Arbeitsaufwand, der innerhalb eines bestimmten Zeitrahmens abgeschlossen werden muss und ein bestimmtes Budget und eine bestimmte Anzahl von Ressourcen erfordern muss. Um es überschaubar zu machen, unterteilen Sie das Projekt in eine Reihe von Aufgaben. Das Abschließen aller Aufgaben führt zum Abschluss des Projekts. Informationen zur Planung eines Projekts finden Sie unter <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Projektübersicht planen</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektzuweisung Geplante Stunden]</td> 
   <td> <p>In einem Bericht mit dem Aufgabengebiet der [!UICONTROL Initiative] wird die Anzahl der [!UICONTROL Geplante Stunden] angezeigt, die einem Aufgabengebiet zugeordnet sind, das Aufgaben oder Problemen im Projekt zugewiesen wurde. Dieses Feld und der Berichtstyp [!UICONTROL Initiative Aufgabengebiet] werden in Ihrer [!DNL Workfront] nur angezeigt, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] Lizenz erworben hat. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Die [!DNL Workfront Scenario Planner] - Übersicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektdetails]</td> 
   <td>Die Details des aktuellen Status eines Projekts.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt budgetierte Kosten]</td> 
   <td> <p> Dies sind die [!UICONTROL Budgetierten Kosten] eines Projekts, wie sie in Listen und Berichten angezeigt werden.</p><p>Siehe auch "[!UICONTROL Budgetierte Kosten]" in diesem Artikel.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Projektverwaltung]</td> 
   <td>Ein Satz von Richtlinien, der die Schwellenwerte für die Projekterstellung, -kategorisierung und -benennung steuert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Projektmehraufwand]</td> 
   <td>In einem [!UICONTROL Hour]-Bericht ist dieses Feld für Finanzinformationen reserviert, die sich auf die Stunden beziehen, die mit dem Stundentyp [!UICONTROL Project Time] protokolliert wurden. Projekte können über eigene Abrechnungssätze verfügen. Wenn für ein Projekt direkt eine Stunde protokolliert wird, werden diese Sätze in Berechnungen verwendet. Basierend auf den Projekteinstellungen können Projekte auch verschiedene Währungen haben und es kann eine Währungsumrechnung für diese Stunden geben. Mit dem [!UICONTROL Project Overhead]-Objekt können [!DNL Workfront] diese Informationen abrufen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektbesitzer]</td> 
   <td>Der Benutzer, der für die Verwaltung von Umfang, Zeitleiste und Zuweisungen eines Projekts verantwortlich ist. Die standardmäßige genehmigende Person für Änderungsaufträge, finanzielle Änderungen und Lieferungen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektplanung]</td> 
   <td>Prozesse zum Entwickeln und Verwalten des Projektplans.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektsponsor]</td> 
   <td>Ein spezielles Stakeholder-Profil, auf das sich jeder Ihrer Benutzer beziehen sollte. In [!DNL Workfront] werden diese als [!UICONTROL Zugriffsebenen] bezeichnet</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projektteams]</td> 
   <td> <p>Die einem Projekt zugewiesene Sammlung von Benutzern oder Rollen</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Übersicht über das Projektteam</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt-Tracking]</td> 
   <td>Die Daten, mit denen Status und Umfang eines Projekts gemessen werden</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Ein geschätzter Zeitstempel, der angibt, wann die Arbeit abgeschlossen wird, basierend auf den geplanten Stunden und dem abgeschlossenen Prozentsatz einer Aufgabe, eines Problems oder Projekts.</p> <p>Dies bezieht sich auf Daten oder die [!UICONTROL Dauer] von Aufgaben, Problemen oder Projekten. Normalerweise kennzeichnet es Daten und Zeiträume, die dem Lebenszyklus der Arbeitselemente eher entsprechen, nachdem einige Arbeiten bereits abgeschlossen wurden oder einige Zeit vergangen ist. </p> <p>Beispielsweise ist das [!UICONTROL Projected Completion Date] (Voraussichtliches Abschlussdatum) einer Aufgabe das Datum, an dem [!DNL Workfront] schätzt, dass die Aufgabe abgeschlossen sein wird. Es basiert darauf, wie viel Arbeit bisher daran geleistet wurde, wie viele Personen ihr zugewiesen sind und wie viel Zeit seit dem Startdatum vergangen ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frist für Korrekturabzug]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. einen Bericht [!UICONTROL Document Version] und einen Bericht [!UICONTROL Korrekturabzugsgenehmigung]), zeigt dieses Feld den Wochentag, das Datum, die Tageszeit und das Jahr der Korrekturabzugsfrist an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. ein Bericht [!UICONTROL Document Version])  und [!UICONTROL Korrekturabzug-Genehmigung]), zeigt dieses Feld den Entscheidungsstatus des Korrekturabzugs an (ausstehend, Änderungen erforderlich oder genehmigt)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzug-Name]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. einem Bericht [!UICONTROL Document Version] und einem Bericht [!UICONTROL Proof Approval]), zeigt dieses Feld den Namen des Korrekturabzugs an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugseiten]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. einem Bericht [!UICONTROL Document Version] und einem Bericht [!UICONTROL Korrekturabzug-Genehmigung]), zeigt dieses Feld die Anzahl der im Korrekturabzug enthaltenen Seiten an.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-Fortschritt]</td> 
   <td> <p>In Berichten, die das Objekt [!UICONTROL Document Version] enthalten (z. B. einen Bericht [!UICONTROL Document Version] und einen Bericht [!UICONTROL Proof Approval]), zeigt den Fortschrittsstatus des Korrekturabzugs an ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Übersicht über den Korrekturabzug</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Übersicht über den Korrekturabzug und den Status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Ein Überprüfungsprozess, bei dem ein oder mehrere Benutzer Inhalte markieren und kommentieren, die in einem Bild, einem Textdokument, einem Video oder interaktiven Web-Inhalten geändert werden sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Öffentlich]</td> 
   <td>In einem [!UICONTROL Hinweis] oder [!UICONTROL Dokument] macht diese Option dieses Objekt anderen Benutzern oder sogar Personen von außerhalb [!DNL Workfront] zugänglich. Für eine [!UICONTROL Warteschlange für Hilfeanfragen] bedeutet [!UICONTROL Public], dass alle Benutzer, die Probleme an ein Projekt senden können, Probleme über den Bereich [!UICONTROL Anfragen] senden können.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL-Qualität]</td> 
   <td>Die Wahrnehmung der Arbeitsqualität innerhalb der Organisation.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlange]</td> 
   <td>Wird auch als Helpdesk-Warteschlange oder [!UICONTROL Warteschlange für Hilfeanfragen] bezeichnet. Dies ist ein Projekt, das im Bereich [!UICONTROL Anfragen] veröffentlicht wurde, um Benutzern zu ermöglichen, Probleme an es zu senden. Normalerweise werden Warteschlangen für bestimmte Themen wie [!UICONTROL Bugs], [!UICONTROL Project Requests] usw. erstellt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlangeneigenschaften]</td> 
   <td>Diese Einstellungen definieren Problemübermittlungsregeln für ein Projekt, das im Bereich [!UICONTROL Anfragen] veröffentlicht wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Warteschlangenthema]</td> 
   <td> <p>Eine Eigenschaft in einer [!UICONTROL Warteschlange für Hilfeanfragen], mit der Benutzer, die ein Problem einreichen, ein Thema auswählen können. Themen können:</p> 
    <ul> 
     <li>Mit einem benutzerdefinierten Datenformular verknüpft sein.</li> 
     <li>Weisen Sie das Problem automatisch einem Benutzer, einer Rolle oder einem Team über den Routing-Regelsatz für das ausgewählte Thema zu.</li> 
     <li>Verschieben Sie das Problem über den für das ausgewählte Thema festgelegten Routingregel in ein anderes Projekt oder eine andere Warteschlange.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Warteschlangenthemen erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In einem Bericht der [!UICONTROL Zugriffsebene] können Sie manuell einen [!UICONTROL-Rang] der [!UICONTROL-Zugriffsebene] angeben. Auf diese Weise können Sie als [!DNL Workfront]-Admin den mit den einzelnen Zugriffsebenen verbundenen Komplexitätsgrad visuell erkennen. Beispielsweise können Sie niedrigere Zahlen für komplexere Zugriffsebenen ([!UICONTROL Plan]-Ebene) und höhere Zahlen für weniger komplexe Zugriffsebenen ([!UICONTROL Anforderer]-Ebene) angeben. Sie können die standardmäßigen Zugriffsebenen nicht nach Rang ordnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL bereit]</td> 
   <td> <p>Dieses Feld in einem Aufgabenbericht gibt an, ob eine [!UICONTROL Agile]-Aufgabe im Rückstand als [!UICONTROL Ready] markiert wurde. Dieses Flag gilt nur für [!UICONTROL Agile]-Aufgaben, bei denen es sich um Aufgaben handelt, die einem [!UICONTROL Agile]-Team zugewiesen sind. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL-Eintrag]</td> 
   <td> <p>In Workfront Planning ist ein Datensatz eine eindeutige Instanz eines Datensatztyps.</p>
<p>Nachdem Sie einem Arbeitsbereich einen Datensatztyp hinzugefügt haben, können Sie damit beginnen, Datensätze dieses Typs auf der Seite des Datensatztyps hinzuzufügen.</p>
<p>Beispiel: „Kampagne“ kann ein Datensatztyp sein und „Sommerkampagne für EMEA“ ist ein Datensatz des Datensatztyps der Kampagne.</p>
<p>Weitere Informationen zum Erstellen von Datensätzen finden Sie unter <a href="/help/quicksilver/planning/records/create-records.md">Erstellen von Datensätzen</a>. </p> <p>Workfront Planning benötigt eine zusätzliche Lizenz. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Datensatztyp]</td> 
   <td> <p>Der Objekttyp von Workfront Planning.</p>
<p>Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in Workfront Planning eigene Objekttypen erstellen. Workfront Planning-Objekttypen werden als Datensatztypen bezeichnet.</p>
<p>In Workfront werden beispielsweise die Objekttypen „Programm“, "Portfolio", „Projekt“, „Aufgabe“ oder „Problem“ bereits erstellt.</p>
<p>In Workfront Planning können Sie beliebige Datensatztypen erstellen, die den Workflows Ihres Unternehmens entsprechen. Später können Sie definieren, wie die Datensatztypen miteinander oder mit Formularabhängigkeiten in Beziehung stehen.</p> Weitere Informationen zum Erstellen von Datensatztypen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-record-types.md">Erstellen von Datensatztypen</a>. </p> <p>Workfront Planning benötigt eine zusätzliche Lizenz. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Wiederholungsfrequenz]</td> 
   <td> <p>Ein Feld, das im Feld [!UICONTROL Aufgabendetails] oder [!UICONTROL Aufgabe bearbeiten] eines übergeordneten Elements wiederkehrender Aufgaben angezeigt wird. Dies ist die Häufigkeit, mit der die Aufgaben in der Wiederholung auftreten. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Referenznummer]</td> 
   <td> <p>Projekte, Aufgaben und Probleme werden beim Erstellen automatisch mit einer eindeutigen Referenznummer verknüpft. Sie können die [!UICONTROL-Referenznummer] auf der Seite [!UICONTROL-Details] der Projekte, Aufgaben oder Probleme oder in einer Liste oder einem Bericht einsehen. </p> <p><b>TIPP</b><p><br>Sie können Referenznummern verwenden, wenn zwei Elemente denselben Namen haben, da Referenznummern immer eindeutig sind. </p> <p>[!DNL Workfront] generiert automatisch sequenzielle Referenznummern auf Systemebene. Jedes Projekt, jede Aufgabe oder jedes Problem erhält die nächste verfügbare Zahl in der Sequenz. <br></p> <p>Wenn beispielsweise Benutzer A eine Aufgabe erstellt, können [!DNL Workfront] der Aufgabe automatisch die Referenznummer 100 zuweisen. Wenn Benutzer B unmittelbar danach ein Problem erstellt, weist [!DNL Workfront] dem Problem die Referenznummer 101 zu. Referenznummern können nicht manuell bearbeitet werden. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ablehnungsproblem]</td> 
   <td>In einem Projekt- oder Aufgabenbericht ist dies das Problem, das erstellt wird, wenn die Genehmigung für das Projekt oder die Aufgabe abgelehnt wird. Informationen zu Ablehnungsproblemen finden Sie im Artikel <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>. </td> 
  </tr>

<tr>
  <td>Beziehungstypen</td>
  <td><p>Workfront-Objekte werden immer über einen der folgenden Beziehungstypen miteinander verbunden:</p>

<ul><li> <b>Eins zu viele</b>: In dieser Beziehung kann ein Objekt mit mehreren anderen Objekten unterschiedlichen Typs verbunden werden. Beispielsweise kann ein Projekt mehrere Aufgaben haben. Die Beziehung zwischen Projekt und Aufgaben ist eine Eins-zu-viele-Beziehung. Sie können diese Beziehung nicht in einem Bericht über die Standardschnittstelle anzeigen. Sie müssen den Textmodus-Reporting verwenden, um 1:n-Beziehungen anzuzeigen.</li>
  <li><b>Eins-zu</b>: In dieser Beziehung kann ein Objekt nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise kann ein Projekt nur über eine Gruppe verfügen. Die Beziehung zwischen Projekt und Gruppe ist eine Eins-zu-eins-Beziehung. Sie können 1:1-Beziehungen zwischen Objekten in einem Standardbericht anzeigen.</li>
  <li><b>Viele zu eins</b>: In dieser Beziehung können mehrere Objekte nur mit einem anderen Objekt eines anderen Typs verbunden werden. Beispielsweise können mehrere Aufgaben mit demselben Projekt verbunden werden. Die Beziehung zwischen Aufgaben und Projekt ist eine Viele-zu-Eins-Beziehung. Sie können in einem Standardbericht viele zu 1-Beziehungen zwischen Objekten anzeigen. </li>
  <li><b>Viele zu viele</b>: In dieser Beziehung können mehrere Objekte desselben Typs mit mehreren Objekten eines anderen Typs verbunden werden. Beispielsweise können mehrere Benutzende mehreren „Andere Teams“ und die Teams mehreren Benutzenden angehören. Sie können diese Beziehung nicht in einem Bericht über die Standardschnittstelle anzeigen. Sie müssen den Textmodus-Reporting verwenden, um viele bis viele Beziehungen anzuzeigen. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Verbleibende Risikokosten]</td> 
   <td> <p>Ein Projektfeld, das die Differenz zwischen den [!UICONTROL Geplante Risikokosten] eines Projekts und der Summe aller [!UICONTROL Ist-Kosten] aller Risiken im Projekt anzeigt. </p> <p>Die [!UICONTROL Verbleibende Risikokosten] für ein Projekt werden anhand der folgenden Formel berechnet:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Neuplanung]</td> 
   <td>Ändern der Termine eines Projekts zur Behebung oder Behebung von Problemen. Beispielsweise müsste ein Projekt, das mehrere Monate zurückgestellt wurde, neu geplant werden, um genaue Termine widerzuspiegeln. Hierbei handelt es sich um einen manuellen Vorgang, bei dem Sie entweder die Daten des Projekts oder die der Aufgaben anpassen. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Bericht]</td> 
   <td>Ein Diagramm oder eine Tabelle, das bzw. die Informationen zu einem bestimmten [!DNL Workfront] und seinen zugehörigen Attributen enthält.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL-Anfrage]</td> 
   <td> <p>Eine Art von Problem, das in einer einzigen zentralisierten Warteschlange ausgelöst wird und nicht mit einem laufenden Arbeitsaufwand in Zusammenhang steht.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Anfrage-Warteschlange]</td> 
   <td>Der Rückstand an Problemen, der von einem Traffic- und Triage-Prozess verwaltet wird.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anforderungsgeschwindigkeit]</td> 
   <td>Gesamtarbeitszykluszeit für die Aufnahme und den Abschluss einer Anfrage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anforderer]</td> 
   <td>In der Regel ein Lizenztyp. Ein Benutzer mit der Lizenz Anforderer kann Anfragen für neue Arbeiten im System senden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reservierte Zeit]</td> 
   <td>Tage, die für die persönliche Zeit eines Benutzers angegeben werden, was bedeutet, dass der Benutzer nicht für Arbeiten zur Verfügung steht. Siehe "[!UICONTROL arbeitsfreie Tage]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problem lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Problem zu verweisen, das das Problem löst. </p> <p>Informationen zum Anzeigen auflösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen auflösbarer und auflösender Objektinformationen in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projekt auflösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf das Projekt zu verweisen, das das Problem löst. </p> <p>Informationen zum Anzeigen auflösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen auflösbarer und auflösender Objektinformationen in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabe lösen]</td> 
   <td> <p>Verwenden Sie in einem Problembericht dieses Feld in Ansichten oder Filtern, um auf die Aufgabe zu verweisen, die das Problem löst. </p> <p>Informationen zum Anzeigen auflösender Objekte in Berichten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Anzeigen auflösbarer und auflösender Objektinformationen in einem Bericht</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über auflösende und auflösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ressource]</td> 
   <td>Benutzer oder Rollen, die in [!DNL Workfront] vorhanden und Projekt-Teams, Aufgaben und Problemen zugewiesen sind. Sie sind für den Abschluss der Arbeiten im Zusammenhang mit Projekten, Aufgaben oder Problemen verantwortlich. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Ressourcenverwaltung]</td> 
   <td> <p>[!UICONTROL Resource Management] ist ein Tool-Set für Unternehmen, mit dem Sie die Nutzung Ihrer Ressourcen auf der Grundlage ihrer Verfügbarkeit genau vorhersagen können, sodass die erforderlichen Arbeiten termingerecht und im Budget abgeschlossen werden. </p> <p>Mit Tools für das Ressourcen-Management können Sie die langfristige Kapazität und den kurzfristigen Planungsbedarf für Ihre Ressourcen planen. </p> <p>Informationen zum Ressourcen-Management in [!DNL Workfront] finden Sie <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Erste Schritte mit dem Ressourcen-Management</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenmanager-IDs]</td> 
   <td><p>In einem Projektbericht können Sie diese Option beim Erstellen eines Filters verwenden, um einen bestimmten Ressourcen-Manager zu finden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenmanager]</td> 
   <td> <p>In einem Projektbericht oder einer Listenansicht ist dies ein Informationsfeld, das Benutzende anzeigt, die für die Durchführung von Ressourcenverwaltungsaktivitäten für das Projekt vorgesehen sind.  Wenn Sie "[!UICONTROL Resource Manager]" in einem Bericht verwenden, wird eine Liste der Ressourcen-Manager angezeigt, wobei jeder Ressourcen-Manager des Projekts durch ein Komma getrennt ist. Sie können bis zu 30 Ressourcenmanager für ein bestimmtes Projekt bestimmen.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Ressourcenmanager für ein Projekt oder eine </a> bestimmen“.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Ressourcenplaner - budgetierte Stunden] </td> 
   <td>Die budgetierten Stunden für das Projekt und die damit verbundenen Ressourcen im [!UICONTROL Resource Planner]. Siehe auch "[!UICONTROL Budgetierte Stunden]" in diesem Artikel. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Ressourcenplaner] </td> 
   <td>Ein erweitertes [!DNL Workfront]-Tool, mit dem Sie Ressourcen projektübergreifend, für Aufgabengebiete oder für Benutzende anzeigen und verwalten können. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Ressourcenplaner - Übersicht</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenplaner budgetierte Lohnkosten]</td> 
   <td> <p>Dies sind die Kosten, die mit den Stunden verknüpft sind, die mithilfe des Ressourcenplaners für Projektrollen budgetiert wurden. </p> <p>Siehe auch „Budgetierte Lohnkosten“ in diesem Artikel. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenpools]</td> 
   <td> <p>Ressourcenpools sind Sammlungen von Benutzern, die mit einem Projekt verknüpft werden können. Die Benutzer im selben Ressourcenpool gehören normalerweise derselben Abteilung an, verfügen über ähnliche oder komplementäre Fähigkeiten oder werden aus demselben Budget finanziert. Sie können mehrere Ressourcenpools mit einem Projekt oder einem Benutzer verknüpfen. Ein Ressourcenpool kann ausschließlich einem Projekt zugewiesen oder von mehreren Projekten gemeinsam genutzt werden.</p> 
   <p>Weitere Informationen zu Ressourcenpools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Ressourcenpools - Übersicht </a>.</p> 
   <p>In Projektberichten zeigen Ressourcenpools alle Pools an, die mit einem Projekt verknüpft sind. Dieses Objekt kann nicht in einer Gruppierung verwendet werden.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ressourcenauslastung]</td> 
   <td>Ein Bericht, der die Anzahl der in einem bestimmten Zeitraum verfügbaren Stunden und die für jeden Benutzer im Bericht geplante Anzahl der Stunden ausgibt. Dies wird auch in [!UICONTROL Durchschnittliche Stunden pro Tag] und einen Zuordnungsprozentsatz berechnet.</td> 
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
   <td>[!UICONTROL Umsatztyp]</td> 
   <td>Der Umsatztyp bestimmt, wie der Aufgabe Einnahmen zufließen. Einige Beispiele sind [!UICONTROL Fester Wert pro Stunde], [!UICONTROL Role pro Stunde] und [!UICONTROL Role pro Stunde mit Begrenzung]. Informationen zur Umsatzverfolgung in [!DNL Workfront] finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>In der Regel ein Lizenztyp. Ein Benutzer mit einer [!UICONTROL Reviewer]-Lizenz kann Arbeitselemente im System überprüfen und genehmigen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risiko]</td> 
   <td> <p>Dies kann sich auf die folgenden Konzepte in [!DNL Workfront] beziehen:</p> 
    <ul> 
     <li> <p>Ein Feld in einem Projekt, das anzeigt, wie riskant ein Projekt sein kann. Sie können die Ausführung Ihrer Projekte nach dem Risikoniveau priorisieren. Projekte können die folgenden Risikostufen aufweisen:</p> <p>- [!UICONTROL Sehr niedrig]</p> <p>- [!UICONTROL Niedrig]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL hoch]</p> <p>- [!UICONTROL Sehr hoch]</p> <p>Die von Ihnen für ein Projekt angegebenen Risikostufen können nicht angepasst werden. </p> <p> Informationen zum Aktualisieren des Risikos eines Projekts finden Sie im Abschnitt „Projekteinstellungen“ des Artikels <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>. Sie können das Risikofeld eines Projekts in Berichten anzeigen. </p> </li> 
     <li> <p>Ein Ereignis, das während der Laufzeit eines Projekts auftreten kann und potenzielle Auswirkungen auf die Kosten, den Umfang oder den Zeitplan des Projekts identifiziert. Sie definieren potenzielle Risiken für ein Projekt und verknüpfen die Wahrscheinlichkeit ihres Auftretens oder die Kosten, während Sie den Business Case des Projekts erstellen. Informationen zum Hinzufügen von Risiken zum Business-Case des Projekts finden Sie unter „Erstellen und Bearbeiten von Risiken in Projekten“. </p> <p>Sie können die im [!UICONTROL Business Case] definierten Risiken nicht in Berichten anzeigen. Sie können nur verschiedene Arten von Risikokosten in Berichten und Listen anzeigen. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risikokosten]</td> 
   <td> <p>Die mit den Risiken eines Projekts verbundenen Kosten. Im Folgenden finden Sie Risikokosten im Zusammenhang mit Projekten, die Sie in Berichten anzeigen können:</p> 
    <ul> 
     <li> <p>[!UICONTROL Istkosten]: Ein Feld für ein Risiko, das die tatsächlichen Kosten für das eingetretene Risiko anzeigt. Zusätzlich zu Berichten und Listen können Sie es beim Bearbeiten oder Erstellen eines Risikos im Feld [!UICONTROL Risiko bearbeiten] suchen. </p> <p>Informationen zu Projekt-, Aufgaben- oder Problemkosten finden Sie unter "[!UICONTROL Istkosten]" in diesem Artikel. </p> </li> 
     <li> <p>[!UICONTROL Geplante Risikokosten]: Ein Feld im Projekt, das die Summe aller [!UICONTROL Potenziellen Risikokosten] für das Projekt anzeigt. Siehe auch "[!UICONTROL Geplante Risikokosten]" in diesem Artikel. </p> <p>Informationen zu potenziellen Risikokosten finden Sie unter <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Berechnung potenzieller Risikokosten </a>. </p> </li> 
     <li> <p>[!UICONTROL Verbleibende Risikokosten]: Ein Feld im Projekt, das die Differenz zwischen der Summe der [!UICONTROL Istkosten] aller Risiken und den [!UICONTROL geplanten Risikokosten] anzeigt. Siehe auch „Verbleibende Risikokosten“ in diesem Artikel. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risikomanagement]</td> 
   <td>Prozesse zur Identifizierung, Minderung und Überwachung von Risiken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Siehe "[!UICONTROL Aufgabengebiet]" in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Automatisches Zuweisen oder Verschieben eines Problems, normalerweise aufgrund eines Warteschlangenthemas oder als Standardroute (Routing-Regel) für die Warteschlange.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Routingregel]</td> 
   <td>Eine Einstellung für Projekte und Warteschlangenthemen, mit der ein Problem automatisch einem Benutzer, einer Rolle oder einem Team zugewiesen oder in ein anderes Projekt oder Warteschlangenthema verschoben wird. Routing-Regeln werden im Allgemeinen mit Warteschlangen für Hilfeanfragen verwendet, um eingehende Probleme automatisch zuzuweisen.</td> 
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
   <td>[!UICONTROL Gespeicherte Suche]</td> 
   <td>Eine Suche, für die die Suchkriterien gespeichert wurden. Gespeicherte Suchen erleichtern die Ausführung derselben Suchvorgänge, ohne dass die Suchkriterien erneut eingegeben werden müssen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Ein Szenario besteht aus einer Reihe von Schritten (Modulen), die angeben, wie Daten zwischen Apps/Services übertragen und transformiert werden sollen.</p> <p>Informationen zu Szenarien in [!DNL Workfront Fusion] finden Sie unter Übersicht über <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion] Szenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (im [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Im [!DNL Scenario Planner] ist ein Szenario eine Kopie eines Plans. </p> <p>Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Die [!DNL Scenario Planner] - Übersicht</a>. </p> <p>Informationen zum Erstellen von Szenarien finden Sie unter <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Erstellen und Vergleichen von Planszenarien in der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitplan]</td> 
   <td>Der wöchentliche Arbeitszeitplan, einschließlich Arbeitszeiten, kombiniert mit Urlaubstagen (z. B. Feiertage) und Ausnahmetagen (z. B. Samstags-Arbeitstag). Sie können Zeitpläne mit Projekten und Benutzern verknüpfen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitplan-Ausnahme]</td> 
   <td>Wird auch als [!UICONTROL Modified Shift] bezeichnet. Tage im Gegensatz zu den regulären Wochenarbeitszeiten, wie durch den Zeitplan definiert. Ein Samstag, der für die Arbeit geplant ist, wenn der Zeitplan so eingerichtet ist, dass er nur von Montag bis Freitag funktioniert, wäre beispielsweise eine [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Geplanter Bericht]</td> 
   <td> <p>Wenn Sie einen Bericht mit Berichten erstellen, können Sie Informationen zu den Zeitplänen des Berichts anzeigen, wenn der Bericht für die Bereitstellung mithilfe des Felds [!UICONTROL Geplanter Bericht] geplant ist. Dieses Feld zeigt in einer Aufzählungsliste mehrere Werte an, einen für jeden Zeitplan jedes Berichts. Weitere Informationen zur Planung von Berichten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Übersicht über die Berichtbereitstellung</a>.</p> <p>Da dieses Feld mehrere Werte aufweist, kann es nicht in einer Gruppierung verwendet werden. Der Zugriff ist nur über einen Filter oder eine Ansicht möglich. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Umfangsänderung]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll], das, falls aktiv, bei jeder Änderung am Umfang eines Projekts oder einer Aufgabe eine Notiz erzeugt, z. B. wenn eine [!UICONTROL Task Duration] oder die [!UICONTROL Vorgänger] geändert werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Abschnitt]</td> 
   <td>Ein Bereich auf dem Bildschirm mit einer eigenen Kopfzeile, der erstellt wurde, um die benutzerdefinierten Daten für Anzeigezwecke zu organisieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abschnittsumbruch]</td> 
   <td>Eine Lücke oder ein Rand zwischen Abschnitten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sicherheit]</td> 
   <td>Die Einstellungen, die es einem Benutzer ermöglichen, mit bestimmten Objekten im System zu interagieren und nicht mit anderen. Siehe auch "[!UICONTROL Zugriffsebenen]" in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Der Bereich, in dem Administratoren Systemkonfigurationen und -einstellungen einrichten können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schweregrad]</td> 
   <td> <p>[!UICONTROL Severity] ist ein Hinweis darauf, wie wahrscheinlich es ist, dass ein Element die Fertigstellung der Arbeit beeinträchtigt. Beispielsweise kann ein Problem mit hohem [!UICONTROL Severity] den Abschluss einer Aufgabe vollständig blockieren, aber ein Problem mit niedrigem [!UICONTROL Severity] kann nur kosmetischer Natur sein.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> des Problemschweregrads </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schweregrade]</td> 
   <td>Siehe "[!UICONTROL Severity]" in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Freigabe]</td> 
   <td>Aktion, bei der es anderen Benutzern erlaubt wird, ein bestimmtes Element in [!DNL Workfront] anzuzeigen oder zu bearbeiten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack-Datum]</td> 
   <td>In einer Aufgabenansicht oder einem Bericht zeigt [!UICONTROL Slack Date] das exakte Datum an, an dem sich eine Aufgabe definitiv auf das [!UICONTROL Abschlussdatum] des Projekts auswirken könnte. Informationen über das [!UICONTROL Slack-Datum] einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Übersicht über das Task-Slack-Datum</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Beim Zuweisen von Aufgaben oder Problemen zu Benutzern gibt [!DNL Workfront] Empfehlungen ([!UICONTROL Smart Assignments]) dazu, wer die besten Benutzer sind, um die Arbeit abzuschließen. Diese Empfehlungen beziehen sich auf die Zeit, die ihnen für die Fertigstellung zur Verfügung steht, und auf ihre Beziehung zum Projekt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Smart Assignments - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Gibt das übergeordnete Objekt eines anderen Objekts an. Beispiel: Ein an eine Aufgabe angehängtes Dokument hat den Namen der Aufgabe im Feld [!UICONTROL Source] eines Berichts oder einer Ansicht von [!UICONTROL Document]. Ein unter einem Projekt protokolliertes Problem hat den Namen des Projekts im Feld [!UICONTROL Source] eines Problemberichts oder einer Ansicht. </p> 
   <p>Die folgenden Berichte zeigen eine Source-Spalte an, in der Sie Informationen zum übergeordneten Objekt anzeigen können:</p>
  <ul><li>Problemberichte</li>
    <li>Stundenberichte</li>
    <li>Dokumentieren von Berichten </li>
    </ul>
   <p>Wenn Benutzende keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, wird die Source-Spalte des Berichts leer angezeigt, selbst wenn der Bericht so konfiguriert ist, dass er angezeigt wird oder mit den Zugriffsrechten eines anderen Benutzers bereitgestellt werden soll. </p>
   <p> Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, empfehlen wir, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der Sie den Namen des übergeordneten Objekts anzeigen können. </p>
    <p>Sie können beispielsweise einen der folgenden Punkte zu einem Bericht mit einer Source-Spalte hinzufügen: </p>
    <ul><li>Die Spalten „Projektname“, „Aufgabenname“ oder „Problemname“ für ein Dokument oder einen Stundenbericht.</li>
    <li>Die Spalten „Projektname“ oder „Aufgabenname“ für einen Problembericht. </li> </ul>
    Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p>Das Datum, an dem die Arbeit an einem Element beginnen soll. In [!DNL Workfront] gibt es mehrere Startdaten: </p> 
    <ul> 
     <li>[!UICONTROL geplant]</li> 
     <li>[!UICONTROL Tatsächlich]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>In einem [!UICONTROL Rate-Bericht] ist dies das Datum, an dem ein neuer Abrechnungssatz für ein Aufgabengebiet auf Projektebene beginnt. Die mit dem Projekt verknüpften Stunden nach diesem Datum werden mit diesem Abrechnungssatz multipliziert, um den Projektumsatz zu berechnen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Ein Indikator, der eine Workflow-Position eines Arbeitselements oder eines strategischen Ziels signalisiert.</p> <p>Bei Projekten ist der [!UICONTROL Status] eine Einstellung des Projekts, die angibt, ob das Projekt:</p> 
    <ul> 
     <li>[!UICONTROL Aktuell]</li> 
     <li>[!UICONTROL im Halten] </li> 
     <li>[!UICONTROL abgeschlossen] </li> 
     <li>[!UICONTROL eingestellt]</li> 
    </ul> <p>Weitere Informationen zum Projektstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Zugriff auf die Liste der Systemprojektstatus</a>.</p>
    <p>Bei Aufgaben ist der [!UICONTROL Status] eine Einstellung der Aufgabe, die angibt, ob die Aufgabe:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL wird ausgeführt]</li> 
     <li>[!UICONTROL abgeschlossen]</li> 
    </ul> <p>Weitere Informationen zum Aufgabenstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Zugriff auf die Liste der Systemaufgabenstatus</a></p> <p>Bei Problemen ist der [!UICONTROL Status] eine Einstellung zum Problem, die angibt, ob dieses Problem:</p> 
    <ul> 
     <li>[!UICONTROL Neu]</li> 
     <li>[!UICONTROL wird ausgeführt]</li> 
     <li>[!UICONTROL wartet auf Feedback]</li> 
     <li>[!UICONTROL im Halten]</li> 
     <li>[!UICONTROL aufgelöst]</li> 
     <li>[!UICONTROL wird nicht aufgelöst]</li> 
     <li>[!UICONTROL kann nicht duplizieren]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL erneut geöffnet]</li> 
    </ul> <p>Weitere Informationen zum Problemstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemanfragestatus</a>.</p> 
    <p>Bei strategischen Zielen ist der [!UICONTROL Status] eine Einstellung für das Ziel, die angibt, ob das Ziel:</p> 
     <ul> 
      <li>[!UICONTROL aktiv]</li> 
      <li>[!UICONTROL-Entwurf]</li> 
      <li>[!UICONTROL inaktiv]</li> 
      <li>[!UICONTROL geschlossen]</li> 
     </ul> 
     <p>Weitere Informationen zu strategischen Zielen finden Sie auch unter "[!UICONTROL Goal]" oder "[!UICONTROL Goals]" in diesem Artikel. </p> 
     <p>Für strategische Ziele ist dieses Feld nur sichtbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Informationen zum Verwalten strategischer Ziele mithilfe von [!DNL Workfront Goals] finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] - Übersicht</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusänderung]</td> 
   <td>Ein [!UICONTROL Audit-Protokoll]. Eine Notiz wird erzeugt, wenn ein Benutzer den Status des Projekts, der Aufgabe oder des Problems ändert.</td> 
  </tr> 
  <tr> 
   <td>Status-Symbole</td> 
   <td> <p>Sie können das integrierte Feld [!UICONTROL Status Icons] als Spalte in Ihren Ansichten hinzufügen, um die Sichtbarkeit Ihrer wichtigsten Punkte zu verbessern, z. B.:</p> 
    <ul> 
     <li>An ein Objekt sind Dokumente angehängt</li> 
     <li>Ein Objekt ist mit einem Genehmigungsprozess verknüpft</li> 
     <li>Einem Objekt sind zusätzliche Notizen zugeordnet</li> 
     <li>Kosten sind fakturierbar oder erstattungsfähig </li> 
     <li>Eine Aufgabe befindet sich auf einem kritischen Weg</li> 
     <li>Ein Benutzer gehört zu einem Unternehmen, einem Team oder befindet sich in einer anderen Zeitzone </li> 
    </ul> <p>Sie können das Feld [!UICONTROL Status Icons] in den Ansichten der folgenden Objekte hinzufügen: </p> 
    <ul> 
     <li>[!UICONTROL Aufgaben]</li> 
     <li>[!UICONTROL Probleme]</li> 
     <li>[!UICONTROL-Projekte]</li> 
     <li>[!UICONTROL Vorlagenaufgaben]</li> 
     <li>[!UICONTROL-Vorlagen]</li> 
     <li>[!UICONTROL Ausgaben]</li> 
     <li>[!UICONTROL-Dokumente]</li> 
     <li>[!UICONTROL Benutzer]</li> 
    </ul> <p>Weitere Informationen finden Sie <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statusaktualisierung]</td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht zeigt dieses Feld die neueste Statusaktualisierung an, die Objektbesitzer im Bereich '[!UICONTROL Updates]' bereitgestellt haben. Bei Projekten bedeutet dies, dass die Kommentare des Projektbesitzers sowie bei Aufgaben und Problemen die Kommentare der Beauftragten sind.</p> 
   <p> Kommentare, die beim Aktualisieren des Status eines Objekts gemacht werden, werden nicht in der Spalte [!UICONTROL Status Update] angezeigt.</p> <p>Um den Status [!UICONTROL New],' '[!UICONTROL In Process]' und '[!UICONTROL Complete]' anzuzeigen, verwenden Sie die Spalte [!UICONTROL Status].</p> <p>Weitere Informationen zum Status finden Sie im Artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aufgabenstatus aktualisieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Status]</td> 
   <td>Siehe "[!UICONTROL Status]" in diesem Artikel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Ein Diagramm, das den Status von Storys (Aufgaben in der agilen Methodik) und ihren Fortschritt hin zum Abschluss darstellt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Eine Metrik zum Messen der Schwierigkeit oder Komplexität einer Story. Agile-Teams können wählen, ob sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Eine Metrik zum Messen der Schwierigkeit oder Komplexität einer Story. Agile-Teams können wählen, ob sie Stunden oder Punkte verwenden möchten.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategisch]</td> 
   <td>Langfristige Arbeit, die die Organisation oder die Funktionsweise der Organisation ändert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategische Ausrichtung]</td> 
   <td>Unternehmensziele über Portfolios und Programme hinweg messen und ausrichten.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Dies wird bei Verwendung der Textmodus-Oberfläche in Berichtsspalten verwendet. </p>
   <p>Mit dem <code>[!UICONTROL stretch]</code> wird ermittelt, welche Spalten zusätzlichen Platz belegen, der für die Ansicht nicht benötigt wird. Die Breite der Benutzeroberfläche des Arbeitsbereichs beträgt für einen typischen Benutzer etwa 850 Pixel. Das heißt, wenn man eine Aussicht mit vier hat
   Spalten (jeweils 150 Pixel), die Ihre Ansicht belegt 600 von 850 Pixel. Die Benutzeroberfläche von enthält 250 zusätzliche Pixel, die den Spalten hinzugefügt werden, für die ein Dehnungsprozentsatz angegeben ist. </p>
   <p>Die Ausdehnung einer Spalte wird erzwungen, wenn Sie die zusätzliche Codezeile verwenden: <code>[!UICONTROL usewidths=true]</code> für mindestens eine der Spalten in der Ansicht. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Abonnentinnen und Abonnenten]</td> 
   <td> <p>Benutzer, die Projekte, Aufgaben oder Probleme abonnieren.</p> <p>Wenn Sie dieses Feld in einem Bericht verwenden, wird eine Liste von Abonnenten angezeigt, wobei jeder Abonnent durch ein Komma getrennt ist.</p> <p>Weitere Informationen finden Sie im Artikel <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonnieren von Elementen in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Übersichtsaufgabe]</td> 
   <td>Siehe "[!UICONTROL Parent Task]" in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teilaufgabe]</td> 
   <td>Eine untergeordnete Aufgabe, die sich unter einer übergeordneten Aufgabe befindet.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Ein Satz von Richtlinien, der Änderungen und die Wartung eines Systems steuert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Systemintegration]</td> 
   <td>Der Prozess der Verbindung verschiedener Computersysteme und Softwareanwendungen physisch oder funktional, um als ein koordiniertes Ganzes zu fungieren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabe]</td> 
   <td> <p>Eine Aktivität, die als Schritt zum Erreichen eines endgültigen Ziels (Abschluss des Projekts) ausgeführt werden muss.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Aufgaben - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabenattribut]</td> 
   <td>Andere Felder oder Objekte, die mit einer Aufgabe verknüpft sind und bestimmte Details über die Aufgabe angeben. Einige Beispiele sind [!UICONTROL Geplantes Abschlussdatum] und [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufgabenbeschränkung]</td> 
   <td>Siehe "[!UICONTROL constraint type]" und "[!UICONTROL constraint date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabenverwaltung]</td> 
   <td>Ein Satz von Richtlinien, der die Schwellenwerte für die Erstellung, Zuweisung, Schließung und Sichtbarkeit von Aufgaben steuert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Aufgabenbesitzer]</td> 
   <td>Das Team oder der Benutzer, das bzw. der für die Schätzung des Aufwands und den Abschluss der Aufgabe verantwortlich ist</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Eine Sammlung von Benutzern, die ähnliche Ziele oder Geschäftsziele verfolgen. Diese Benutzer können gemeinsam einem Arbeitselement zugewiesen werden, indem das Team dem Arbeitselement zugewiesen wird.</p> <p>Weitere Informationen zu Teams finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams - Übersicht</a>.</p> <p>Projekte können über ein [!UICONTROL Project Team] verfügen, das alle Benutzer oder Rollen enthält, die mit der Arbeit am Projekt verknüpft sind.</p> <p>Weitere Informationen zu Projekt-Teams finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteam - Übersicht</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL-Vorlage]</td> 
   <td> <p>Projektvorlagen sind allgemeine Entwürfe Ihrer am häufigsten wiederholten Projekte. Beim Erstellen einer Projektvorlage können Sie Aufgaben, Warteschlangenthemen, benutzerdefinierte Formulare definieren, Dokumente oder Genehmigungen anhängen, um so Zeit zu sparen, die Sie beim Erstellen eines neuen Projekts benötigen. </p> <p>Sie können Vorlagen an vorhandene Projekte anhängen oder sie zum Erstellen neuer Projekte verwenden. Alle in der Vorlage angegebenen Informationen werden in die Projekte übertragen, die damit erstellt werden. </p> <p>Weitere Informationen zu Vorlagen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Übersicht über Projektvorlagen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorlagenaufgabe]</td> 
   <td>Eine Aufgabe, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, das mithilfe der Vorlage erstellt wird.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Eine [!UICONTROL Note] und ihre Sammlung von Antworten, die sich auf ein bestimmtes Thema beziehen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> In einer [!UICONTROL Document]-Liste oder einem Bericht wird eine Vorschau des Dokuments in einer Miniaturansicht angezeigt. </p> <p> Wählen Sie <strong>[!UICONTROL Thumbnail]</strong>  So zeigen Sie eine 33-66 Pixel breite Miniaturansicht im Bericht an. </p> <p>Die Größe der Miniaturansicht wird angepasst, wenn Sie die Breite der Spalte in einer Liste oder einem Bericht ändern.</p> <p>Siehe auch "[!UICONTROL Large Thumbnail]" in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausfallzeit]</td> 
   <td>Sie können einen [!UICONTROL Auszeiten]-Bericht erstellen, um anzuzeigen, wann Benutzer Auszeiten in ihrem Profil angegeben haben. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeittabelle]</td> 
   <td> <p>Eine Arbeitszeitkarte, mit der Benutzende die tatsächlichen Stunden eingeben können, die sie mit der Arbeit an Projekten, Aufgaben oder Problemen verbracht haben, oder die Stunden, die sie für andere Aktivitäten aufgewendet haben, die nicht mit der Arbeit zusammenhängen, z. B. Meetings oder Schulungen. Zusätzlich zur Eingabe der aufgewendeten Arbeitszeit können Sie auch angeben, ob die Zeit arbeitsbezogen ist oder sich auf die Gemeinzeit beläuft, indem Sie „Stundentypen“ verwenden, um Ihre Zeiteinträge zu definieren. Informationen zu Arbeitszeittabellen finden Sie unter <a href="../../../timesheets/timesheets/timesheets-overview.md">Arbeitszeittabellen - Übersicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeittabellen-Profil]</td> 
   <td> <p>Ein [!UICONTROL Arbeitszeittabellen-Profil] ist eine Vorlage, mit der [!DNL Workfront] automatisch Arbeitszeittabellen für die ihnen zugeordneten Benutzer erstellt. </p> <p>Sie können eine Reihe von Einstellungen konfigurieren, die für jede Arbeitszeittabelle beim Erstellen gelten. Einige dieser Einstellungen sind: Wie oft die Arbeitszeittabelle erstellt werden soll (wöchentlich, jede zweite Woche, zweimal im Monat oder monatlich), der Starttag der Arbeitszeittabelle, die Arbeitszeittabellen-Genehmiger, die verfügbaren [!UICONTROL Stundentypen], die Benutzende aufgezeichneten Stunden zuordnen können.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID des obersten übergeordneten Elements] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und ihren Untergruppen in einer Liste oder einem Bericht identifizieren und filtern.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name des obersten übergeordneten Elements] </td> 
   <td> <p>In diesem Feld können Sie Daten zu einer Gruppe der obersten Ebene und ihren Untergruppen in einer [!UICONTROL-Ansicht] für eine Liste oder einen Bericht identifizieren.</p> <p>Sie können dies auch mit dem Feld [!UICONTROL ID des obersten übergeordneten Elements] tun.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gesamtstunden]</td> 
   <td> <p>In einem [!UICONTROL-Projektbericht] zeigt dieses Feld die gerundete Summe aller Projektstunden an, die bei der letzten Berechnung der Projektfinanzen aufgewendet wurden. [!UICONTROL Tatsächliche Stunden] spiegeln die genauen Stunden wider, die für das Projekt protokolliert werden. In der Regel sollte die [!UICONTROL Actual Hours] mit der [!UICONTROL Total Hours] übereinstimmen. Wenn sich die Gesamtstunden von [!UICONTROL] erheblich vom Feld [!UICONTROL Tatsächliche Stunden] unterscheidet, müssen Sie die Finanzierungsdaten für das Projekt neu berechnen.</p> <p>Weitere Informationen zur Neuberechnung der Projektfinanzen finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Neuberechnen der Projektfinanzen</a>.</p> <p>In einer Arbeitszeittabellen-[!UICONTROL Standard]-Ansicht bezieht sich dieses Feld auf die Gesamtstunden, die für Elemente für die auf einer Arbeitszeittabelle angezeigten Datumsangaben protokolliert wurden. Das Feld [!UICONTROL Gesamtstunden] für Arbeitszeittabellen in dieser integrierten Ansicht verweist auf das Feld "[!UICONTROL hoursDuration]", das den Stundenunterschied zwischen dem Start- und dem Enddatum der Arbeitszeittabelle dynamisch berechnet. Auf diese Weise wird die Spalte [!UICONTROL Gesamtstunden] in Rot angezeigt, wenn der/die Benutzende mehr Zeit protokolliert als die verfügbaren Stunden im Zeitrahmen der Arbeitszeittabelle. Weitere Informationen finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Gesamtstunden auf der Arbeitszeittabelle anzeigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Überwachungsmodus]</td> 
   <td> <p>Ein Attribut einer Aufgabe. Dadurch wird festgelegt, wie und wann die voraussichtlichen Zeitpläne für eine Aufgabe aktualisiert werden. Beispiel:</p> 
    <ul> 
     <li>[!UICONTROL Benutzer Muss aktualisieren] erfordert, dass eine Aufgabe manuell aktualisiert wird. Andernfalls wird es zu [!UICONTROL Behind Schedule], dann zu [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] führt eine Aufgabe automatisch aus, wenn das Fälligkeitsdatum oder das geplante Abschlussdatum von [!UICONTROL] überschritten ist.</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Übersicht über den Aufgabenverfolgungsmodus</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL-Trigger]</td> 
   <td>Ein Ereignis, das ein Szenario startet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problemaufgabe]</td> 
   <td>Eine unvollständige Aufgabe mit der Bedingung [!UICONTROL Late], [!UICONTROL Behind Schedule] oder [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nicht zugewiesene Aufgabe]</td> 
   <td>Eine Aufgabe, die keinem Benutzer, keiner Funktion und keinem Team zugewiesen ist.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktualisierungstyp]</td> 
   <td> <p>Eine Einstellung für ein Projekt, die bestimmt, wann die voraussichtliche Zeitleiste des Projekts neu berechnet wird. Der [!UICONTROL Update Type] kann die folgenden Werte haben:</p> 
    <ul> 
     <li>[!UICONTROL Automatisch und Bei Änderung]</li> 
     <li>[!Nur UICONTROL automatisch]</li> 
     <li>[!Nur UICONTROL Manuell] </li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Auswahl des Projektaktualisierungstyps </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Benutzer]</td> 
   <td>Ein Konto, das in [!DNL Workfront] erstellt wurde, damit sich eine Person anmelden und mit dem System interagieren kann.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Benutzerdelegierung]</p> </td> 
   <td> <p>Ein berichtspflichtiges Objekt, das Ihnen Folgendes mitteilt:</p> 
    <ul> 
     <li>Welche Benutzenden haben Aufgaben-, Problem- und Projektgenehmigungen delegiert</li> 
     <li>Welche Benutzenden Aufgaben, Probleme und Projektgenehmigungen delegiert wurden</li> 
     <li>Wann diese Delegierungen beginnen und enden</li> 
    </ul> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Erstellen eines Berichts zur Benutzerdelegierung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Benutzeroberfläche]</td> 
   <td>Alle visuellen und interaktiven Aspekte der [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzeroberflächeneinstellungen]</td> 
   <td>[!UICONTROL Benutzeroberflächeneinrichtung]. [!DNL Workfront] können diese Einstellungen ändern, um Aspekte der Benutzeroberfläche anzupassen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL-Nutzung]</td> 
   <td>Die Verfügbarkeit für einen Benutzer oder eine Rolle basierend auf dem zugewiesenen Zeitplan, der PTO und der aktuellen Arbeitslast.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerauslastung]</td> 
   <td> <p>Eine Suche kombiniert mit einem Bericht, der zeigt, wie Benutzer (Ressourcen) zugewiesen oder überlastet sind. Siehe "[!UICONTROL Ressourcenauslastung]" in diesem Artikel.</p> </td> 
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
   <td>Ein Maß für die Gesamtarbeitszykluszeit (wie lange es dauert, eine Arbeit abzuschließen) und für die Häufigkeit der Arbeit in der ursprünglich festgelegten Zeit (Work-to-Commit-Verhältnis).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL-Ansicht]</td> 
   <td> <p>Ansichten beziehen sich auf ein Berichtselement, mit dem Sie die Spalten in einem Bericht oder in einer Liste von Objekten ändern können.</p> 
   <p> Ansicht bezieht sich auch auf das Recht eines Benutzers, nur Informationen zu einem Objekt anzuzeigen, je nach Zugriffsebene oder auf einer Berechtigungsfreigabeebene für dieses Objekt.</p> 
   <p>In Workfront Planning werden Datensätze auf der Seite „Datensatztyp“ in einem der folgenden Ansichtstypen angezeigt:</p>
   <ul><li>Tabelle</li>
   <li>Timeline</li>
   <li>Kalender</li></ul>
   <p>In Workfront Planning enthalten Ansichten die Filter, Gruppierungen, Sortierungen und andere Einstellungen, die auf die Datensätze auf dem Bildschirm angewendet wurden.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/views/manage-record-views.md">Verwalten von Datensatzansichten</a>.</p>   
   <p>Workfront Planning benötigt eine zusätzliche Lizenz.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Symbole anzeigen]</td> 
   <td> <p> Dies ist dasselbe Feld wie Status-Symbole, es ist jedoch nur für die folgenden Ansichten verfügbar: </p> 
    <ul> 
     <li> [!UICONTROL-Dokumente] </li> 
    </ul> <p> Weitere Informationen finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Integrierte Statussymbole in Ansichten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe letzten Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe letztes Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe letztes Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht im letzten Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe diesen Monat]</td> 
   <td> <p>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Monat angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe dieses Quartal]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Quartal angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aufrufe dieses Jahr]</td> 
   <td>In einer Berichtsliste wird angezeigt, wie oft der Bericht in diesem Jahr angezeigt wurde.<br>Weitere Informationen zu Nutzungsinformationen in Berichtslisten finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Anzeigen der Berichtsnutzung</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In einem Bericht wird bei Verwendung der [!UICONTROL Textmodus]-Schnittstelle die Codezeile verwendet, in der Sie die Breite jeder Spalte in Pixel angeben können. Workfront bietet eine empfohlene Breite für jedes Feld.
Je nach Typ des Felds und Format können Sie jedoch Anpassungen vornehmen.
Sie müssen die zusätzliche <code>[!UICONTROL usewidths=true]</code> Codezeile verwenden, um die für die Spalte angegebene Breite zu erzwingen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht werden mithilfe der folgenden Anweisung im Textmodus die geplanten Stunden des Projekts, der Aufgabe oder des Problems angezeigt:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Textmodus-Syntax</a>. </p> 
   <p><b>TIPP</b> 
   <p>Wenn Sie in einem Problembericht eines der Felder [!UICONTROL Geplante Stunden] hinzufügen, wird dem Bericht das <code>work </code>Feld "" hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeit]</td> 
   <td> <p>Einer der beiden primären Lizenztypen. Diese hat weniger Zugriff als [!UICONTROL Plan], kann jedoch Aktualisierungen im System erstellen und vornehmen. Ein Benutzer mit einer Arbeitslizenz verfügt über mehr Funktionen als ein Lizenzinhaber für [!UICONTROL External], [!UICONTROL Reviewer] oder [!UICONTROL Requester].</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] - Übersicht</a>.</p> <p>Arbeit kann sich auf die Anzahl der [!UICONTROL Geplanten Stunden] für ein Projekt, eine Aufgabe oder ein Problem beziehen. Weitere Informationen finden Sie im Feld "[!UICONTROL work]" in dieser Tabelle. </p> <p><b>TIPP</b></p> <p> Wenn Sie in einem Problembericht eines der Felder [!UICONTROL Geplante Stunden] hinzufügen, wird dem Bericht das <code>work </code>Feld "" hinzugefügt. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Struktur für Arbeitsaufschlüsselung]</td> 
   <td>Eine hierarchische Struktur der Aufgaben, die vom Projektteam basierend auf der Beziehung zwischen übergeordneter und untergeordneter Ebene ausgeführt werden sollen.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>Ein Projekt-Manager kann dieses Feld anstelle von [!UICONTROL Geplante Stunden] verwenden, um den für die Erfüllung einer Aufgabe erforderlichen Aufwand zu schätzen. Dieses Feld ist nur sichtbar, wenn die folgenden Bedingungen erfüllt sind:</p> 
     <ul> 
      <li> <p>Die Aufgabe hat einen einfachen [!UICONTROL Dauertyp]. </p> <p><b>TIPP</b></p> <p> Wenn Sie die Aufgabe [!UICONTROL Duration Type] auf einen anderen Typ aktualisieren, wird dieses Feld ausgeblendet. </p> </li> 
      <li>Der Projekt-Manager hat das Feld [!UICONTROL Work Effort verwenden] aktiviert, um die [!UICONTROL Geplante Stunden] der Aufgabe im Projekt automatisch zu berechnen. </li> 
     </ul> 
     <p>Informationen zur Verwendung von [!UICONTROL Work Effort] anstelle von [!UICONTROL Planned Hours] zur Schätzung des Aufgabenaufwands finden Sie unter <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort Overview</a>. </p> 
     <p>Dieses Feld kann in Aufgabenberichten und Listen angezeigt werden.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitselement]</td> 
   <td> <p>Dieses Feld bezieht sich auf Aufgaben oder Probleme in [!DNL Workfront]. </p> <p>Der Bericht [!UICONTROL Arbeitselement] zeigt Informationen zu Aufgaben und Problemen an. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work-Management-Mix]</td> 
   <td>Ein [!UICONTROL Work Performance Indicator] (WPI) für den Anteil der Arbeit, die Ihrem Unternehmen zugewiesen ist, im Vergleich zur Veränderung Ihres Unternehmens. Die Mix-API hilft Ihnen auf Organisationsebene zu verstehen, ob auf Ihre Strategie eine echte Arbeitszuweisung angewendet wurde.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work-Management-Ressource]</td> 
   <td>Eine Bezeichnung einer Rolle im System, die berechtigt ist, Arbeit zu erhalten oder die Zeit zu verfolgen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work-Management-Rolle und Zuständigkeiten]</td> 
   <td>Definieren der Verantwortlichen und Stakeholder für die Verwaltung des Umfangs, der Ausführung und der Genehmigungen der bezeichneten Anfrage, Aufgabe, des Projekts, Programms oder Portfolios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management SLA]</td> 
   <td>Eine quantifizierbare Metrik, auf die sich alle Interessengruppen geeinigt haben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work-Management-Stakeholder]</td> 
   <td>Eine Sammlung von Benutzern mit einem begründeten Interesse an den Ergebnissen einer Arbeitsanfrage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Touchpoints]</td> 
   <td>Digitalisierte Aufzeichnungen über die Kommunikation zwischen den Stakeholdern</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indikatoren für Arbeitsleistung] </td> 
   <td> <p>Mischverhältnis, Kapazität, Geschwindigkeit, Qualität und Interaktion.</p> <p>WPI ist ein gebräuchliches Akronym für [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Arbeitsprozess]</td> 
   <td> <p>Die Methode, in der Arbeit empfangen, priorisiert und ausgeführt wird. Die Art und Weise, wie Sie die Arbeit ausführen, wird in der Regel als „Workflow“ oder „Projektplan“ bezeichnet (eine Liste von Aufgaben mit Daten, Vorgängerbeziehungen usw.). </p> <p>Beispiele für einen Arbeitsprozess können die Produktion eines einzelnen Assets oder die Bereitstellung einer Kampagne mit mehreren Assets sein. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow-Vorlage]</td> 
   <td>Im Bericht [!UICONTROL Korrekturabzug-Genehmigung] zeigt dieses Feld alle Workflow-Vorlagen an, die an einen Korrekturabzug angehängt sind. Wenn keine Vorlagen angehängt sind, ist die Spalte leer.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>

<p>Stellt den Prozentsatz der Vollzeitäquivalenzzeit ([!UICONTROL FTE]) dar, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne Gemeinkosten. [!UICONTROL Arbeitszeit] muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.</p>
   </p>Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer seinen gesamten [!UICONTROL FTE] für die tatsächliche, projektbezogene Arbeit aufwendet.  </p>
   <p>Anhand dieser Zahl berechnet das System die Verfügbarkeit des Nutzers für die tatsächliche, projektbezogene Arbeit. </p>
   <p> Zeitplanausnahmen und Ausfallzeiten können sich auch auf die Benutzerkapazität auswirken. </p>
   <p>Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>. </p>
    <p>Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung im Bereich [!UICONTROL Setup]. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>. </p> 
   <p>Sie können die [!UICONTROL Arbeitszeit] eines Benutzers aktualisieren, wenn Sie den Benutzer bearbeiten oder erstellen. Weitere Informationen finden Sie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Bearbeiten des Benutzerprofils</a></p> 
   <b>TIPP</b> 
   <p>Legen Sie den Wert [!UICONTROL Work Time] auf 1 fest, um anzugeben, dass der Benutzer für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arbeitszeit]</td> 
   <td>In der Workfront-Dokumentation wird dieser Begriff verwendet, um die für die Arbeit aufgewendete Zeit anhand eines Zeitplans zu beschreiben.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In einem Projekt-, Aufgaben- oder Problembericht wird bei Verwendung der folgenden Anweisung im Textmodus die Anzahl der geplanten Stunden für das Projekt, die Aufgabe oder das Problem angezeigt, gefolgt vom Wort „Stunden“:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Informationen zur Verwendung des Textmodus finden Sie unter <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Übersicht über die Textmodus-Syntax</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>In Workfront Planning ist ein Workspace eine Sammlung von Datensatztypen, die den Betriebslebenszyklus eines bestimmten Unternehmens definieren. Ein Arbeitsbereich ist der Arbeitsrahmen einer Organisationseinheit.</p>
   <p>Workfront Planning benötigt eine zusätzliche Lizenz. </p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Erstellen von Arbeitsbereichen</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


