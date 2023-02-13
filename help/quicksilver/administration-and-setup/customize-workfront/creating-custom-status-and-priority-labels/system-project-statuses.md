---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Systemprojektstatus
description: Workfront verfügt über neun integrierte Systemprojektstatus. Die ersten 3 in der Tabelle unten sind erforderlich, d. h. Sie können sie entsperren, umbenennen und neu anordnen, aber nicht ausblenden oder löschen. Das Ändern des Projektstatus ist normalerweise ein manueller Prozess. Manchmal wird der Projektstatus jedoch automatisch geändert, je nach anderen Faktoren, die im System auftreten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Systemprojektstatus

Workfront verfügt über neun integrierte Systemprojektstatus.

Die ersten 3 in der Tabelle unten sind erforderlich, d. h. Sie können sie entsperren, umbenennen und neu anordnen, aber nicht ausblenden oder löschen.

Das Ändern des Projektstatus ist normalerweise ein manueller Prozess. Es gibt jedoch einige Szenarien, die in der folgenden Liste beschrieben werden, wenn der Projektstatus automatisch geändert wird, abhängig von anderen Faktoren, die im System auftreten.

Die folgenden Projektstatus werden mit Ihrer Workfront-Instanz bereitgestellt:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Systemprojektstatus</th> 
   <th>Der Projektstatus tritt auf, wenn</th> 
   <th>Was geschieht in diesem Status?</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planung (erforderlicher Status)</td> 
   <td> <p>Der Projektmanager plant den Zeitplan des Projekts, die Zuweisung der Aufgaben und die Genehmigungen. Der Projektmanager legt diesen Status für ein Projekt manuell fest.</p> <p>Tipp: Es wird empfohlen, den Standardstatus für neue Projekte in Workfront auf "Planung"festzulegen. Als Workfront-Administrator können Sie den Standardstatus für alle Ihre neuen Projekte im Bereich Projekte unter Projekteinstellungen ändern.</p> </td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig auf den Projektlisten im Projektbereich von Workfront anzeigen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsliste nicht aus. Nur Genehmigungen und akzeptierte Arbeitselemente werden in der Liste der Hausaufgaben angezeigt.</p> <p>Solange ein Projekt diesen Status aufweist, werden keine Benachrichtigungen gesendet.</p> <p>Es wird empfohlen, dass alle Änderungen, die auf eine Aktualisierung in der Zeitleiste des Projekts Trigger werden können, oder alle Änderungen an Aufgaben und Problemzuweisungen vorgenommen werden, während sich das Projekt im Planungsstatus befindet. Dadurch wird die Anzahl der Benachrichtigungen, die Benutzer erhalten, minimiert.</p> <p>Die Timeline des Projekts wird vom System nicht automatisch berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Aktueller (erforderlicher Status)</td> 
   <td> <p>Benutzer arbeiten daran. Der Projektmanager sollte ein Projekt auf "Aktuell"umstellen, um zu signalisieren, dass es gestartet wurde.</p> <p>Dies ist der Standardstatus für neue Projekte in Workfront.</p> <p>Tipp: Als Workfront-Administrator können Sie den Standardstatus für neue Projekte im Bereich "Projekte"unter "Projekteinstellungen"ändern. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig auf den Projektlisten im Projektbereich von Workfront anzeigen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsliste aus. Sie können damit beginnen, Aufgaben und Probleme zu übernehmen, und sie in ihre Liste "Arbeiten auf"verschieben.</p> <p>Außerdem werden bei einem aktuellen Projekt alle Benachrichtigungen über Timeline-Änderungen, Zuweisungen, erforderliche Aktionen und Genehmigungen an Benutzer des Projekt-Teams gesendet.</p> <p>Die Timeline des Projekts wird automatisch vom System berechnet, wenn der Aktualisierungstyp des Projekts auf Automatisch, Bei Änderung oder Automatisch und Bei Änderung eingestellt ist.</p> <p>Tipp: Es empfiehlt sich, die Projektplananpassungen auf ein Minimum zu beschränken, wenn sich ein Projekt in diesem Status befindet, damit Benutzer nicht zu viele Benachrichtigungen erhalten.</p> </td> 
  </tr> 
  <tr> 
   <td>Abgeschlossen (erforderlicher Status)</td> 
   <td> <p> Das Projekt ist abgeschlossen:</p> 
    <ul> 
     <li> <p>Wenn der Abschlussmodus des Projekts auf Manuell eingestellt ist, wählt der Projektmanager diesen Status manuell aus, um die Benutzer im Projektteam aufzufordern, die Arbeit an dem Projekt zu beenden.</p> </li> 
    </ul> 
    <ul> 
     <li>Wenn der Abschlussmodus des Projekts auf Automatisch eingestellt ist, markiert Workfront das Projekt automatisch als abgeschlossen, wenn alle Aufgaben und Probleme im Projekt als abgeschlossen markiert sind. </li> 
    </ul> <p><b>WICHTIG</b>: Sie können ein Projekt nur dann als abgeschlossen markieren, wenn alle Aufgaben, Probleme und Genehmigungen im Projekt gelöst sind.</p> </td> 
   <td>
    <ul>
     <li>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsanfragen oder Arbeiten an Listen nicht aus.</li>
     <li>Alle mit dem Projekt zusammenhängenden Benachrichtigungen mit Ausnahme einer Statusänderungsbenachrichtigung werden nicht mehr an die Benutzer im Projektteam gesendet. </li>
     <li>Die Zeitleiste des Projekts wird vom System nicht mehr berechnet.</li>
     <li>Das Projekt kann nicht kopiert werden.</li>
    </ul><p>Sie können Benutzer daran hindern, zusätzliche Aktionen auszuführen, wenn ein Projekt als abgeschlossen markiert ist. </p><p>Weitere Informationen zum Einschränken von Aktionen auf Projekte, die als abgeschlossen gekennzeichnet sind, finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Eingestellt</td> 
   <td>Das Projekt ist noch nicht abgeschlossen, aber aufgrund von Hindernissen oder Änderungen des Umfangs kann das Projekt nicht weiter bearbeitet werden und wurde aufgegeben. Der Projekt-Manager ändert den Status Dead , um die Benutzer im Projekt-Team darauf hinzuweisen, dass dieses Projekt nie beendet wird und sie nicht mehr daran arbeiten sollten.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht mehr in der Arbeitsliste angezeigt.</p> <p>Genehmigungsentscheidungen können nicht für Aufgaben oder Probleme erteilt werden.</p> <p>Benachrichtigungen über Timeline-Änderungen, Zuweisungen, erforderliche Aktionen und Genehmigungen werden nicht an Benutzer im Projekt-Team gesendet.</p> <p>Die Zeitleiste des Projekts wird vom System nicht automatisch berechnet, da das Projekt als abgeschlossen empfunden wird.</p> <p>Sie können Benutzer daran hindern, bestimmte Aktionen auszuführen, wenn ein Projekt als "Inaktiv"gekennzeichnet ist. Weitere Informationen zur Beschränkung von Aktionen auf Projekte mit Behinderungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Zurückgestellt</td> 
   <td>Das Projekt ist noch nicht abgeschlossen, aber aufgrund einiger Verzögerungen muss das Projekt vorübergehend ausgesetzt werden. Der Projektmanager wählt diesen Status aus, um Benutzer im Projektteam aufzufordern, die Projektarbeit zum aktuellen Zeitpunkt zu beenden.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht mehr in der Arbeitsliste angezeigt. </p> <p>Genehmigungsentscheidungen können nicht für Aufgaben oder Probleme erteilt werden.</p> <p>Benachrichtigungen über Timeline-Änderungen, Zuweisungen, erforderliche Aktionen und Genehmigungen werden nicht an Benutzer im Projekt-Team gesendet.</p> <p> <p><b>NOTE</b>: Wenn Sie ein Projekt auf "Warten"platzieren, wird die Zeitleiste des Projekts nicht angehalten. Das Projekt kann auch dann als "Risiko"oder "In Schwierigkeiten"angezeigt werden, wenn niemand aktiv an dem Projekt arbeitet. Wenn Sie das Projekt erneut auf "Aktuell"zurücksetzen, müssen die Daten der verbleibenden offenen Aufgaben möglicherweise manuell angepasst werden, damit das Projekt den aktualisierten Fortschritt anzeigen kann.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Angefordert</td> 
   <td>Der Projektstatus wird automatisch als vom System angefordert markiert, wenn der geschäftliche Fall einer Projektanfrage abgeschlossen und zur Genehmigung eingereicht wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Geschäftsfalls finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Überprüfen angeforderter Projekte</a>.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme im Projekt, die ihnen zugewiesen sind, füllen ihre Arbeitsliste nicht aus.</p> <p>Alle mit dem Projekt zusammenhängenden Benachrichtigungen mit Ausnahme einer Statusänderungsbenachrichtigung werden an keine Benutzer gesendet.</p> <p>Die Timeline des Projekts wird vom System nicht automatisch berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Genehmigt</td> 
   <td>Der Projektstatus wird automatisch als "Genehmigt"markiert, wenn der geschäftliche Fall einer Projektanfrage genehmigt wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Geschäftsfalls finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Überprüfen angeforderter Projekte</a>.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig auf den Projektlisten im Projektbereich von Workfront anzeigen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsliste nicht aus.</p> <p>Alle mit dem Projekt zusammenhängenden Benachrichtigungen mit Ausnahme einer Statusänderungsbenachrichtigung werden an keine Benutzer gesendet.</p> <p>Die Timeline des Projekts wird vom System nicht automatisch berechnet. </p> </td> 
  </tr> 
  <tr> 
   <td>Abgelehnt</td> 
   <td>Der Projektstatus wird automatisch als Abgelehnt markiert, wenn der Geschäftsszenario einer Projektanforderung abgelehnt wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Geschäftsfalls finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Überprüfen angeforderter Projekte</a>.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsliste nicht aus.</p> <p>Alle mit dem Projekt zusammenhängenden Benachrichtigungen mit Ausnahme einer Statusänderungsbenachrichtigung werden an keine Benutzer gesendet.</p> <p>Die Timeline des Projekts wird vom System nicht automatisch berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Idee</td> 
   <td>Der Projektstatus wird automatisch als Idee markiert, wenn Sie eine Projektanforderung senden. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Geschäftsfalls finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Überprüfen angeforderter Projekte</a>.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt nicht standardmäßig auf ihren Projektlisten im Projektbereich von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, füllen ihre Arbeitsliste nicht aus.</p> <p>Alle mit dem Projekt zusammenhängenden Benachrichtigungen mit Ausnahme einer Statusänderungsbenachrichtigung werden an keine Benutzer gesendet.</p> <p>Die Timeline des Projekts wird vom System nicht automatisch berechnet.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Die folgenden Projektstatus können nicht in den Status &quot;Dead&quot;, &quot;On Hold&quot;oder &quot;Complete&quot;geändert werden:
>
>* Angefordert
>* Idee
>* Genehmigt
>* Abgelehnt (oder deren Entsprechung)
>

