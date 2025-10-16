---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Systemweite Projektvoreinstellungen konfigurieren
description: Als  [!DNL Adobe Workfront]  können Sie die Standardeinstellungen für alle im System erstellten Projekte konfigurieren. Diese Voreinstellungen wirken sich auf das Verhalten von Projekten, Aufgaben und Problemen aus.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '2670'
ht-degree: 1%

---

# Systemweite Projektvoreinstellungen konfigurieren

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Als [!DNL Adobe Workfront] können Sie die Standardeinstellungen für alle im System erstellten Projekte konfigurieren. Diese Voreinstellungen wirken sich auf das Verhalten von Projekten, Aufgaben und Problemen aus.

>[!NOTE]
>
>Standardmäßig sind diese Einstellungen gesperrt und Gruppenadministratoren können sie nicht auf Gruppenebene ändern, es sei denn, Sie entsperren sie für alle Gruppen im System. Weitere Informationen finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL -Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Projektvoreinstellungen für die gesamte Organisation konfigurieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte]**.

1. Fahren Sie auf der **Projektvoreinstellungen** mit einem der vier unten aufgeführten Abschnitte fort, um Voreinstellungen für [!UICONTROL Projektstatus], [!UICONTROL Timelines], [!UICONTROL Business Cases] und [!UICONTROL Life after Death] zu konfigurieren.
1. Wenn Sie möchten, dass alle Gruppen im Unternehmen dieselben Projektvoreinstellungen verwenden, stellen Sie sicher, dass jede Voreinstellung gesperrt ist ![Umschalter für Sperren](assets/lock-toggle-button.png) (dies ist die Standardeinstellung).

   >[!IMPORTANT]
   >
   >Wenn eine Projektvoreinstellung gesperrt ist, werden alle Änderungen, die Sie an dieser Voreinstellung vornehmen, von allen Gruppen im System übernommen. Es ist wichtig, mit den Benutzenden und Gruppen in Ihrer Organisation zu kommunizieren, um sicherzustellen, dass alle Anforderungen bei der Konfiguration der Projektvoreinstellungen berücksichtigt werden.

   Informationen zum Entsperren einer Voreinstellung, sodass alle Gruppen sie selbst konfigurieren und verwalten können, finden Sie unter [Projekteinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

* [[!UICONTROL Projektstatus]](#project-status)
* [[!UICONTROL Timelines]](#timelines)
* [[!UICONTROL Business Cases]](#business-cases)
* [[!UICONTROL Leben nach dem Tod]](#life-after-death)

### Projektstatus {#project-status}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte im gesamten System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erlauben Sie Benutzern, Projekte ohne Vorlage zu erstellen]</td> 
   <td>  <p>Diese Einstellung ermöglicht es Benutzenden, Projekte ohne Vorlage zu erstellen, wenn sie ein Projekt aus den folgenden Bereichen erstellen: </p>
      <ul>
        <li>
        <p>Verwenden der Option [!UICONTROL Neues Projekt] in einer Projektliste</p>
        </li>
          <li>
          <p>Konvertieren eines Problems in ein Projekt über die Problemseite</p>
          </li>
         </ul>
        <p>Diese Einstellung ist standardmäßig aktiviert. </p> 
        <p><b>NOTIZ</b></p>
        <p> Ein Gruppenadministrator kann diese Einstellung für eine Gruppe ändern. Wenn ein(e) Benutzende(r) mehreren Gruppen mit unterschiedlichen Voreinstellungen angehört, kann er/sie ein Projekt ohne Vorlage erstellen, wenn diese Einstellung für die Hauptgruppe aktiviert ist.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Den Status eines neuen Projekts auf] setzen</td> 
   <td> <p>Status neuer Projekte ermitteln.</p>  <p><b>HINWEIS</b>  
     <ul> 
      <li>Wenn Sie oder ein anderer [!DNL Workfront] den hier ausgewählten Status ausblendet, ändert sich der Standardstatus in den ersten Status in der Statusliste.</li> 
     </ul> 
     <ul> 
      <li> <p>Wenn ein gesperrter System- oder Gruppenstatus als Standardstatus festgelegt ist und später von jemandem entsperrt wird, versucht das System, ihn durch einen gesperrten Status desselben Statustyps zu ersetzen.</p> <p>Wenn er keinen finden kann, sucht er nach dem erforderlichen Status:</p> 
       <ul> 
        <li>Wenn ein erforderlicher Status vorhanden ist, der dem entsperrten Standardstatus entspricht, wird der erforderliche Status zum Standardstatus, selbst wenn er entsperrt ist.</li> 
        <li>Wenn keiner der erforderlichen Status dem entsperrten Standardstatus entspricht, wird der erste erforderliche Status in der Statusliste zum Standardstatus.</li> 
       </ul> <p>Informationen zu erforderlichen Status finden Sie in den Artikeln <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemprojektstatus</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der </a> und <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemanfragestatus</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prozentwert der Fertigstellung berechnen auf der Basis von]</td> 
   <td> <p>Workfront berechnet den abgeschlossenen Prozentsatz eines Projekts oder einer übergeordneten Aufgabe anhand des abgeschlossenen Prozentsatzes jeder Aufgabe im Projekt und entweder anhand der Dauer oder der geplanten Stunden jeder Aufgabe.</p><p>Der abgeschlossene Prozentsatz jeder Aufgabe wird von den Aufgabenzugewiesenen manuell festgelegt.</p><p>Hier können Sie auswählen, ob Workfront die Aufgabendauer oder die geplanten Aufgabenstunden zur Berechnung des Prozentsatzes der abgeschlossenen Projekte verwenden soll.</p> <p>Wenn Sie [!UICONTROL Dauer] auswählen, bestimmt die Dauer jeder Aufgabe in einem Projekt den Gesamtprozentsatz der Fertigstellung für das Projekt und die Dauer jeder Unteraufgabe den Gesamtprozentsatz der Fertigstellung für die übergeordnete Aufgabe.</p> <p>Wenn Sie [!UICONTROL Dauer] auswählen, stellen Sie sicher, dass Sie die [!UICONTROL Typische Stunden pro Arbeitstag] und [!UICONTROL Typische Arbeitstage pro Woche] im Abschnitt [!UICONTROL Timelines] angeben. [!DNL Workfront] verwendet diese Informationen, wenn der Prozentsatz der Fertigstellung einer Aufgabe auf der Grundlage der Dauer berechnet wird. </p> <p>Wenn Sie die Option [!UICONTROL Geplante Stunden] auswählen, stellen Sie sicher, dass für alle Aufgaben in jedem Projekt der Betrag von [!UICONTROL Geplante Stunden] definiert ist und dass der Betrag nicht null ist.</p><p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Übersicht über die prozentuale Fertigstellung eines Projekts</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL : Legt die Projektbedingung basierend auf dem Verlaufsstatus automatisch fest]</td> 
   <td> <p>Diese Voreinstellung ermöglicht es Benutzern, die [!UICONTROL -Bedingung] eines Projekts manuell auf ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) festzulegen oder die [!UICONTROL -Bedingung] (Fortschrittsstatus) automatisch basierend auf dem Fortschritt des Projekts auf der Timeline festlegen [!DNL Workfront]. Weitere Informationen über den Zustand von Projekten finden Sie unter <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Projektbedingung und Bedingungstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Baselines automatisch erstellen]</p> </td> 
   <td> <p>Diese Voreinstellung erstellt automatisch eine Baseline (Momentaufnahme) der Aufgaben- und Projektdetails, wenn sich der Status des Projekts in [!UICONTROL Current] ändert. Informationen zum Erstellen von Baselines finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Erstellen von Projekt-Baselines</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index-Methode] </p> </td> 
   <td> <p>Die Leistungsindexmethode (PIM) für das Projekt steuert die Methode, die [!DNL Workfront] verwendet, um Earned Value-Metriken wie [!UICONTROL Cost Performance Index] (CPI) und [!UICONTROL Estimate At Completion] (EAC) zu berechnen. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calculate [!UICONTROL Cost Performance Index] (CPI)</a> und <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate at Completion] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Stundenbasiert]</strong>: [!DNL Workfront] verwendet [!UICONTROL Geplante Stunden], um Leistungsmetriken wie EAC und CPI zu berechnen. Wenn das PIM auf der Grundlage von Stunden berechnet wird, wird die EAC als Anzahl von Stunden angezeigt. Stellen Sie sicher, dass Sie einen anderen Wert für [!UICONTROL Geplante Stunden] als null haben.</li> 
     <li> <p><strong>[!UICONTROL Kostenbasiert]</strong>: [!DNL Workfront] verwendet [!UICONTROL Geplante Lohnkosten], um Leistungsmetriken wie EAC und CPI zu berechnen. Stellen Sie sicher, dass Ihre Aufgabengebiete oder Benutzer den Stundensätzen „Kosten pro Stunde“ zugeordnet sind. Wenn die PIM auf der Grundlage von Kosten berechnet wird, wird die EAC als Währungswert angezeigt.</p> <p>Der Projekt-Manager kann diese Einstellung auf Projektebene ändern, indem er den Bereich [!UICONTROL Finance] in [!UICONTROL Projektdetails] verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Projektbereich Finance</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schätzung bei Abschluss &#x200B;]</p> </td> 
   <td> <p>Legen Sie fest, welche Daten [!DNL Workfront] zur Berechnung der [!UICONTROL Estimate at Completion] (EAC) verwendet, die die erwarteten Gesamtkosten eines Projekts darstellen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Auf Projektebene berechnen]</strong>: Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt wird durch Eingabe von [!UICONTROL Ist-Stunden] oder [!UICONTROL Ist-Arbeitskosten] in die BK-Formeln bestimmt. Diese Berechnung enthält [!UICONTROL Tatsächliche Stunden] oder [!UICONTROL Kosten und Ausgaben], die der übergeordneten Aufgabe oder dem übergeordneten Projekt direkt hinzugefügt werden.</li> 
     <li> <p><strong>[!UICONTROL Rollup from tasks/subtasks]</strong>: Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt werden bestimmt, indem die BK für jede untergeordnete Aufgabe zusammengefasst werden. Diese Berechnung schließt [!UICONTROL Ist-Stunden] oder [!UICONTROL Ist-Kosten und -Ausgaben] aus, die der übergeordneten Aufgabe oder dem übergeordneten Projekt direkt hinzugefügt werden.</p> <p>Der Projekt-Manager kann diese Einstellung auf Projektebene ändern, indem er den Bereich [!UICONTROL Finance] in [!UICONTROL Projektdetails] verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Projektbereich Finance</a>.</p> </li> 
    </ul> <p>Weitere Informationen dazu, wie der EAC berechnet, finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculate [!UICONTROL Estimate at Completion] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Timelines {#timelines}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte im gesamten System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeitplan ab]</td> 
   <td> <p>Legen Sie fest, ob neue Projekte ab dem Startdatum oder ab dem Abschlussdatum geplant werden, wenn sie erstellt werden.</p> 
    <ul> 
     <li><strong>[!UICONTROL Startdatum]</strong>: Für neue Aufgaben wird standardmäßig die Aufgabenbeschränkung [!UICONTROL Sofort as possible] verwendet, und die Projektverantwortlichen werden aufgefordert, ein [!UICONTROL Geplantes Startdatum] für das Projekt anzugeben.</li> 
     <li><strong>[!UICONTROL Abschlussdatum]</strong>: Für neue Aufgaben wird standardmäßig die Aufgabenbeschränkung [!UICONTROL As Late As Possible] verwendet, und die Projektverantwortlichen werden aufgefordert, ein [!UICONTROL Geplantes Abschlussdatum] für das Projekt anzugeben.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerauszeit]</td> 
   <td> <p>Legen Sie fest, ob die Ausfallzeit des Primären Verantwortlichen für eine Aufgabe die geplanten Termine für diese Aufgabe in einem Projekt anpasst.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL : Auszeiten von Benutzern in Aufgabenlaufzeiten berücksichtigen]</strong>: Jede für den Primären Beauftragten einer Aufgabe geplante Auszeit passt die geplanten Termine der Aufgabe an, wenn die Auszeit während der Aufgabenlaufzeit eintritt. Dies ist die Standardeinstellung. </p> <p>Wenn beispielsweise eine Aufgabe mit der Einschränkung [!UICONTROL As Sofort As Without As Possible] für den 1. Juni geplant ist, um sie am 3. Juni abzuschließen, und der Primäre Verantwortliche für den 2. Juni Ausfallzeiten markiert hat, werden die Termine der Aufgabe auf den 1. Juni bis zum 4. Juni angepasst.</p> <p><b>WICHTIG</b>:</p> <p>Die Dauer der Aufgabe ändert sich nicht, wenn Sie diese Einstellung auswählen. Je nach Aufgabenbeschränkung ändern sich nur die geplanten Termine.</p> </li> 
     <li><strong>[!UICONTROL Benutzer-Ausfallzeit in Aufgabendauer ignorieren]</strong>: Die geplanten Termine jeder Aufgabe in einem Projekt bleiben wie ursprünglich geplant, auch wenn der Primäre Verantwortliche einer Aufgabe während ihrer Laufzeit Ausfallzeiten hat.</li> 
    </ul> <p>Beachten Sie bei der Auswahl von Optionen für diese Einstellung Folgendes:</p> 
    <ul> 
     <li>Wenn Sie diese Einstellung ändern, erben nur die Projekte und Vorlagen, die nach der Änderung erstellt wurden, die aktualisierte Einstellung. </li> 
     <li> <p>Der Wert der Aufgabenbeschränkung der Aufgabe bestimmt, welche geplanten Aufgabendaten angepasst werden sollen: </p> 
      <ul> 
       <li>Das geplante Startdatum</li> 
       <li>Das geplante Abschlussdatum</li> 
       <li>Beide Daten</li> 
       <li>Kein Datum. </li> 
      </ul> <p>Wenn beispielsweise eine Aufgabe eine Einschränkung von [!UICONTROL Feste Datumswerte] aufweist, werden die Datumswerte nicht angepasst, wenn der Primäre Verantwortliche Ausfallzeiten hat, selbst wenn die Option [!UICONTROL Benutzerauszeit in Aufgabendauer berücksichtigen] ausgewählt ist. Informationen zu Aufgabenbeschränkungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Aufgabenbeschränkungen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Projektzeitleisten werden automatisch neu berechnet]</p> </td> 
   <td> <p>Legen Sie fest, wann die Zeitleiste eines Projekts neu berechnet wird. Informationen zur Neuberechnung der Projekt-Zeitleiste finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Neuberechnen von Projekt-Zeitleisten</a>.</p> <p>Die folgenden Optionen sind standardmäßig aktiviert. Sie können eine oder mehrere der folgenden Einstellungen auswählen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>: Wählen Sie diese Option, um die Projektzeitleisten jede Nacht neu zu berechnen. Alle Änderungen, die Sie am Projekt vornehmen und die sich auf die Zeitleiste auswirken könnten, sind nicht sofort sichtbar. [!DNL Workfront​​​] berechnet Timelines nachts nur für Projekte neu, bei denen die beiden folgenden Bedingungen erfüllt sind:</p> <p> 
       <ul> 
        <li>Sie haben den Status [!UICONTROL Aktuell]</li> 
        <li>In den letzten 3 Monaten ein Update erhalten haben</li> 
        <li>einen der folgenden Aktualisierungstypen hatten:</li>
        <ul>
        <li>Automatisch UND bei Änderung</li>
        <li>Nur Änderung</li>
        <li>Nur automatisch</li> 
      </ul>       
    <b>TIPP:</b>
    <p>Projekte, die den Aktualisierungstyp „Nur manuelle Aktualisierung“ aufweisen, sind von dieser Einstellung nicht betroffen.</p>
    <li> <p><strong>Wenn sich der Projektumfang ändert</strong>: Wählen Sie diese Option, um die Projektzeitleisten sofort nach einer Änderung des Projektumfangs neu zu berechnen. Informationen dazu, was eine Änderung des Projektumfangs ausmacht, finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Neuberechnen von Projektzeitleisten</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Wenn mehrere Benutzer einer Aufgabe zugewiesen sind, verwenden Sie den Zeitplan von]</p> </td> 
   <td> <p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern, die seinen Aufgaben zugewiesen sind, kein Zeitplan zugewiesen ist, berechnet [!DNL Workfront] anhand des Systemstandardzeitplans den Zeitplan der Aufgaben.</p> <p>Wenn Sie derselben Aufgabe in einem Projekt mehrere Benutzer zuweisen und dem Projekt ein Zeitplan zugewiesen ist und den Benutzern, die den Aufgaben zugewiesen sind, auch ein Zeitplan zugewiesen ist, verwendet [!UICONTROL Workfront] die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primär Assignment]</strong>: [!DNL Workfront] berechnet Zeitleisten anhand des Zeitplans der Primären Zuweisung für die Aufgabe.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] berechnet die Zeitleiste jeder Aufgabe anhand des Zeitplans des Projekts.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>Wenn eine Benutzerin bzw. ein Benutzer einer Aufgabe zugeteilt ist, den Zeitplan verwenden von …</p> </td> 
   <td> 
<p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern, die seinen Aufgaben zugewiesen sind, kein Zeitplan zugewiesen ist, berechnet [!DNL Workfront] anhand des Systemstandardzeitplans den Zeitplan der Aufgaben.</p>

<p>Wenn Sie einer Aufgabe in einem Projekt einen Benutzer zuweisen und sowohl dem Projekt als auch dem Benutzer, der den Aufgaben zugewiesen ist, Zeitpläne zugeordnet sind, verwendet [!UICONTROL Workfront] die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>[!UICONTROL User]</strong>: [!DNL Workfront] berechnet Zeitleisten anhand des Zeitplans des zugewiesenen Benutzers für die Aufgabe.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] berechnet die Zeitleiste der Aufgabe anhand des Zeitplans des Projekts.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Zeitleistenberechnungen] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typische Stunden pro Arbeitstag]</strong>: Legen Sie die Anzahl der Stunden in einem typischen Arbeitstag für die Benutzer fest, die an Projekten arbeiten werden. Der Standardwert ist 8 Stunden.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typische Arbeitstage pro Woche]</strong>: Legen Sie die Standard-Arbeitswoche für die Benutzer fest, die an Projekten arbeiten. Der Standardwert ist 5 Tage.</li> 
    </ul> <p>Diese zwei Optionen konvertieren Tage in Stunden bzw. Wochen in Tage.</p> <p>Wenn Sie beispielsweise eine Aufgabe mit acht geplanten Stunden haben und die Dauer auf der Grundlage der geplanten Stunden berechnet wird, wandelt [!DNL Workfront] diese Stunden in Tage um, um die Dauer als Tage anzuzeigen.</p> <p>Aus dem Feld Typische [!UICONTROL Arbeitstage pro Woche] berechnet [!DNL Workfront] den Vollzeitäquivalenzwert (VZÄ) für Ihr System. Dies wird von [!DNL Workfront] bei der Berechnung der Zuweisungen für Benutzer verwendet.</p> <p>Diese Werte werden verwendet, wenn Sie Projektzeitleisten planen, Ressourcen budgetieren oder Zeit für Projekte protokollieren. </p> <p>Sie werden nicht verwendet, wenn Sie Arbeitszeittabellen für Benutzer im System erstellen, wie in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Konfigurieren] Arbeitszeittabelle und Stundeneinstellungen beschrieben</a>.</p> <p><b>HINWEIS</b>:</p> <p>[!DNL Workfront] Administratoren können die Voreinstellungen für [!UICONTROL Timeline Calculations] nicht entsperren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Quartale]</p> </td> 
   <td> <p>Konfigurieren Sie benutzerdefinierte jährliche Quartale für die Benutzer, die an Projekten arbeiten werden. Benutzerdefinierte Quartale sind in der Regel Quartale, die nicht der herkömmlichen Aufschlüsselung von Quartalen während eines Kalenderjahres entsprechen. Sie können mehrere benutzerdefinierte Quartale hinzufügen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Quartale </a>.</p>  <p><b>HINWEIS</b>: </p><p>[!DNL Workfront] Administratoren können die Voreinstellungen für [!UICONTROL Custom Quarters] nicht entsperren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Business Cases] {#business-cases}

Sie können einen Business Case für neu erstellte Projekte im gesamten System erstellen, um Projektanfragen zu senden. Sie können Voreinstellungen definieren, um zu bestimmen, welche Bereiche im Formular **[!UICONTROL Business Case]** sichtbar sind. Es wird empfohlen, diese Optionen zu aktivieren, damit andere Tools, wie z. B. der [!UICONTROL Portfolio Optimizer], ordnungsgemäß aktualisiert werden. Weitere Informationen zu den einzelnen Feldern finden Sie unter [Definieren eines Business-Case: Artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nachdem der [!DNL Workfront]-Administrator die Abschnitte zum [!UICONTROL Business Case] aktiviert hat, kann ein Projektinhaber dann einen Business Case auf Projektebene erstellen. Informationen zum Erstellen eines Business-Case finden Sie [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Leben nach dem Tod]  {#life-after-death}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte im gesamten System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Wenn ein Projekt als Abgeschlossen gekennzeichnet wurde, können Benutzer weiterhin] </p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, um festzulegen, ob eine Aufgabe oder ein Problem gelöscht werden kann, nachdem der Projektstatus als [!UICONTROL Abgeschlossen] markiert wurde.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aufgaben löschen]</strong>: Ermöglicht Benutzern das Löschen von Aufgaben aus einem Projekt, nachdem das Projekt als [!UICONTROL Complete] markiert wurde.<br></li> 
     <li><strong>[!UICONTROL Probleme löschen]</strong>: Ermöglicht Benutzern das Löschen von Problemen aus einem Projekt, nachdem das Projekt als [!UICONTROL Complete] markiert wurde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nachdem ein Projekt als Abgeschlossen, Eingestellt oder mit dem Hinweis Ausstehende Genehmigungen, gekennzeichnet wurde, können Benutzer weiterhin]</p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, was mit Aufgaben, Problemen, Dokumenten und anderen Objekten in einem Projekt geschieht, nachdem der Projektstatus <strong>[!UICONTROL Abgeschlossen]</strong>, <strong>[!UICONTROL Eingestellt]</strong> markiert wurde oder <strong>[!UICONTROL Ausstehende Genehmigung]</strong> ist.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aufgaben hinzufügen und bearbeiten:]</strong> Ermöglicht Benutzern Folgendes:
      <ul>
       <li><p>Aufgaben innerhalb eines Projekts bearbeiten, nachdem das Projekt als [!UICONTROL Abgeschlossen], [!UICONTROL Eingestellt] oder als [!UICONTROL Ausstehende Genehmigung] gekennzeichnet wurde.</p>
           <p>Hinweis: Auch wenn diese Option nicht ausgewählt ist, können Benutzer Ausgabeneinträge hinzufügen und bearbeiten. Die Protokollierung von Stunden hat eine separate Einstellung. Informationen zum Zulassen oder Verhindern der Zeitprotokollierung für Projekte mit dem Status Abgeschlossen oder Inaktiv finden Sie unter <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Arbeitszeittabelle und Stundeneinstellungen konfigurieren</a>.</p></li>
       <li>Aufgaben zu einem Projekt hinzufügen.</li>
      </ul></li>
     <li><strong>[!UICONTROL Probleme hinzufügen und bearbeiten]</strong>: Ermöglicht Benutzern Folgendes:
      <ul>
       <li>Probleme innerhalb eines Projekts bearbeiten, nachdem das Projekt als [!UICONTROL Abgeschlossen], [!UICONTROL Eingestellt] oder [!UICONTROL Ausstehende Genehmigung] gekennzeichnet wurde.</li>
       <li>Probleme zu einem Projekt hinzufügen, nachdem das Projekt als [!UICONTROL Abgeschlossen] oder [!UICONTROL Eingestellt] gekennzeichnet wurde. (Sie können keine Probleme zu einem Projekt hinzufügen, das [!UICONTROL Ausstehende Genehmigung] ist.)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Dokumente zum Projekt und zu seinen Aufgaben und Problemen hinzufügen]</strong>: Ermöglicht Benutzern das Hinzufügen von Dokumenten zu einem Projekt (oder das Hinzufügen von Dokumenten zu Aufgaben und Problemen innerhalb des Projekts), nachdem das Projekt als [!UICONTROL abgeschlossen] oder [!UICONTROL eingestellt] markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
     <li> <p><strong>[!UICONTROL Vorlagen anhängen]</strong>: Ermöglicht Benutzern das Anhängen von Vorlagen an ein Projekt, nachdem das Projekt als [!UICONTROL Abgeschlossen] oder [!UICONTROL Eingestellt] markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
