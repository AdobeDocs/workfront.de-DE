---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Übersicht über die Systemprojektstatus
description: Workfront verfügt über neun integrierte Systemprojektstatus. Die ersten 3 in der folgenden Tabelle sind erforderlich, was bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können. Das Ändern eines Projektstatus ist in der Regel ein manueller Prozess. Manchmal wird jedoch ein Projektstatus automatisch geändert, abhängig von anderen Aktivitäten, die im System stattfinden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 0%

---

# Übersicht über die Systemprojektstatus

<!--Audited: 12/2023-->

Workfront verfügt über neun integrierte Systemprojektstatus.

Die ersten 3 in der folgenden Tabelle sind erforderlich, was bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können.

Das Ändern eines Projektstatus ist in der Regel ein manueller Prozess. Es gibt jedoch einige in der folgenden Liste beschriebene Szenarien, in denen ein Projektstatus je nach anderen Aktivitäten im System automatisch geändert wird.

Workfront stellt die folgenden Projektstatus für Ihre Adobe Workfront-Instanz bereit:

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
   <th>Dieser Projektstatus tritt auf, wenn</th> 
   <th>Was passiert in diesem Status?</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planung (erforderlicher Status)</td> 
   <td> <p>Der Projektleiter plant den Zeitplan des Projekts, die Zuweisung der Aufgaben und die Validierungen. Der Projekt-Manager legt diesen Status für ein Projekt manuell fest.</p> <p><b>TIPP</p> <p> Es wird empfohlen, den Standardstatus für neue Projekte in Workfront auf Planning festzulegen. Als Workfront-Administrator können Sie den Standardstatus für alle Ihre neuen Projekte im Bereich „Projekte“ der Projektvoreinstellungen ändern.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Systemweite Projektvoreinstellungen konfigurieren</a>.</p></td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht in ihrer Arbeitsliste aufgeführt. In der Startseiten-Arbeitsliste werden nur Genehmigungen und akzeptierte Arbeitselemente angezeigt.</p> <p>Während ein Projekt diesen Status aufweist, werden keine Benachrichtigungen gesendet.</p> <p>Trigger Es wird empfohlen, alle Änderungen vorzunehmen, durch die eine Aktualisierung der Zeitleiste des Projekts oder Änderungen an Aufgaben und Problemzuweisungen vorgenommen werden können, während sich das Projekt im Planungsstatus befindet. Dies minimiert die Anzahl der Benachrichtigungen, die Benutzer erhalten.</p> <p>Die Zeitleiste des Projekts wird nicht automatisch vom System berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Aktuell (erforderlicher Status)</td> 
   <td> <p>Benutzende arbeiten an Aufgaben und Problemen im Projekt. Der Projektmanager sollte ein Projekt in „aktuell“ umwandeln, um zu signalisieren, dass es gestartet wurde.</p> <p>Dies ist der Standardstatus für neue Projekte in Workfront.</p> <p><b>TIPP</b></p>

<p> Als Workfront-Administrator können Sie den Standardstatus für neue Projekte im Bereich „Projekte“ der Projektvoreinstellungen ändern. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden in ihrer Arbeitsliste aufgeführt. Sie können anfangen, Aufgaben und Probleme zu bearbeiten, und sie in ihre Liste „Arbeiten an“ verschieben.</p> <p>In einem aktuellen Projekt werden alle Benachrichtigungen zu Zeitleistenänderungen, Zuweisungen, erforderlichen Aktionen und Genehmigungen an die Benutzer im Projektteam gesendet.</p> <p>Die Zeitleiste des Projekts wird automatisch vom System berechnet, wenn der Aktualisierungstyp des Projekts auf „Automatisch“, „Bei Änderung“ oder „Automatisch“ und „Bei Änderung“ eingestellt ist.</p> <p><b>TIPP</b></p> <p> Wenn ein Projekt diesen Status aufweist, empfiehlt es sich, die Anpassungen am Projektplan auf ein Minimum zu beschränken, damit die Benutzer nicht zu viele Benachrichtigungen erhalten.</p> </td> 
  </tr> 
  <tr> 
   <td>Abgeschlossen (erforderlicher Status)</td> 
   <td> <p> Alle Aufgaben und Probleme des Projekts sind abgeschlossen und das Projekt ist abgeschlossen.</p> 
     <p>Wenn der Fertigstellungsmodus des Projekts auf Manuell festgelegt ist, wählt der Projekt-Manager diesen Status manuell, um die Benutzer im Projekt-Team darüber zu informieren, dass sie nicht mehr an dem Projekt arbeiten sollen.</p> 
    <p>Wenn der Fertigstellungsmodus des Projekts auf Automatisch festgelegt ist, markiert Workfront ein Projekt automatisch als abgeschlossen, wenn alle Aufgaben und Probleme im Projekt als abgeschlossen markiert sind. 
    <p><b>WICHTIG</b> </p>
    <p>Sie können ein Projekt nur dann als abgeschlossen markieren, wenn alle Aufgaben, Probleme und Genehmigungen für das Projekt erledigt sind.</p> </td> 
   <td>
    <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht in ihren Arbeitsanfragen oder Arbeitsauftragslisten aufgeführt. </p>
    <p>Alle projektbezogenen Benachrichtigungen mit Ausnahme einer Benachrichtigung bezüglich einer Statusänderung werden nicht mehr an die Benutzenden im Projekt-Team gesendet.</p>
    <p>Die Zeitleiste des Projekts wird nicht mehr vom System berechnet. </p>
    <p>Das Projekt kann nicht kopiert werden.</p>
    <p>Sie können Benutzer daran hindern, zusätzliche Aktionen auszuführen, wenn ein Projekt als Abgeschlossen markiert ist. </p><p>Weitere Informationen zum Einschränken von Aktionen für Projekte, die als abgeschlossen markiert sind, finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Projektvoreinstellungen</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Eingestellt</td> 
   <td>Das Projekt ist noch nicht abgeschlossen, aber aufgrund von Hindernissen oder einer Änderung des Projektumfangs kann das Projekt nicht weiter bearbeitet werden und wurde aufgegeben. Der Projekt-Manager ändert den Status in „Eingestellt“, um die Benutzer im Projekt-Team darauf hinzuweisen, dass dieses Projekt nie abgeschlossen wird und sie nicht mehr daran arbeiten sollten.</td> 
   <td> <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, verschwinden aus ihrer Arbeitsliste.</p> <p>Genehmigungsentscheidungen können nicht für Aufgaben oder Probleme erteilt werden.</p> <p>Benachrichtigungen über Änderungen der Zeitleiste, Zuweisungen, erforderliche Aktionen und Genehmigungen werden nicht an Benutzer im Projektteam gesendet.</p> <p>Die Zeitleiste des Projekts wird vom System nicht automatisch berechnet, da das Projekt als abgeschlossen wahrgenommen wird.</p> <p>Sie können Benutzer daran hindern, bestimmte Aktionen auszuführen, wenn ein Projekt als Eingestellt markiert ist. Weitere Informationen zum Einschränken von Aktionen für inaktive Projekte finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Projektvoreinstellungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Zurückgestellt</td> 
   <td>Das Projekt ist noch nicht abgeschlossen, muss jedoch aufgrund einiger Verzögerungen vorübergehend ausgesetzt werden. Der Projekt-Manager verwendet diesen Status, um die Benutzer im Projekt-Team darauf hinzuweisen, dass sie zum aktuellen Zeitpunkt nicht mehr an dem Projekt arbeiten.</td> 
   <td> <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, verschwinden aus ihrer Arbeitsliste. </p> <p>Genehmigungsentscheidungen können nicht für Aufgaben oder Probleme erteilt werden.</p> <p>Benachrichtigungen über Änderungen der Zeitleiste, Zuweisungen, erforderliche Aktionen und Genehmigungen werden nicht an Benutzer im Projektteam gesendet.</p> <p> <p><b>NOTIZ</b></p>  <p>Wenn Sie ein Projekt in den Haltezustand versetzen, wird die Zeitleiste des Projekts nicht angehalten. Das Projekt kann weiterhin als Gefährdet oder In Schwierigkeiten angezeigt werden, selbst wenn niemand aktiv an dem Projekt arbeitet. Wenn Sie das Projekt erneut auf „aktuell“ zurücksetzen, müssen die Daten der verbleibenden offenen Aufgaben möglicherweise manuell angepasst werden, damit das Projekt den aktualisierten Fortschritt anzeigen kann.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Angefordert</td> 
   <td>Der Projektstatus wird vom System automatisch als angefordert markiert, wenn der Business Case für eine Projektanfrage abgeschlossen und zur Genehmigung eingereicht wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Business Case finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Angeforderte Projekte überprüfen</a>.</td> 
   <td> <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die ihnen zugewiesenen Aufgaben und Probleme im Projekt werden nicht in ihrer Arbeitsliste aufgeführt.</p> <p>Alle Benachrichtigungen, die sich auf das Projekt beziehen, mit Ausnahme einer Statusänderungsbenachrichtigung, werden nicht an Benutzer gesendet.</p> <p>Die Zeitleiste des Projekts wird nicht automatisch vom System berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Genehmigt</td> 
   <td>Der Projektstatus wird automatisch als „Genehmigt“ gekennzeichnet, wenn der Business-Case für eine Projektanfrage genehmigt wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Business Case finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Angeforderte Projekte überprüfen</a>.</td> 
   <td> <p>Benutzer des Projektteams können das Projekt standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht in ihrer Arbeitsliste aufgeführt.</p> <p>Alle Benachrichtigungen, die sich auf das Projekt beziehen, mit Ausnahme einer Statusänderungsbenachrichtigung, werden nicht an Benutzer gesendet.</p> <p>Die Zeitleiste des Projekts wird nicht automatisch vom System berechnet. </p> </td> 
  </tr> 
  <tr> 
   <td>Abgelehnt</td> 
   <td>Der Projektstatus wird automatisch als abgelehnt markiert, wenn der Business-Case für eine Projektanfrage abgelehnt wurde. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Business Case finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Angeforderte Projekte überprüfen</a>.</td> 
   <td> <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht in ihrer Arbeitsliste aufgeführt.</p> <p>Alle Benachrichtigungen, die sich auf das Projekt beziehen, mit Ausnahme einer Statusänderungsbenachrichtigung, werden nicht an Benutzer gesendet.</p> <p>Die Zeitleiste des Projekts wird nicht automatisch vom System berechnet.</p> </td> 
  </tr> 
  <tr> 
   <td>Idee</td> 
   <td>Der Projektstatus wird beim Senden einer Projektanfrage automatisch als „Idee“ gekennzeichnet, bevor Sie den Business Case abschließen. Weitere Informationen zum Anfordern eines Projekts mithilfe eines Business Case finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Angeforderte Projekte überprüfen</a>.</td> 
   <td> <p>Benutzende des Projektteams können das Projekt nicht standardmäßig in ihren Projektlisten (ohne benutzerdefinierten Filter) im Bereich Projekte von Workfront sehen. Die Aufgaben und Probleme, die ihnen im Projekt zugewiesen sind, werden nicht in ihrer Arbeitsliste aufgeführt.</p> <p>Alle Benachrichtigungen, die sich auf das Projekt beziehen, mit Ausnahme einer Statusänderungsbenachrichtigung, werden nicht an Benutzer gesendet.</p> <p>Die Zeitleiste des Projekts wird nicht automatisch vom System berechnet.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Die folgenden Projektstatus können nicht in den Status „Eingestellt“, „Gesperrt“ oder „Abgeschlossen“ geändert werden:
>
>* Angefordert
>* Idee
>* Genehmigt
>* Abgelehnt (oder gleichwertig)
>
