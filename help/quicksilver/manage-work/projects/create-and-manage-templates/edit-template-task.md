---
product-area: templates
keywords: Aufgabe,Standardeinstellungen,Automatisieren,Erstellung
navigation-topic: templates-navigation-topic
title: Vorlagenaufgabe bearbeiten
description: Nachdem Sie eine Vorlage erstellt haben, können Sie die Informationen zu den Vorlagenaufgaben bearbeiten. Die Informationen, die Sie bei einer Vorlagenaufgabe aktualisieren, werden mit Projektaufgaben verknüpft, nachdem Sie die Vorlage zum Erstellen eines Projekts oder zum Anhängen der Vorlage an ein Projekt verwendet haben.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '2629'
ht-degree: 4%

---

# Vorlagenaufgaben bearbeiten

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

Nachdem Sie eine Vorlage erstellt haben, können Sie die Informationen zu den Vorlagenaufgaben bearbeiten. Die Informationen, die Sie bei einer Vorlagenaufgabe aktualisieren, werden mit Projektaufgaben verknüpft, nachdem Sie die Vorlage zum Erstellen eines Projekts oder zum Anhängen der Vorlage an ein Projekt verwendet haben.

Informationen zum Erstellen einer Vorlage finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Sie können jeweils nur eine Vorlagenaufgabe bearbeiten oder Vorlagenaufgaben stapelweise bearbeiten.

>[!NOTE]
>
>Vorlagenaufgaben, die zu verschiedenen Vorlagen gehören, können nicht stapelweise bearbeitet werden. Sie können nur Vorlagenaufgaben bearbeiten, die derselben Vorlage angehören.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen </td> 
   <td> <p>Verwalten von Berechtigungen für eine Vorlage. </p> <p>Sie können eine Vorlagenaufgabe nicht freigeben. </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Erstellen Sie eine Vorlage.

  Informationen zum Erstellen einer Vorlage finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Vorlagenaufgaben bearbeiten

Sie können eine Vorlagenaufgabe mithilfe der Bereiche Vorlagenaufgabe bearbeiten oder Vorlagenaufgaben-Details bearbeiten.

{{step1-to-templates}}

1. Klicken Sie auf den Namen einer Vorlage, um sie zu öffnen.
1. Klicken Sie **linken Bedienfeld** Vorlagenaufgaben“.
1. Klicken Sie auf den Namen einer Vorlagenaufgabe in der Liste, um die Vorlagenaufgabe zu öffnen.
1. Gehen Sie wie folgt vor, um eingeschränkte Informationen zur Vorlagenaufgabe zu bearbeiten:
   1. (Optional) Klicken Sie **linken** auf „Updates“, um der Vorlagenaufgabe Aktualisierungen hinzuzufügen. Vorlagenaufgaben-Aktualisierungen werden nicht in Projektaufgaben übertragen, wenn die Vorlage zum Erstellen eines Projekts verwendet wird.
   1. (Optional) Klicken Sie **linken** auf „Dokumente“, um der Vorlagenaufgabe Dokumente hinzuzufügen. Die Dokumente werden an die Projektaufgaben übertragen, wenn Sie die Vorlage zum Erstellen des Projekts verwenden.
   1. (Bedingt) Um eingeschränkte Informationen zu einer Vorlagenaufgabe zu bearbeiten, klicken Sie im linken Bereich auf **Vorlagenaufgabendetails** und gehen Sie dann in die Bereiche des Abschnitts Details , um Informationen für die einzelnen Bereiche zu bearbeiten.
   1. (Optional) Führen Sie einen der folgenden Schritte aus:
      * Klicken Sie auf das **Alle reduzieren**-Symbol ![Alle reduzieren](assets/collapse-all-icon.png), um alle Bereiche zu reduzieren.
      * Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png) und wählen Sie dann einen der folgenden Bereiche aus oder klicken Sie auf **Alle bearbeiten**, um Informationen in allen Bereichen zu bearbeiten:

         * Übersicht
         * Benutzerdefinierte Forms
Namen von benutzerdefinierten Formularen werden nur angezeigt, wenn der Vorlagenaufgabe benutzerdefinierte Formulare beigefügt sind.
         * Finanzielle Details

        >[!TIP]
        >
        >Um Informationen zu allen Feldern zu erhalten, die im Bereich Details angezeigt werden, setzen Sie den Vorgang mit Bearbeiten aller Felder im Feld Vorlagenaufgabe bearbeiten fort, wie unten beschrieben.

   1. (Optional) Klicken Sie im linken Bereich auf **Teilaufgaben**, um untergeordnete Elemente für die Vorlagenaufgabe hinzuzufügen. Das Hinzufügen von Teilaufgaben für Vorlagenaufgaben ähnelt dem Hinzufügen von Projektaufgaben-Teilaufgaben. Weitere Informationen finden Sie im Abschnitt „Erstellen von Teilaufgaben aus dem Abschnitt „Teilaufgaben“ im Artikel [Erstellen von Teilaufgaben](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Optional) Klicken Sie **linken** auf „Ausgaben“ und fügen Sie den Vorlagenaufgaben Kosten hinzu. Kosten für Vorlagenaufgaben werden auf zukünftige Projektaufgaben übertragen, wenn die Vorlage zum Erstellen eines Projekts verwendet wird.
   1. (Optional) Klicken Sie **linken** auf „Genehmigungen“, um Genehmigungen zu erstellen oder den Vorlagenaufgaben globale Genehmigungen oder Genehmigungen auf Gruppenebene beizufügen. Die Genehmigungen werden auf zukünftige Projektaufgaben übertragen.
   1. (Optional) Klicken Sie im linken Bereich auf **Vorgänger**, um Vorgänger für die Vorlagenaufgaben hinzuzufügen. Das Hinzufügen von Vorlagenaufgabe-Vorgängern ähnelt dem Hinzufügen von Projektaufgaben-Vorgängern. Weitere Informationen finden Sie unter [Erstellen einer Vorgängerbeziehung im Bereich Vorgänger](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Optional) Um mehrere Vorlagenaufgaben in großen Mengen zu bearbeiten, wählen Sie mehrere Vorlagenaufgaben aus und klicken Sie dann **Bearbeiten** oben in der Vorlagenliste.
1. (Bedingt) Um alle Informationen zu einer Vorlagenaufgabe oder zu mehreren Aufgaben gleichzeitig zu bearbeiten, wählen Sie diese aus einer Liste aus und klicken Sie dann oben in der Liste auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png).

   Das **Vorlagenaufgabe bearbeiten** wird angezeigt.

   >[!TIP]
   >
   >Sie können auch eine Vorlagenaufgabe in einer Liste auswählen und dann rechts neben dem Namen der Vorlagenaufgabe in der Kopfzeile auf **Bearbeiten** klicken, um das Feld **Vorlagenaufgabe bearbeiten** zu öffnen.

   ![Vorlagenaufgabe bearbeiten](assets/edit-template-tasks-box-classic-350x356.png)

   <!--1. (Conditional) In the Production environment, -->
1. Erwägen Sie, Informationen in einem der folgenden Abschnitte anzugeben:

   * [Übersicht](#overview)
   * [Finanzielle Details](#finance)
   * [Einstellungen](#settings)
   * [Arbeitsaufträge](#assignments)
   * [Benutzerdefinierte Formulare](#custom-forms)
   * [Kommentar](#comment)

<!--1. Continue editing the template task as described in the Edit a template task using the old experience section in this article (********add hashtag anchor here*******)-->

<!--1. <span class="preview">(Conditional) In the Preview environment, click **Try new experience** in the upper-right corner of the **Edit Template Task** box </span>, then continue editing the template task as described in the Edit a template task using the new experience section in this article (********add hashtag anchor here*******).</span>
1. (Optional) Click **Switch back to old experience** at the bottom of the Edit Template Task box  
-->


<!--### Edit a template task using the old experience
(and make all the headers below "####")-->

### Übersicht {#overview}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie auf **Übersicht**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. Aktualisieren Sie eines der folgenden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>Geben Sie einen Namen für die Vorlagenaufgabe an. Dieses Feld wird nicht angezeigt, wenn Vorlagenaufgaben stapelweise bearbeitet werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie zusätzliche Informationen zur Vorlagenaufgabe hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Geben Sie einen Weblink an, der sich auf die Informationen zur Vorlagenaufgabe bezieht.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Dies ist eine visuelle Markierung, mit der Sie Ihre Vorlagenaufgaben priorisieren können. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Kein</strong> </p> </li> 
        <li> <p><strong>Niedrig</strong> </p> </li> 
        <li> <p> <b>normal</b></p> </li> 
        <li> <p><b>Hoch</b> </p> </li> 
        <li> <p><b>Dringend</b> </p> </li> 
       </ul> <p>Je nach den vom Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Prioritäten für Sie unterschiedlich sein. Weitere Informationen zum Bearbeiten von Prioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dauertyp</strong> </td> 
      <td> <p>Die zukünftige Aufgabe, die aus dieser Vorlage erstellt wird, hat diesen Dauertyp. <br>Duration Type gibt die Beziehung zwischen folgenden Elementen an:</p> <p>- Anzahl der einer Aufgabe zugewiesenen Ressourcen</p> <p>- der Gesamtaufwand, der zum Abschließen der Aufgabe erforderlich ist</p> <p>- die Gesamtdauer der Aufgabe. </p> <p>Mit Dauertypen können Sie konsistente Ressourcenzuweisungen auf der Grundlage der Anforderungen der Aufgabe festlegen. Weitere Informationen zum Dauertyp einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den Dauertyp</a>.</p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Berechnete Zuweisung</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Berechnete Arbeit</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Leistungsgesteuert</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Einfach</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dauer</strong> </td> 
      <td> <p>Geben Sie die Dauer künftiger Aufgaben in Minuten, Stunden, Tagen, Wochen oder Monaten an. Die zukünftige Aufgabe, die aus dieser Vorlage erstellt wird, hat die hier angegebene Dauer.</p> <p>Standardmäßig misst Workfront die Dauer in Tagen. Dies ist die Zeit, die Sie einplanen, damit die Aufgabe unvollständig bleibt, bevor sie abgeschlossen werden muss. Sie können die Dauer einer Aufgabe nicht angeben, wenn der <strong>Dauertyp</strong> der Aufgabe "<strong>Einfach</strong> lautet oder wenn die <strong>Aufgabenbeschränkung</strong> <strong>Feste Termine</strong> ist.</p> <p><b>WICHTIG</b></p> <p>Die Dauer ist in der Regel der Zeitraum zwischen dem geplanten Start und dem geplanten Abschlussdatum einer Vorlagenaufgabe und wirkt sich daher auf die Zeitleiste der Vorlage aus. Dadurch wird der Zeitrahmen des zukünftigen Projekts festgelegt, das aus der Vorlage erstellt wird. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplante Stunden</strong> </td> 
      <td> <p>Geben Sie die Anzahl der geplanten Stunden für die zukünftige Aufgabe für das mit dieser Vorlage erstellte Projekt an. Dies ist die tatsächliche Zeit, die die Verantwortlichen für die Aufgabe benötigen würden, um diese abzuschließen. Sie können die Anzahl der geplanten Stunden für eine Aufgabe nur angeben, wenn <strong>Dauertyp</strong> auf "<strong> Zuordnung“ </strong>. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Aufgabenbeschränkung</strong> </td> 
      <td> <p>Die Aufgabe für das Projekt, die aus dieser Vorlage erstellt wurde, unterliegt dieser Einschränkung. Aufgabeneinschränkungen identifizieren, wann eine Aufgabe abgeschlossen werden muss. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li><strong>Feste Daten</strong>. Geben Sie <strong> „Geplanter Start</strong> und ein <strong>Geplantes Abschlussdatum“ an</strong></li> 
        <li><strong>Muss beginnen am</strong>. Geben Sie <strong>Geplantes Startdatum“ an</strong></li> 
        <li><strong>Muss beendet werden am</strong>. Geben Sie <strong> „Geplantes Abschlussdatum“ </strong>.</li> 
        <li><strong>So bald wie möglich</strong> </li> 
        <li><strong>So spät wie möglich</strong> </li> 
        <li style="font-weight: bold;"><strong>Früheste verfügbare Zeit</strong> </li> 
        <li style="font-weight: bold;"><strong>Letzte verfügbare Zeit</strong> </li> 
        <li>Start nicht später als. Geben Sie <strong>Geplantes Startdatum“ </strong>.</li> 
        <li><strong>Start nicht früher als</strong>. Geben Sie <strong>Geplantes Startdatum“ </strong>.</li> 
        <li><strong>Beenden Sie spätestens</strong>. Geben Sie <strong> „Geplantes Abschlussdatum“ </strong>.</li> 
        <li><strong>Beenden Sie nicht früher als</strong>. Geben Sie <strong> „Geplantes Abschlussdatum“ </strong>.</li> 
       </ul> <p>Weitere Informationen zur Aufgabenbeschränkung finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Aufgabenbeschränkung - Übersicht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Starttag</span><span style="font-weight: normal;"> (optional und bedingt)</span> </td> 
      <td> <p> Sie können den Starttag einer Vorlagenaufgabe nur angeben, wenn die Aufgabenbeschränkung eine der folgenden ist:</p> 
       <ul> 
        <li>Muss beginnen am</li> 
        <li>Nicht früher starten als</li> 
        <li>Nicht später anfangen als</li> 
        <li>Feste Daten</li> 
       </ul> <p>Dies entspricht dem Datum innerhalb der Zeitleiste des zukünftigen Projekts, an dem die Aufgabe gestartet wird. Für alle anderen Einschränkungen berechnet Workfront den Starttag basierend auf der Abhängigkeit der Vorgänger zwischen den Aufgaben. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abschlusstag</strong><span style="font-weight: normal;"> (optional und bedingt)</span> </td> 
      <td> <p> Sie können den Abschlusstag einer Vorlagenaufgabe nur angeben, wenn die Aufgabenbeschränkung eine der folgenden ist:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Muss beendet werden am</li> 
        <li>Nicht früher beenden als (NFBA)</li> 
        <li>Nicht später beenden als (NSBA)</li> 
        <li>Feste Daten</li> 
       </ul> <p>Dies entspricht dem Datum innerhalb der Zeitleiste des zukünftigen Projekts, an dem die Aufgabe abgeschlossen wird. Für alle anderen Einschränkungen berechnet Workfront den Abschlusstag anhand der Dauer und der Vorgängerabhängigkeit. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Änderungen speichern**.

### Finanzielle Details {#finance}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie auf **Finanzen**.

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. Aktualisieren Sie eines der folgenden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Kostentyp</strong> </td> 
      <td> <p>Geben Sie den Kostentyp für die zukünftige Aufgabe an. Dadurch wird bestimmt, wie die Kosten für die Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet werden. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Keine Kosten</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Festgelegt pro Stunde</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Benutzer pro Stunde</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Stundensatz nach Funktion</span> </p> </li> 
       </ul> <p>Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Umsatztyp</strong> </td> 
      <td> <p>Geben Sie den Umsatztyp für die zukünftige Aufgabe an. Dadurch wird bestimmt, wie der Umsatz für die Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet wird.</p> <p style="font-weight: normal;">Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Nicht fakturierbar</p> </li> 
        <li> <p style="font-weight: normal;">Benutzer pro Stunde</p> </li> 
        <li> <p style="font-weight: normal;">Stundensatz nach Funktion</p> </li> 
        <li> <p style="font-weight: normal;">Festgelegt pro Stunde</p> </li> 
        <li> <p style="font-weight: normal;">Benutzende pro Stunde mit Begrenzung</p> </li> 
        <li> <p style="font-weight: normal;">Stundensatz nach Funktion mit Begrenzung</p> </li> 
        <li> <p style="font-weight: normal;">Benutzer pro Stunde plus festgelegt</p> </li> 
        <li> <p style="font-weight: normal;">Stundensatz nach Funktion plus fest</p> </li> 
        <li> <p style="font-weight: normal;">Festeinnahmen</p> </li> 
       </ul> <p>Weitere Informationen zur Umsatzverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Änderungen speichern**.

### Einstellungen {#settings}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie auf **Einstellungen**.

   ![Einstellungen für Vorlagenaufgaben bearbeiten](assets/edit-template-tasks-settings-classic-350x231.png)

1. Aktualisieren Sie eines der folgenden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Meilenstein</b></p></strong> </td> 
      <td> <p>Einen Meilenstein auswählen, der der ausgewählten Vorlagenaufgabe zugeordnet werden soll.</p>

   <p><b>WICHTIG</b></p>
   <p>Sie müssen einen Meilensteinpfad mit einer Vorlage verknüpfen, damit dieses Feld angezeigt wird. Weitere Informationen finden Sie unter <a href="../create-and-manage-templates/edit-templates.md">Projektvorlagen bearbeiten</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Überwachungsmodus</strong> </td> 
      <td> <p>Geben Sie an, wie der Fortschrittsstatus der zukünftigen Aufgabe verfolgt werden soll. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Benutzer muss aktualisieren</strong> </p> </li> 
        <li> <p><strong>Angenommen, der Vorgang ist pünktlich</strong> </p> </li> 
        <li> <p><strong>Späte Warnungen ignorieren</strong> </p> </li> 
        <li> <p><strong>AutoVervollständigen</strong> </p> </li> 
        <li> <p><strong>Vorgänger</strong> </p> </li> 
       </ul> <p>Weitere Informationen zum Tracking-Modus für Aufgaben finden Sie unter <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Übersicht über den Tracking-Modus für Aufgaben</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Genehmigungsprozess</strong> </td> 
      <td> <p>Wählen Sie den Genehmigungsprozess aus, den Sie mit der Vorlagenaufgabe verknüpfen möchten. Ihr Workfront-Administrator muss Aufgabengenehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Vorlagenaufgaben verknüpfen können. <span>Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.</p> <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen Folgendes: </p> 
       <ul> 
       <li>In der Liste werden nur aktive Genehmigungsprozesse angezeigt. </li> 
       <li> <p>In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Genehmigungsprozesse, die einer anderen Gruppe als der der Vorlage zugeordnet sind, werden nicht in der Liste angezeigt.</p> <p>Wichtig: Wenn sich die mit der Vorlage verknüpfte Gruppe ändert, wird der gruppenspezifische Genehmigungsprozess zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>. </p> </li> 
       <li> <p>Wenn Sie einen Genehmigungsprozess für den einmaligen Gebrauch hinzugefügt haben, wird er in diesem Feld als "&lt;Custom&gt;" angezeigt. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>Beim Massenbearbeiten von Vorlagenaufgaben gibt es die folgenden Szenarien:</p> 
       <ul> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus derselben Vorlagengruppe auswählen, werden in diesem Feld sowohl Genehmigungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt.</p> </li> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus verschiedenen Vorlagengruppen auswählen, werden in diesem Feld nur Genehmigungsprozesse auf Systemebene angezeigt.</p> </li> 
       <li> <p>Wenn einer der Vorlagenaufgaben ein Genehmigungsprozess für den einmaligen Gebrauch angehängt ist, wird sie durch den von Ihnen ausgewählten Genehmigungsprozess auf <span>- oder </span> ersetzt. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Erinnerungsnachrichten</strong> </td> 
      <td> <p>Wählen Sie aus, welche Erinnerungsnachrichten Sie an die Vorlagenaufgabe anhängen möchten. Sie werden an zukünftige Aufgaben des Projekts angehängt, das aus dieser Vorlage erstellt wird. Ihr Systemadministrator muss Erinnerungsnachrichten konfigurieren, bevor Sie sie für eine Aufgabe auswählen können. Weitere Informationen zum Konfigurieren von Erinnerungsnachrichten finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsnachrichten</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Änderungen speichern**.

### Arbeitsaufträge {#assignments}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Arbeitsaufträge**.

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Klicken Sie **Verantwortlichen hinzufügen**, um der Vorlagenaufgabe einen neuen Verantwortlichen hinzuzufügen. Sie können einer Aufgabe Benutzer, Rollen oder Teams zuweisen. Sie können mehrere Verantwortliche für eine Aufgabe haben. Den zukünftigen Aufgaben werden dieselben Ressourcen zugewiesen, wenn sie aus dieser Vorlagenaufgabe erstellt werden.
1. (Optional) Wenn mehrere Verantwortliche vorhanden sind, wählen Sie das **Verantwortlicher**, um anzugeben, welcher Benutzer oder welche Rolle als Aufgabenbesitzer oder Primärer Verantwortlicher gilt. Workfront markiert den ersten Benutzer oder das erste Aufgabengebiet, das Sie einer Vorlagenaufgabe zuweisen, als Eigentümer oder Primärer Bevollmächtigter.
1. (Bedingt und optional) Wenn Ihre Aufgabenbeschränkung „Berechnete Arbeit“ oder „Arbeitsaufwand“ ist, geben Sie **Zuordnung %** (Zuordnungsprozentsatz) für jeden Zugewiesenen an. Dies ist die Zeit aus dem Zeitplan des Verantwortlichen, die er für diese Aufgabe aufwenden kann. Wenn Sie den Zuordnungsprozentsatz für einen Verantwortlichen ändern, werden auch die geplanten Stunden einer Aufgabe geändert.
1. (Bedingt und optional) Wenn Ihre Aufgabenbeschränkung „Einfach“ ist, geben Sie die **Stunden** jedes Verantwortlichen an

   Oder

   Geben Sie die Gesamtzahl (**Stunden** für die Vorlagenaufgabe an. Dadurch wird die Gesamtstundenzahl gleichmäßig auf alle Bevollmächtigten verteilt.

1. (Bedingt und optional) Wenn die Aufgabenbeschränkung „Einfach“ ist, geben Sie die **Dauer** der Vorlagenaufgabe in Tagen an. Dies wird die Dauer der Aufgabe, die aus dieser Vorlage erstellt wurde.
1. (Optional) Wählen Sie eine Rolle aus **Dropdown-Menü „Rolle des Verantwortlichen** aus. Dies ist die Rolle, die der Beauftragte bei dieser zukünftigen Aufgabe erfüllen kann. Im Dropdown-Menü werden nur die Aufgabengebiete angezeigt, die jedem Bearbeiter in seinem Profil zugeordnet sind.
1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Änderungen speichern**.

### Benutzerdefinierte Formulare {#custom-forms}

Sie können benutzerdefinierte Formulare definieren, die standardmäßig an Aufgaben angehängt werden, wenn die Aufgaben zu einem Projekt hinzugefügt werden. Informationen dazu, wie Sie das Projekt so einrichten, dass es benutzerdefinierte Formulare für Standardaufgaben enthält, finden Sie im Abschnitt „Aufgaben“ im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Sie können auch benutzerdefinierte Formulare zu zukünftigen Aufgaben eines Projekts hinzufügen, wenn das Projekt aus einer Vorlage erstellt wird, indem Sie die benutzerdefinierten Formulare zu den Vorlagenaufgaben hinzufügen.

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Benutzerdefinierte Forms**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Wählen Sie das oder die benutzerdefinierten Formulare aus, die Sie mit der Vorlagenaufgabe verknüpfen möchten.

   Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können.
In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt.
Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Sie können einer Vorlagenaufgabe bis zu zehn benutzerdefinierte Formulare hinzufügen.
Die Formulare werden automatisch zu den Aufgaben hinzugefügt, die aus der Vorlage erstellt wurden.
1. (Bedingt und optional) Wenn Sie ein benutzerdefiniertes Formular an die Vorlagenaufgabe angehängt haben, bearbeiten Sie alle Felder im Formular. Sie müssen alle erforderlichen Felder angeben, bevor Sie die Vorlagenaufgabe speichern können.

   >[!NOTE]
   >
   >Je nachdem, wie der Workfront-Administrator die Berechtigungen für die Abschnitte in Ihrem benutzerdefinierten Formular festgelegt hat, können nicht alle dieselben Felder in einem bestimmten benutzerdefinierten Formular anzeigen oder bearbeiten. Die Berechtigungen zum Bearbeiten von Feldern in einem Abschnitt eines benutzerdefinierten Formulars hängen von den Berechtigungen ab, die Sie für die Vorlagenaufgabe oder die zukünftige Aufgabe haben.\
   >Informationen zum Festlegen von Berechtigungen für Abschnitte eines benutzerdefinierten Formulars finden Sie unter [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Informationen zum Festlegen von Aufgabenberechtigungen finden Sie unter [Freigeben einer Aufgabe](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Informationen zum Festlegen von Vorlagenberechtigungen finden Sie unter [Freigeben einer Vorlage](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung des folgenden Abschnitts fort.

   Oder

   Klicken Sie auf **Änderungen speichern**.

### Kommentar {#comment}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Kommentar**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Geben Sie im Feld Verfügbar einen Kommentar an, der im Aktualisierungsverlauf der Vorlagenaufgabe angezeigt werden soll. Dieser Kommentar ist für alle sichtbar, die Ansichtszugriff auf die Vorlage und die Vorlagenaufgabe und Zugriff auf Ansichtsnotizen haben.
1. Klicken Sie auf **Änderungen speichern**.

   Wenn Sie oder ein anderer Benutzer ein Projekt aus dieser Vorlage erstellt, werden alle Einstellungen, die Sie auf Vorlagenaufgaben angewendet haben, zu den Einstellungen für die Projektaufgaben.

<!--
<div class="preview"> 

### Edit a template task using the new experience

Consider specifying information in any of the following sections:

   * [Template task name](#template-task-name)
   * [Overview](#overview-1)
   * [Assignments](#assignments-1)
   * [Finance](#finance-1)
   * [Custom Forms](#custom-forms-1)
   * [Settings](#settings-1)
   * [Comment](#comment-1)

#### Template Task Name

1. Begin editing a template task as described above.
1. In the Edit Template Task box, click **Template Task Name** and add a name for the template task. 

   This view is not available when editing template tasks in bulk. 

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**. 

#### Overview {#overview-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Overview** in the left panel. 

   ![Template task edit overview section](assets/template-task-edit-overview.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add additional information about the template task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>This is a visual flag for you which allows you to prioritize your template tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>None</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>High</b> </p> </li> 
        <li> <p><b>Urgent</b> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Constraint</strong> </td> 
      <td> <p>The task on the project created from this template will have this constraint. Task Constraints identify when a task must be completed. </p> <p>Select from the following options:</p> 
       <ul> 
        <li><strong>Fixed Dates</strong>. Specify a <strong>Planned Start</strong> and a <strong>Planned Completion Date.</strong></li> 
        <li><strong>Must Start On</strong>. Specify a <strong>Planned Start Date.</strong></li> 
        <li><strong>Must Finish On</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>As Soon as Possible</strong> </li> 
        <li><strong>As Late as Possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Earliest Available Time</strong> </li> 
        <li style="font-weight: bold;"><strong>Latest Available Time</strong> </li> 
        <li>Start No Later Than. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Start No Earlier Than</strong>. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Finish No Later Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>Finish No Earlier Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
       </ul> <p>For more information on Task Constraint, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Start Day</span><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Start Day of a template task only when the Task&nbsp;Constraint is one of the following:</p> 
       <ul> 
        <li>Must Start On</li> 
        <li>Start No&nbsp;Earlier Than</li> 
        <li>Start No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will start. For all other constraints, Workfront calculates the Start Day based on predecessor dependency between the tasks. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Day</strong><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Completion Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Must Finish On</li> 
        <li>Finish No Earlier Than</li> 
        <li>Finish No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will complete. For all other constraints, Workfront calculates the Completion Day based on Duration and predecessor dependency. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Specify a web link that relates to the information about the template task.</td> 
     </tr> 

     <tr> 
      <td role="rowheader"><strong>Work Effort</strong> </td> 
      <td>Choose from the following options:
      <ul><li>Small</li>
      <li>Medium</li>
      <li>Large</li></ul>

      <p><b>IMPORTANT</b></p>
      <p>The Work Effort field displays when editing a template task only when you select the <b>Use Work Effort to automatically calculate task Planned Hours</b> setting when editing the template.</p>

      </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Assignments {#assignments-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Assignments** in the left panel.

   ![Template task edit assignments](assets/template-task-edit-assignments.png)

1. In the Search people, role, or teams field, start typing the name of an assignee, then select it when it displays in the list

   Or

   Click **Assign to me** to assign the template task to yourself.
1. Consider updating the following information: 

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 

<tr> 
      <td role="rowheader"><strong>Duration Type</strong> </td> 
      <td> <p>The future task created from this template will have this Duration Type. <br>The Duration Type identifies the relationship between the following:</p> 
      <ul>
      <li><p>Number of resources assigned to a task</p> </li>
      <li><p>The total effort required to complete the task</p></li> 
      <li><p>The total duration of the task </p></li></ul> <p>Using Duration Types, you can set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Assignment</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Work</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Effort Driven</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duration</strong> </td> 
      <td> <p>Specify the Duration of the future tasks, in minutes, hours, days, weeks, or months. The future task created from this template will have the Duration specified here.</p> <p>By default, Workfront measures Duration in days. This is the amount of time that you allow for the task to remain incomplete, before it must be completed. You cannot specify the Duration of a task when the <strong>Duration Type</strong> of the task is <strong>Simple</strong>, or when the <strong>Task Constraint</strong> is <strong>Fixed Dates</strong>.</p> <p><b>IMPORTANT</b></p> <p>Duration is typically the amount of time between the Planned Start and the Planned Completion Dates of a template task, and for this reason, it affects the timeline of the template. This determines the timeline of the future project created from the template. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Hours</strong> </td> 
      <td> <p>Specify the number of Planned Hours for the future task on the project created with this template. This is the amount of actual time it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the <strong>Duration Type</strong> is set to <strong>Calculated Assignment</strong>. </p> </td> 
     </tr> 
  </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Finance {#finance-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Finance** in the left panel.

   ![Template task edit finance section](assets/template-task-edit-finance.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cost Type</strong> </td> 
      <td> <p>Specify the Cost Type for the future task. This is going to determine how the Cost on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>No Cost</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixed Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>User Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Role Hourly</span> </p> </li> 
       </ul> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Revenue Type</strong> </td> 
      <td> <p>Specify the Revenue Type for the future task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks.</p> <p style="font-weight: normal;">Select from the following options: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Not Billable</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Hourly</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Revenue</p> </li> 
       </ul> <p>For more information about tracking revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.


#### Custom Forms {#custom-forms}

You can define custom forms to be automatically attached by default to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms, see the "Tasks" section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

You can also add custom forms to the future tasks of a project when the project is created from a template, by adding the custom forms to the template tasks. 

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Custom Forms** in the left panel.

   ![Template task edit custom forms section](assets/template-task-edit-custom-forms.png)

1. Select the custom form or forms that you want to associate with the template task. 

   You must build the custom forms before they are available to select in this field. 
   Only active custom forms display in the list. 

   For more information about building custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

   You can add up to ten custom forms to a template task. 
   The forms are automatically added to the tasks created from the template. 
1. (Conditional and optional) If you attached a custom form to the template task, edit any fields on the form. You must specify all required fields before you can save the template task.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the template task or the future task.   
   >For information about setting permissions on sections of a custom form, see [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).   
   >For information about setting task permissions, see [Share a task](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).   
   >For information about setting template permissions, see [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save**.

#### Settings {#settings-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task Box**, click **Settings** in the left panel.

   ![Template task edit settings section](assets/template-task-edit-settings.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milestone</b></p></strong> </td> 
      <td> <p>Choose a milestone to associate with the selected template task.</p>
      
   <p><b>IMPORTANT</b></p>
   <p>You must associate a milestone path with a template for this field to display. For more information, see <a href="../create-and-manage-templates/edit-templates.md">Edit project templates</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Tracking Mode</strong> </td> 
      <td> <p>Specify how the progress status of the future task will be tracked. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>User Must Update</strong> </p> </li> 
        <li> <p><strong>Assume on Time</strong> </p> </li> 
        <li> <p><strong>Ignore Late Warnings</strong> </p> </li> 
        <li> <p><strong>Autocomplete</strong> </p> </li> 
        <li> <p><strong>Predecessor</strong> </p> </li> 
       </ul> <p>For more information about the Tracking Mode on tasks, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notifications</strong> </td> 
      <td> <p>Select which Reminder Notifications you would like to attach to the template task. They will be attached to the future tasks on the project created from this template. Your system administrator must configure Reminder Notifications before you can select them on a task. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template task. Your Workfront administrator must define system-level task Approval Processes before you can associate them with template tasks. <span>A user with administrative access to Approval processes can also create group-specific approval processes.</span> For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
       <ul> 
       <li>Only active approval processes display in the list. </li> 
       <li> <p>System-wide and group-specific approval processes display in the list. Approval processes associated with a group other than that of the template do not display in the list.</p> <p>Important: If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
       <li> <p>If you added a single-use approval process, it displays as "&lt;Custom&gt;" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p>  </li> 
       <li> <p>When bulk-editing template tasks, the following scenarios exist:</p> 
       <ul> 
       <li> <p>When you select template tasks from the same template group, both system-level and group-level approval processes display in this field.</p> </li> 
       <li> <p>When you select template tasks from different template groups, only system-level approval processes display in this field.</p> </li> 
       <li> <p>When any of the template tasks has a single-use approval process attached, it is replaced by the system-level <span>or group-level approval process</span> you select. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Comment {#comment-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Comment** in the left panel.

   ![Template task edit Comment section](assets/template-task-edit-comment.png)

1. In the **Add an update to the template task** area, specify a comment that you want to display in the updates stream of the template task in the available field. This comment is visible for everyone with View access to the template and the template task and with access to view Notes.
1. Click **Save**.

   When you or another user creates a project from this template, all settings you applied to template tasks become the settings for the project tasks.

</div>

-->