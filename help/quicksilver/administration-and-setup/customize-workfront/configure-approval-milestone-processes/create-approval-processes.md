---
title: Erstellen eines Genehmigungsprozesses für Arbeitselemente
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Sie können einen Genehmigungsprozess erstellen, den Benutzer an ein Arbeitselement (Projekt, Aufgabe, Problem, Vorlage oder Vorlagenaufgabe), ein Dokument oder einen Korrekturabzug anhängen können. Ein Genehmigungsprozess stellt sicher, dass designierte Beauftragte für das Objekt bestimmte Änderungen überprüfen, bevor das Objekt im System fortschreitet.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2193'
ht-degree: 1%

---

# Einen Genehmigungsprozess für Arbeitselemente erstellen

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Sie können einen Genehmigungsprozess erstellen, den Benutzer an ein Arbeitselement (Projekt, Aufgabe, Problem, Vorlage oder Vorlagenaufgabe), ein Dokument oder einen Korrekturabzug anhängen können. Ein Genehmigungsprozess stellt sicher, dass designierte Beauftragte für das Objekt bestimmte Änderungen überprüfen, bevor das Objekt im System fortschreitet.

In diesem Artikel wird beschrieben, wie Sie globale Genehmigungsprozesse auf Systemebene oder Gruppenebene für Arbeitselemente (Projekt, Aufgabe, Problem, Vorlage oder Vorlagenaufgabe) erstellen.

Informationen zu Genehmigungen, die mit Dokumenten oder Korrekturabzügen verbunden sind, finden Sie in den folgenden Artikeln:

* [Dokumentgenehmigungen anfordern](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Benutzer können auch einen einmaligen Genehmigungsprozess für ein Projekt, eine Aufgabe, ein Problem, eine Vorlage oder eine Vorlagenaufgabe erstellen, für die sie über Verwaltungsberechtigungen verfügen.
>
>In diesem Artikel wird der Begriff „globaler Genehmigungsprozess“ verwendet, um von Genehmigungsprozessen für den einmaligen Gebrauch zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Auf Gruppenebene ist ein globaler Genehmigungsprozess auf Arbeitselemente und Status beschränkt, die zu der Gruppe gehören.
>
>Informationen zu einmaligen Genehmigungsprozessen finden Sie unter [Übersicht über Genehmigungsprozesse](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) und [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>Genehmigungsprozess auf Systemebene oder zur einmaligen Verwendung: Beliebig</p>
   <p>Genehmigungsprozess auf Gruppenebene: Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Wenn Sie Systemadministrator sind oder administrativen Zugriff auf Genehmigungsprozesse haben, können Sie für eine bestimmte Gruppe einen Genehmigungsprozess auf Systemebene oder auf Gruppenebene erstellen.</p> 
   <p>Wenn Sie Gruppenadministrator sind, können Sie Genehmigungsprozesse auf Gruppenebene für von Ihnen verwaltete Gruppen erstellen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines globalen Genehmigungsprozesses auf Systemebene oder Gruppenebene für Arbeitselemente

{{step-1-to-setup}}

1. (Bedingt) Wenn Sie einen Genehmigungsprozess auf Systemebene erstellen, klicken Sie im linken Bereich auf **Prozesse** > **Genehmigungen**.

   Oder

   Wenn Sie einen Genehmigungsprozess auf Gruppenebene erstellen, klicken Sie auf **Gruppen** ![Symbol ](assets/groups-icon.png), klicken Sie auf den Namen der Gruppe und dann auf **Genehmigungen**.

   <!--hidden for the new tab redesign - August 2023: 
   ![Approvals area in setup](assets/approvals-area-in-setup-processes.png)
   -->

1. Wählen Sie entweder die **Projektgenehmigungen**, **Aufgabengenehmigungen** oder **Problemgenehmigungen** aus.

1. Klicken Sie **Neuer Genehmigungsprozess**.
1. Geben Sie die folgenden Informationen in dem angezeigten Feld ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name des Genehmigungsprozesses</td> 
      <td><p>Geben Sie einen beschreibenden Namen für den Genehmigungsprozess ein. Benutzer sehen diesen Namen, wenn sie den Genehmigungsprozess auf ein Objekt anwenden, wie beschrieben unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td><p>Geben Sie eine Beschreibung des Genehmigungsprozesses ein. Dies wird im Abschnitt <b>Genehmigungen</b> im Bereich <b>Setup</b> neben dem Namen des Genehmigungsprozesses angezeigt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>Lassen Sie diese Option aktiviert, wenn Sie möchten, dass andere Benutzer den Genehmigungsprozess an von ihnen erstellte Projekte, Aufgaben und Probleme anhängen können. </p> <p>Diese Option ist standardmäßig aktiviert.</p> <p> Tipp: Das Kennzeichnen eines Genehmigungsprozesses als inaktiv ist nützlich, wenn Ihr Unternehmen ihn nicht mehr verwenden muss, Sie aber historische Informationen zu seiner Verwendung beibehalten möchten.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Dieser Genehmigungsprozess kann genutzt werden von </td> 
      <td> <p>Wenn Sie möchten, dass der Genehmigungsprozess für Projekte, Aufgaben, Probleme und Vorlagen verfügbar ist, die nur zu einer bestimmten Gruppe gehören, geben Sie den Namen der Gruppe ein und wählen Sie dann den Namen aus, wenn er angezeigt wird:</p> 
       <ul> 
       <li>Wenn Sie Systemadministrator sind oder administrativen Zugriff auf Genehmigungsprozesse haben, können Sie bei der Eingabe des Namens eine beliebige Gruppe im System sehen. <b>Alle Gruppen</b> ist standardmäßig ausgewählt. </li> 
       <li>Wenn Sie ein Gruppenadministrator ohne administrativen Zugriff auf Genehmigungsprozesse sind, können Sie den Genehmigungsprozess jeder Gruppe zuweisen, die Sie verwalten, wenn Sie ihren Namen eingeben. Die <b>Alle Gruppen</b>-Option ist nicht verfügbar.</li> 
       </ul> 
       <p>Diese Option ist nicht für Genehmigungsprozesse zur einmaligen Verwendung verfügbar.</p> 
       <p><b>WARNUNG</b>: Wenn Sie Änderungen an dem gruppenspezifischen Genehmigungsprozess vornehmen, können sich die vorhandenen Genehmigungsprozesse ändern, die bereits Arbeitselementen zugeordnet wurden. Weitere Informationen zu diesen Änderungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>.</p> 
       <p>Informationen zum Auflisten und Verwalten der Genehmigungsprozesse Ihrer Gruppe auf der Seite Ihrer Gruppe finden Sie unter <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Genehmigungsprozesse auf Gruppenebene</a>. </p> 
       <p>Informationen zum administrativen Zugriff auf Genehmigungsprozesse finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren Sie einen Pfad für den Genehmigungsprozess mithilfe der folgenden Optionen.

   Unter einem Pfad geben Sie an, was im Genehmigungsprozess passieren soll. Sie erstellen Phasen in einem Pfad, um anzugeben, wer die Genehmigungsarbeit in welcher Reihenfolge ausführen muss.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Genehmigungsprozess starten, wenn der Status festgelegt ist auf</p> </td> 
      <td> <p>Wählen Sie den Status aus, der den Genehmigungsprozess für Arbeitselemente zum Trigger bringen soll. Wenn jemand ein Arbeitselement auf diesen Status aktualisiert, beginnt der Genehmigungsprozess. </p> <p>Derselbe Status kann nicht für mehrere Genehmigungsprozesspfade ausgewählt werden.</p> <p>Die verfügbaren Status basieren auf dem, was unter der Option <b>Diese Genehmigung kann verwendet werden von</b> (in der obigen Tabelle erläutert) ausgewählt wurde:</p> 
       <ul> 
       <li> Wenn <b>Alle Gruppen</b> ausgewählt ist, sind nur systemweite Status verfügbar
       <li> <p>Wenn eine bestimmte Gruppe ausgewählt ist, sind nur die für diese Gruppe verfügbaren Status verfügbar</p> </li> 
       </ul> <p>Informationen zur Funktionsweise von Genehmigungsprozessen mit Status finden Sie im Abschnitt <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Wie Genehmigungsprozesse auf Status </a>) im Artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über Genehmigungsprozesse</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name der Phase</td> 
      <td>(Optional) Geben Sie einen Namen ein, der den ersten Schritt des Pfads beschreibt. Wenn Sie keinen Namen für das Stadium angeben, lautet der Standardname (<b> 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigende Personen</td> 
      <td> <p>Geben Sie den Namen des Benutzers, Teams oder Aufgabengebiets ein, den Sie als Genehmiger für dieses Stadium angeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Sie können nur aktive Benutzer, <span>Aufgabengebiete</span> und Teams hinzufügen. </p>

   <p><b>TIPP</b>:</p>

   <p>Beachten Sie beim Hinzufügen eines Benutzers als Genehmiger den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.</p>
      <p>Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Gewähren des Benutzerzugriffs</a>. </p>

   <p><b>HINWEIS</b>:

   Durch das Hinzufügen eines Benutzers, Teams oder einer Rolle als genehmigende Person werden diesem Benutzer bzw. dieser Person nicht automatisch Berechtigungen für das Objekt erteilt, das mit dieser Genehmigung verknüpft ist. Sie erhalten Berechtigungen für das Objekt, wenn der Genehmigungsschritt ausgelöst wird. Andernfalls müssen die Objekte für sie freigegeben werden, bevor sie eine Genehmigungsentscheidung treffen können. </p> <p>Sie können eine Person auch als genehmigende Person festlegen, indem Sie die Rolle der Person angeben. Beispielsweise können Sie einen Projektbesitzer, Projektsponsor, Portfolio-Inhaber, Programm-Inhaber oder Manager als genehmigende Person zuweisen. Diese Optionen werden automatisch angezeigt, wenn Sie mit der Eingabe beginnen.</p>

   <p><b>WICHTIG</b>:  
       <ul> 
       <li> <p>Wenn Sie dem Projektsponsor eine Genehmigung zuweisen und niemand als Sponsor eines Projekts angegeben ist, wird die Genehmigung dem Projektbesitzer erneut zugewiesen. Wenn niemand als Eigentümer des Projekts festgelegt ist, wird die Genehmigung dem Workfront-Administrator zugewiesen. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Wenn Sie eine Genehmigung einer Funktion zuweisen und die <b>Genehmigende Person, die nicht Mitglied des Projektteams sein muss (für Genehmigungsprozesse, die eine Funktion beinhalten)</b> deaktiviert ist, aber es keine Funktionen im Projektteam gibt, die mit der Funktion in der Genehmigung übereinstimmen, wird die Genehmigung dem Projektbesitzer neu zugewiesen. Weitere Informationen zu den Genehmigungseinstellungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurieren globaler Genehmigungseinstellungen</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Wenn Sie dem Projektbesitzer eine Genehmigung zuweisen und niemand als Eigentümer eines Projekts bestimmt wird, wird die Genehmigung dem Workfront-Hauptadministrator neu zugewiesen, wie im Abschnitt „Kundeninformationen“ im Bereich „Setup“ angegeben. Weitere Informationen finden Sie <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Konfigurieren der grundlegenden Informationen für Ihr System</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Sie können diesen Vorgang wiederholen, um mehrere genehmigende Personen zur Phase hinzuzufügen. Ein einzelner Schritt kann eine Kombination aus Benutzern, Teams und Aufgabengebieten als genehmigende Personen enthalten. Die Anzahl der genehmigenden Personen, die einem Schritt hinzugefügt werden können, ist unbegrenzt.</p> <p><b>WICHTIG</b>:  <p>Wenn Sie Aufgabengebiete als genehmigende Personen zuweisen, können alle mit diesem Aufgabengebiet verbundenen Benutzer, die auch im Projektteam sind, eine Entscheidung über die Genehmigung treffen. </p> <p>Wenn Sie ein Team als genehmigende Person zuweisen, kann jeder Benutzer in diesem Team eine Entscheidung über die Genehmigung treffen. </p> <p>Weitere Informationen über das Projektteam finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteam - Übersicht</a>. Weitere Informationen zur Genehmigung von Arbeiten finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Genehmigen von Arbeiten </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur eine Entscheidung ist <br> <br> erforderlich (Wird nur angezeigt, wenn Sie mehrere genehmigende Personen zum Schritt hinzufügen) </td> 
      <td> <p>Wählen Sie diese Option aus, wenn eine der genehmigenden Personen in der Phase das Arbeitselement in dieser Phase genehmigen oder ablehnen kann. Diese Aktion ermöglicht es dem Arbeitselement, die Phase zu verlassen. </p> <p>Wenn diese Option nicht ausgewählt ist, müssen alle identifizierten genehmigenden Personen die Phase (in beliebiger Reihenfolge) genehmigen oder ablehnen, bevor das Element die Phase verlässt. Wenn eine der genehmigenden Personen das Stadium ablehnt, wird der Prozess unterbrochen und von vorne gestartet, damit die erforderlichen Änderungen vorgenommen werden können. Die genehmigenden Personen können die Phase dann erneut genehmigen oder ablehnen.</p> <p>Wenn ein Team als genehmigende Person benannt wird, kann jedes Teammitglied einen Schritt gewähren oder ablehnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Phase hinzufügen</p> </td> 
      <td><p>(Optional) Fügen Sie dem Pfad einen weiteren Schritt hinzu, indem Sie die Optionen verwenden, die in den drei obigen Zeilen erläutert werden. Sie können dem Pfad so viele Phasen hinzufügen, wie Sie benötigen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Auswählen, was passiert, wenn die Genehmigung abgelehnt wird</p> </td> 
      <td> <p>Wählen Sie die Aktion aus, die Sie ausführen möchten, wenn das Arbeitselement in einem beliebigen Schritt des Pfads abgelehnt wird:</p> 
       <ul> 
       <li><b>Problem erstellen</b>: (Nur für Projekt- und Aufgabengenehmigungsprozesse verfügbar) Ein Problem wird in dem Projekt oder der Aufgabe erstellt, in dem/der der Genehmigungsprozess ausgeführt wird. Die der Aufgabe standardmäßig zugewiesene Ressource oder der Projektbesitzer wird dem Problem zugewiesen. Standardmäßig lautet der Name des erstellten Problems <b>Genehmigung abgelehnt (&lt;Projekt- oder Aufgabenname&gt;)</b>. Hierbei handelt es sich um ein Ablehnungsproblem, das je nach Genehmigungsprozess, in dem die Ablehnung stattfand, unter der Aufgabe oder dem Projekt eingegeben wird.</li> 
       <li> <p><b>Status festlegen auf</b>: Wählen Sie eine der folgenden Optionen:</p> 
       <ul> 
       <li><b>Vorheriger Status</b>: Das abgelehnte Projekt, die abgelehnte Aufgabe oder das abgelehnte Problem wird auf den Status vor dem Status zurückgesetzt, der den Genehmigungsprozess aktiviert.</li> 
       <li><p><b>Beliebiger anderer Status in der Liste</b>: Das abgelehnte Objekt wechselt in den ausgewählten Status, z. B. „Zurückgestellt“. Sie können einen der Standardstatus oder einen benutzerdefinierten Status auswählen, den Sie Ihrem Workfront-System hinzugefügt haben.</p>
       <p>Wenn Sie einen mit einem Genehmigungsprozess verknüpften Status als Ablehnungsstatus auswählen, wechselt das abgelehnte Objekt in den ausgewählten Status und erhält die Kennzeichnung „Genehmigung ausstehend“.</p> 
       <p> Wenn Sie beispielsweise für den Ablehnungsstatus Halten auswählen und der Halten -Status mit einem Genehmigungsprozess verknüpft ist, wird das abgelehnte Objekt in den Status „Wird gehalten - Genehmigung ausstehend“ versetzt, was eine Genehmigung erfordert.</p>

   </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie **Pfad hinzufügen**, um einen weiteren Pfad zum Genehmigungsprozess hinzuzufügen, der auf die Liste der Optionen im vorherigen Schritt verweist.

   Der neue Pfad muss mit einem anderen Status verknüpft sein. Der Pfad gibt Trigger, wenn das Element aktualisiert wird, um diesen Status anzuzeigen. Sie können nicht zwei Pfade für denselben Status haben.

1. Klicken Sie auf **Speichern**.
1. Nachdem der Genehmigungsprozess erstellt wurde, fahren Sie mit einem der folgenden Schritte fort:

   * Ordnen Sie bestimmte Projekte, Aufgaben oder Probleme systemweit dem Genehmigungsprozess zu, wie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) beschrieben.
   * Benachrichtigen Sie Benutzende außerhalb von Workfront darüber, dass ihnen der Genehmigungsprozess zur Verfügung steht, um sie mit ihren Projekten, Aufgaben oder Problemen zu verknüpfen, wie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) beschrieben.
   * Erstellen Sie einen weiteren Genehmigungsprozess, der ausgelöst wird, wenn dieser Genehmigungsprozess abgelehnt wird und das Element einen anderen Status erhält. Auf diese Weise können Sie Genehmigungsprozesse miteinander verknüpfen.

Weitere Informationen zum Bearbeiten eines Genehmigungsprozesses finden Sie unter [Bearbeiten eines Genehmigungsprozesses](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Validierungsprozess einem Arbeitselement zuordnen

Wenn Sie einen Genehmigungsprozess für ein Arbeitselement (Projekt, Aufgabe oder Problem) erstellen möchten, müssen Sie

1. Erstellen Sie zuerst den Genehmigungsprozess
1. Erstellen des Arbeitselements
1. Verknüpfen Sie den Genehmigungsprozess mit dem Arbeitselement

Anweisungen zum Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Jeder Workfront-Benutzer mit Verwaltungsberechtigungen für ein Projekt, eine Aufgabe oder ein Problem kann Genehmigungsprozesse für den einmaligen Gebrauch erstellen, die nur für das Objekt verwendet werden, in dem sie erstellt wurden. Weitere Informationen finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeiten](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Benutzer können globale Genehmigungsprozesse für ein einzelnes Arbeitselement ändern

Standardmäßig können Benutzende mit Verwaltungsberechtigungen für Projekte, Aufgaben und Probleme Genehmigungsprozesse für den einmaligen Gebrauch erstellen. Informationen zum Hinzufügen von einmaligen Genehmigungsprozessen zu Projekten, Aufgaben und Problemen finden Sie im Abschnitt [Verknüpfen eines einmaligen Genehmigungsprozesses mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) im Artikel [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Benutzer können auch Einstellungen für globale Genehmigungsprozesse ändern, die mit einem Arbeitselement verknüpft sind. Diese Änderungen wirken sich nur auf das Projekt, die Aufgabe oder das Problem aus, das mit dem Genehmigungsprozess auf Systemebene verknüpft ist. Weitere Informationen finden Sie im Abschnitt [Ändern eines globalen Genehmigungsprozesses für die Verwendung für ein bestimmtes Objekt](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) im Artikel [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).
