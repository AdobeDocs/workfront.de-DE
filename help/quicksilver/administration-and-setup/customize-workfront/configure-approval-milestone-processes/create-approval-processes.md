---
title: Erstellen eines Genehmigungsprozesses für Arbeitselemente
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Sie können einen Validierungsprozess erstellen, den Benutzer an ein Arbeitselement (Projekt, Aufgabe, Problem, Vorlage, Vorlagenaufgabe), ein Dokument oder einen Testversand anhängen können. Durch einen Genehmigungsprozess wird sichergestellt, dass bestimmte Bevollmächtigte bestimmte Änderungen am Objekt überprüfen, bevor das Objekt im System fortfährt.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: d98bb6b6bb8ff3bff6f367f1376948d5104887e5
workflow-type: tm+mt
source-wordcount: '2202'
ht-degree: 1%

---

# Erstellen eines Genehmigungsprozesses für Arbeitselemente

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Sie können einen Validierungsprozess erstellen, den Benutzer an ein Arbeitselement (Projekt, Aufgabe, Problem, Vorlage, Vorlagenaufgabe), ein Dokument oder einen Testversand anhängen können. Durch einen Genehmigungsprozess wird sichergestellt, dass bestimmte Bevollmächtigte bestimmte Änderungen am Objekt überprüfen, bevor das Objekt im System fortfährt.

In diesem Artikel wird beschrieben, wie Sie globale Genehmigungsprozesse auf Systemebene oder Gruppenebene für Arbeitselemente (Projekt-, Aufgaben-, Problem-, Vorlagen- oder Vorlagenaufgaben) erstellen.

Informationen zu Genehmigungen, die mit Dokumenten oder Testsendungen verknüpft sind, finden Sie in den folgenden Artikeln:

* [Dokumentgenehmigungen anfordern](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Übersicht über den automatisierten Workflow](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Benutzer können auch einen einmaligen Genehmigungsprozess für ein Projekt, eine Aufgabe, ein Problem, eine Vorlage oder eine Vorlagenaufgabe erstellen, für die sie über Verwaltungsberechtigungen verfügen.
>
>In diesem Artikel wird der Begriff &quot;globaler Genehmigungsprozess&quot;verwendet, um von einem Genehmigungsprozess für die einmalige Verwendung zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Auf Gruppenebene ist ein globaler Genehmigungsprozess auf Arbeitselemente und Status beschränkt, die zur Gruppe gehören.
>
>Informationen zu Genehmigungsprozessen für die einmalige Verwendung finden Sie unter [Übersicht über den Genehmigungsprozess](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) und [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neuer Plan: Standard </p>
 <p>oder</p> 
<p>Aktueller Plan: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Wenn Sie Workfront-Administrator sind oder über Administratorzugriff auf Genehmigungsprozesse verfügen, können Sie einen Validierungsprozess auf Systemebene oder einen Validierungsprozess auf Gruppenebene für eine bestimmte Gruppe erstellen.</p> 
   <p>Als Gruppenadministrator können Sie Genehmigungsprozesse auf Gruppenebene für von Ihnen verwaltete Gruppen erstellen.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines globalen Genehmigungsprozesses auf Systemebene oder Gruppenebene für Arbeitselemente

{{step-1-to-setup}}

1. (Bedingt) Wenn Sie einen Validierungsprozess auf Systemebene erstellen, klicken Sie auf **Prozesse** > **Genehmigungen** im linken Bereich.

   Oder

   Wenn Sie einen Validierungsprozess auf Gruppenebene erstellen, klicken Sie auf **Gruppen** ![](assets/groups-icon.png), klicken Sie auf den Namen der Gruppe und dann auf **Genehmigungen**.

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. Wählen Sie entweder **Projektgenehmigungen**, **Aufgabenvalidierungen** oder **Emissionsgenehmigungen** Registerkarte.

1. Klicks **Neuer Genehmigungsprozess**.
1. Geben Sie die folgenden Informationen in das angezeigte Feld ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name des Genehmigungsprozesses</td> 
      <td><p>Geben Sie einen beschreibenden Namen für den Genehmigungsprozess ein. Benutzer sehen diesen Namen, wenn sie den Genehmigungsprozess auf ein Objekt anwenden, wie unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td><p>Geben Sie eine Beschreibung des Validierungsprozesses ein. Dies wird im <b>Genehmigungen</b> im Abschnitt <b>Einrichtung</b> neben dem Namen des Validierungsprozesses.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>Lassen Sie diese Option aktiviert, wenn Sie möchten, dass andere Benutzer den Genehmigungsprozess an von ihnen erstellte Projekte, Aufgaben und Probleme anhängen können. </p> <p>Diese Option ist standardmäßig aktiviert.</p> <p> Tipp: Die Kennzeichnung eines Validierungsprozesses als inaktiv ist nützlich, wenn Ihr Unternehmen ihn nicht mehr verwenden muss, Sie jedoch historische Informationen über seine Verwendung beibehalten möchten.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Dieser Genehmigungsprozess kann genutzt werden von </td> 
      <td> <p>Wenn der Validierungsprozess für Projekte, Aufgaben, Probleme und Vorlagen verfügbar sein soll, die nur zu einer bestimmten Gruppe gehören, geben Sie zunächst den Namen der Gruppe ein und wählen Sie dann den Namen aus, wenn er angezeigt wird:</p> 
       <ul> 
       <li>Wenn Sie Systemadministrator sind oder über Administratorzugriff auf Genehmigungsprozesse verfügen, können Sie beim Eingeben des Namens jede Gruppe im System sehen. <b>Alle Gruppen</b> ist standardmäßig ausgewählt. </li> 
       <li>Wenn Sie Gruppenadministrator ohne Administratorzugriff auf Genehmigungsprozesse sind, können Sie den Genehmigungsprozess jeder von Ihnen verwalteten Gruppe zuweisen, wenn Sie deren Namen eingeben. Die <b>Alle Gruppen</b> ist nicht verfügbar.</li> 
       </ul> 
       <p>Diese Option steht nicht für Genehmigungsprozesse zur einmaligen Verwendung zur Verfügung.</p> 
       <p><b>WARNUNG</b>: Wenn Sie Änderungen am gruppenspezifischen Validierungsprozess vornehmen, ändern sich möglicherweise die vorhandenen Genehmigungsprozesse, die bereits mit Arbeitselementen verknüpft sind. Weitere Informationen zu diesen Änderungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>.</p> 
       <p>Informationen zur Auflistung und Verwaltung der Validierungsprozesse Ihrer Gruppe auf der Seite Ihrer Gruppe finden Sie unter <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Validierungsprozesse auf Gruppenebene</a>. </p> 
       <p>Informationen zum administrativen Zugriff auf Genehmigungsprozesse finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren Sie einen Pfad für den Genehmigungsprozess mit den folgenden Optionen.

   In einem Pfad geben Sie an, was im Genehmigungsprozess passieren soll. Sie erstellen Bühnen in einem Pfad, um anzugeben, wer die Validierungsarbeit durchführen muss und in welcher Reihenfolge.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Genehmigungsprozess starten, wenn der Status festgelegt ist auf</p> </td> 
      <td> <p>Wählen Sie den Status aus, der den Genehmigungsprozess für Arbeitselemente Trigger. Wenn ein Arbeitselement auf diesen Status aktualisiert wird, beginnt der Genehmigungsprozess. </p> <p>Derselbe Status kann nicht für mehrere Genehmigungsprozess-Pfade ausgewählt werden.</p> <p>Die verfügbaren Status basieren auf dem, was unter der Option ausgewählt wurde. <b>Diese Genehmigung kann von</b> (Erläuterung in der obigen Tabelle):</p> 
       <ul> 
       <li> Wenn <b>Alle Gruppen</b> ausgewählt ist, sind nur systemweite Status verfügbar.
       <li> <p>Wenn eine bestimmte Gruppe ausgewählt ist, sind nur die für diese Gruppe verfügbaren Status verfügbar</p> </li> 
       </ul> <p>Informationen zur Funktionsweise des Genehmigungsprozesses mit Status finden Sie im Abschnitt . <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Wie Validierungsprozesse auf Status basieren</a> im Artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über den Genehmigungsprozess</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name der Phase</td> 
      <td>(Optional) Geben Sie einen Namen ein, der den ersten Schritt des Pfads beschreibt. Wenn Sie keinen Staging-Namen angeben, lautet der Standardname <b>Stufe 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigende Personen</td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens des Benutzers, Teams oder der Rolle, die Sie als Genehmiger für diese Phase festlegen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Sie können nur aktive Benutzer hinzufügen. <span>Vorgangsrollen</span>und Teams. </p>

   <p><b>TIPP</b>:</p>

   <p>Beachten Sie beim Hinzufügen eines Benutzers als Genehmiger den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.</p>
      <p>Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Benutzern Zugriff gewähren</a>. </p>

   <p><b>NOTE</b>:

   Wenn Benutzer, Teams oder Rollen als Genehmiger hinzugefügt werden, erhalten sie nicht automatisch Berechtigungen für das mit dieser Genehmigung verknüpfte Objekt. Sie erhalten Berechtigungen für das Objekt, wenn der Genehmigungsschritt ausgelöst wird. Andernfalls müssen die Objekte für sie freigegeben werden, bevor sie eine Genehmigungsentscheidung treffen können. </p> <p>Sie können eine Person auch als Genehmiger festlegen, indem Sie die Rolle der Person festlegen. Sie können beispielsweise einen Projekteigentümer, einen Projektsponsor, Portfolio-Inhaber, Programmeigentümer oder Manager als Genehmiger zuweisen. Diese Optionen werden automatisch angezeigt, wenn Sie mit der Eingabe beginnen.</p>

   <p><b>WICHTIG</b>:  
       <ul> 
       <li> <p>Wenn Sie dem Projektsponsor eine Genehmigung zuweisen und niemand als Sponsor eines Projekts benannt ist, wird die Genehmigung dem Projekteigentümer neu zugewiesen. Wenn niemand als Projekteigentümer bestimmt wurde, wird die Genehmigung dem Workfront-Administrator zugewiesen. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Wenn Sie einer Rolle eine Genehmigung zuweisen, wird die <b>Genehmiger muss nicht im Projektteam sein (für Genehmigungsprozesse, die eine Rolle enthalten)</b> deaktiviert ist, es gibt jedoch keine Rollen im Projektteam, die mit der Rolle bei der Genehmigung übereinstimmen. Die Genehmigung wird dem Projekteigentümer neu zugewiesen. Weitere Informationen zu den Validierungseinstellungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Globale Genehmigungseinstellungen konfigurieren</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Wenn Sie dem Projekteigentümer eine Genehmigung zuweisen und niemand als Projekteigentümer bestimmt wird, wird die Genehmigung dem Workfront-Hauptadministrator neu zugewiesen, wie im Abschnitt Kundeninformationen im Bereich Einrichtung angegeben. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Grundlegende Informationen für Ihr System konfigurieren</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Sie können diesen Vorgang wiederholen, um mehrere Genehmiger zur Bühne hinzuzufügen. Eine einzelne Phase kann eine Kombination aus Benutzern, Teams und Rollen als Genehmiger enthalten. Die Anzahl der Genehmiger, die Sie einer Bühne hinzufügen können, ist unbegrenzt.</p> <p><b>WICHTIG</b>:  <p>Wenn Sie Auftragsrollen als Genehmiger zuweisen, können alle Benutzer, die mit dieser Auftragsrolle verknüpft sind und sich ebenfalls im Projektteam befinden, eine Entscheidung über die Genehmigung treffen. </p> <p>Wenn Sie ein Team als Genehmiger zuweisen, kann jeder Benutzer in diesem Team eine Entscheidung über die Genehmigung treffen. </p> <p>Weitere Informationen zum Projektteam finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Übersicht über das Projektteam</a>. Weitere Informationen zur Genehmigung der Arbeit finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Validierung der Arbeit </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur eine Entscheidung ist erforderlich <br> <br>(Wird nur angezeigt, wenn Sie mehrere Genehmiger zur Bühne hinzufügen.) </td> 
      <td> <p>Wählen Sie diese Option aus, wenn einer der Genehmiger auf der Bühne das Arbeitselement in dieser Phase genehmigen oder ablehnen kann. Diese Aktion ermöglicht es dem Arbeitselement, die Phase zu verlassen. </p> <p>Wenn diese Option nicht ausgewählt ist, müssen alle identifizierten Genehmiger die Phase (in beliebiger Reihenfolge) genehmigen oder ablehnen, bevor das Element die Bühne verlässt. Wenn einer der Genehmiger die Phase ablehnt, wird der Prozess unterbrochen und neu gestartet, damit die erforderlichen Änderungen vorgenommen werden können. Anschließend können die Genehmiger die Phase erneut genehmigen oder ablehnen.</p> <p>Wenn ein Team als Genehmiger bestimmt wird, kann jedes Mitglied des Teams eine Phase gewähren oder ablehnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Phase hinzufügen</p> </td> 
      <td><p>(Optional) Fügen Sie dem Pfad eine weitere Phase hinzu, indem Sie die in den drei oben erläuterten Zeilen erläuterten Optionen verwenden. Sie können dem Pfad beliebig viele Bühnen hinzufügen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie aus, was passiert, wenn die Validierung abgelehnt wird</p> </td> 
      <td> <p>Wählen Sie die Aktion aus, die ausgeführt werden soll, wenn das Arbeitselement in einer beliebigen Phase des Pfads abgelehnt wird:</p> 
       <ul> 
       <li><b>Erstellen eines Problems</b>: (Nur für Projekt- und Aufgabengenehmigungsprozesse verfügbar) Es wird ein Problem im Projekt oder in der Aufgabe erstellt, in dem der Genehmigungsprozess ausgeführt wird. Die standardmäßig zugewiesene Ressource für die Aufgabe oder der Eigentümer des Projekts wird dem Problem zugewiesen. Standardmäßig lautet der Name des erstellten Problems <b>Genehmigung abgelehnt (&lt;project or="" task="" name=""&gt;)</b>. Dies ist ein Zurückweisungsproblem, das je nach Validierungsprozess, in dem die Zurückweisung erfolgte, unter die Aufgabe oder das Projekt eingegeben wurde.</li> 
       <li> <p><b>Status festlegen auf</b>: Wählen Sie eine der folgenden Optionen aus:</p> 
       <ul> 
       <li><b>Vorheriger Status</b>: Das abgelehnte Projekt, die zurückgewiesene Aufgabe oder das abgelehnte Problem kehrt zum Status zurück, bevor der Status aktiv ist.</li> 
       <li><p><b>Jeder andere Status in der Liste</b>: Das zurückgewiesene Objekt wechselt in den von Ihnen gewählten Status, z. B. "Auf Halten". Sie können einen der Standardstatus oder einen benutzerdefinierten Status auswählen, den Sie Ihrem Workfront-System hinzugefügt haben.</p>
       <p>Wenn Sie als Zurückweisungsstatus den einem Validierungsprozess zugeordneten Status auswählen, wechselt das zurückgewiesene Objekt in den ausgewählten Status und wird als "Genehmigung ausstehend"markiert.</p> 
       <p> Wenn Sie beispielsweise für den Zurückweisungsstatus die Option "Auf Halten"wählen und der Status "Auf Halten"mit einem Genehmigungsprozess verknüpft ist, wird das zurückgewiesene Objekt in den Status "Auf Halten - Genehmigung ausstehend"versetzt, was die Genehmigung erfordert.</p>

   </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf **Pfad hinzufügen** , um einen weiteren Pfad zum Genehmigungsprozess hinzuzufügen, der auf die Liste der Optionen im vorherigen Schritt verweist.

   Der neue Pfad muss mit einem anderen Status verknüpft sein. Der Pfad wird beim Aktualisieren des Elements Trigger, um diesen Status anzuzeigen. Es können nicht zwei Pfade für denselben Status vorhanden sein.

1. Klicken Sie auf **Speichern**.
1. Nachdem der Genehmigungsprozess erstellt wurde, fahren Sie mit einem der folgenden Schritte fort:

   * Verknüpfen Sie den Genehmigungsprozess mit bestimmten Projekten, Aufgaben oder Problemen im gesamten System, wie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Benachrichtigen Sie Benutzer außerhalb von Workfront darüber, dass der Genehmigungsprozess für sie verfügbar ist, um sie mit ihren Projekten, Aufgaben oder Problemen zu verknüpfen, wie hier beschrieben: [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Erstellen Sie einen weiteren Validierungsprozess, der ausgelöst wird, wenn dieser Validierungsprozess abgelehnt wird und das Element einen anderen Status erhält. Auf diese Weise können Sie Genehmigungsprozesse miteinander verknüpfen.

Informationen zum Bearbeiten eines Genehmigungsprozesses finden Sie unter [Validierungsprozess bearbeiten](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement

Wenn Sie einen Genehmigungsprozess für ein Arbeitselement (Projekt, Aufgabe oder Problem) erstellen möchten,

1. Erstellen Sie zuerst den Validierungsprozess.
1. Arbeitselement erstellen
1. Verknüpfen des Genehmigungsprozesses mit dem Arbeitselement

Anweisungen zum Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Jeder Workfront-Benutzer mit Verwaltungsberechtigungen für ein Projekt, eine Aufgabe oder ein Problem kann Genehmigungsprozesse für einzelne Verwendungszwecke erstellen, die nur für das Objekt verwendet werden, in dem sie erstellt wurden. Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Benutzer können globale Genehmigungsprozesse für ein einzelnes Arbeitselement ändern

Standardmäßig können Benutzer, die Berechtigungen für Projekte, Aufgaben und Probleme verwalten, Genehmigungsprozesse für einzelne Anwendungen erstellen. Informationen zum Hinzufügen von Genehmigungsprozessen für die einmalige Verwendung zu Projekten, Aufgaben und Problemen finden Sie im Abschnitt [Verknüpfen eines einmaligen Genehmigungsprozesses mit einer Projekt-, Aufgaben-, Problem-, Vorlagen- oder Vorlagenaufgabe](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) im Artikel [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Benutzer können auch Einstellungen für globale Genehmigungsprozesse ändern, die mit einem Arbeitselement verknüpft sind. Diese Änderungen betreffen nur das Projekt, die Aufgabe oder das Problem, das mit dem Genehmigungsprozess auf Systemebene verbunden ist. Weitere Informationen finden Sie im Abschnitt . [Globalen Genehmigungsprozess zur Verwendung für ein bestimmtes Objekt ändern](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) im Artikel [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).
