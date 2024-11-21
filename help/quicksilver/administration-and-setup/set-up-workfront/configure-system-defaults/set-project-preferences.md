---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Konfigurieren von systemweiten Projektvoreinstellungen
description: Als [!DNL Adobe Workfront] Administrator können Sie die Standardeinstellungen für alle im System erstellten Projekte konfigurieren. Diese Voreinstellungen wirken sich auf Projekt-, Aufgaben- und Problemverhalten aus.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '2721'
ht-degree: 1%

---

# Systemweite Projektvoreinstellungen konfigurieren

<!--Audited: 12/2023-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


Als [!DNL Adobe Workfront] -Administrator können Sie die Standardeinstellungen für alle im System erstellten Projekte konfigurieren. Diese Voreinstellungen wirken sich auf Projekt-, Aufgaben- und Problemverhalten aus.

>[!NOTE]
>
>Standardmäßig sind diese Voreinstellungen gesperrt und Gruppenadministratoren können sie nicht auf Gruppenebene ändern, es sei denn, Sie entsperren sie für alle Gruppen im System. Weitere Informationen finden Sie unter [Sperren oder Entsperren von Projektvoreinstellungen für alle Gruppen im System](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] Plan</p></td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren von Projektvoreinstellungen für die gesamte Organisation

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Projekte]**.

1. Fahren Sie auf der Seite **Projekteinstellungen** mit einem der vier unten aufgeführten Abschnitte fort, um die Voreinstellungen für [!UICONTROL Projektstatus], [!UICONTROL Zeitpläne], [!UICONTROL Geschäftsfälle] und [!UICONTROL Lebensdauer nach dem Tod] zu konfigurieren.
1. Wenn Sie möchten, dass alle Gruppen in der Organisation dieselben Projektvoreinstellungen verwenden, stellen Sie sicher, dass jede Voreinstellung gesperrt ist ![](assets/lock-toggle-button.png) (dies ist die Standardeinstellung).

   >[!IMPORTANT]
   >
   >Wenn eine Projektvoreinstellung gesperrt ist, werden alle Änderungen, die Sie an dieser Voreinstellung vornehmen, von allen Gruppen im System übernommen. Es ist wichtig, mit den Benutzern und Gruppen in Ihrer gesamten Organisation zu kommunizieren, um sicherzustellen, dass alle Anforderungen bei der Konfiguration der Projektvoreinstellungen berücksichtigt werden.

   Weitere Informationen zum Entsperren einer Voreinstellung, sodass alle Gruppen sie selbst konfigurieren und verwalten können, finden Sie unter [Sperren oder Entsperren von Projekteigenschaften für alle Gruppen im System](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

* [[!UICONTROL Projektstatus]](#project-status)
* [[!UICONTROL Zeitleisten]](#timelines)
* [[!UICONTROL Geschäftsszenarios]](#business-cases)
* [[!UICONTROL Lebensdauer nach Tod]](#life-after-death)

### Projektstatus {#project-status}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte im gesamten System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzer können Projekte ohne Vorlage erstellen]</td> 
   <td>  <p>Mit dieser Voreinstellung können Benutzer Projekte ohne Verwendung einer Vorlage erstellen, wenn sie ein Projekt aus den folgenden Bereichen erstellen: </p>
      <ul>
        <li>
        <p>Verwenden Sie die Option [!UICONTROL Neues Projekt] in einer Liste von Projekten</p>
        </li>
          <li>
          <p>Konvertieren eines Problems von der Seite des Problems in ein Projekt</p>
          </li>
         </ul>
        <p>Diese Voreinstellung ist standardmäßig aktiviert. </p> 
        <p><b>NOTIZ</b></p>
        <p> Ein Gruppenadministrator kann diese Voreinstellung für eine Gruppe ändern. Wenn ein Benutzer mehreren Gruppen mit unterschiedlichen Voreinstellungen angehört, kann er ein Projekt ohne Vorlage erstellen, wenn diese Voreinstellung für seine Startseite aktiviert ist.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Status des neuen Projekts auf festlegen]</td> 
   <td> <p>Bestimmen Sie den Status neuer Projekte.</p>  <p><b>NOTE</b>  
     <ul> 
      <li>Wenn Sie oder ein anderer [!DNL Workfront] -Administrator den hier ausgewählten Status ausblendet, ändert sich der Standardstatus in den ersten Status in der Statusliste.</li> 
     </ul> 
     <ul> 
      <li> <p>Wenn ein gesperrtes System oder ein Gruppenstatus als Standardstatus festgelegt ist und später von einem anderen entsperrt wird, versucht das System, es durch einen gesperrten Status des gleichen Statustyps zu ersetzen.</p> <p>Wenn er keinen finden kann, sucht er nach einem erforderlichen Status:</p> 
       <ul> 
        <li>Wenn ein erforderlicher Status vorhanden ist, der dem entsperrten Standardstatus entspricht, wird der erforderliche Status zum Standardstatus, auch wenn er entsperrt ist.</li> 
        <li>Wenn keiner der erforderlichen Status dem entsperrten Standardstatus entspricht, wird der erste erforderliche Status in der Statusliste zum Standardstatus.</li> 
       </ul> <p>Informationen zu den erforderlichen Status finden Sie in den Artikeln <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemprojektstatus</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemaufgabenstatus</a> und <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemfehlerstatus</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prozentsatz abschließen basierend auf] berechnen</td> 
   <td> <p>Workfront berechnet den prozentualen Abschluss einer Projekt- oder einer übergeordneten Aufgabe anhand des Prozentsatzes, der für jede Aufgabe im Projekt abgeschlossen ist, und entweder anhand der Dauer oder der geplanten Stunden jeder Aufgabe.</p><p>Der prozentuale Abschluss jeder Aufgabe wird von Aufgabenverantwortlichen manuell festgelegt.</p><p>Hier können Sie auswählen, ob Workfront die Dauer oder die geplanten Stunden für die Berechnung des Prozentsatzes der abgeschlossenen Projekte verwendet.</p> <p>Wenn Sie die [!UICONTROL Dauer] auswählen, bestimmt die Dauer jeder Aufgabe in einem Projekt den Gesamtprozentsatz der Abschlüsse für das Projekt und die Dauer jeder Unteraufgabe bestimmt den Gesamtprozentsatz der Abschlüsse für die übergeordnete Aufgabe.</p> <p>Wenn Sie [!UICONTROL Dauer] auswählen, stellen Sie sicher, dass Sie im Abschnitt [!UICONTROL Timelines] die [!UICONTROL Typischen Arbeitsstunden pro Arbeitstag] und [!UICONTROL Typische Arbeitstage pro Woche] angeben. [!DNL Workfront] verwendet diese Informationen bei der Berechnung des Prozentsatzes der Fertigstellung einer Aufgabe auf Grundlage der Dauer. </p> <p>Wenn Sie die Option [!UICONTROL Geplante Stunden] auswählen, stellen Sie sicher, dass für alle Aufgaben in jedem Projekt der Betrag von [!UICONTROL Geplante Stunden] definiert ist und der Betrag nicht null ist.</p><p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Übersicht über die Fertigstellung des Projekts</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatische Festlegung der Projektbedingung auf der Grundlage des Fortschrittsstatus]</td> 
   <td> <p>Diese Voreinstellung ermöglicht es Benutzern, die [!UICONTROL-Bedingung] eines Projekts manuell auf ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) oder die automatische Festlegung der [!UICONTROL-Bedingung] (Fortschrittsstatus) anhand des Projektfortschritts auf der Timeline auf [!DNL Workfront] festzulegen. Weitere Informationen zur Bedingung von Projekten finden Sie unter <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Überblick über Projektbedingungen und Bedingungstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Grundlinien automatisch erstellen]</p> </td> 
   <td> <p>Diese Voreinstellung erstellt automatisch eine Grundlinie (Momentaufnahme) der Aufgaben- und Projektdetails, wenn sich der Status des Projekts in [!UICONTROL Aktuell] ändert. Informationen zum Erstellen von Grundlinien finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Erstellen von Projekt-Grundlinien</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Leistungsindex-Methode] </p> </td> 
   <td> <p>Die Leistungsindex-Methode (PIM) für das Projekt steuert die Methode, die [!DNL Workfront] zur Berechnung von Earned Value-Metriken wie [!UICONTROL Cost Performance Index] (CPI) und [!UICONTROL Estimate At Complete] (EAC) verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Berechnen des [!UICONTROL Cost Performance Index] (CPI)</a> und <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Schätzung nach Abschluss berechnen] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Stunden]</strong>: [!DNL Workfront] verwendet [!UICONTROL Plante Stunden] zur Berechnung von Leistungsmetriken wie EAC und CPI. Wenn die PIM auf der Grundlage von Stunden berechnet wird, wird die EAC als Anzahl von Stunden angezeigt. Stellen Sie sicher, dass Sie einen anderen Wert als null für [!UICONTROL Geplante Stunden] haben.</li> 
     <li> <p><strong>[!UICONTROL Kostenbasiert]</strong>: [!DNL Workfront] verwendet [!UICONTROL Planete Arbeitskosten] zur Berechnung von Leistungsmetriken wie EAC und CPI. Stellen Sie sicher, dass Ihre Arbeitsplatzrollen oder -benutzer den Kosten pro Stunde zugeordnet sind. Wenn der PIM auf der Grundlage von Kosten berechnet wird, wird der EAC als Währungswert angezeigt.</p> <p>Der Projektmanager kann diese Einstellung auf Projektebene ändern, indem er den Bereich [!UICONTROL Finance] in [!UICONTROL Projektdetails] verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Projekt [!UICONTROL Finance]-Bereich</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schätzung bei Abschluss ]</p> </td> 
   <td> <p>Bestimmen Sie, welche Daten [!DNL Workfront] zur Berechnung der [!UICONTROL Schätzung bei Abschluss] (EAC) verwendet, die die voraussichtlichen Gesamtkosten eines Projekts darstellt.</p> 
    <ul> 
     <li><strong>[!UICONTROL Auf Projektebene berechnen]</strong>: Die EAC für die übergeordnete Aufgabe und das Projekt wird durch Eingabe von [!UICONTROL Tatsächliche Stunden] oder [!UICONTROL Tatsächliche Arbeitskosten] in die EAC-Formeln bestimmt. Diese Berechnung umfasst [!UICONTROL Tatsächliche Stunden] oder [!UICONTROL Kosten und Ausgaben], die direkt zur übergeordneten Aufgabe oder Projekt hinzugefügt werden.</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>: Die EAC für die übergeordnete Aufgabe und das Projekt wird durch Addition der EAC für jede untergeordnete Aufgabe bestimmt. Bei dieser Berechnung werden [!UICONTROL Tatsächliche Stunden] oder [!UICONTROL Tatsächliche Kosten und Ausgaben] ausgeschlossen, die direkt zur übergeordneten Aufgabe oder Projekt hinzugefügt werden.</p> <p>Der Projektmanager kann diese Einstellung auf Projektebene ändern, indem er den Bereich [!UICONTROL Finance] in [!UICONTROL Projektdetails] verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Informationen im Bereich [!UICONTROL Finance] des Projekts verwalten</a>.</p> </li> 
    </ul> <p>Weitere Informationen zur Berechnung der EAC finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Berechnung der [!UICONTROL Schätzung bei Abschluss] (EAC)</a>.</p> </td> 
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
   <td> <p>Bestimmen Sie, ob neue Projekte ab dem Startdatum oder ab dem Abschlussdatum geplant werden, wenn sie erstellt werden.</p> 
    <ul> 
     <li><strong>[!UICONTROL Startdatum]</strong>: Neue Aufgaben werden standardmäßig auf die [!UICONTROL Aufgabenkonbeschränkung gesetzt, und Projektmanager werden aufgefordert, ein [!UICONTROL Geplantes Startdatum] für das Projekt anzugeben.</li> 
     <li><strong>[!UICONTROL Abschlussdatum]</strong>: Für neue Aufgaben wird standardmäßig die [!UICONTROL Task-Beschränkung so spät wie möglich] festgelegt. Projektmanager werden aufgefordert, ein [!UICONTROL Geplantes Abschlussdatum] für das Projekt anzugeben.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Bestimmen Sie, ob durch die Zeitabstände des Primären Verantwortlichen einer Aufgabe die für diese Aufgabe geplanten Zeitpunkte für ein Projekt angepasst werden.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Anwenderzeit in Aufgabendauern berücksichtigen]</strong>: Durch jede für den Primären Verantwortlichen einer Aufgabe geplante Zeitüberschreitung werden die geplanten Zeitpunkte der Aufgabe angepasst, wenn die Zeitdauer während der Aufgabendauer abgelaufen ist. Dies ist die Standardeinstellung. </p> <p>Wenn beispielsweise eine Aufgabe mit einer Beschränkung von [!UICONTROL So bald wie möglich] am 1. Juni beginnen und am 3. Juni abgeschlossen sein soll und der Primäre Verantwortliche den 2. Juni für die Zeitüberschreitung markiert hat, werden die geplanten Termine der Aufgabe auf den 1. bis 4. Juni angepasst.</p> <p><b>WICHTIG</b>:</p> <p>Die Dauer der Aufgabe ändert sich bei Auswahl dieser Einstellung nicht. Je nach Aufgabenbegrenzung ändern sich nur die geplanten Datumswerte.</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task duration]</strong>: Die geplanten Termine jeder Aufgabe eines Projekts bleiben wie ursprünglich geplant, auch wenn der Primäre Verantwortliche einer Aufgabe während ihrer Dauer eine Zeitverzögerung hat.</li> 
    </ul> <p>Beachten Sie bei der Auswahl der Optionen für diese Einstellung Folgendes:</p> 
    <ul> 
     <li>Wenn Sie diese Einstellung ändern, übernehmen nur die nach der Änderung erstellten Projekte und Vorlagen die aktualisierte Einstellung. </li> 
     <li> <p>Der Wert der Aufgabenbegrenzung bestimmt, welche geplanten Aufgabendaten angepasst werden sollen: </p> 
      <ul> 
       <li>Das geplante Startdatum</li> 
       <li>Das geplante Abschlussdatum</li> 
       <li>Beide Datumsangaben</li> 
       <li>Keines der beiden Datum. </li> 
      </ul> <p>Wenn eine Aufgabe beispielsweise die Begrenzung [!UICONTROL Feste Datumswerte] aufweist, werden die Daten nicht angepasst, wenn der Primäre Verantwortliche eine Zeitverzögerung hat, selbst wenn die Option [!UICONTROL Benutzerzeitlimit in Aufgabendauer berücksichtigen] ausgewählt ist. Informationen zu Aufgabenbegrenzungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Aufgabenbegrenzungen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Projektzeitpläne werden automatisch neu berechnet]</p> </td> 
   <td> <p>Bestimmen Sie, wann die Timeline eines Projekts neu berechnet wird. Weitere Informationen zur Neuberechnung der Projekt-Timeline finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projekt-Timeline neu berechnen</a>.</p> <p>Die folgenden Optionen sind standardmäßig aktiviert. Sie können eine oder mehrere der folgenden Einstellungen auswählen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Jede Nacht]</strong>: Wählen Sie diese Option aus, um die Projektzeitpläne jede Nacht neu zu berechnen. Änderungen, die Sie am Projekt vornehmen und die sich auf die Timeline auswirken können, sind nicht sofort sichtbar. [!DNL Workfront​​​] berechnet die Zeitpläne nur bei Projekten nachts neu, bei denen beide der folgenden Bedingungen erfüllt sind:</p> <p> 
       <ul> 
        <li>Status von [!UICONTROL Aktuell]</li> 
        <li>In den letzten drei Monaten wurde ein Update durchgeführt</li> 
        <li>Sie hatten einen Aktualisierungstyp von einem der folgenden:</li>
        <ul>
        <li>Automatisch UND bei Änderung</li>
        <li>Nur Änderung</li>
        <li>Nur automatisch</li> 
      </ul>       
    <b>TIPP:</b>
    <p>Projekte mit dem Aktualisierungstyp "Nur Manuell"sind von dieser Einstellung nicht betroffen.</p>
    <li> <p><strong>Wenn sich der Umfang eines Projekts ändert</strong>: Wählen Sie diese Option aus, um die Projekt-Timelines unmittelbar bei einer Änderung des Projektumfangs neu zu berechnen. Informationen dazu, was eine Änderung des Projektumfangs darstellt, finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projektzeitpläne neu berechnen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Wenn mehrere Benutzer einer Aufgabe zugewiesen sind, verwenden Sie den Zeitplan des]</p> </td> 
   <td> <p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern kein Zeitplan zugewiesen wurde, verwendet [!DNL Workfront] den standardmäßigen Systemzeitplan zur Berechnung der Zeitleiste der Aufgaben.</p> <p>Wenn Sie mehrere Benutzer derselben Aufgabe in einem Projekt zuweisen und dem Projekt ein Zeitplan zugewiesen ist und den den Aufgaben zugewiesenen Benutzern auch ein Zeitplan zugewiesen ist, verwendet [!UICONTROL Workfront] die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>[!UICONTROL Primäre Zuweisung]</strong>: [!DNL Workfront] verwendet den Zeitplan der Primären Zuweisung für die Aufgabe zur Berechnung der Zeitpläne.</li> 
     <li><strong>[!UICONTROL Projekt]</strong>: [!DNL Workfront] verwendet den Zeitplan des Projekts zur Berechnung der Zeitleiste jeder Aufgabe.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p><span class="preview">Wenn eine Benutzerin bzw. ein Benutzer einer Aufgabe zugeteilt ist, den Zeitplan verwenden von …</span></p> </td> 
   <td> <div class="preview">
<p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern kein Zeitplan zugewiesen wurde, verwendet [!DNL Workfront] den standardmäßigen Systemzeitplan zur Berechnung der Zeitleiste der Aufgaben.</p>

<p>Wenn Sie einen Benutzer einer Aufgabe in einem Projekt zuweisen und sowohl dem Projekt als auch dem den Aufgaben zugewiesenen Benutzer Zeitpläne zugeordnet sind, verwendet [!UICONTROL Workfront] die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>[!UICONTROL Benutzer]</strong>: [!DNL Workfront] verwendet den Zeitplan des zugewiesenen Benutzers für die Aufgabe zur Berechnung der Zeitleisten.</li> 
     <li><strong>[!UICONTROL Projekt]</strong>: [!DNL Workfront] verwendet den Zeitplan des Projekts zur Berechnung der Zeitleiste der Aufgabe.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p>
</div></td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline-Berechnungen] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typische Stunden pro Arbeitstag]</strong>: Legen Sie die Anzahl der Stunden an einem typischen Arbeitstag für die Benutzer fest, die an Projekten arbeiten werden. Der Standardwert ist 8 Stunden.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Typische Arbeitstage pro Woche]</strong>: Legen Sie die standardmäßige Arbeitswoche für die Benutzer fest, die an Projekten arbeiten. Der Standardwert ist 5 Tage.</li> 
    </ul> <p>Diese beiden Optionen konvertieren Tage in Stunden oder Wochen in Tage.</p> <p>Wenn Sie beispielsweise eine Aufgabe mit 8 geplanten Stunden haben und die Dauer auf der Grundlage geplanter Stunden berechnet wird, wandelt [!DNL Workfront] diese Stunden in Tage um, um die Dauer als Tage anzuzeigen.</p> <p>Im Feld Typische [!UICONTROL Arbeitstage pro Woche] berechnet [!DNL Workfront] den Wert des Vollzeitäquivalents (FTE) für Ihr System. Dies wird von [!DNL Workfront] bei der Berechnung der Zuordnung für Benutzer verwendet.</p> <p>Diese Werte werden verwendet, wenn Sie Zeitpläne für Projekte planen, Ressourcen in den Budgets einplanen oder die Zeit für die Projektabwicklung einplanen. </p> <p>Sie werden nicht verwendet, wenn Sie Timesheets für Benutzer im System erstellen, wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Konfigurieren] Timesheet- und Stundenvoreinstellungen</a> beschrieben.</p> <p><b>NOTE</b>:</p> <p>[!DNL Workfront] -Administratoren können die Voreinstellungen für [!UICONTROL Timeline-Berechnungen] nicht entsperren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Benutzerdefinierte Quartal]</p> </td> 
   <td> <p>Konfigurieren Sie benutzerdefinierte Jahresquartale für die Benutzer, die an Projekten arbeiten werden. Benutzerdefinierte Quartale sind in der Regel Quartale, die nicht mit der herkömmlichen Verteilung der Quartale in einem Kalenderjahr übereinstimmen. Sie können mehrere benutzerdefinierte Quartale hinzufügen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Quartale für Projekte aktivieren</a>.</p>  <p><b>NOTE</b>: </p><p>[!DNL Workfront] -Administratoren können die Voreinstellungen von [!UICONTROL Benutzerdefinierte Quartal] nicht entsperren.</p> </td> 
  </tr> 
 </tbody> 
</table>








### [!UICONTROL Geschäftsszenarios] {#business-cases}

Sie können im gesamten System ein Business Case für neu erstellte Projekte erstellen, um Projektanforderungen einzureichen. Sie können Voreinstellungen definieren, um festzulegen, welche Bereiche im Formular **[!UICONTROL Geschäftsszenario]** sichtbar sind. Es wird empfohlen, diese Optionen zu aktivieren, damit andere Tools wie der [!UICONTROL Portfolio Optimizer] ordnungsgemäß aktualisiert werden. Weitere Informationen dazu, was die einzelnen Felder anzeigen, finden Sie unter [Definieren eines Geschäftsfalls: Artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nachdem der [!DNL Workfront] -Administrator die Abschnitte im [!UICONTROL Geschäftsszenario] aktiviert hat, kann ein Projektinhaber dann einen Geschäftsfall auf Projektebene erstellen. Informationen zum Erstellen eines Geschäftsfeldes finden Sie unter [Erstellen eines Geschäftsfeldes für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Lebensdauer nach Tod] {#life-after-death}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte im gesamten System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nachdem ein Projekt als abgeschlossen markiert wurde, können noch Personen] </p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) dahingehend fest, ob eine Aufgabe oder ein Problem gelöscht werden kann, nachdem der Projektstatus mit [!UICONTROL Complete] gekennzeichnet wurde.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aufgaben löschen]</strong>: Ermöglicht Benutzern das Löschen von Aufgaben aus einem Projekt, nachdem das Projekt als [!UICONTROL Abgeschlossen] gekennzeichnet wurde.<br></li> 
     <li><strong>[!UICONTROL Löschprobleme]</strong>: Ermöglicht Benutzern das Löschen von Problemen aus einem Projekt, nachdem das Projekt als [!UICONTROL Abgeschlossen] gekennzeichnet wurde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nachdem ein Projekt als "Abgeschlossen", "Dead"oder "Ausstehende Genehmigung"markiert wurde, können Personen dennoch]</p> </td> 
   <td> <p>Legen Sie die Regeln für Ihr Unternehmen (oder Ihre Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, die festlegen, was mit Aufgaben, Problemen, Dokumenten und anderen Objekten in einem Projekt geschieht, nachdem der Projektstatus mit "<strong>[!UICONTROL Complete]</strong>", "<strong>[!UICONTROL Dead]</strong>"oder "<strong>[!UICONTROL Ausstehende Genehmigung]</strong>" markiert wurde.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aufgaben hinzufügen und bearbeiten]</strong> Ermöglicht Benutzern Folgendes:
      <ul>
       <li>Bearbeiten Sie Aufgaben innerhalb eines Projekts, nachdem das Projekt mit [!UICONTROL Complete], [!UICONTROL Dead] gekennzeichnet wurde oder [!UICONTROL Pending Approval] lautet. Dazu gehören das Hinzufügen von Stunden und das Ändern von Ausgabeneinträgen für eine Aufgabe.</li>
       <li>Aufgaben zu einem Projekt hinzufügen.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Probleme hinzufügen und bearbeiten]</strong>: Ermöglicht Benutzern Folgendes:
      <ul>
       <li>Bearbeiten Sie Probleme innerhalb eines Projekts, nachdem das Projekt mit [!UICONTROL Complete], [!UICONTROL Dead] oder [!UICONTROL Pending Approval] gekennzeichnet wurde.</li>
       <li>Fügen Sie einem Projekt Probleme hinzu, nachdem das Projekt mit [!UICONTROL Complete] oder [!UICONTROL Dead] gekennzeichnet wurde. (Sie können einem Projekt mit dem Status [!UICONTROL Ausstehende Genehmigung] keine Probleme hinzufügen.)</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Dokumente zum Projekt und seinen Aufgaben und Problemen hinzufügen]</strong>: Ermöglicht Benutzern das Hinzufügen von Dokumenten zu einem Projekt (oder das Hinzufügen von Dokumenten zu Aufgaben und Problemen innerhalb des Projekts), nachdem das Projekt mit [!UICONTROL Complete] oder [!UICONTROL Dead] gekennzeichnet wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>: Ermöglicht Benutzern, Vorlagen an ein Projekt anzuhängen, nachdem das Projekt als [!UICONTROL Complete] oder [!UICONTROL Dead] markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
