---
product-area: projects
navigation-topic: manage-projects
title: Projekte bearbeiten
description: Sie können ein Projekt in Adobe Workfront beliebig oft bearbeiten. Idealerweise sollten Sie ein Projekt bearbeiten, wenn sich das Projekt im Planungsstatus befindet.
author: Alina
feature: Work Management, Projects
role: User
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: 2ca8539855c2b08d71f47ad2e1b698496456f022
workflow-type: tm+mt
source-wordcount: '7513'
ht-degree: 1%

---

# Projekte bearbeiten

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

Sie können ein Projekt in Adobe Workfront beliebig oft bearbeiten. Es wird empfohlen, Projekte nur geringfügig nach Statusänderungen in &quot;Aktuell&quot;zu bearbeiten, um Verwirrung zu vermeiden, indem Benachrichtigungen über Änderungen an das gesamte Projektteam gesendet werden.

Idealerweise sollten Sie ein Projekt bearbeiten, wenn sich das Projekt im Planungsstatus befindet. Weitere Informationen zum Projektteam finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard </p> 
   Oder
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
     <p>Berechtigungen für ein Projekt verwalten </p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einschränkungen bei der Bearbeitung von Projekten

Es gibt einige Einschränkungen, die Sie daran hindern können, Projekte zu bearbeiten.

Beachten Sie beim Bearbeiten von Projekten Folgendes:

* Sie können keine Projekte bearbeiten, die sich in einem Genehmigungsprozess befinden, außer zur Protokollierung und Änderung des Status.
* Sie können nur dann Dokumente oder Vorlagen an ein Projekt anhängen, das den Status &quot;Abgeschlossen&quot;, &quot;Unbeendet&quot;oder &quot;Ausstehende Genehmigung&quot;aufweist, wenn diese Funktion im Bereich &quot;Projekteinstellungen&quot;von Ihrem Workfront-Administrator oder einem Gruppenadministrator aktiviert wurde. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Konfigurieren von systemweiten Projekteigenschaften](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sie können die folgenden Informationen zu einem Projekt nur im Status &quot;Dead&quot;oder &quot;Complete&quot;bearbeiten:

   * Ändern Sie bestehende Ausgaben.
   * Fügen Sie benutzerdefinierte Formulare hinzu, entfernen Sie sie oder bearbeiten Sie sie.

## Projekt bearbeiten

Durch Bearbeiten eines Projekts können Sie Informationen und Einstellungen für das Projekt sowie Aufgaben und Probleme im Projekt ändern.

Einige in diesem Artikel erwähnte Einstellungen können von ihrem Standardstatus in der Vorlage geändert werden, aus der das Projekt erstellt wurde.

Weitere Informationen zum Bearbeiten von Vorlagen finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Informationen zum Erstellen eines Projekts aus einer Vorlage finden Sie unter [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

{{step1-to-projects}}

1. (Optional) Klicken Sie in der oberen rechten Ecke auf **Projekte, die ich verwende** oder **Projekte, deren Eigentümer ich bin** , um Projekte anzuzeigen, deren Eigentümer Sie sind, oder Projekte, deren Teil Sie sind.

   ![](assets/projects-on-my-own-buttons-350x302.png)

   >[!NOTE]
   >
   >Wenn Sie Gruppenadministrator sind, können Sie die Projekte Ihrer Gruppe im Bereich Gruppen sowie im Bereich Projekte anzeigen und bearbeiten. Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Klicken Sie auf den Namen des Projekts, das Sie bearbeiten möchten, um die Projektseite zu öffnen.

1. (Optional) Um beschränkte Informationen zu einem Projekt zu bearbeiten, klicken Sie im linken Bereich auf **Projektdetails** . Wenn Sie alle Informationen zum Projekt bearbeiten möchten, fahren Sie mit Schritt 5 fort. <!--accurate?!-->

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layoutvorlage geändert hat, werden die Felder im Bereich Projektdetails möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Gehen Sie wie folgt vor, um Informationen im Abschnitt Details zu bearbeiten:

   1. (Optional) Klicken Sie oben rechts auf das Symbol **Alle reduzieren** ![](assets/collapse-icon.png) , um alle Bereiche zu reduzieren.
   1. (Optional und bedingt) Wenn ein Bereich ausgeblendet wird, klicken Sie neben jedem Bereich auf den Pfeil **rechts zeigen** ![](assets/right-pointing-arrow.png) , um den zu bearbeitenden Bereich zu erweitern.
   1. Weitere Informationen zur Bearbeitung von Informationen auf der Registerkarte Projektdetails finden Sie in den folgenden Artikeln:

      * [Verwalten von Informationen im Bereich &quot;Projektübersicht&quot;](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [Verwalten von Informationen im Bereich &quot;Projekt-Finanzen&quot;](../../../manage-work/projects/project-finances/manage-project-finance-area.md)

   1. (Optional) Um ein benutzerdefiniertes Formular anzuhängen, geben Sie den Namen eines Formulars in das Feld **Benutzerdefiniertes Formular hinzufügen** ein, wählen Sie es aus, wenn es in der Liste angezeigt wird, und klicken Sie dann auf **Änderungen speichern**.
   1. (Optional) Klicken Sie auf das Symbol **Exportieren** ![](assets/export.png), um die Übersicht und die benutzerdefinierten Formulardaten in eine PDF-Datei zu exportieren, und klicken Sie dann auf **Exportieren**. Wählen Sie aus den folgenden Optionen aus:

      * Alle auswählen (wird nur angezeigt, wenn mindestens ein benutzerdefiniertes Formular angehängt ist)
      * Übersicht
      * Der Name eines oder mehrerer benutzerdefinierter Formulare

      Die PDF-Datei wird auf Ihren Computer heruntergeladen.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Weitere Informationen finden Sie unter [Exportieren benutzerdefinierter Formulare und Objektdetails](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Informationen zu den Feldern, die im Abschnitt Projektdetails angezeigt werden, erhalten Sie, wenn Sie mit der Bearbeitung des Projekts im Feld Projekt bearbeiten fortfahren, wie unten beschrieben.
1. Um alle Informationen zum Projekt zu bearbeiten, klicken Sie auf das Menü **Mehr** neben dem Namen des Projekts und dann auf **Bearbeiten**.![](assets/qs-more-menu.png)

   Oder

   Wählen Sie aus einer Liste von Projekten ein oder mehrere Projekte aus und klicken Sie dann oben in der Liste auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) .

   Weitere Informationen zum Bearbeiten von Projekten in großen Mengen finden Sie im Abschnitt [Projekte stapelweise bearbeiten](#edit-projects-in-bulk) in diesem Artikel.

   Das Feld **Projekt bearbeiten** wird geöffnet.

   >[!IMPORTANT]
   >
   >Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, damit die Option &quot;Bearbeiten&quot;angezeigt wird.

   Alle Projektfelder sind im Feld Projekt bearbeiten verfügbar und werden nach den im linken Bereich aufgelisteten Bereichen gruppiert.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layoutvorlage geändert hat, werden die Bereiche im linken Bereich des Felds &quot;Projekt bearbeiten&quot;oder die in diesen Bereichen aufgelisteten Felder möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Bedingt) Wenn Sie auf das Menü **Mehr** und dann auf **Bearbeiten** geklickt haben, aktualisieren Sie die Informationen in einem der folgenden Bereiche, die im linken Bereich aufgelistet sind:

   * [Projektname](#project-name)
   * [Überblick](#overview)
   * [Benutzerdefinierte Formulare](#custom-forms)
   * [Finance](#finance)
   * [Projekteinstellungen](#project-settings)
   * [Aufgabeneinstellungen](#task-settings)
   * [Problemeinstellungen](#issue-settings)
   * [Zugriff](#access)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator unsere Layoutvorlage für den Bereich Details des Projekts eingerichtet hat, können sich die Abschnitte und Felder im Feld Projekt bearbeiten in Ihrer Umgebung unterscheiden. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Projektname {#project-name}

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Projektname** .

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. Aktualisieren Sie den Namen des Projekts.

   Sie können den Projektnamen nicht bearbeiten, wenn Sie Projekte stapelweise bearbeiten.

### Übersicht {#overview}

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Überblick** .

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. Aktualisieren Sie die folgenden Informationen zum Projekt:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader"><strong>Beschreibung</strong> </td> 
         <td> <p>Fügen Sie zusätzliche Informationen zum Projekt hinzu.</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Status</strong> </td> 
         <td> <p>Wählen Sie den Status des Projekts aus. Sie können ein Projekt nicht als abgeschlossen markieren, bevor alle Aufgaben und Probleme abgeschlossen sind. Weitere Informationen zum Projektstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemprojektstatus</a></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Priorität</strong> </td> 
         <td> <p> <p>Dies ist nur ein visuelles Flag für Sie, mit dem Sie Ihre Projekte priorisieren können.</p> <p>Je nach den von Ihrem Workfront-Administrator ausgewählten Projekteinstellungen können die Prioritätsnamen für Sie unterschiedlich sein. Weitere Informationen zu Bearbeitungsprioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>URL</strong> </td> 
         <td> <p>Geben Sie einen Web-Link an, der sich auf Informationen zu diesem Projekt bezieht.</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Bedingungstyp</strong> </td> 
         <td> <p>Wählen Sie zwischen den folgenden Bedingungstypen aus: 
         <ul> 
         <li><strong>Manuell:</strong> Der Projektinhaber legt die Bedingung für das Projekt manuell fest.</li> 
         <li><strong>Fortschrittsstatus:</strong> Workfront legt die Bedingung automatisch basierend auf dem Fortschrittsstatus von Aufgaben auf dem kritischen Pfad fest. Weitere Informationen zum Fortschritt finden Sie unter <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Aufgabenfortschrittsstatus - Übersicht</a>.</li> 
         </ul><p>Ihr Workfront-Administrator<span> oder ein Gruppenadministrator</span> wählt die Standardeinstellung für die Berechnung der Projektbedingung für Ihr System aus <span> oder Ihre Gruppe</span>. Weitere Informationen zum Festlegen der Projektnormen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projekteigenschaften konfigurieren</a>. </p></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Bedingung</strong> </td> 
         <td> <p> <p>(Wird nur angezeigt, nachdem Sie für den Bedingungstyp <strong> die Option <strong>Manuell</strong> ausgewählt haben): Wählen Sie eine Bedingung aus, um anzugeben, wie das Projekt ausgeführt wird.</strong> </p> <p>Informationen dazu, wie Projektbedingungen automatisch oder manuell festgelegt werden können, finden Sie unter <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Überblick über Projektbedingungen und Bedingungstyp</a></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Zeitplanmodus</strong> </td> 
         <td> <p>Geben Sie an, ob das Projekt ab dem Startdatum oder ab dem Abschlussdatum geplant ist. Diese Auswahl bestimmt die geplanten Termine der Aufgaben für das Projekt. 
         <ul> 
         <li><strong>Startdatum</strong>: Die erste Aufgabe des Projekts hat standardmäßig dasselbe geplante Startdatum wie das Projekt. Informationen zum geplanten Startdatum der Aufgabe finden Sie unter <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Übersicht über das geplante Startdatum der Aufgabe</a>. Die Projekt-Timeline berechnet vom Startdatum aus und das Abschlussdatum des Projekts wird vom System basierend auf der Dauer aller Aufgaben berechnet. </li> 
         <li><strong>Abschlussdatum</strong>: Die letzte Aufgabe des Projekts hat dasselbe geplante Abschlussdatum wie das Projekt. Die Projekt-Timeline berechnet vom Abschlussdatum aus und das Projektstartdatum wird vom System berechnet, indem die Dauer aller Aufgaben vom Abschlussdatum des Projekts abgezogen wird. </li> 
         </ul><p>Ihr Workfront-Administrator<span> oder ein Gruppenadministrator</span> wählt die Standardeinstellung für den Zeitplanmodus für Ihr System oder Ihre Gruppe aus. Weitere Informationen zum Festlegen der Projektnormen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projekteigenschaften konfigurieren</a>.</p></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Vorgesehenes Startdatum und -uhrzeit</strong> </td> 
         <td> <p> <p>Geben Sie das Datum an, an dem Sie <strong>Vom Startdatum planen</strong> auswählen. <br></p> <p>Dies ist ein schreibgeschütztes Feld, wenn Sie <strong>Vom Abschlussdatum planen</strong> auswählen.<br></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Geplantes Abschlussdatum und -zeit</strong> </td> 
         <td> <p>Geben Sie das Datum an, an dem Sie <strong>vom Abschlussdatum planen</strong> auswählen. </p> <p>Dies ist ein schreibgeschütztes Feld, wenn Sie <strong>Vom Startdatum planen</strong> auswählen.<br></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Portfolio</strong></td> 
         <td>Geben Sie ein Portfolio an, zu dem das Projekt gehört. Sie müssen zuerst ein Portfolio erstellen, bevor es in der Dropdownliste angezeigt wird. Nur aktive Portfolios können mit einem Projekt verknüpft werden. Weitere Informationen zum Erstellen von Portfolios finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Erstellen eines Portfolios </a>.
         <p><b>NOTIZ</b></p>
         <p>Sie müssen über Verwaltungsberechtigungen für das Portfolio verfügen, um es zum Projekt hinzufügen oder entfernen zu können.</p>
      </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Programm</strong></td> 
         <td> <p>Wenn Sie ein Portfolio für das Projekt ausgewählt haben, geben Sie ein Programm für das Projekt an. Einige Portfolios haben möglicherweise keine Programme. Sie müssen zunächst ein Programm erstellen, bevor es in dieser Dropdown-Liste angezeigt wird. Nur aktive Programme können mit einem Projekt verknüpft werden. </p> <p>Weitere Informationen zum Erstellen von Programmen finden Sie unter <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Programm erstellen</a>.</p> 
      <p><b>NOTIZ</b></p>
         <p>Sie müssen über Verwaltungsberechtigungen für das Programm verfügen, um es zum Projekt hinzufügen oder entfernen zu können.</p>   
      </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Gruppe</strong></td> 
         <td> <p> <p>Geben Sie den Namen der mit dem Projekt verknüpften Gruppe an. </p>Dies ist ein erforderliches Feld. Sie können kein Projekt haben, das keiner Gruppe zugeordnet ist. </p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">"klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> Standardmäßig wird eine der folgenden Gruppen bei der Erstellung automatisch mit einem Projekt verknüpft, es sei denn, Sie geben eine andere Gruppe an:</p> 
         <ul> 
         <li> <p><span>Wenn das Projekt aus dem Bereich "Projekte"erstellt wird, wird die Startseite des Projekterstellers mit dem Projekt verknüpft.</span> </p> <p>Dies gilt auch, wenn das Projekt über den Abschnitt Projekte in einem Portfolio oder Programm erstellt wird.</p> </li> 
         <li> <p>Wenn das Projekt über die Hauptseite einer Gruppe im Bereich Einrichtung erstellt wird, wird diese Gruppe mit dem Projekt verknüpft.</p> </li> 
         </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
         <p><b>HINWEISE</b></p>
         <ul>
         <li><p>Wenn das Projekt oder seine Aufgaben oder Probleme mit einem benutzerdefinierten Status auf Gruppenebene verknüpft sind, kann das Ändern der Gruppe des Projekts dazu führen, dass sich der Status des Projekts, der Aufgaben oder Probleme entsprechend der neuen Gruppe ändern.</p></li>
         <li><p>Wenn das Projekt oder seine Aufgaben oder Probleme bereits mit einem Validierungsprozess auf Gruppenebene mithilfe benutzerdefinierter Status auf Gruppenebene verknüpft sind, kann das Ändern der Gruppe zu einem Konflikt zwischen den Genehmigungsstatus der vorherigen Gruppe und den auf Systemebene vorhandenen führen.</p>
         <p>Erwägen Sie, die Genehmigungsprozesse auf Gruppenebene für das Projekt oder dessen Aufgaben oder Probleme zu entfernen, bevor Sie die Gruppe aktualisieren.</p>
         <p>Informationen zum Erstellen von Genehmigungsprozessen auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Genehmigungsprozesse auf Gruppenebene</a>.</p>
         <p>Informationen zum Erstellen eines benutzerdefinierten Status auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Gruppenstatus</a></p></li></ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Firma</strong> </td> 
         <td> <p>Geben Sie ein mit dem Projekt verknüpftes Unternehmen an. Sie müssen ein Unternehmen erstellen, bevor Sie es mit einem Projekt verknüpfen können. Nur aktive Unternehmen können mit einem Projekt verknüpft werden. Informationen zum Erstellen von Unternehmen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Erstellen und Bearbeiten von Unternehmen</a>.</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Projektbesitzer</strong> </td> 
         <td> <p>Beginnen Sie mit der Eingabe des Namens eines Benutzers, der ihn zum Projekt hinzufügen soll, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Der Benutzer wird dem Projektteam hinzugefügt und erhält automatisch die Berechtigung zum Verwalten des Projekts. Der Benutzer, der als Projekteigentümer bestimmt wurde, muss ein aktiver Workfront-Benutzer sein.</p>
         </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Projektsponsor</strong> </td> 
         <td> <p>Beginnen Sie mit der Eingabe des Namens eines Benutzers, der ihn zum Projekt hinzufügen soll, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Der Benutzer wird dem Projektteam hinzugefügt und erhält automatisch Ansichtsberechtigungen für das Projekt. Der Benutzer, der als Projektsponsor benannt wurde, muss ein aktiver Benutzer von Workfront sein.<br></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Ressourcenmanager</strong> </td> 
         <td> <p> Beginnen Sie mit der Eingabe der Namen der Benutzer, die zum Projekt hinzugefügt werden sollen, und wählen Sie sie aus, wenn sie in der Liste angezeigt werden. Die Benutzer werden dem Projektteam hinzugefügt und erhalten automatisch Verwaltungsberechtigungen für das Projekt und können den Aufgaben und Problemen im Projekt Ressourcen zuweisen. Benutzer behalten die Verwaltungsberechtigungen für das Projekt bei, selbst wenn sie aus dem Feld "Ressourcen-Manager"entfernt wurden. Sie können mehr als einen Ressourcen-Manager angeben.<br></p> </td> 
      </tr>

   <tr> 
         <td role="rowheader"><strong>Urheber eines konvertierten Problems</strong> </td> 
         <td> <p> Standardmäßig wird dieses Feld automatisch mit dem Namen des Benutzers ausgefüllt, der das Problem erstellt hat, aus dem das Projekt konvertiert wurde. Sie können diesen Namen mit dem Namen eines anderen Benutzers in Workfront aktualisieren. <br></p> </td> 
      </tr>

   </tbody> 
      </table>

   >[!TIP]
   >
   >Beachten Sie beim Aktualisieren der Felder &quot;Projekteigentümer&quot;, &quot;Projektsponsor&quot;und &quot;Ressourcen-Manager&quot;den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
   >
   >Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
   >
   >Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort

   Oder

   Klicken Sie auf **Speichern**.

### Benutzerdefinierte Formulare {#custom-forms}

Je nach Zugriffsebene und Ihrer Berechtigung für das Projekt gibt es die folgenden Szenarien:

* Wenn Sie nicht über die Berechtigung &quot;Benutzerdefiniertes Formular bearbeiten&quot;für das Projekt verfügen, können Sie die Felder für die angehängten benutzerdefinierten Formulare nicht bearbeiten. Sie können nur die Felder in den benutzerdefinierten Formularen anzeigen, die an das Projekt angehängt sind.
* Wenn Sie Zugriff auf einen Abschnitt in einem benutzerdefinierten Formular haben, können Sie die Felder in diesem Abschnitt nicht bearbeiten.
* Wenn Sie keinen Zugriff auf einen Abschnitt in einem der benutzerdefinierten Formulare haben, die an das Projekt angehängt sind, wird der Abschnitt nicht im Feld Projekt bearbeiten angezeigt.

Bei der Auswahl von mehr als einem Projekt zur Massenbearbeitung gibt es die folgenden Szenarien:

* Wenn Sie nicht über die Berechtigung &quot;Benutzerdefiniertes Formular bearbeiten&quot;für mindestens eines der ausgewählten Projekte verfügen, können Sie die Felder für die angehängten benutzerdefinierten Formulare nicht bearbeiten. Sie können nur die Felder in den angehängten benutzerdefinierten Formularen anzeigen
* Wenn Sie Zugriff auf einen Abschnitt in einem benutzerdefinierten Formular haben, können Sie die Felder in diesem Abschnitt nicht bearbeiten. Sie können nur die Felder in diesem Abschnitt anzeigen.
* Wenn Sie keinen Zugriff auf einen Abschnitt in einem der benutzerdefinierten Formulare haben, die an mindestens ein Projekt angehängt sind, wird der Abschnitt nicht im Feld Projekte bearbeiten angezeigt.
* Wenn Sie erforderliche Felder in einem der benutzerdefinierten Formulare haben, die an alle Projekte angehängt sind, und Sie ein Feld auswählen, ohne es tatsächlich zu bearbeiten, müssen Sie die Änderungen in diesem Feld verwerfen oder Informationen hinzufügen, bevor Sie die ausgewählten Projekte speichern können. Wenn Sie kein erforderliches Feld auswählen, können Sie die ausgewählten Projekte auch dann speichern, wenn das erforderliche Feld leer ist.

Informationen zum Zugriff auf benutzerdefinierte Formulare finden Sie in den folgenden Artikeln:

* [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [Formular organisieren und in der Vorschau anzeigen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)

So bearbeiten Sie Informationen zu benutzerdefinierten Formularen beim Bearbeiten eines Projekts:

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms** .

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. Klicken Sie auf das Feld **Benutzerdefiniertes Formular hinzufügen** und wählen Sie ein Formular aus der Liste aus, um es an das Projekt anzuhängen. Standardmäßig werden die ersten 40 Formulare in alphabetischer Reihenfolge angezeigt. Wenn das Formular nicht in der Liste angezeigt wird, geben Sie den Namen ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Sie können einem Projekt bis zu zehn benutzerdefinierte Formulare hinzufügen.


1. (Bedingt) Wenn Sie ein benutzerdefiniertes Formular an das Projekt angehängt haben, bearbeiten Sie alle Felder im Formular. Sie müssen alle erforderlichen Felder angeben, bevor Sie das Projekt speichern können.
1. (Optional) Klicken Sie auf das Symbol **X** rechts neben dem Namen eines benutzerdefinierten Formulars, um es zu entfernen, und klicken Sie dann auf **Entfernen**.
1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort

   Oder

   Klicken Sie auf **Speichern**.

### Finanzielle Details {#finance}

Je nach Zugriffsebene und Ihrer Berechtigung für das Projekt gibt es die folgenden Szenarien:

* Wenn Sie Zugriff auf Finanzdaten anzeigen und Finanzberechtigungen für das Projekt anzeigen können, können Sie nur die Felder im Abschnitt Finanzen anzeigen. Die Felder in diesem Abschnitt können nicht bearbeitet werden.
* Wenn Sie Zugriff auf Finanzdaten bearbeiten und Finanzberechtigungen für das Projekt verwalten haben, können Sie die Felder in diesem Abschnitt aktualisieren.

Wenn Sie mehrere Projekte auswählen, um sie stapelweise zu bearbeiten, gibt es die folgenden Szenarien:

* Wenn Sie mindestens ein Projekt auswählen, für das Sie über View Finance-Berechtigungen (anstelle von &quot;Manage Finance&quot;-Berechtigungen) verfügen, können Sie die Felder in diesem Abschnitt nur für alle ausgewählten Projekte anzeigen. Sie können die Felder im Abschnitt Finanzen nicht stapelweise bearbeiten.
* Wenn Sie mindestens ein Projekt auswählen, für das Sie keine Finanzberechtigungen haben, wird dieser Abschnitt überhaupt nicht angezeigt.

So bearbeiten Sie Felder im Finanzbereich:


1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Finance** .

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. Aktualisieren Sie die folgenden Finanzinformationen für das Projekt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Währung</strong> </td> 
      <td> <p> <p>Geben Sie die Währung für das Projekt an, wenn sie sich von der Standardwährung Ihres Systems unterscheidet. Sie können die Währung eines Projekts nicht ändern, wenn bereits finanzielle Informationen zum Projekt vorhanden sind. Dieses Feld ist nicht sichtbar, wenn Sie nur die Standardwährung im System haben. </p> <p>Weitere Informationen zur Währung finden Sie unter <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong> </td> 
      <td> Geben Sie ein Budget für das Projekt an. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Leistungsindex-Methode</strong> </td> 
      <td> <p>Wählen Sie "<b>Stündbasiert</b>"oder "<b>Kostenbasiert</b>", um anzugeben, ob die Metriken zum Earned Value des Projekts (z. B. Kosten-Leistungs-Index oder Geschätzte tatsächliche Kosten) anhand von Stunden oder Kosten berechnet werden. </p> <p>Weitere Informationen zur Leistungsindex-Methode finden Sie unter <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Festlegen der Leistungsindex-Methode (PIM)</a>. </p> <p>Ihr Workfront-Administrator<span> oder ein Gruppenadministrator</span> wählt die standardmäßige Leistungsindex-Methodeneinstellung für Ihr System oder Ihre Gruppe aus. Weitere Informationen zum Festlegen der Projektnormen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projekteigenschaften konfigurieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schätzen nach Abschluss</strong> </td> 
      <td> <p> <p>Geben Sie an, wie Workfront die Schätzung bei Abschluss (EAC) berechnen soll. </p>
      Wählen Sie aus den folgenden Optionen aus: 
      <ul><li><b>Kalkulation auf Projektebene</b></li>
      <li><b>Aufrollen aus Aufgaben/Unteraufgaben</b></li> </ul>
      <p>Weitere Informationen zur Berechnung der Schätzung bei Abschluss finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schätzung bei Abschluss berechnen (EAC)</a>.</p> <p>Ihr Workfront- oder Gruppenadministrator wählt die standardmäßige Einstellung Geschätzte bei Abschluss für Ihr System oder Ihre Gruppe aus. Weitere Informationen zum Festlegen der Projektnormen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projekteigenschaften konfigurieren</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplanter Vorteil</strong> </td> 
      <td> <p>Schätzen Sie, welchen Nutzen das Projekt für Sie hat. Dies wird im Geschäftsfall des Projekts und im Portfolio Optimizer verwendet. Weitere Informationen zum geplanten Nutzen eines Projekts finden Sie unter <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Übersicht über den geplanten Nutzen eines Projekts</a>. Der geplante Nutzen eines Projekts wird bei der Berechnung des Nettowerts eines Projekts berücksichtigt. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Verwalten von Projekten im Portfolio Optimizer</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tatsächlicher Vorteil</strong> </td> 
      <td> <p>Schätzen des tatsächlichen Nutzens des Projekts. Dies ist ein Währungsbetrag, der den Vorteil darstellt, den Ihr Unternehmen oder Ihre Abteilung nach Abschluss dieses Projekts erzielen würde. </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>Feste Kosten</strong> </td> 
      <td> <p>Geben Sie die Festkosten für das Projekt an. Dies unterscheidet sich von den Arbeitskosten, die sich aus den Stunden auf dem Projekt ergeben, und den Kosten, die aus den Kosten des Projekts entstehen. Die Fixkosten eines Projekts werden bei der Berechnung des Nettowerts eines Projekts berücksichtigt und sind Teil der Budgetierten Kosten.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fester Umsatz</strong> </td> 
      <td> <p>Geben Sie den festen Umsatz für das Projekt an.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Projekteinstellungen {#project-settings}

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Projekteinstellungen** .

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Aktualisieren Sie die folgenden Informationen:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Milestone-Pfad</strong> </td> 
       <td> <p>Wählen Sie einen Milestone-Pfad für das Projekt aus. In der Liste werden nur aktive Meilensteinpfade angezeigt.</p> <p>Weitere Informationen zu Meilensteinpfaden finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Meilensteinpfad erstellen</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Abschlussmodus</strong> </td> 
      <td> <p>Steuert, wie das Projekt als abgeschlossen markiert wird. Wählen Sie aus den folgenden Optionen aus: 
       <ul> 
       <li><p><strong>Automatisch</strong>: Das Projekt wird als abgeschlossen markiert, wenn alle Aufgaben und Probleme abgeschlossen sind.</p><p>Der Projektstatus wird nur dann automatisch in Abgeschlossen geändert, wenn der Projektstatus Aktuell ist, wenn die Aufgaben abgeschlossen sind. </p></li> 
       <li><strong>Manuell</strong>: Sie müssen den Status "Fertig stellen"für das Projekt manuell auswählen, wenn alle Aufgaben und Probleme abgeschlossen sind.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Zusammenfassung - Fertigstellungsmodus</strong></td> 
       <td> <p>Steuert, wie die übergeordneten Aufgaben als abgeschlossen markiert werden. Wählen Sie aus den folgenden Optionen aus: 
       <ul> 
       <li><strong>Automatisch</strong>: Die übergeordneten Aufgaben sind als "Abgeschlossen"markiert und aktualisieren ihren Prozentsatz automatisch, wenn die untergeordneten Aufgaben abgeschlossen und der Prozentsatz an abgeschlossen der untergeordneten Aufgaben aktualisiert wird. </li> 
       <li><strong>Manuell</strong>: Sie müssen den prozentualen Abschluss und den Status der übergeordneten Aufgaben manuell aktualisieren, unabhängig davon, welche Änderungen an den untergeordneten Aufgaben vorgenommen werden. Auf diese Weise können Sie eine übergeordnete Aufgabe als abgeschlossen markieren, selbst wenn die Unteraufgaben unvollständig sind. </li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Update-Typ</strong></td> 
       <td> <p>Steuert, wann die Änderungen, die Sie an der Projekt-Timeline vornehmen, im Projekt oder in den übergeordneten Aufgaben gespeichert werden. Beispielsweise können Sie mit den folgenden Änderungen am Projekt-Trigger die Timeline des Projekts aktualisieren: 
       <ul> 
       <li>Datum der Aufgaben aktualisieren</li> 
       <li>Ändern von Vorgängerbeziehungen von Aufgaben</li> 
       <li><p>Ändern Sie die Beziehungen zwischen über- und untergeordneten Elementen, fügen Sie Zuweisungen hinzu oder entfernen Sie sie, und ändern Sie darüber hinaus die Aufgabenbegrenzung oder den Dauertyp.</p><p>Wenn die Aufgaben aktualisiert werden, werden ihre übergeordneten Objekte (übergeordnete Aufgaben oder das Projekt) zu dem durch den Aktualisierungstyp angegebenen Zeitpunkt aktualisiert. </p><p>Wenn die übergeordneten Objekte nicht unmittelbar nach der Änderung aktualisiert werden, wenn Sie "Automatisch und bei Änderung"oder "Nur ändern"auswählen, aktualisieren Sie die Seite.</p><p>Wählen Sie aus den folgenden Optionen aus: </p><p>- <strong>Automatisch und Bei Änderung</strong> (Standardeinstellung): Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem das Projekt abhängig ist (Bei Änderung). Die Projekt-Timeline wird auch jede Nacht aktualisiert (automatisch).</p><p>Dies ist die empfohlene Einstellung für dieses Feld, da dadurch sichergestellt wird, dass das Projekt stets auf dem neuesten Stand ist.</p><p>Wenn Sie eine Aktion für eine Aufgabe oder ein Projekt ausführen, für die eine Timeline-Neuberechnung Trigger wird, werden alle verfügbaren Daten sofort angezeigt, sodass Sie mit der Arbeit fortfahren können. Bei Projekten mit mehr als 100 Aufgaben werden Daten, die eine längere Neuberechnung erfordern, kurz als Fragezeichen angezeigt (zwischen 1 und 5 Sekunden oder bis zu einer Minute bei großen Projekten). Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.</p><p>- <strong>Nur ändern</strong>: Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem das Projekt abhängig ist. Sie können diese Option auswählen, wenn Änderungen selten im Projekt oder in anderen Projekten auftreten, von denen die Timeline abhängig ist.</p><p>- <strong>Nur Automatisch</strong>: Die Projekt-Timeline wird jede Nacht aktualisiert. Die Timeline wird nicht unmittelbar nach den Änderungen aktualisiert.</p><p>Sie können diese Option auswählen, wenn täglich im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, viele Änderungen vorgenommen werden. Beachten Sie jedoch, dass Sie diese Einstellung ausgewählt haben, da das Projekt nicht gleichzeitig mit den Änderungen aktualisiert wird.</p><p>- <strong>Nur manuell</strong>: Die Projekt-Timeline wird nur aktualisiert, wenn Sie die Option zum Neuberechnen der Timeline auswählen. Weitere Informationen zum manuellen Neuberechnen der Projekt-Timeline finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Projekt-Timeline neu berechnen</a>. </p><p>Sie können diese Option auswählen, wenn Sie gleichzeitig viele Änderungen am Projekt vornehmen und möchten, dass die Timeline-Neuberechnung erfolgt, nachdem alle Änderungen vorgenommen wurden (und nicht nach jeder einzelnen Änderung).</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Zeitplan</strong> </td> 
       <td> <p>Wählen Sie einen Zeitplan für Ihr Projekt aus. Dieser Zeitplan sollte mit dem für die meisten Personen übereinstimmen, die an dem Projekt arbeiten. Sie müssen einen Zeitplan erstellen, bevor Sie ihn einem Projekt oder einem Benutzer zuweisen können. Wenn Sie keine benutzerdefinierten Zeitpläne in Ihrem System erstellt haben, wird der Standardzeitplan ausgewählt.</p> <p>Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Zeitlimit für Benutzer</strong> </td> 
       <td> <p>Bestimmt, ob durch die Abwesenheit des Primären Verantwortlichen einer Aufgabe die für das Projekt geplanten Aufgabendaten angepasst werden. </p><p>Ihr Workfront-Administrator<span> oder ein Gruppenadministrator</span> wählt die Standardeinstellung für diese Einstellung für Ihr System <span> oder Ihre Gruppe</span> aus. Weitere Informationen zum Festlegen der Projektnormen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projekteigenschaften konfigurieren</a>. </p><p>Wählen Sie eine der folgenden Optionen aus:<br> - <strong>Betrachten Sie die Zeitdauer der Aufgaben als Zeitlimit für die Aufgaben</strong>: Bei Auswahl dieser Option werden die geplanten Zeitpunkte der Aufgaben entsprechend der Zeitdauer des Primären Aufgabenempfängers angepasst, wenn während der Aufgabendauer eine Zeitüberschreitung auftritt. </p><p>Wenn beispielsweise eine Aufgabe mit der Begrenzung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen sein soll und der Primäre Verantwortliche den 2. Juni für die Zeitüberschreitung markiert hat, sind die geplanten Aufgabenzeiträume vom 1. bis 4. Juni, wenn diese Auswahl aktiviert ist. Je nach Aufgabenbegrenzung gibt es die folgenden Szenarien: </p> 
       <ul> 
       <li>Bei Aufgabenbegrenzungen, die sich auf die Planung ab einem Startdatum beziehen (so bald wie möglich, früheste verfügbare Zeit, Start nicht früher als, Start nicht später als, Muss beginnen am), ändert sich das geplante Startdatum nicht, jedoch das geplante Abschlussdatum.</li> 
       <li>Bei Aufgabenbegrenzungen, die sich auf die Planung ab einem Fertigstellungsdatum beziehen (so spät wie möglich, aktuelle verfügbare Zeit, nicht früher beenden als, Später beenden muss beenden am), ändert sich das geplante Abschlussdatum nicht, jedoch das geplante Startdatum.</li> 
       <li>Bei Aufgaben mit einer Beschränkung von Feste Datumswerte ändern sich weder das geplante Start- noch das Abschlussdatum. </li> 
       </ul><p>Die Dauer der Aufgabe ändert sich bei Auswahl dieser Einstellung nicht. Je nach Aufgabenbegrenzung ändern sich nur die geplanten Datumswerte. Informationen zur Aufgabenbegrenzung finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Aufgabenbegrenzung - Übersicht</a>. </p><p>- <strong>Ignorieren der Benutzerzeit in Aufgabendauern</strong>: Bei Auswahl dieser Option bleiben die geplanten Termine der Aufgaben im Projekt wie ursprünglich geplant, auch wenn der Primäre Verantwortliche der Aufgabe während der Aufgabendauer eine Zeitüberschreitung hat. </p><p>Beachten Sie bei der Auswahl der Optionen für diese Einstellung Folgendes:</p> 
       <ul> 
       <li><p>Die Standardoption für diese Einstellung für ein neues Projekt ist dieselbe wie für die Projektanvoreinstellung auf Systemebene. </p><p>Weitere Informationen zu den Projektvoreinstellungen auf Systemebene finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektanvoreinstellungen konfigurieren</a>. </p></li> 
       <li>Wenn Sie eine Vorlage an ein vorhandenes Projekt anhängen, wird die Einstellung im Projekt so aktualisiert, dass sie mit der Vorlage übereinstimmt. </li> 
       <li><p>Workfront entscheidet, welche geplanten Aufgabendaten an den Aufgabenbegrenzungswert der Aufgabe angepasst werden sollen. Je nachdem, was das ist, kann entweder das geplante Start- oder das geplante Abschlussdatum betroffen sein oder beides könnte sogar gleich bleiben. Wenn eine Aufgabe beispielsweise die Begrenzung fester Datumswerte aufweist, werden die Daten nicht angepasst, wenn der Primäre Verantwortliche eine Zeitüberschreitung aufweist, selbst wenn <strong>Betrachten Sie die Zeitdauer der Aufgabe als "Zeitlimit für bestimmte Benutzer"</strong> ausgewählt ist. </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Ressourcenteilungsmodus</strong> </td> 
       <td> <p> <p>Wählen Sie aus den folgenden Optionen aus:</p> <p>- <strong>Manuell</strong>: Sie müssen Ihre Ressourcen manuell auf Ebene gestalten (dies ist die Standardeinstellung)</p> <p>- <strong>Automatisch</strong>: Workfront verwaltet Ihre Ressourcen.</p> <p>Weitere Informationen zur Ressourcenebene finden Sie unter <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level-Ressourcen im Gantt-Diagramm </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Risiko</strong> </td> 
       <td> <p> <p>Definieren Sie das Risiko Ihres Projekts. Das Risiko ist nur ein Indikator dafür, wie riskant ein Projekt sein kann. Sie können die Ausführung Ihrer Projekte je nach Risikograd priorisieren.</p> <p> <p>Wählen Sie aus den folgenden Risikostufen aus:</p> <p>- Sehr niedrig</p> <p>- Niedrig</p> <p>- MEDIUM</p> <p>- Hoch</p> <p>- Sehr hoch</p> <p>Die Risikostufen, die Sie hier angeben, können nicht angepasst werden.</p> <p>Diese hängen nicht mit den potenziellen Risiken zusammen, die während der Lebensdauer eines Projekts auftreten könnten und die Sie auf der Registerkarte Risiken des Projekts oder im Geschäftsfall aufzeichnen sollten. Informationen zu potenziellen Projektrisiken finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">Bearbeiten und Erstellen von Risikotypen</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Ressourcenpools</strong> </td> 
       <td> <p> <p>Geben Sie die Ressourcen-Pools an, die mit dem Projekt verknüpft sind. Resource Pools sind Sammlungen von Benutzern, die zur gleichen Zeit für die Fertigstellung eines Projekts benötigt werden und eine Projektbudgetierung im Resource Planer ermöglichen. Weitere Informationen zu Ressourcen-Pools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Überblick über Ressourcen-Pools </a>. </p> <p>Wenn Sie Projekte stapelweise bearbeiten, werden in diesem Feld nur die Ressourcen-Pools angezeigt, die für alle ausgewählten Projekte gelten. Wenn die ausgewählten Projekte keine gemeinsamen Ressourcen-Pools haben, ist dieses Feld leer. Die Ressourcen-Pools, die Sie hier angeben, überschreiben die einzelnen Ressourcen-Pools der Projekte.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>Erlauben Sie den Abrechnungssätzen auf Unternehmensebene, die Abrechnungsraten auf Projektebene außer Kraft zu setzen</strong></td> 
       <td>Wählen Sie diese Option aus, damit die Abrechnungsraten auf Unternehmensebene die historischen Auftragsrollenraten außer Kraft setzen können, wenn diese nicht als abgerechnet gekennzeichnet sind. Wenn Sie diese Option aktivieren, werden die historischen Rollenraten bei Aufträgen außer Kraft gesetzt, wenn sie als abgerechnet gekennzeichnet sind. <br>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">Außerkraftsetzen der Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Genehmigung des Zeitaufwands für dieses Projekt verlangen</strong></td> 
       <td> <p> Wählen Sie diese Option aus, damit der Projekteigentümer die im Projekt angemeldete Zeit genehmigen muss. Wenn Sie Rechnungsdatensätze verwenden und diese Option auswählen, werden nur die genehmigten Stunden im Projekt als verfügbare Abrechnungszeiten für die Rechnungsdatensätze angezeigt. Die Genehmigung der Zeit für das Projekt ist unabhängig von der Genehmigung von Timesheets. </p> <p>Weitere Informationen dazu, wie Sie Zeit für die Genehmigung eines Projekts benötigen, finden Sie unter <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Anfordern der Zeit für die Genehmigung eines Projekts</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Filtern der Stündentypen</strong> und </span> <strong>Stündentypen</strong></td> 
       <td> <p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
       <li> <p>Wählen Sie <strong>Nein</strong> aus, um alle projektspezifischen Stundentypen für das Projekt verfügbar zu machen. (Dies ist die Standardauswahl)</p> <p>Oder</p> </li> 
       <li>Wählen Sie "<strong>Ja</strong>", um nur eine Untergruppe der projektspezifischen Stundentypen für das Projekt verfügbar zu machen, und wählen Sie dann im Feld "<b>Stunden-Typen</b>"die Stundentypen aus, die Sie verfügbar machen möchten.</li> 
       <p><b>TIPP</b></p>
       <p>Das Feld <b>Stündungstypen</b> kann nicht bearbeitet werden, wenn Sie <b>Nein</b> auswählen.</p> 
       <p>Wenn Sie diese Option auswählen, stehen nur die ausgewählten Stundentypen zur Verfügung, die bei der Protokollierung von Stunden im Projekt (oder bei Aufgaben und Problemen im Projekt) ausgewählt werden. Sie müssen mindestens einen Stundentyp auswählen. Wenn Sie diese Option wählen und keine Stundentypen auswählen, werden alle Stundentypen für das Projekt zur Verfügung gestellt.</p> </ul>

   <p>Dieselbe Stundentyp muss auf der Ebene der einzelnen Benutzer ausgewählt werden, damit der Benutzer diese Stundenoptionen im Projekt sehen kann. Weitere Informationen zum Definieren von Stundentypen auf Benutzerebene finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Protokollzeit</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Erinnerungsbenachrichtigung</strong> </td> 
       <td> <p> <p>Wählen Sie die Erinnerungsbenachrichtigung aus, die mit dem Projekt verknüpft werden soll. Sie müssen Erinnerungsbenachrichtigungen für Projekte konfigurieren, damit dieses Feld während der Bearbeitung eines Projekts angezeigt wird. Weitere Informationen zum Konfigurieren von Erinnerungsbenachrichtigungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsbenachrichtigungen</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Genehmigungsprozess</strong></td> 
       <td> <p>Wählen Sie den Genehmigungsprozess aus, den Sie mit dem Projekt verknüpfen möchten. Ihr Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Projekten verknüpfen können. <span>Ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse kann auch gruppenspezifische Validierungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.</p> <p>Beachten Sie beim Hinzufügen von Validierungsprozessen Folgendes: </p> 
       <ul> 
       <li>In der Liste werden nur aktive Validierungsprozesse angezeigt. </li> 
       <li> <p>Systemweite und gruppenspezifische Validierungsprozesse werden in der Liste angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.</p> <p>Wenn sich die mit dem Projekt verknüpfte Gruppe ändert, wird der gruppenspezifische Validierungsprozess zu einem Validierungsprozess für die einmalige Verwendung. Weitere Informationen dazu, wie sich Änderungen an der Gruppe des Projekts oder am Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>Bei der Massenbearbeitung von Projekten gibt es die folgenden Szenarien:</p> 
       <ul> 
       <li> <p>Wenn Sie Projekte aus derselben Gruppe auswählen, werden in diesem Feld sowohl Validierungsprozesse auf Systemebene als auch auf Gruppenebene angezeigt.</p> </li> 
       <li> <p>Wenn Sie Projekte aus unterschiedlichen Gruppen auswählen, werden in diesem Feld nur Validierungsprozesse auf Systemebene angezeigt.</p> </li> 
       <li> <p>Wenn an einem Projekt ein Genehmigungsprozess für die einmalige Verwendung angehängt ist, wird es durch den von Ihnen ausgewählten Genehmigungsprozess auf Systemebene oder Gruppenebene ersetzt. </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Einstellungen für die Aufgabe {#task-settings}

Sie können die Standardeinstellungen definieren, die mit allen neuen Aufgaben verknüpft werden sollen, wenn Sie sie zum Projekt hinzufügen.

Informationen dazu, wie sich diese Einstellungen auf die Erstellung neuer Aufgaben auswirken, finden Sie im Abschnitt [Standardeinstellungen für Aufgaben beim Hinzufügen von Aufgaben zu einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) im Artikel [Übersicht über Aufgaben erstellen](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Aufgabeneinstellungen** .

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. Wählen Sie im Feld &quot;**Task Default Approval Process**&quot;den Aufgabengenehmigungsprozess aus, den Sie beim Hinzufügen zu dem Projekt mit allen neuen Aufgaben verknüpfen möchten.

   Ihr Workfront-Administrator (oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse) muss einen Validierungsprozess auf Systemebene oder Gruppenebene für eine Aufgabe erstellen, bevor Sie sie mit einem Projekt verknüpfen können. In der Liste werden nur aktive Validierungsprozesse angezeigt. Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). Informationen dazu, wie sich Änderungen an der Gruppe des Projekts oder am Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter [Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   Bei der Massenbearbeitung von Projekten gibt es die folgenden Szenarien:

   * Wenn Sie mehrere Projekte aus derselben Gruppe auswählen, werden in diesem Feld sowohl systemspezifische als auch gruppenspezifische Aufgabengenehmigungsprozesse angezeigt.
   * Wenn Sie mehrere Projekte aus verschiedenen Gruppen auswählen, werden in diesem Feld nur Aufgabengenehmigungsprozesse auf Systemebene angezeigt.

1. Wählen Sie im Feld **Task Default Custom Forms** das benutzerdefinierte Formular oder die Formulare aus, die beim Hinzufügen zum Projekt mit allen neuen Aufgaben verknüpft werden sollen. Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Sie können bis zu zehn benutzerdefinierte Formulare mit einer Aufgabe verknüpfen.
1. (Optional) Wählen Sie **Arbeitsaufwand verwenden, um die geplante Aufgabe automatisch zu berechnen**, wenn Sie die Verwaltung des Arbeitsaufwands durch Verwendung von Arbeitsaufwand anstelle von geplanten Stunden aktivieren möchten.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. (Bedingt und optional) Wenn Sie &quot;Arbeitsaufwand verwenden&quot;ausgewählt haben, um die geplante Aufgabe automatisch zu berechnen, klicken Sie auf das Dropdown-Menü für jede Aufwandsstufe und wählen Sie für jede Ebene einen Prozentsatz aus. Die folgenden Prozentwerte sind Standardwerte:

   | Größe | Prozentsatz |
   |---|---|
   | Klein | 25 % |
   | Mittel | 50 % |
   | Groß | 75 % |

   >[!TIP]
   >
   >Wenn der Projektaktualisierungstyp auf Automatisch gesetzt ist und Sie diese Einstellung auswählen, werden die geplanten Stunden der Aufgaben entsprechend der Aufgabendauer und dem Prozentsatz des Arbeitsaufwands aktualisiert, wenn sie auf null gesetzt sind. Weitere Informationen zur Verwendung von &quot;Arbeitsaufwand&quot;zur Planung von Arbeitsaufwand für eine Aufgabe finden Sie unter [Arbeitsaufwand - Übersicht](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Problemeinstellungen {#issue-settings}

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Problemeinstellungen** .

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. (Optional) Deaktivieren Sie die Option **Zulassen, dass Benutzer Probleme inline hinzufügen**. Sie ist standardmäßig ausgewählt.

   Wenn Sie diese Option deaktivieren, können Benutzer keine Probleme inline zum Projekt oder den Aufgaben im Abschnitt Probleme hinzufügen.

   >[!TIP]
   >
   >Deaktivieren Sie diese Option, wenn Sie Benutzer dazu zwingen möchten, die Felder für neue Probleme oder die benutzerdefinierten Formulare, die neuen Problemen zugeordnet sind, auszufüllen. Wenn Benutzer Probleme inline eingeben können, können sie die Felder Neues Problem und benutzerdefinierte Formulare beim Erstellen von Problemen umgehen. Informationen zum Festlegen von Feldern und benutzerdefinierten Formularen für neue Probleme finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Wenn Sie diese Option deaktivieren, können Benutzer mit der Berechtigung, dem Projekt oder den Aufgaben Probleme hinzuzufügen, dies auf folgende Weise tun:

   * Klicken Sie oben in der Liste der Probleme im Abschnitt Probleme des Projekts oder der Aufgaben auf Neues Problem .
   * Wenn das Projekt als Anforderungswarteschlange konfiguriert ist, kann es eine neue Anforderung im Bereich Anforderungen eingeben.

   >[!NOTE]
   >
   >Wenn Projekte stapelweise bearbeitet werden, ist diese Einstellung aktiviert, wenn sie für mindestens ein Projekt aktiviert ist, und sie ist deaktiviert, wenn sie für alle ausgewählten Projekte deaktiviert ist.

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. (Optional) Fahren Sie je nach den zu ändernden Informationen mit der Bearbeitung der folgenden Abschnitte fort.

   Oder

   Klicken Sie auf **Speichern**.

### Zugriff {#access}

1. Beginnen Sie mit der Bearbeitung Ihres Projekts wie oben beschrieben.
1. Klicken Sie im linken Bereich auf **Zugriff** .

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. Geben Sie die folgenden **Zugriffsinformationen** für das Projekt an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Wenn jemand einer Aufgabe zugewiesen ist</strong></td> 
      <td><p>Wählen Sie unter "<strong>Anzeigen</strong>", "<strong>Contribute", "</strong>"oder "<strong>Verwalten</strong>" den Zugriff auf eine Aufgabe aus. Der einer Aufgabe zugewiesene Benutzer erhält automatisch diesen Zugriff auf die Aufgabe.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Gewähren Sie außerdem Zugriff auf das Projekt</strong></td> 
      <td><p>Wählen Sie aus dem Zugriff auf das Projekt <strong>Ansicht</strong>, <strong>Contribute</strong> oder <strong>Verwalten</strong> aus. Der einer Aufgabe zugewiesene Benutzer erhält automatisch auch diesen Zugriff auf das Projekt.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Wenn jemand einem Problem zugewiesen ist</strong></td> 
      <td><p>Wählen Sie unter "<strong>Anzeigen</strong>", "<strong>Contribute", "</strong>"oder "<strong>Verwalten</strong>" den Zugriff auf ein Problem aus. Dem einem Problem zugewiesenen Benutzer wird automatisch dieser Zugriff auf das Problem gewährt. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Ein Problem freigeben </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Gewähren Sie außerdem Zugriff auf das Projekt</strong></td> 
      <td><p>Wählen Sie aus dem Zugriff auf das Projekt <strong>Ansicht</strong>, <strong>Contribute</strong> oder <strong>Verwalten</strong> aus. Der einem Problem zugewiesene Benutzer erhält automatisch auch diesen Zugriff auf das Projekt.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Wenn ein Benutzer eine Anforderung sendet: Gewähren Sie ihm Zugriff</strong></td> 
      <td><p>Wählen Sie unter "<strong>Anzeigen</strong>", "<strong>Contribute</strong>"oder "<strong>Verwalten</strong>"den Zugriff auf die Anforderung aus. Wenn das Projekt auch eine Anforderungswarteschlange ist und ein Benutzer eine Anforderung an das Projekt sendet, erhält er diesen Zugriff auf die von ihm gesendete Anfrage. Informationen zum Einrichten eines Projekts als Anforderungswarteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Benutzer aus demselben Unternehmen erben dieselben Berechtigungen für alle Anforderungen.</strong></td> 
      <td><p>Wählen Sie dieses Feld aus, wenn Sie möchten, dass Personen desselben Unternehmens denselben Zugriff auf alle Anforderungen des Projekts haben, unabhängig davon, ob sie sie gesendet haben oder nicht.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Wenn jemand Zugriff auf dieses Projekt erhält: Geben Sie den Standardzugriff für an...</strong></td> 
      <td><p>Wählen Sie die Zugriffsoptionen aus, die Benutzer für das Projekt haben sollen, wenn das Projekt für sie freigegeben ist. Wählen Sie die spezifischen Optionen für ihren Zugriff aus, wenn sie beim Freigeben des Projekts für sie als <strong>Betrachter</strong>, <strong>Mitwirkende</strong> oder <strong>Manager</strong> gekennzeichnet sind. </p><p>Der Zugriff auf <strong>Löschen</strong> auf der Berechtigungsebene <strong>Verwalten</strong> bestimmt, ob Benutzer das Projekt selbst löschen können. Benutzer mit Zugriff auf das Projekt <strong>Verwalten</strong> können Aufgaben und Probleme innerhalb des Projekts löschen, unabhängig davon, ob diese Option aktiviert ist oder ob sie über <strong>Verwalten</strong> -Berechtigungen für die Aufgaben und Probleme verfügen. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

### Verknüpfte Ordner

Die Funktion für verknüpfte Ordner erstellt automatisch Ordner in Adobe Experience Manager Assets und verbindet diese Ordner mit Workfront.

Dieser Abschnitt wird nur angezeigt, wenn die folgenden Punkte zutreffen:

* Ihr Unternehmen wurde in die Adobe Admin Console migriert
* Ihr Unternehmen hat die Integration mit Adobe Experience Manager aktiviert und konfiguriert.
* Die Vorlage, mit der dieses Projekt erstellt wird, hat verknüpfte Ordner aktiviert und konfiguriert.

Anweisungen zum Bearbeiten von verknüpften Ordnern finden Sie unter [Workflow-Werte in einem Projekt bearbeiten](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#edit-workflow-values-in-a-project) im Artikel Verwenden von Workflows in der Experience Manager Assets-Integration.

>[!NOTE]
>
>Da verknüpfte Ordner beim Erstellen des Projekts erstellt werden, ist die Bearbeitung des Workflows für verknüpfte Ordner in einem vorhandenen Projekt nicht wirksam. Die Bearbeitung dieser Werte beim Erstellen eines Projekts funktioniert erwartungsgemäß.

## Bearbeiten eines Projekts in der Projektheader (begrenzt)

Sie können eine begrenzte Anzahl von Informationen in der Projektheader bearbeiten.

Ihr System- oder Gruppenadministrator kann die Felder anpassen, die in der Projektheader angezeigt werden.

![](assets/project-header-350x18.png)

Die folgenden Felder sind standardmäßig in der Projektheader enthalten.

* Projektname
* Prozent abgeschlossen
* Projektbesitzer
* Geplantes Abschlussdatum und -zeit

  >[!NOTE]
  >
  >Sie können dieses Feld nur bearbeiten, wenn das Projekt ab dem Abschlussdatum geplant ist. Wenn das Projekt ab dem Startdatum geplant ist, berechnet Workfront das geplante Abschlussdatum und die geplante Abschlusszeit basierend auf der Dauer der Aufgaben.

* Bedingung

  >[!NOTE]
  >
  >Sie können dieses Feld nur bearbeiten, wenn der Bedingungstyp des Projekts &quot;Manuell&quot;ist. Wenn der Bedingungstyp auf Fortschrittsstatus gesetzt ist, berechnet Workfront die Bedingung basierend auf dem Fortschritt der Aufgaben. Weitere Informationen finden Sie unter [Überblick über Projektbedingungen und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* Status
* Entscheidungsfindung bei Genehmigungseinstellungen, wenn Sie in einem aktuellen Genehmigungsprozess als Genehmiger festgelegt sind

## Stapelweises Bearbeiten von Projekten

Sie können Projekte stapelweise bearbeiten und Informationen für alle ausgewählten Projekte gleichzeitig aktualisieren.

Beachten Sie beim Massenbearbeitung von Projekten Folgendes:

* Die Informationen, die Sie für alle ausgewählten Projekte ändern, überschreiben die vorhandenen Informationen zu einzelnen Projekten, mit Ausnahme des Felds Ressourcen-Manager .

  Durch Hinzufügen eines neuen Ressourcen-Managers bei der Massenbearbeitung von Projekten wird dieser Manager zu allen ausgewählten Projekten hinzugefügt. Wenn andere Ressourcen-Manager mit den ausgewählten Projekten verknüpft sind, bleiben sie zusätzlich zu dem über die Massenbearbeitung hinzugefügten in den Projekten.

* Wenn Sie Projekte auswählen, die für dasselbe Feld unterschiedliche Werte aufweisen, wird im Feld &quot;Projekte bearbeiten&quot;die Anzeige &quot;Mehrere Werte&quot;angezeigt. Felder, bei denen es sich um Kontrollkästchen, Optionsfelder und Umschalter handelt, weisen neben ihnen die Anzeige &quot;Mehrere Werte&quot;auf.

  ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* Wenn sich die ausgewählten Optionen in mindestens einem der ausgewählten Projekte unterscheiden, werden neben der Anzeige &quot;Mehrere Werte&quot;Felder mit mehreren Optionen auf eine der folgenden Arten angezeigt:

   * Kontrollkästchen-Felder haben eine Zeile anstelle eines Kontrollkästchens für die Option, die für einige, aber nicht für alle ausgewählten Projekte aktiviert ist.

     ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * Felder vom Typ Umschalten werden abgeblendet angezeigt, wobei der Umschalter in der Mitte für die Option aktiviert ist, der für einige, aber nicht für alle ausgewählten Projekte aktiviert ist.

  ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * Felder vom Typ Radiobutton, für die einige Optionen, aber nicht alle ausgewählt sind, zeigen alle Optionsfelder als leer an.

     ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)

* Wenn Sie eine Option in einem Feld mit mehreren Optionen aktualisieren (z. B. ein Feld, das als Satz von Umschaltern oder Kontrollkästchen angezeigt wird), müssen alle anderen Optionen zwischen den ausgewählten Projekten übereinstimmen.

  >[!IMPORTANT]
  >
  >Sie können beispielsweise ein Kontrollkästchen mit drei Kontrollkästchen (Option 1, Option 2 und Option 3) und Option 1 ist für alle Projekte deaktiviert und Option 2 und 3 für einige und deaktiviert für andere Projekte, die Sie ausgewählt haben. Wenn Sie Option 1 für alle Projekte aktivieren möchten, müssen Sie auch Option 2 und 3 für alle ausgewählten Projekte zuordnen, bevor Sie Ihre Änderungen speichern können. Sie müssen sie also entweder auswählen oder die Auswahl aufheben, damit sie für alle ausgewählten Projekte übereinstimmen. Wenn Sie keine der Optionen ändern, können Sie das Feld unverändert speichern und die Projekte behalten ihre aktuelle Auswahl für alle Optionen bei.

* Wenn Sie mehrere Projekte auswählen, die zu verschiedenen Gruppen gehören, werden im Feld Status die Status auf Systemebene und nicht der Status auf Gruppenebene angezeigt.

So bearbeiten Sie mehrere Projekte:

{{step1-to-projects}}

1. Wählen Sie mehrere Projekte in der Liste aus.
1. Klicken Sie oben in der Liste auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) .
Das Dialogfeld **Projekte bearbeiten** wird geöffnet.

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layoutvorlage geändert hat, werden die Bereiche im linken Bereich des Felds &quot;Projekt bearbeiten&quot;oder die in diesen Bereichen aufgelisteten Felder möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klicken Sie auf **Überblick** , um allgemeine Informationen zu den ausgewählten Projekten zu bearbeiten.  Weitere Informationen zum Bearbeiten des Übersichtsbereichs finden Sie im Abschnitt [Überblick](#overview) in diesem Artikel.

   >[!TIP]
   >
   >Die von Ihnen bearbeiteten Felder werden mit einem hellvioletten Hintergrund angezeigt.

1. Klicken Sie auf **Benutzerdefinierter Forms** , um benutzerdefinierte Formulare zu bearbeiten, hinzuzufügen oder zu ersetzen, die mit den ausgewählten Projekten verknüpft sind.

   Die benutzerdefinierten Formulare, die an alle ausgewählten Projekte angehängt sind, werden im Unterabschnitt **Benutzerdefinierte Formulare im gemeinsamen** im Bereich **Benutzerdefinierter Forms** angezeigt.

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   Die Namen der Formulare, die für alle ausgewählten Projekte gelten, werden im linken Bereich des Felds Projekte bearbeiten angezeigt.

1. Beginnen Sie mit der Eingabe des Namens eines benutzerdefinierten Formulars in das Feld **Benutzerdefiniertes Formular hinzufügen** .


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   Die benutzerdefinierten Formulare, die bereits an die ausgewählten Projekte angehängt sind, werden im Unterabschnitt **Angehängte Formulare** im Feld **Benutzerdefiniertes Formular hinzufügen** angezeigt.

   Zusätzliche benutzerdefinierte Formulare, die mit Projekten verknüpft werden können, aber nicht an die ausgewählten Projekte angehängt sind, werden im Unterabschnitt **Forms zum Hinzufügen von** im Feld **Benutzerdefiniertes Formular hinzufügen** angezeigt.

1. Klicken Sie auf , um weitere benutzerdefinierte Formulare in den Unterabschnitten **Benutzerdefiniertes Formular hinzufügen** oder **Forms auszuwählen, um** hinzuzufügen, wenn sie in der Liste angezeigt werden.

   Wenn ein benutzerdefiniertes Formular bereits an einige der ausgewählten Projekte angehängt ist, wird neben dem Namen des Formulars angegeben, wie viele Projekte bereits über das Formular verfügen, wenn Sie ein Formular hinzufügen.

1. (Optional) Klicken Sie auf das Symbol &quot;**x**&quot;rechts neben dem Namen eines benutzerdefinierten Formulars und dann auf &quot;**Entfernen**&quot;, um es aus allen ausgewählten Projekten zu entfernen.

   >[!CAUTION]
   >
   >Wenn Sie benutzerdefinierte Formulare entfernen, gehen alle vorhandenen benutzerdefinierten Feldinformationen in den Formularen verloren. Dies kann nicht wiederhergestellt werden.

   Weitere Informationen zum Bearbeiten benutzerdefinierter Formulare finden Sie im Abschnitt [Benutzerdefinierter Forms](#custom-forms) in diesem Artikel.

1. Klicken Sie auf **Finanzen** , um die Finanzinformationen für alle ausgewählten Projekte zu bearbeiten.
Weitere Informationen zum Bearbeiten des Finanzbereichs finden Sie im Abschnitt [Finanzen](#finance) in diesem Artikel.
1. Klicken Sie auf **Projekteinstellungen** , um die Einstellungen für alle ausgewählten Projekte zu bearbeiten.
Weitere Informationen zum Bearbeiten des Bereichs Projekteinstellungen finden Sie im Abschnitt [Projekteinstellungen](#project-settings) in diesem Artikel.
1. Klicken Sie auf **Aufgabeneinstellungen** , um die Aufgabeneinstellungen für alle ausgewählten Projekte zu bearbeiten.
Weitere Informationen zum Bearbeiten des Bereichs &quot;Aufgabeneinstellungen&quot;finden Sie im Abschnitt [Aufgabeneinstellungen](#task-settings) in diesem Artikel.
1. Klicken Sie auf **Problemeinstellungen** , um die Problemeinstellungen für alle ausgewählten Projekte zu bearbeiten.
Weitere Informationen zum Bearbeiten des Bereichs &quot;Problemeinstellungen&quot;finden Sie im Abschnitt [Problemeinstellungen](#issue-settings) in diesem Artikel.
1. Klicken Sie auf **Zugriff** , um die Zugriffseinstellungen für alle ausgewählten Projekte zu bearbeiten.
Weitere Informationen zum Bearbeiten des Zugriffsbereichs finden Sie im Abschnitt [Zugriff](#access) in diesem Artikel.
1. (Optional) Wenn Sie eine der Informationen entfernen möchten, die Sie im Feld &quot;Projekte bearbeiten&quot;hinzugefügt haben, halten Sie den Mauszeiger über ein bearbeitetes Feld und klicken Sie dann oben rechts im Feld auf das Symbol **x** für die Löschung.

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. (Optional) Klicken Sie unten auf der Seite **Projekte bearbeiten** auf **Abbrechen** , um alle Änderungen an allen Projekten zu entfernen.
1. Klicken Sie auf **Speichern**.


<!-- Old information for how to bulk edit in classic/ before project bulk edit redesign: 

### Edit projects in bulk in the Production environment

To edit projects in bulk:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Projects**.  
1. Select several projects in the list.
1. Click **Edit**.

   The **Edit Projects** dialog box opens.

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. Specify the information on all selected projects in the following sections:

   * **Overview**

     For information, see the [Overview](#overview) section in this article.
   
   * **Finance**

     For information, see the [Finance](#finance) section in this article.
   
   * **Portfolio**

     For information, see the "Project association" section in the [Overview](#overview) section in this article.
   
   * **Settings**

     For information, see the [Project Settings](#project-settings) section in this article.
   
   * **Access**

     For information, see the [Access](#access) section in this article.
   
   * **Custom Forms**

     For information, continue with step 7 below.

     <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     

   * **Tasks**

     For information, see the [Task Settings](#task-settings) section in this article.
   
   * **Issues**

     For information, see the   [Issue Settings](#issue-settings) section in this article.
   
   * **Comment**

     For information, continue with step 9 below.

     <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     


1. (Optional) In the Settings area, select any of the following options:

   * **Recalculate Costs and Revenues**: Select this option to recalculate Costs and Revenues on all projects selected.
   * **Recalculate Timelines**: Select this option to recalculate the Timelines of all projects selected.
   * **Recalculate Scorecards**: Select this option to recalculate the Scorecard values for all projects selected.

   ![recalculate_costs__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. Click **Custom Forms** to edit the custom forms attached to all the projects selected.

   If the projects selected do not have any common custom forms, no forms are listed in this section.

   You can edit only the fields on the forms that are attached to all projects selected and which you have permissions to edit. 

1. (Optional) In the Custom Forms section, select the **Recalculate Custom Expressions** option to ensure that all Calculated Custom Fields that are on the Custom Forms attached to the projects selected are up to date.

   >[!IMPORTANT]
   >
   >We recommend not to select more than 500 projects at a time when you recalculate custom expressions.

1. (Optional) Click **Comment**, then select the Post an update to each project box and specify a comment that you want to display in the updates stream of the project in the available field and do one of the following:

   * Click the **People** icon ![](assets/people-icon-updates-classic.png) to tag a user who will be notified about your comment.
   * Click the **Lock** icon ![](assets/lock-icon-open-updates-classic.png) to restrict your comment only to people within your company.

   This comment is visible for everyone with View access to the project and with access to view Notes.

1. Click **Save Changes**.

   All changes you made are now visible on all the selected projects.

-->