---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben bearbeiten
description: Sie können Informationen zu Aufgaben bearbeiten, die Sie erstellt haben oder für die Sie Beitragsberechtigungen oder Verwaltungsberechtigungen besitzen.
author: Alina
feature: Work Management
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: f8d596121f90d4f0c57e65cc415d1df87c14730c
workflow-type: tm+mt
source-wordcount: '3711'
ht-degree: 4%

---

# Aufgaben bearbeiten

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


Sie können Informationen zu Aufgaben bearbeiten, die Sie erstellt haben oder für die Sie Beitragsberechtigungen oder Verwaltungsberechtigungen besitzen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <ul> 
     <li> <p>Beitragen Sie Berechtigungen zu einer Aufgabe, um sie im Bereich "Aufgabendetails"zu bearbeiten </p> </li> 
     <li> <p>Berechtigungen für eine Aufgabe verwalten, um sie im Feld "Aufgabe bearbeiten"zu bearbeiten</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Beitragen oder höhere Berechtigungen zum Projekt</p> </li> 
    </ul> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Einschränkungen bei der Bearbeitung von Aufgaben

Es gibt einige Einschränkungen, die Sie daran hindern können, Aufgaben zu bearbeiten.

Beachten Sie beim Bearbeiten von Aufgaben Folgendes:

* Aktualisieren von Benachrichtigungen für Trigger zu Aufgaben, die einen aktuellen Status aufweisen. Um Verwirrung bei Benutzern zu vermeiden, die den Aufgaben zugewiesen sind, begrenzen Sie Bearbeitungsaufgaben so weit wie möglich, wenn das Projekt den Status Aktuell aufweist.
* Sie können keine Aufgaben bearbeiten, die sich in einem Genehmigungsprozess befinden. Sie können die Zeit nur protokollieren oder den Status einer Aufgabe in einem Genehmigungsprozess aktualisieren.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Sie können Dokumente nur dann bearbeiten und Aufgaben in einem Projekt hinzufügen, für das der Status &quot;Abgeschlossen&quot;, &quot;Dead&quot;oder &quot;Ausstehende Genehmigung&quot;lautet, wenn der Workfront-Administrator oder ein Gruppenadministrator diese Funktion im Bereich &quot;Projekteinstellungen&quot;aktiviert hat. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Sie können die folgenden Informationen zu einer Aufgabe jederzeit bearbeiten, wenn das Projekt als abgeschlossen, ungültig oder in einem Genehmigungsprozess markiert wurde:

   * Protokollzeit
   * Bestehende Ausgaben bearbeiten
   * Benutzerdefiniertes Formular anhängen

## Aufgabe in einer Liste bearbeiten

Sie können Aufgabeninformationen in einer Liste von Aufgaben bearbeiten, indem Sie in der Ansicht der Liste angezeigte Inline-Bearbeitungsfelder verwenden.

Informationen zum Bearbeiten von Aufgaben in Listen finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Bearbeiten einer Aufgabe in einer Liste mithilfe der Zusammenfassung

Sie können eine Aufgabe in einer Liste über das Bedienfeld &quot;Zusammenfassung&quot;bearbeiten. Informationen zum Bearbeiten einer Aufgabe im Bereich &quot;Zusammenfassung&quot;finden Sie im Abschnitt &quot;Aufgabe in der Zusammenfassung bearbeiten&quot;im [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) Artikel.

## Bearbeiten einer Aufgabe im Feld &quot;Aufgabe bearbeiten&quot;

Sie können eine Aufgabe in den Bereichen Aufgabe bearbeiten oder Aufgabendetails bearbeiten. Die folgenden Schritte beschreiben die Bearbeitung einer Aufgabe im Feld &quot;Aufgabe bearbeiten&quot;.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Projekte** und klicken Sie auf den Namen eines Projekts, um es zu öffnen.
1. Klicken **Aufgaben** im linken Bereich.
1. Klicken Sie auf die Aufgabe, die Sie bearbeiten möchten.
1. (Bedingt) Um beschränkte Informationen über eine Aufgabe zu bearbeiten, klicken Sie als Benutzer mit Beitragsberechtigungen für die Aufgabe auf **Aufgabendetails** im linken Bereich.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Bearbeiten Sie Informationen in den folgenden Bereichen im Abschnitt Aufgabendetails :

   * **Übersicht**

     Dieser Bereich wird standardmäßig erweitert.

   * **Benutzerdefinierte Formulare**

     Namen von Zollformularen werden nur angezeigt, wenn benutzerdefinierte Formulare an das Objekt angehängt sind.

   * **Finanzielle Details**

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layout-Vorlage geändert hat, werden die Felder im Bereich &quot;Aufgabendetails&quot;möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Informationen zu den Feldern, die im Abschnitt &quot;Aufgabendetails&quot;angezeigt werden, erhalten Sie, wenn Sie die Aufgabe im Feld &quot;Aufgabe bearbeiten&quot;bearbeiten möchten, wie unten beschrieben.

   Gehen Sie wie folgt vor, um Informationen im Abschnitt Details zu bearbeiten:

   1. (Optional) Klicken Sie auf die **Alle reduzieren** icon ![](assets/collapse-all-icon.png) in der oberen rechten Ecke, um alle Bereiche zu reduzieren.
   1. (Optional und bedingt) Wenn ein Bereich ausgeblendet wird, klicken Sie auf die Schaltfläche **Rechtspfeil** ![](assets/right-pointing-arrow.png) neben jedem Bereich, um den Bereich zu erweitern, den Sie bearbeiten möchten.
   1. Weitere Informationen zum Bearbeiten von Informationen auf der Registerkarte &quot;Aufgabendetails&quot;finden Sie in den folgenden Artikeln:

      * [Verwalten von Aufgabeninformationen im Bereich &quot;Aufgabendetails - Übersicht&quot;](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Verwalten von Aufgabenfinanzen im Abschnitt &quot;Aufgabendetails&quot;](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Optional) Wenn keine benutzerdefinierten Formulare an die Aufgabe angehängt sind, beginnen Sie mit der Eingabe des Namens eines Formulars im **Benutzerdefiniertes Formular hinzufügen** und wählen Sie es aus, wenn es in der Liste angezeigt wird, und klicken Sie dann auf **Änderungen speichern**.
   1. (Optional) Klicken Sie auf die **Export** icon ![](assets/export.png) , um die Übersicht und die benutzerdefinierten Formulardaten in eine PDF-Datei zu exportieren, und klicken Sie dann auf **Export**. Wählen Sie aus den folgenden Optionen aus:

      * Alle auswählen (wird nur angezeigt, wenn mindestens ein benutzerdefiniertes Formular angehängt ist)
      * Übersicht
      * Der Name eines oder mehrerer benutzerdefinierter Formulare

      Die PDF-Datei wird auf Ihren Computer heruntergeladen.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Weitere Informationen finden Sie unter [Exportieren benutzerdefinierter Formulare und Objektdetails](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Bedingt) Um alle Informationen über die Aufgabe zu bearbeiten, klicken Sie als Benutzer mit Verwaltungsberechtigungen für die Aufgabe auf die **Mehr** Menü ![](assets/more-icon.png) neben dem Namen der Aufgabe klicken Sie auf **Bearbeiten**.

   Oder

   Wählen Sie aus einer Aufgabenliste eine Aufgabe aus und klicken Sie auf die Schaltfläche **Bearbeiten** icon ![](assets/edit-icon.png) oben in der Liste.

   Das Feld Aufgabe bearbeiten wird geöffnet.

   >[!IMPORTANT]
   >
   >Sie müssen über Verwaltungsberechtigungen für die Aufgabe verfügen, damit die Option &quot;Bearbeiten&quot;angezeigt wird.

   Alle Aufgabenfelder sind im Feld Aufgabe bearbeiten verfügbar und werden nach den im linken Bereich aufgelisteten Bereichen gruppiert.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layout-Vorlage geändert hat, werden die Felder im Bereich &quot;Aufgabendetails&quot;möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Ziehen Sie in Erwägung, Informationen in einem der folgenden Abschnitte anzugeben:

   * [Aufgabenname](#task-name)
   * [Übersicht](#overview)
   * [Arbeitsaufträge](#assignments)
   * [Benutzerdefinierte Formulare](#Custom%C2%A0F)
   * [Finanzielle Details](#finance)
   * [Einstellungen](#settings)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator unsere Layout-Vorlage einrichtet, werden die Felder im Feld &quot;Aufgabe bearbeiten&quot;möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Aufgabenname {#task-name}

1. Beginnen Sie mit der Bearbeitung Ihrer Aufgabe wie oben beschrieben.
1. Klicken **Aufgabenname** im linken Bereich.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Aktualisieren Sie den Namen der Aufgabe.

1. Klicken **Speichern** oder fahren Sie mit den folgenden Abschnitten fort.

### Übersicht {#overview}

1. Beginnen Sie mit der Bearbeitung Ihrer Aufgabe wie oben beschrieben.
1. Klicken **Übersicht** im linken Bereich.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Aktualisieren Sie die folgenden Informationen zur Aufgabe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Fügen Sie zusätzliche Informationen zur Aufgabe hinzu. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Abschnitt mit grundlegenden Informationen</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Wählen Sie den Status der Aufgabe aus, der angibt, in welcher Entwicklungsphase sich die Aufgabe befindet.</p> <p><b>TIPP</b>

   Sie können den Aufgabenstatus in der Aufgabenkopfzeile aktualisieren. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Priorität</td> 
      <td> <p>Dies ist eine visuelle Markierung für Sie, mit der Sie Ihre Aufgaben priorisieren können. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
      <li> <p> Keine</p> </li> 
      <li> <p> Niedrig </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Hoch </p> </li> 
      <li> <p> Dringend </p> </li> 
       </ul> <p>Je nach den von Ihrem Workfront-Administrator ausgewählten Projekteinstellungen können die Prioritätsnamen für Sie unterschiedlich sein. Weitere Informationen zu Aufgabenprioritäten finden Sie unter <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Aktualisieren der Aufgabenpriorität</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Abschnitt "Aufgabendaten und Einschränkungen"</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabenbeschränkung</td> 
      <td> <p>Entscheiden Sie, wann die Aufgabe abgeschlossen sein muss, indem Sie eine Aufgabenbegrenzung angeben. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
      <li> <p><span>Feste Daten</span> </p> <p>Geben Sie eine <strong>Geplanter Start</strong> und <strong>Geplantes Abschlussdatum</strong>. </p> </li> 
      <li> <p><span>Muss beginnen am</span> </p> <p>Geben Sie eine <strong>Geplantes Startdatum</strong>. </p> </li> 
      <li> <p><span>Muss beendet werden am</span> </p> <p>Geben Sie eine <strong>Geplantes Abschlussdatum</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>So bald wie möglich</span></p> </li> 
      <li> <p><span>So bald wie möglich</span></p> </li> 
      <li> <p><span>Frühestmögliche Zeit</span></p> </li> 
      <li> <p> <span>Spätestmögliche Zeit</span></p> </li> 
      <li> <p><span>Nicht später anfangen als</span> </p> </li> 
      <li> <p>Angeben eines geplanten Startdatums</p> </li> 
      <li> <p><span>Nicht früher anfangen als</span> </p> <p>Geben Sie eine <strong>Geplantes Startdatum</strong>. </p> </li> 
      <li> <p> Beenden <span>Nicht später als</span></p> <p>Geben Sie eine <strong>Geplantes Abschlussdatum</strong>. </p> </li> 
      <li> <p> Beenden <span>Keine frühere als</span></p> <p>Geben Sie eine <strong>Geplantes Abschlussdatum</strong></p> </li> 
       </ul> <p>Weitere Informationen zur Aufgabenbegrenzung finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbegrenzungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datum und Uhrzeit der Veröffentlichung</td> 
      <td> <p>Dies ist das Datum, bis zu dem der Aufgabe zugewiesene Benutzer verpflichtet, sie abzuschließen. Dies kann sich vom geplanten Abschlussdatum unterscheiden. Nur Beauftragte können dieses Feld bearbeiten. Weitere Informationen zum Festlegen von Datumswerten in Workfront finden Sie unter <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Datum bestätigen - Übersicht</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Startdatum und geplante Startzeit</td> 
      <td> <p>Wann die Aufgabe beginnen soll. Das geplante Startdatum einer Aufgabe wird durch eine Reihe von Faktoren bestimmt und beeinflusst:</p> 
       <ul> 
      <li>Je nach systemweiter Voreinstellung für das geplante Startdatum der Aufgabe kann das Anfangsdatum einer neuen Aufgabe für ein Projekt entweder heute oder standardmäßig das Anfangsdatum des Projekts sein. <span>Der Gruppenadministrator für die mit dem Projekt verknüpfte Gruppe kann diese Voreinstellung auch für die Gruppe festlegen.</span> Weitere Informationen zu den Aufgabenvoreinstellungen auf Systemebene oder Gruppenebene finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Systemweite Aufgaben- und Problemeinstellungen konfigurieren</a>.</li> 
      <li>Je nach den Vorgängern der Aufgabe wählt Workfront das geplante Startdatum als nächstes Verfügbarkeitsdatum aus, nachdem die Vorgängerbeziehung beendet oder begonnen hat. Weitere Informationen zu Vorgängerbeziehungen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Übersicht über die Vorgänger von Aufgaben</a>.</li> 
      <li>Der Projektmanager oder Aufgabenbesitzer kann das geplante Startdatum manuell festlegen, wenn die Aufgabenbegrenzung entweder "Feste Datumswerte"oder "Muss am"lautet. Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbegrenzungen</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Abschlussdatum und -zeit</td> 
      <td> <p>Das erwartete Abschlussdatum, wie zum Zeitpunkt der Aufgabenplanung angezeigt. Das geplante Abschlussdatum kann anhand mehrerer Faktoren festgelegt werden:</p> 
       <ul> 
      <li>Das geplante Abschlussdatum wird ausgehend vom geplanten Startdatum berechnet, indem die Dauer der Aufgabe zum geplanten Startdatum hinzugefügt wird. Wenn der Projektmanager oder Workfront die Dauer der Aufgabe angibt, kann dieser Trigger das geplante Abschlussdatum aktualisieren. Wenn sich das geplante Datum ändert, liegt dies häufig daran, dass die Dauer der aktualisiert wurde.</li> 
      <li>Der Projektmanager oder Aufgabenbesitzer kann das geplante Abschlussdatum manuell festlegen, wenn die Aufgabenbegrenzung entweder "Feste Datumswerte"oder "Muss abgeschlossen am"lautet. Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbegrenzungen</a>.</li> 
      <li>Wenn sich der Dauer-Typ der Aufgabe ändert und sich die Anzahl der Ressourcen für die Aufgaben gleichzeitig ändert, ändert sich auch das geplante Abschlussdatum. Weitere Informationen zu Dauer-Typen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und -dauer</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliches Startdatum und -zeitpunkt</td> 
      <td> <p>Geben Sie ein tatsächliches Startdatum für die Aufgabe an. Der Standardwert wird normalerweise automatisch ausgefüllt, wenn Sie den Status der Aufgabe in "Wird ausgeführt"ändern. Das tatsächliche Startdatum kann auch vom Projektmanager oder Aufgabenbesitzer manuell geändert werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datum und Uhrzeit des tatsächlichen Abschlusses</td> 
      <td> <p>Geben Sie das Datum und die Uhrzeit an, zu der die Aufgabe abgeschlossen ist. Das Standarddatum und die Standardzeit, zu der eine Aufgabe abgeschlossen wird, entsprechen immer dem Zeitpunkt, zu dem der Status Abgeschlossen wird. Das tatsächliche Abschlussdatum kann auch manuell vom Projektmanager oder Aufgabenbesitzer geändert werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Arbeitszeitabschnitt</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Work Effort </td> 
      <td>

   <p>Der für die Ausführung der Aufgabe erforderliche Arbeitsaufwand. Ihr Projektmanager kann beschließen, dieses Feld anstelle von "Geplante Stunden"zu verwenden, um den für die Erfüllung einer Aufgabe erforderlichen Aufwand abzuschätzen. Dieses Feld ist nur sichtbar, wenn die folgenden Bedingungen erfüllt sind:</p> 
      <ul> 
      <li> <p>Die Aufgabe hat einen einfachen Dauerhaltungstyp. </p> <p><b>TIPP</b>

   Wenn Sie den Aufgabentyp ändern, wird dieses Feld abgeblendet. </p> </li>
   <li>Ihr Projektmanager hat die Option "Use Work Effort"aktiviert, um die Aufgabe "Geplante Stunden"für das Projekt automatisch zu berechnen. </li> 
      </ul> 
      <p>Wählen Sie aus den folgenden Optionen aus:</p> 
      <ul> 
      <li>Klein</li> 
      <li>Mittel <span style="font-weight: normal;">(dies ist der Standardwert für eine neue Aufgabe)</span></li> 
      <li>Groß</li> 
      </ul> 
      <p><b>NOTIZ</b>

   Durch die Aktualisierung des Aufwands kann die Aufgabe &quot;Geplante Stunden&quot;aktualisiert werden. Die Aktualisierung ist sofort möglich, wenn der Projektaktualisierungstyp Automatisch ist. Wenn der Projektaktualisierungstyp manuell ist, müssen Sie die Timeline neu berechnen, um die aktualisierten geplanten Stunden anzuzeigen. </p>

   <p>Informationen zur Verwendung von "Arbeitsaufwand"anstelle von "Geplante Stunden"zur Schätzung des Aufgabenaufwands finden Sie unter <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Speichern** oder fahren Sie mit den folgenden Abschnitten fort.

### Arbeitsaufträge {#assignments}

1. Beginnen Sie mit der Bearbeitung Ihrer Aufgabe wie oben beschrieben.
1. Klicken **Zuweisungen** im linken Bereich.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Klicken **Suchen nach Personen, Rollen und Teams** und geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie der Aufgabe zuweisen möchten, und klicken Sie dann auf die Aufgabe oder drücken Sie die Eingabetaste , wenn sie in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Wenn der Name des Benutzers ein Sonderzeichen enthält, müssen Sie das Sonderzeichen in das Suchfeld einfügen.

   >[!TIP]
   >
   >Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
   >
   >Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
   >
   >* Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
   >* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.

1. (Optional) Geben Sie durch Auswahl der **Inhaber** neben ihrem Namen. Ein Team kann nicht der Hauptverantwortliche einer Aufgabe sein.
1. (Bedingt und optional) Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Dauertyp</td> 
      <td> <p>Dadurch wird die Beziehung zwischen folgenden Elementen identifiziert: </p> 
       <ul> 
      <li> <p>Die Anzahl der Ressourcen, die einer Aufgabe zugewiesen sind </p> </li> 
      <li> <p>Der zum Abschließen der Aufgabe erforderliche Gesamtaufwand </p> </li> 
      <li> <p> Die Gesamtdauer der Aufgabe. </p> </li> 
       </ul> <p>Ihr Workfront-Administrator <span> oder einem Gruppenadministrator</span> wählt die standardmäßige Dauer-Typ -Einstellung für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>. </p> <p>Mit den Ereignistypen können Sie konsistente Ressourcenzuweisungen entsprechend den Anforderungen der Aufgabe festlegen. Weitere Informationen zum Dauer-Typ einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und -dauer</a>. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
      <li> <p>Berechnete Zuweisung </p> </li> 
      <li> <p> Berechnete Arbeit </p> </li> 
      <li> <p>Leistungsgesteuert </p> </li> 
      <li> <p>Einfach</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Dauer pro Termin</td> 
      <td> <p>Dies wird nur bei den übergeordneten wiederkehrenden Aufgaben angezeigt. Er zeigt die Dauer jeder wiederkehrenden Aufgabe an, wie sie bei der Erstellung der Aufgabe definiert wurde. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> <p> <b>NOTIZ</b>

   Die in einzelnen wiederkehrenden Aufgaben geänderten Zeiträume zeigen nicht den in diesem Feld angegebenen Wert an. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td> 
      <div> 
      <div> 
      <p>Dies ist der Zeitraum, in dem Sie einer Aufgabe erlauben, offen zu bleiben, bevor sie abgeschlossen wird. </p> 
      <p><b>WICHTIG</b>

   Da die Aufgabendauer normalerweise die Zeit zwischen dem geplanten Start und dem geplanten Abschlussdatum ist, wirkt sich dies auf die Zeitleiste des Projekts aus.</p>

   <p>Gehen Sie wie folgt vor, um die Dauer der Aufgabe und die Zeiteinheit anzugeben:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Geben Sie die Zeitdauer ein und wählen Sie aus den im Dropdown-Menü verfügbaren Zeiteinheiten aus.</p> <p><b>TIPP</b></p>
      Wenn Sie die Dauer von Aufgaben in einer Aufgabenliste aktualisieren, können Sie die Abkürzung für die Zeiteinheit verwenden. </p> </li> 
      </ul> 
      <p> In der folgenden Tabelle können Sie aus den Optionen für die reguläre Zeit oder die verstrichene Zeit auswählen: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Zeiteinheit</td> 
      <td>Abkürzung</td> 
      </tr> 
      <tr> 
      <td>Minuten</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Stunden</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Tage. Dies ist die Standardeinstellung. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Wochen</td> 
      <td>W </td> 
      </tr> 
      <tr> 
      <td>Monate</td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Verstrichene Minuten</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Verstrichene Stunden</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Verstrichene Tage</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Verstrichene Wochen</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Verstrichene Monate</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>NOTIZ</b>

   <p>Die verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und eine Verspätung umfasst. Mit anderen Worten, vergangene Zeit ist der Durchgang von Kalendertagen.

   Bei der regulären Zeit werden Feiertage, Wochenenden und eine Zeitüberschreitung berücksichtigt und von der Dauer der Aufgabe ausgeschlossen. Weitere Informationen zur Aufgabendauer finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und -dauer</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Geplante Stunden</td> 
   <td> <p>Geben Sie die Anzahl der geplanten Stunden für die Aufgabe in Stunden an. Dies ist die tatsächliche Zeit, die die Bevollmächtigten der Aufgabe benötigen würden, um sie abzuschließen. Sie können die Anzahl der geplanten Stunden für eine Aufgabe nur angeben, wenn für den Typ "Dauer"die Option "Berechnete Zuweisung"ausgewählt ist. Weitere Informationen zu Dauer-Typen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und -dauer</a>.</p> 
   <b>NOTIZ</b>
   <p>
   Bei der Erstellung wiederkehrender Aufgaben sind die geplanten Stunden die Aufgaben jedes Vorkommens. Die geplanten Stunden der übergeordneten Aufgaben entsprechen der Gesamtzahl aller geplanten Stunden von allen Vorkommen. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Zuteilung</td> 
   <td> <p>Wenn Ihre Aufgabenbegrenzung für berechnete Arbeit oder für anstrengende Arbeit gilt, geben Sie die <strong>Zuteilung %</strong> (Zuweisungsprozentsatz) für jeden Bevollmächtigten. Dies ist die Zeit ab dem Zeitplan des Bevollmächtigten, die er für diese Aufgabe verbringen kann. Wenn Sie den Zuordnungsprozentsatz für einen Verantwortlichen ändern, ändern sich die geplanten Stunden einer Aufgabe. </p> <p>Wenn die Aufgabenbegrenzung einfach ist, können Sie Folgendes angeben:</p> 
      <ul> 
      <li> <p>Zuweisungszeiten für jeden Bevollmächtigten.</p> </li> 
      <li> <p>Geplante Stunden der Aufgabe</p> </li> 
      <li> <p>Dauer der Aufgabe</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Rolle des Zugewiesenen</td> 
   <td> <p>Wählen Sie eine Rolle aus dem <strong>Rolle des Bevollmächtigten</strong> Dropdown-Menü, wenn Sie eine Person als Bevollmächtigten ausgewählt haben. Dies ist die Rolle, die der Bevollmächtigte für diese Aufgabe erfüllen kann. </p> <p><b>TIPP</b>

   Im Dropdown-Menü werden nur die mit jedem Bevollmächtigten in seinem Profil verknüpften Vorgangsrollen angezeigt.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Klicken **Speichern** oder fahren Sie mit den folgenden Abschnitten fort.

### Benutzerdefinierte Formulare

Sie können benutzerdefinierte Standardformulare definieren, die automatisch an Aufgaben angehängt werden, wenn die Aufgaben einem Projekt hinzugefügt werden. Informationen zum Einrichten des Projekts, um benutzerdefinierte Standardformulare für Aufgaben für alle neuen Aufgaben einzuschließen, finden Sie im Abschnitt &quot;Aufgaben&quot;im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Beginnen Sie mit der Bearbeitung der Aufgabe wie oben beschrieben.
1. Klicken **Benutzerdefinierte Forms** im linken Bereich oder klicken Sie auf den Namen eines benutzerdefinierten Formulars, falls es bereits angehängt ist.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Klicken **Benutzerdefiniertes Formular hinzufügen** und wählen Sie das benutzerdefinierte Formular oder die Formulare aus, die Sie mit der Aufgabe verknüpfen möchten. Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt.

   Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).Sie können einer Aufgabe bis zu zehn benutzerdefinierte Formulare hinzufügen.

1. (Bedingt) Wenn Sie ein benutzerdefiniertes Formular an die Aufgabe angehängt haben, bearbeiten Sie alle Felder im Formular. Sie müssen alle erforderlichen Felder angeben, bevor Sie die Aufgabe speichern können.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator die Berechtigungen für die Abschnitte in Ihrem benutzerdefinierten Formular festgelegt hat, können nicht alle die gleichen Felder in einem bestimmten benutzerdefinierten Formular anzeigen oder bearbeiten. Die Berechtigungen zum Bearbeiten von Feldern in einem Abschnitt eines benutzerdefinierten Formulars hängen von den Berechtigungen ab, die Sie für die Aufgabe selbst haben. Informationen zum Festlegen von Aufgabenberechtigungen finden Sie unter [Aufgabe freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Klicken **Speichern** oder fahren Sie mit den folgenden Abschnitten fort.

### Finanzielle Details {#finance}

1. Beginnen Sie mit der Bearbeitung Ihrer Aufgabe, wie im Abschnitt [Aufgaben bearbeiten](#Edit2) in diesem Artikel.
1. Klicken **Finanzen** im linken Bereich.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostenart</td> 
      <td> <p>Geben Sie den Kostentyp für die Aufgabe an. Auf diese Weise wird bestimmt, wie die Kosten der Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet werden. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p>Keine Kosten</p> </li> 
        <li> <p>Festgelegt pro Stunde </p> </li> 
        <li> <p> Benutzer pro Stunde </p> </li> 
        <li> <p> Stundensatz nach Funktion</p> </li> 
       </ul> <p>Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a> . Ihr Workfront-Administrator oder Gruppenadministrator wählt die Standardeinstellung für den Kostentyp für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Umsatztyp</td> 
      <td> <p>Geben Sie den Umsatztyp für die Aufgabe an. Auf diese Weise wird bestimmt, wie der Umsatz aus der Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet wird. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
      <li> <p> Nicht fakturierbar </p> </li> 
      <li> <p>Benutzer pro Stunde </p> </li> 
      <li> <p>Stundensatz nach Funktion </p> </li> 
      <li> <p>Festgelegt pro Stunde </p> </li> 
      <li> <p>Benutzer pro Stunde m/Obergrenze </p> </li> 
      <li> <p>Stundensatz nach Funktion m/Obergrenze </p> </li> 
      <li> <p>Benutzer pro Stunde plus festgelegt </p> </li> 
      <li> <p>Stundensatz nach Funktion plus fest </p> </li> 
      <li> <p>Festeinnahmen </p> </li> 
       </ul> <p>Weitere Informationen zur Umsatzverfolgung finden Sie unter<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a> . </p> <p>Ihr Workfront-Administrator oder Gruppenadministrator wählt die standardmäßige Einstellung "Umsatztyp"für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Speichern** oder fahren Sie mit dem folgenden Abschnitt fort.

### Einstellungen {#settings}

1. Beginnen Sie mit der Bearbeitung Ihrer Aufgabe, wie im Abschnitt [Aufgaben bearbeiten](#Edit2) in diesem Artikel.
1. Klicken **Einstellungen** im linken Bereich.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Überwachungsmodus</td> 
      <td> <p>Geben Sie an, wie der Fortschritt der Aufgabe verfolgt werden soll. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
      <li> <p> Benutzer muss aktualisieren </p> </li> 
      <li> <p>Zeitliche Annahme </p> </li> 
      <li> <p>Späte Warnungen ignorieren</p> </li> 
      <li> <p> Automatische Vervollständigung </p> </li> 
      <li> <p>Vorgänger </p> </li> 
       </ul> <p>Weitere Informationen zum Tracking-Modus für Aufgaben finden Sie unter <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Übersicht über den Task Tracking Mode</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenabgleich</td> 
      <td> <p>Wählen Sie die <strong>Aus Ressourcenebene ausschließen</strong> -Feld, wenn die der Aufgabe zugewiesenen Ressourcen von der Ebene ausgeschlossen werden sollen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abgleichsverzögerung</td> 
      <td> <p>Geben Sie die Verzögerung der Einstufung in Stunden an. </p> <p> Weitere Informationen zu Verzögerungen beim Leveln finden Sie unter <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Zeitverzögerung für Aufgabenebene aktualisieren</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td> <p>Wählen Sie einen Validierungsprozess aus, den Sie mit der Aufgabe verknüpfen möchten. Ihr Workfront-Administrator muss Validierungsprozesse auf Systemebene definieren, bevor Sie sie mit Aufgaben verknüpfen können. Benutzer mit Administratorzugriff auf Genehmigungsprozesse können auch gruppenspezifische Validierungsprozesse erstellen. </p> <p>Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>. Beachten Sie beim Hinzufügen von Validierungsprozessen Folgendes: </p> 
       <ul>

   <li> <p>In der Liste werden nur aktive Validierungsprozesse angezeigt. </p> </li>

   <li> <p>Systemweite und gruppenspezifische Validierungsprozesse werden in der Liste angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt. </p>

   <p><b>WICHTIG</b>

   Wenn sich die Gruppe des Projekts ändert, wird der zuvor angehängte gruppenspezifische Validierungsprozess zu einem Validierungsprozess für die einmalige Verwendung. Weitere Informationen dazu, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Validierungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>. </p>

   </li>

   <li> <p>Sie können Standardgenehmigungsverfahren definieren, die automatisch an Aufgaben angehängt werden, wenn die Aufgaben einem Projekt hinzugefügt werden. Weitere Informationen zum Einrichten des Projekts, um standardmäßige Aufgabengenehmigungsprozesse einzuschließen, finden Sie im Abschnitt "Aufgaben"im Artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projekte bearbeiten</a>. </p> </li>

   <li> <p>Bei der Massenbearbeitung gibt es die folgenden Szenarien: </p> 
      <ul> 
      <li> <p>Wenn Sie mehrere Aufgaben aus derselben Gruppe auswählen, werden in diesem Feld sowohl Validierungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt. </p> </li> 
      <li> <p>Wenn Sie mehrere Aufgaben aus verschiedenen Gruppen auswählen, werden in diesem Feld nur Validierungsprozesse auf Systemebene angezeigt. </p> </li> 
      <li> <p>Wenn an eine der Aufgaben ein Validierungsprozess für die einmalige Verwendung angehängt wird, wird dieser durch den von Ihnen ausgewählten Validierungsprozess auf Systemebene oder Gruppenebene ersetzt. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Klicken Sie auf **Speichern**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Bearbeiten einer Aufgabe in der Aufgabenkopfzeile (begrenzt)

Sie können eine begrenzte Anzahl von Informationen in der Aufgabenüberschrift bearbeiten.

Ihr System- oder Gruppenadministrator kann die in der Aufgabenüberschrift angezeigten Felder anpassen. Weitere Informationen finden Sie unter [Objektüberschriften mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Die folgenden Felder sind standardmäßig in der Projektheader enthalten:

* Name der Aufgabe
* Prozent abgeschlossen
* Arbeitsaufträge
* Geplantes Abschlussdatum und -zeit

  >[!CAUTION]
  >
  >Einige Aufgabenbeschränkungen und andere Abhängigkeiten können die Bearbeitung dieses Felds verhindern. Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter [Übersicht über Aufgabenbegrenzungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Status
* Entscheidungsfindung bei Genehmigungseinstellungen, wenn Sie in einem aktuellen Genehmigungsprozess als Genehmiger festgelegt sind

## Stapelweises Bearbeiten von Aufgaben

Sie können Aufgaben stapelweise in einer Liste bearbeiten und alle zugehörigen Informationen gleichzeitig aktualisieren, wenn Sie die Änderungen, die Sie an Aufgaben in der Liste vornehmen, automatisch speichern.

Informationen zum Massenspeichern von Aufgaben finden Sie im Abschnitt &quot;Aufgaben stapelweise bearbeiten&quot;im Artikel [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
