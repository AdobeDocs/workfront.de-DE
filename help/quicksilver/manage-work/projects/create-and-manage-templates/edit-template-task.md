---
product-area: templates
keywords: Aufgabe,Standardeinstellungen,Automatisieren,Erstellung
navigation-topic: templates-navigation-topic
title: Vorlagenaufgabe bearbeiten
description: Nachdem Sie eine Vorlage erstellt haben, können Sie die Informationen zu den Vorlagenaufgaben bearbeiten. Die Informationen, die Sie bei einer Vorlagenaufgabe aktualisieren, werden mit Projektaufgaben verknüpft, nachdem Sie die Vorlage zum Erstellen eines Projekts oder zum Anhängen der Vorlage an ein Projekt verwendet haben.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: c9fa6d97607990710e6c2a74f3b373d06201d721
workflow-type: tm+mt
source-wordcount: '7460'
ht-degree: 5%

---

# Vorlagenaufgaben bearbeiten

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen sind ab einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Nachdem Sie eine Vorlage erstellt haben, können Sie die Informationen zu den Vorlagenaufgaben bearbeiten. Die Informationen, die Sie bei einer Vorlagenaufgabe aktualisieren, werden mit Projektaufgaben verknüpft, nachdem Sie die Vorlage zum Erstellen eines Projekts oder zum Anhängen der Vorlage an ein Projekt verwendet haben.

Informationen zum Erstellen einer Vorlage finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

Sie können jeweils nur eine Vorlagenaufgabe bearbeiten oder Vorlagenaufgaben stapelweise bearbeiten.

>[!NOTE]
>
>Vorlagenaufgaben, die zu verschiedenen Vorlagen gehören, können nicht stapelweise bearbeitet werden. Sie können nur Vorlagenaufgaben bearbeiten, die derselben Vorlage angehören.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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

Das Bearbeiten von Vorlagenaufgaben unterscheidet sich je nach der Umgebung, in der Sie die Aufgaben bearbeiten möchten.

### Bearbeiten von Vorlagenaufgaben in der Produktionsumgebung

>[!NOTE]
>
><span class="preview">Einige Kunden können Vorlagenaufgaben in ihren Produktionsumgebungen auf die gleiche Weise bearbeiten wie in ihrer Vorschau-Umgebung.</span>
>
><span class="preview">Informationen zum Bearbeiten von Aufgaben in der Vorschau-Umgebung finden Sie im Abschnitt [Bearbeiten von Vorlagenaufgaben in der Vorschau-](#edit-template-tasks-in-the-preview-environment)) in diesem Artikel. </span>


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

   Das **Vorlagenaufgabe bearbeiten** wird in der neuen -Version angezeigt.

   ![Neues Erlebnis für Vorlagenaufgabe bearbeiten](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Sie können auch eine Vorlagenaufgabe in einer Liste auswählen und dann rechts neben dem Namen der Vorlagenaufgabe in der Kopfzeile auf **Bearbeiten** klicken, um das Feld **Vorlagenaufgabe bearbeiten** zu öffnen.

   Fahren Sie mit der Bearbeitung der Vorlagenaufgabe fort, wie im Abschnitt [Bearbeiten einer Vorlagenaufgabe mithilfe des neuen Erlebnisses](#edit-a-template-task-using-the-new-experience) in diesem Artikel beschrieben.

1. (Optional) Klicken Sie **Zurück zum alten Erlebnis wechseln** unten im Feld **Vorlagenaufgabe bearbeiten**, um das Feld **Vorlagenaufgabe bearbeiten** im alten Erlebnis zu öffnen.

   ![Vorlagenaufgabe bearbeiten](assets/edit-template-tasks-box-classic-350x356.png)

1. Erwägen Sie, Informationen in einem der folgenden Abschnitte anzugeben:

   * [Übersicht](#overview)
   * [Finanzielle Details](#finance)
   * [Einstellungen](#settings)
   * [Arbeitsaufträge](#assignments)
   * [Benutzerdefinierte Formulare](#custom-forms)
   * [Kommentar](#comment)

1. Fahren Sie mit der Bearbeitung der Vorlagenaufgabe fort, wie im Abschnitt [Bearbeiten einer Vorlagenaufgabe mithilfe des alten Erlebnisses](#edit-a-template-task-using-the-old-experience) in diesem Artikel beschrieben.

#### Bearbeiten einer Vorlagenaufgabe mithilfe des alten Erlebnisses

##### Übersicht {#overview}

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
        <li> <p><b>Dringlich</b> </p> </li> 
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
        <li>Nicht früher anfangen als</li> 
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

   ODER

   Klicken Sie auf **Änderungen speichern**.

##### Finanzielle Details {#finance}

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

   ODER

   Klicken Sie auf **Änderungen speichern**.

##### Einstellungen {#settings}

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

   ODER

   Klicken Sie auf **Änderungen speichern**.

##### Arbeitsaufträge {#assignments}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Arbeitsaufträge**.

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Klicken Sie **Verantwortlichen hinzufügen**, um der Vorlagenaufgabe einen neuen Verantwortlichen hinzuzufügen. Sie können einer Aufgabe Benutzer, Rollen oder Teams zuweisen. Sie können mehrere Verantwortliche für eine Aufgabe haben. Den zukünftigen Aufgaben werden dieselben Ressourcen zugewiesen, wenn sie aus dieser Vorlagenaufgabe erstellt werden.
1. (Optional) Wenn mehrere Verantwortliche vorhanden sind, wählen Sie das **Verantwortlicher**, um anzugeben, welcher Benutzer oder welche Rolle als Aufgabenbesitzer oder Primärer Verantwortlicher gilt. Workfront markiert den ersten Benutzer oder das erste Aufgabengebiet, das Sie einer Vorlagenaufgabe zuweisen, als Eigentümer oder Primärer Bevollmächtigter.
1. (Bedingt und optional) Wenn Ihr **Dauertyp** &quot;**Arbeit“** &quot;**Leistungsgesteuert“**, geben Sie die **Zuordnung %** (Zuordnungsprozentsatz) für jeden Zugewiesenen an. Dies ist die Zeit aus dem Zeitplan des Verantwortlichen, die er für diese Aufgabe aufwenden kann. Wenn Sie den Zuordnungsprozentsatz für einen Verantwortlichen ändern, werden auch die geplanten Stunden einer Aufgabe geändert.
1. (Bedingt und optional) Wenn Ihr **Dauertyp** &quot;**&quot; lautet** geben Sie die **Stunden** jedes Verantwortlichen an

   ODER

   Geben Sie die Gesamtzahl (**Stunden** für die Vorlagenaufgabe an. Dadurch wird die Gesamtstundenzahl gleichmäßig auf alle Bevollmächtigten verteilt.

1. (Bedingt und optional) Wenn Ihr **Dauertyp** „Einfach“ ist, geben Sie die **Dauer** der Vorlagenaufgabe in Tagen an. Dies wird die Dauer der Aufgabe, die aus dieser Vorlage erstellt wurde.
1. (Optional) Wählen Sie eine Rolle aus **Dropdown-Menü „Rolle des Verantwortlichen** aus. Dies ist die Rolle, die der Beauftragte bei dieser zukünftigen Aufgabe erfüllen kann. Im Dropdown-Menü werden nur die Aufgabengebiete angezeigt, die jedem Bearbeiter in seinem Profil zugeordnet sind.
1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Änderungen speichern**.

##### Benutzerdefinierte Formulare {#custom-forms}

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

   ODER

   Klicken Sie auf **Änderungen speichern**.

##### Kommentar {#comment}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Kommentar**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Geben Sie im Feld Verfügbar einen Kommentar an, der im Aktualisierungsverlauf der Vorlagenaufgabe angezeigt werden soll. Dieser Kommentar ist für alle sichtbar, die Ansichtszugriff auf die Vorlage und die Vorlagenaufgabe und Zugriff auf Ansichtsnotizen haben.
1. Klicken Sie auf **Änderungen speichern**.

   Wenn Sie oder ein anderer Benutzer ein Projekt aus dieser Vorlage erstellt, werden alle Einstellungen, die Sie auf Vorlagenaufgaben angewendet haben, zu den Einstellungen für die Projektaufgaben.

#### Bearbeiten einer Vorlagenaufgabe mithilfe der neuen Benutzeroberfläche

Nachdem Sie das Feld **Vorlagenaufgabe bearbeiten** in der neuen -Version geöffnet haben, sollten Sie Informationen in einem der folgenden Abschnitte angeben:

* [Name der Vorlagenaufgabe](#template-task-name)
* [Übersicht](#overview-1)
* [Arbeitsaufträge](#assignments-1)
* [Finanzielle Details](#finance-1)
* [Benutzerdefinierte Formulare](#custom-forms-1)
* [Einstellungen](#settings-1)
* [Kommentar](#comment-1)

##### Name der Vorlagenaufgabe

>[!TIP]
>
>Der Abschnitt „Name der Vorlagenaufgabe“ ist nicht verfügbar, wenn Vorlagenaufgaben stapelweise bearbeitet werden.


1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie im Feld Vorlagenaufgabe bearbeiten auf **Name der Vorlagenaufgabe** und fügen Sie einen Namen für die Vorlagenaufgabe hinzu.

   Diese Ansicht ist nicht verfügbar, wenn Vorlagenaufgaben stapelweise bearbeitet werden.

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

##### Übersicht {#overview-1}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken Bereich auf **Übersicht**.

   ![Abschnitt zum Bearbeiten der Vorlagenaufgabe - Übersicht](assets/template-task-edit-overview.png)

1. Aktualisieren Sie eines der folgenden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie zusätzliche Informationen zur Vorlagenaufgabe hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Dies ist eine visuelle Markierung, mit der Sie Ihre Vorlagenaufgaben priorisieren können. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Kein</strong> </p> </li> 
        <li> <p><strong>Niedrig</strong> </p> </li> 
        <li> <p> <b>normal</b></p> </li> 
        <li> <p><b>Hoch</b> </p> </li> 
        <li> <p><b>Dringlich</b> </p> </li> 
       </ul> <p>Je nach den vom Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Prioritäten für Sie unterschiedlich sein. Weitere Informationen zum Bearbeiten von Prioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a>.</p> </td> 
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
        <li>Nicht früher anfangen als</li> 
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
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Geben Sie einen Weblink an, der sich auf die Informationen zur Vorlagenaufgabe bezieht.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Work Effort</strong> </td> 
      <td>Wählen Sie aus den folgenden Optionen:
      <ul><li>Klein</li>
      <li>Mittel</li>
      <li>Groß</li></ul>

   <p><b>WICHTIG</b></p>
      <p>Das Feld Work Effort wird beim Bearbeiten einer Vorlagenaufgabe nur angezeigt, wenn Sie beim Bearbeiten der Vorlage die Einstellung <b>Work Effort zur automatischen Berechnung der geplanten Stunden </b> Aufgabe verwenden auswählen.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

##### Arbeitsaufträge {#assignments-1}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Arbeitsaufträge“.

   ![Vorlagenaufgabe - Zuweisungen bearbeiten](assets/template-task-edit-assignments.png)

1. Beginnen Sie im Feld **Personen, Aufgabengebiete oder Teams suchen** den Namen eines Verantwortlichen einzugeben, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird

   ODER

   Klicken Sie **Mir zuweisen**, um sich die Vorlagenaufgabe selbst zuzuweisen.
1. Es wird erwogen, die folgenden Informationen zu aktualisieren:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody>

   <tr> 
         <td role="rowheader"><strong>Dauertyp</strong> </td> 
         <td> <p>Die zukünftige Aufgabe, die aus dieser Vorlage erstellt wird, hat diesen Dauertyp. <br>Der Dauertyp identifiziert die Beziehung zwischen folgenden Elementen:</p> 
         <ul>
         <li><p>Anzahl der einer Aufgabe zugewiesenen Ressourcen</p> </li>
         <li><p>Der Gesamtaufwand, der zum Abschließen der Aufgabe erforderlich ist</p></li> 
         <li><p>Die Gesamtdauer der Aufgabe </p></li></ul> <p>Mit Dauertypen können Sie konsistente Ressourcenzuweisungen basierend auf den Anforderungen der Aufgabe festlegen. Weitere Informationen zum Dauertyp einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den Dauertyp</a>.</p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
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
   </tbody> 
      </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

##### Finanzielle Details {#finance-1}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Finanzen“.

   ![Abschnitt „Vorlagenaufgabe bearbeiten - Finanzen“](assets/template-task-edit-finance.png)

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

   ODER

   Klicken Sie auf **Speichern**.

##### Benutzerdefinierte Formulare {#custom-forms-1}

Sie können benutzerdefinierte Formulare definieren, die standardmäßig an Aufgaben angehängt werden, wenn die Aufgaben zu einem Projekt hinzugefügt werden. Informationen dazu, wie Sie das Projekt so einrichten, dass es benutzerdefinierte Formulare für Standardaufgaben enthält, finden Sie im Abschnitt „Aufgaben“ im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Sie können auch benutzerdefinierte Formulare zu zukünftigen Aufgaben eines Projekts hinzufügen, wenn das Projekt aus einer Vorlage erstellt wird, indem Sie die benutzerdefinierten Formulare zu den Vorlagenaufgaben hinzufügen.

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Benutzerdefinierte Forms&quot;.

   ![Vorlagenaufgabe - Abschnitt zum Bearbeiten benutzerdefinierter Formulare](assets/template-task-edit-custom-forms.png)

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

   ODER

   Klicken Sie auf **Speichern**.

##### Einstellungen {#settings-1}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken Bereich auf **Einstellungen**.

   ![Abschnitt zum Bearbeiten der Einstellungen der Vorlagenaufgabe](assets/template-task-edit-settings.png)

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
      <td role="rowheader"><strong>Erinnerungsnachrichten</strong> </td> 
      <td> <p>Wählen Sie aus, welche Erinnerungsnachrichten Sie an die Vorlagenaufgabe anhängen möchten. Sie werden an zukünftige Aufgaben des Projekts angehängt, das aus dieser Vorlage erstellt wird. Ihr Systemadministrator muss Erinnerungsnachrichten konfigurieren, bevor Sie sie für eine Aufgabe auswählen können. Weitere Informationen zum Konfigurieren von Erinnerungsnachrichten finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsnachrichten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Genehmigungsprozess</strong> </td> 
      <td> <p>Wählen Sie den Genehmigungsprozess aus, den Sie mit der Vorlagenaufgabe verknüpfen möchten. Ihr Workfront-Administrator muss Aufgabengenehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Vorlagenaufgaben verknüpfen können. <span>Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.</p> <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen Folgendes: </p> 
       <ul> 
       <li>In der Liste werden nur aktive Genehmigungsprozesse angezeigt. </li> 
       <li> <p>In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Genehmigungsprozesse, die einer anderen Gruppe als der der Vorlage zugeordnet sind, werden nicht in der Liste angezeigt.</p> <p>Wichtig: Wenn sich die mit der Vorlage verknüpfte Gruppe ändert, wird der gruppenspezifische Genehmigungsprozess zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>. </p> </li> 
       <li> <p>Wenn Sie einen Genehmigungsprozess für den einmaligen Gebrauch hinzugefügt haben, wird er in diesem Feld als "&lt;Custom&gt;" angezeigt. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit</a>. </p>  </li> 
       <li> <p>Beim Massenbearbeiten von Vorlagenaufgaben gibt es die folgenden Szenarien:</p> 
       <ul> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus derselben Vorlagengruppe auswählen, werden in diesem Feld sowohl Genehmigungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt.</p> </li> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus verschiedenen Vorlagengruppen auswählen, werden in diesem Feld nur Genehmigungsprozesse auf Systemebene angezeigt.</p> </li> 
       <li> <p>Wenn einer der Vorlagenaufgaben ein Genehmigungsprozess für den einmaligen Gebrauch angehängt ist, wird sie durch den von Ihnen ausgewählten Genehmigungsprozess auf <span>- oder </span> ersetzt. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

##### Kommentar {#comment-1}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Kommentar.

   ![Abschnitt zum Bearbeiten von Kommentaren für Vorlagenaufgabe](assets/template-task-edit-comment.png)

1. Geben **im Bereich Aktualisierung zur Vorlagenaufgabe hinzufügen** einen Kommentar an, den Sie im Aktualisierungsprozess der Vorlagenaufgabe im Feld Verfügbar anzeigen möchten. Dieser Kommentar ist für alle sichtbar, die Ansichtszugriff auf die Vorlage und die Vorlagenaufgabe und Zugriff auf Ansichtsnotizen haben.
1. Klicken Sie auf **Speichern**.

   Wenn Sie oder ein anderer Benutzer ein Projekt aus dieser Vorlage erstellt, werden alle Einstellungen, die Sie auf Vorlagenaufgaben angewendet haben, zu den Einstellungen für die Projektaufgaben.


<div class="preview">

### Vorlagenaufgaben in der Vorschau-Umgebung bearbeiten

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

1. (Bedingt) Um alle Informationen zu einer Vorlagenaufgabe oder zu mehreren Aufgaben gleichzeitig zu bearbeiten, wählen Sie diese aus einer Liste aus und klicken Sie dann oben in der Liste auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png).

   Das **Vorlagenaufgabe bearbeiten** wird angezeigt.

   ![Neues Erlebnis für Vorlagenaufgabe bearbeiten](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >Sie können auch eine Vorlagenaufgabe in einer Liste auswählen und dann rechts neben dem Namen der Vorlagenaufgabe in der Kopfzeile auf **Bearbeiten** klicken, um das Feld **Vorlagenaufgabe bearbeiten** zu öffnen.

1. Erwägen Sie, Informationen in einem der folgenden Abschnitte anzugeben:

* [Name der Vorlagenaufgabe](#template-task-name)
* [Übersicht](#overview-2)
* [Arbeitsaufträge](#assignments-2)
* [Finanzielle Details](#finance-2)
* [Benutzerdefinierte Formulare](#custom-forms-2)
* [Einstellungen](#settings-2)
* [Kommentar](#comment-2)

1. Fahren Sie mit der Bearbeitung der Vorlagenaufgaben wie in den folgenden Abschnitten beschrieben fort.

#### Name der Vorlagenaufgabe

>[!TIP]
>
>Der Abschnitt „Name der Vorlagenaufgabe“ ist nicht verfügbar, wenn Vorlagenaufgaben stapelweise bearbeitet werden.


1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie im Feld Vorlagenaufgabe bearbeiten auf **Name der Vorlagenaufgabe** und fügen Sie einen Namen für die Vorlagenaufgabe hinzu.

   Diese Ansicht ist nicht verfügbar, wenn Vorlagenaufgaben stapelweise bearbeitet werden.

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

#### Übersicht {#overview-2}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken Bereich auf **Übersicht**.

   ![Abschnitt zum Bearbeiten der Vorlagenaufgabe - Übersicht](assets/template-task-edit-overview.png)

1. Aktualisieren Sie eines der folgenden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie zusätzliche Informationen zur Vorlagenaufgabe hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Dies ist eine visuelle Markierung, mit der Sie Ihre Vorlagenaufgaben priorisieren können. </p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Kein</strong> </p> </li> 
        <li> <p><strong>Niedrig</strong> </p> </li> 
        <li> <p> <b>normal</b></p> </li> 
        <li> <p><b>Hoch</b> </p> </li> 
        <li> <p><b>Dringlich</b> </p> </li> 
       </ul> <p>Je nach den vom Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Prioritäten für Sie unterschiedlich sein. Weitere Informationen zum Bearbeiten von Prioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a>.</p> </td> 
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
        <li>Nicht früher anfangen als</li> 
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
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Geben Sie einen Weblink an, der sich auf die Informationen zur Vorlagenaufgabe bezieht.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Work Effort</strong> </td> 
      <td>Wählen Sie aus den folgenden Optionen:
      <ul><li>Klein</li>
      <li>Mittel</li>
      <li>Groß</li></ul>

   <p><b>WICHTIG</b></p>
      <p>Das Feld Work Effort wird beim Bearbeiten einer Vorlagenaufgabe nur angezeigt, wenn Sie beim Bearbeiten der Vorlage die Einstellung <b>Work Effort zur automatischen Berechnung der geplanten Stunden </b> Aufgabe verwenden auswählen.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

#### Arbeitsaufträge {#assignments-2}

1. Beginnen Sie mit der Bearbeitung Ihrer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **linken** auf „Arbeitsaufträge“.

   Der **Arbeitsaufträge** wird geöffnet.

   ![Zuweisungen zu Vorlagenaufgaben](assets/assignments-edit-template-tasks-box.png)

1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, Aufgabengebiets oder Teams in das Feld **Personen, Rollen oder Teams suchen** und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.

1. Aktualisieren Sie die folgenden Informationen:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Dauertyp</td> 
   <td> <p>Dadurch wird die Beziehung zwischen folgenden Elementen identifiziert: </p> 
   <ul> 
   <li> <p>Die Anzahl der Ressourcen, die einer Aufgabe zugewiesen sind </p> </li> 
   <li> <p>Der Gesamtaufwand, der zum Abschließen der Aufgabe erforderlich ist </p> </li> 
   <li> <p> Die Gesamtdauer der Aufgabe. </p> </li> 
   </ul> <p>Ihr Workfront-Administrator oder ein Gruppenadministrator wählt die Standardeinstellung für den Dauertyp für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Informationen zum Festlegen von Projektstandards finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen</a>. </p> <p>Mit Dauertypen können Sie konsistente Ressourcenzuweisungen auf der Grundlage der Anforderungen der Aufgabe festlegen. Weitere Informationen zum Dauertyp einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den Dauertyp</a>. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
   <ul> 
   <li> <p>Berechnete Zuweisung </p> </li> 
   <li> <p> Berechnete Arbeit </p> </li> 
   <li> <p>Leistungsgesteuert </p> </li> 
   <li> <p>Einfach</p> </li> 
   </ul> </td> 
   </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Dauer pro Termin</td> 
   <td> <p>Wird nur für das übergeordnete Element der wiederkehrenden Aufgaben angezeigt. Sie zeigt die Dauer jeder wiederkehrenden Aufgabe an, wie sie bei der Erstellung der Aufgabe definiert wurde. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> <p> <b>HINWEIS</b>

   In einzelnen wiederkehrenden Aufgaben geänderte Dauer zeigt nicht den in diesem Feld angegebenen Wert an. </p> </td>
   </tr> 
   <tr> 
   <td role="rowheader">Dauer</td> 
   <td> 
   <div> 
   <div> 
   <p>Dies ist der Zeitraum, den Sie einer Aufgabe erlauben, offen zu bleiben, bevor sie abgeschlossen ist. </p> 
   <p><b>WICHTIG</b></p>
   <p>Da die Aufgabendauer in der Regel die Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum ist, wirkt sich dies auf die Zeitleiste des Projekts aus.</p> 
   <p>Gehen Sie wie folgt vor, um die Dauer der Aufgabe und die Zeiteinheit anzugeben:</p> 
   <ul> 
   <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Geben Sie die Zeitdauer ein und wählen Sie aus den verfügbaren Zeiteinheiten im Dropdown-Menü aus.</p> <p><b>TIPP</b></p>
   Wenn Sie die Dauer von Aufgaben in einer Aufgabenliste aktualisieren, können Sie die Abkürzung für die Zeiteinheit verwenden. </p> </li> 
   </ul> 
   <p> In der folgenden Tabelle können Sie zwischen den Optionen „Reguläre Zeit“ und „Verstrichene Zeit“ wählen: </p> 
   <table style="table-layout:auto"> 
   <col> 
   <col data-mc-conditions=""> 
   <tbody> 
   <tr> 
   <td>Zeiteinheit</td> 
   <td>Abkürzung</td> 
   </tr> 
   <tr> 
   <td>Minutes</td> 
   <td>M</td> 
   </tr> 
   <tr> 
   <td>Stunden</td> 
   <td>H</td> 
   </tr> 
   <tr> 
   <td>Tage. Dies ist der Standardwert. </td> 
   <td>D</td> 
   </tr> 
   <tr> 
   <td>Weeks</td> 
   <td>W</td> 
   </tr> 
   <tr> 
   <td>Months</td> 
   <td>T</td> 
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

   <p>Verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen.

   Die reguläre Zeit berücksichtigt Feiertage, Wochenenden und Auszeiten und schließt sie von der Dauer der Aufgabe aus. Weitere Informationen zur Aufgabendauer finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den </a>). </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Geplante Stunden</td> 
   <td> <p>Anzahl der geplanten Stunden für die Aufgabe angeben (in Stunden) Dies ist die tatsächliche Zeit, die die Verantwortlichen für die Aufgabe benötigen würden, um diese abzuschließen. Sie können die Anzahl der geplanten Stunden für eine Aufgabe nur angeben, wenn als Dauertyp Berechnete Zuweisung festgelegt ist. Weitere Informationen zu Dauertypen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und Dauertyp</a>.</p> 
   <b>HINWEIS</b>
   <p>
   Beim Erstellen wiederkehrender Aufgaben sind die geplanten Stunden die Stunden für jedes Vorkommen. Die geplanten Stunden der übergeordneten Aufgaben sind die Summe aller geplanten Stunden aus allen Vorfällen. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Zuteilung</td> 
   <td> <p>Wenn Ihre Aufgabenbeschränkung auf „Berechnete Arbeit“ oder „Arbeitsaufwand“ basiert, geben Sie <strong>Zuordnung %</strong> (Zuordnungsprozentsatz) für jeden Zugewiesenen an. Dies ist die Zeit aus dem Zeitplan des Verantwortlichen, die er für diese Aufgabe aufwenden kann. Wenn Sie den Zuordnungsprozentsatz für einen Verantwortlichen ändern, werden auch die geplanten Stunden einer Aufgabe geändert. </p> <p>Wenn die Aufgabenbeschränkung einfach ist, können Sie Folgendes angeben:</p> 
   <ul> 
   <li> <p>Zuweisungsstunden jedes Zugewiesenen.</p> </li> 
   <li> <p>Geplante Stunden der Aufgabe</p> </li> 
   <li> <p>Dauer der Aufgabe</p> </li> 
   </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Rolle des Zugewiesenen</td> 
   <td> <p>Wählen Sie eine Rolle aus dem Dropdown<strong>Menü „Rolle des Verantwortlichen</strong> aus, wenn Sie eine Person als Verantwortlicher ausgewählt haben. Dies ist die Rolle, die der Verantwortliche bei dieser Aufgabe erfüllen kann. </p> <p><b>TIPP</b>

   Im Dropdown-Menü werden nur die Aufgabengebiete angezeigt, die jedem Bearbeiter in seinem Profil zugeordnet sind.</p> </td>
   </tr> 
   </tbody> 
   </table>

1. Klicken **auf &quot;**&quot; oder fahren Sie mit den folgenden Abschnitten fort.

#### Finanzielle Details {#finance-2}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Finanzen“.

   ![Abschnitt „Vorlagenaufgabe bearbeiten - Finanzen“](assets/template-task-edit-finance.png)

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

   ODER

   Klicken Sie auf **Speichern**.

#### Benutzerdefinierte Formulare {#custom-forms-2}

Sie können benutzerdefinierte Formulare definieren, die standardmäßig an Aufgaben angehängt werden, wenn die Aufgaben zu einem Projekt hinzugefügt werden. Informationen dazu, wie Sie das Projekt so einrichten, dass es benutzerdefinierte Formulare für Standardaufgaben enthält, finden Sie im Abschnitt „Aufgaben“ im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Sie können auch benutzerdefinierte Formulare zu zukünftigen Aufgaben eines Projekts hinzufügen, wenn das Projekt aus einer Vorlage erstellt wird, indem Sie die benutzerdefinierten Formulare zu den Vorlagenaufgaben hinzufügen.

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Benutzerdefinierte Forms&quot;.

   ![Vorlagenaufgabe - Abschnitt zum Bearbeiten benutzerdefinierter Formulare](assets/template-task-edit-custom-forms.png)

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

   ODER

   Klicken Sie auf **Speichern**.

#### Einstellungen {#settings-2}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken Bereich auf **Einstellungen**.

   ![Abschnitt zum Bearbeiten der Einstellungen der Vorlagenaufgabe](assets/template-task-edit-settings.png)

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
      <td role="rowheader"><strong>Erinnerungsnachrichten</strong> </td> 
      <td> <p>Wählen Sie aus, welche Erinnerungsnachrichten Sie an die Vorlagenaufgabe anhängen möchten. Sie werden an zukünftige Aufgaben des Projekts angehängt, das aus dieser Vorlage erstellt wird. Ihr Systemadministrator muss Erinnerungsnachrichten konfigurieren, bevor Sie sie für eine Aufgabe auswählen können. Weitere Informationen zum Konfigurieren von Erinnerungsnachrichten finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsnachrichten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Genehmigungsprozess</strong> </td> 
      <td> <p>Wählen Sie den Genehmigungsprozess aus, den Sie mit der Vorlagenaufgabe verknüpfen möchten. Ihr Workfront-Administrator muss Aufgabengenehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Vorlagenaufgaben verknüpfen können. <span>Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.</p> <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen Folgendes: </p> 
       <ul> 
       <li>In der Liste werden nur aktive Genehmigungsprozesse angezeigt. </li> 
       <li> <p>In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Genehmigungsprozesse, die einer anderen Gruppe als der der Vorlage zugeordnet sind, werden nicht in der Liste angezeigt.</p> <p>Wichtig: Wenn sich die mit der Vorlage verknüpfte Gruppe ändert, wird der gruppenspezifische Genehmigungsprozess zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>. </p> </li> 
       <li> <p>Wenn Sie einen Genehmigungsprozess für den einmaligen Gebrauch hinzugefügt haben, wird er in diesem Feld als "&lt;Custom&gt;" angezeigt. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit</a>. </p>  </li> 
       <li> <p>Beim Massenbearbeiten von Vorlagenaufgaben gibt es die folgenden Szenarien:</p> 
       <ul> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus derselben Vorlagengruppe auswählen, werden in diesem Feld sowohl Genehmigungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt.</p> </li> 
       <li> <p>Wenn Sie Vorlagenaufgaben aus verschiedenen Vorlagengruppen auswählen, werden in diesem Feld nur Genehmigungsprozesse auf Systemebene angezeigt.</p> </li> 
       <li> <p>Wenn einer der Vorlagenaufgaben ein Genehmigungsprozess für den einmaligen Gebrauch angehängt ist, wird sie durch den von Ihnen ausgewählten Genehmigungsprozess auf <span>- oder </span> ersetzt. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den Informationen, die Sie ändern möchten, mit der Bearbeitung der folgenden Abschnitte fort.

   ODER

   Klicken Sie auf **Speichern**.

#### Kommentar {#comment-2}

1. Beginnen Sie mit der Bearbeitung einer Vorlagenaufgabe, wie oben beschrieben.
1. Klicken Sie **Feld „Vorlagenaufgabe bearbeiten** im linken **auf** Kommentar.

   ![Abschnitt zum Bearbeiten von Kommentaren für Vorlagenaufgabe](assets/template-task-edit-comment.png)

1. Geben **im Bereich Aktualisierung zur Vorlagenaufgabe hinzufügen** einen Kommentar an, den Sie im Aktualisierungsprozess der Vorlagenaufgabe im Feld Verfügbar anzeigen möchten. Dieser Kommentar ist für alle sichtbar, die Ansichtszugriff auf die Vorlage und die Vorlagenaufgabe und Zugriff auf Ansichtsnotizen haben.
1. Klicken Sie auf **Speichern**.

   Wenn Sie oder ein anderer Benutzer ein Projekt aus dieser Vorlage erstellt, werden alle Einstellungen, die Sie auf Vorlagenaufgaben angewendet haben, zu den Einstellungen für die Projektaufgaben.

</div>


