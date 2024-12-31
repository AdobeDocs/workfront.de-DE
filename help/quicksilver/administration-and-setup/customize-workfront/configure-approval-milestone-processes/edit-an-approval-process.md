---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Genehmigungsprozess bearbeiten
description: Wenn Sie ein Adobe Workfront-Administrator sind oder administrativen Zugriff auf Genehmigungsprozesse haben, können Sie alle Genehmigungsprozesse im System anzeigen und bearbeiten.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1950'
ht-degree: 1%

---

# Genehmigungsprozess bearbeiten

Wenn Sie ein Adobe Workfront-Administrator sind oder administrativen Zugriff auf Genehmigungsprozesse haben, können Sie alle Genehmigungsprozesse im System anzeigen und bearbeiten.

Wenn Sie Gruppenadministrator sind, können Sie die Genehmigungsprozesse sehen und bearbeiten, die mit der von Ihnen verwalteten Gruppe oder den von Ihnen verwalteten Gruppen verknüpft sind.

Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Wenn Sie einen globalen Genehmigungsprozess bearbeiten, der bereits verwendet wird, wirken sich Ihre Änderungen auf alle Objekte im System aus, die bereits damit verknüpft sind.
>* Wenn Sie eine neue genehmigende Person zum aktuellen Schritt eines Genehmigungsprozesses hinzufügen, der bereits für ein Objekt gestartet wurde, wird der Prozess für dieses Objekt zurückgesetzt und die genehmigenden Personen müssen von vorne beginnen.
>
>  Wenn Sie jedoch die folgenden Änderungen an einem Genehmigungsprozess vornehmen, der bereits für ein Objekt gestartet wurde, wird dieser Prozess ohne Unterbrechung fortgesetzt:
>
>* Einen Schritt über das aktuelle Stadium hinaus hinzufügen
>* Hinzufügen einer zusätzlichen genehmigenden Person vor dem aktuellen Schritt

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf Genehmigungsprozesse, wenn Sie kein Systemadministrator sind</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Bearbeiten eines vorhandenen Genehmigungsprozesses

{{step-1-to-setup}}

1. (Bedingt) Wenn Sie einen Genehmigungsprozess auf Systemebene bearbeiten, klicken Sie im linken Bereich auf **Prozesse** > **Genehmigungen**.

   Oder

   Wenn Sie einen Genehmigungsprozess auf Gruppenebene bearbeiten, gehen Sie wie folgt vor:

   1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).
   1. Klicken Sie auf den Namen der Gruppe, für die Sie Gruppengenehmigungsprozesse auflisten oder verwalten möchten.
   1. Klicken Sie im linken Bedienfeld auf **Genehmigungen**. Möglicherweise müssen Sie zuerst auf **Mehr anzeigen** klicken.

1. Klicken Sie auf **Registerkarte**, **Aufgabengenehmigungen** oder **Problemgenehmigungen**, je nach dem Typ des Genehmigungsprozesses, den Sie bearbeiten möchten.

1. Wählen Sie den Genehmigungsprozess aus, den Sie bearbeiten möchten, und klicken **oben in** Liste auf „Bearbeiten“. Das Feld Genehmigungsprozess bearbeiten wird angezeigt.

   ![](assets/edit-approval-process-global-area-new.png)

1. Geben Sie die folgenden Informationen in dem angezeigten Feld ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name des Genehmigungsprozesses</td> 
      <td>Geben Sie einen beschreibenden Namen für den Genehmigungsprozess ein. Benutzer sehen diesen Namen, wenn sie den Genehmigungsprozess auf ein Objekt anwenden, wie beschrieben unter <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung des Genehmigungsprozesses ein. Dies wird im Abschnitt <b>Genehmigungen</b> im Bereich <b>Setup</b> neben dem Namen des Genehmigungsprozesses angezeigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>Lassen Sie diese Option aktiviert, wenn Sie möchten, dass andere Benutzer den Genehmigungsprozess an von ihnen erstellte Projekte, Aufgaben und Probleme anhängen können. </p> <p>Diese Option ist standardmäßig aktiviert.</p> <p>Tipp: Das Kennzeichnen eines Genehmigungsprozesses als inaktiv ist nützlich, wenn Ihr Unternehmen ihn nicht mehr verwenden muss, Sie aber historische Informationen zu seiner Verwendung beibehalten möchten.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Dieser Genehmigungsprozess kann genutzt werden von </td> 
      <td> <p>Wenn Sie möchten, dass der Genehmigungsprozess für Projekte, Aufgaben, Probleme und Vorlagen verfügbar ist, die nur zu einer bestimmten Gruppe gehören, geben Sie den Namen der Gruppe ein und wählen Sie dann den Namen aus, wenn er angezeigt wird:</p> 
       <ul> 
        <li>Wenn Sie Systemadministrator sind oder administrativen Zugriff auf Genehmigungsprozesse haben, können Sie bei der Eingabe des Namens eine beliebige Gruppe im System sehen. <b>Alle Gruppen</b> ist standardmäßig ausgewählt. </li> 
        <li>Wenn Sie ein Gruppenadministrator ohne administrativen Zugriff auf Genehmigungsprozesse sind, können Sie den Genehmigungsprozess jeder Gruppe zuweisen, die Sie verwalten, wenn Sie ihren Namen eingeben. Die <b>Alle Gruppen</b>-Option ist nicht verfügbar.</li> 
       </ul> <p>Diese Option ist nicht für Genehmigungsprozesse zur einmaligen Verwendung verfügbar.</p> <p><b>WARNUNG</b>: Wenn Sie Änderungen an dem gruppenspezifischen Genehmigungsprozess vornehmen, können sich die vorhandenen Genehmigungsprozesse ändern, die bereits Arbeitselementen zugeordnet wurden. Weitere Informationen zu diesen Änderungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>.</p> <p>Informationen zum Auflisten und Verwalten der Genehmigungsprozesse Ihrer Gruppe auf der Seite Ihrer Gruppe finden Sie unter <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Genehmigungsprozesse auf Gruppenebene</a>. </p> <p>Informationen zum administrativen Zugriff auf Genehmigungsprozesse finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> </td> 
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
      <li> Wenn <b>Alle Gruppen</b> ausgewählt ist, sind nur systemweit gesperrte Status verfügbar. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Wenn eine bestimmte Gruppe ausgewählt ist, sind nur die für diese Gruppe verfügbaren Status verfügbar</p> </li> 
      </ul> <p>Informationen zur Funktionsweise von Genehmigungsprozessen mit Status finden Sie im Abschnitt <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Wie Genehmigungsprozesse auf Status </a>) im Artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über Genehmigungsprozesse</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name der Phase</td> 
      <td>(Optional) Geben Sie einen Namen ein, der den ersten Schritt des Pfads beschreibt. Wenn Sie keinen Namen für das Stadium angeben, lautet der Standardname (<b> 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigende Personen</td> 
      <td> <p>Geben Sie den Namen des Benutzers, Teams oder Aufgabengebiets ein, den Sie als Genehmiger für dieses Stadium angeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird. Sie können nur aktive Benutzer, Aufgabengebiete und Teams hinzufügen. </p>

   <p><b>TIPP</b>:</p>

   <p>Beachten Sie beim Hinzufügen eines Benutzers als Genehmiger den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.</p>
      <p>Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Benutzern Zugriff gewähren</a></p>.

   <p><b>HINWEIS</b>:

   Durch das Hinzufügen eines Benutzers, Teams oder einer Rolle als genehmigende Person werden diesem Benutzer bzw. dieser Person nicht automatisch Berechtigungen für das Objekt erteilt, das mit dieser Genehmigung verknüpft ist. Sie erhalten Berechtigungen für das Objekt, wenn der Genehmigungsschritt ausgelöst wird. Andernfalls müssen die Objekte für sie freigegeben werden, bevor sie eine Genehmigungsentscheidung treffen können. </p>
   <p>Sie können eine Person auch als genehmigende Person festlegen, indem Sie die Rolle der Person angeben. Beispielsweise können Sie einen Projektbesitzer, Projektsponsor, Portfolio-Inhaber, Programm-Inhaber oder Manager als genehmigende Person zuweisen. Diese Optionen werden automatisch angezeigt, wenn Sie mit der Eingabe beginnen.</p> 
      <p><b>WICHTIG</b>:  
      <ul> 
      <li> Wenn Sie dem Projektsponsor eine Genehmigung zuweisen und niemand als Sponsor eines Projekts angegeben ist, wird die Genehmigung dem Projektbesitzer erneut zugewiesen. Wenn niemand als Eigentümer des Projekts festgelegt ist, wird die Genehmigung dem Workfront-Administrator zugewiesen. </li> 
      <li> Wenn Sie eine Genehmigung einer Funktion zuweisen und die Option <b>Genehmigende Person muss nicht im Projektteam sein</b> deaktiviert ist, aber keine Funktionen im Projektteam mit der Funktion in der Genehmigung übereinstimmen, wird die Genehmigung dem Projektbesitzer neu zugewiesen. Weitere Informationen zu den Genehmigungseinstellungen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurieren globaler Genehmigungseinstellungen</a>.
      </li> 
      <li>Wenn Sie dem Projektbesitzer eine Genehmigung zuweisen und niemand als Eigentümer eines Projekts bestimmt wird, wird die Genehmigung dem Workfront-Hauptadministrator neu zugewiesen, wie im Abschnitt „Kundeninformationen“ im Bereich „Setup“ angegeben. Weitere Informationen finden Sie <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Konfigurieren der grundlegenden Informationen für Ihr System</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Wenn Sie Aufgabengebiete als genehmigende Personen zuweisen, können alle mit diesem Aufgabengebiet verbundenen Benutzer, die auch im Projektteam sind, eine Entscheidung über die Genehmigung treffen. </p> 
      <p>Wenn Sie ein Team als genehmigende Person zuweisen, kann jeder Benutzer in diesem Team eine Entscheidung über die Genehmigung treffen. </p> 
      <p>Weitere Informationen über das Projektteam finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Projektteam - Übersicht</a>. Weitere Informationen zur Genehmigung von Arbeiten finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Genehmigen von Arbeiten </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Es ist nur eine Entscheidung erforderlich</td> 
      <td>(Wird nur angezeigt, wenn Sie mehrere genehmigende Personen zum Schritt hinzufügen.) Wählen Sie diese Option aus, wenn einer der genehmigenden Personen auf dem Schritt das Arbeitselement während dieses Schritts genehmigen oder ablehnen kann. Diese Aktion ermöglicht es dem Arbeitselement, die Phase zu verlassen.  
      <p>Wenn diese Option nicht ausgewählt ist, müssen alle identifizierten genehmigenden Personen die Phase (in beliebiger Reihenfolge) genehmigen oder ablehnen, bevor das Element die Phase verlässt. Wenn eine der genehmigenden Personen das Stadium ablehnt, wird der Prozess unterbrochen und von vorne gestartet, damit die erforderlichen Änderungen vorgenommen werden können. Die genehmigenden Personen können die Phase dann erneut genehmigen oder ablehnen.</p> 
      <p>Wenn ein Team als genehmigende Person benannt wird, kann jedes Teammitglied einen Schritt gewähren oder ablehnen.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Phase hinzufügen</p> </td> 
      <td>(Optional) Fügen Sie dem Pfad einen weiteren Schritt hinzu, indem Sie die Optionen verwenden, die in den drei obigen Zeilen erläutert werden. Sie können dem Pfad so viele Phasen hinzufügen, wie Sie benötigen.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Auswählen, was passiert, wenn die Genehmigung abgelehnt wird</td> 
      <td> <p>Wählen Sie die Aktion aus, die Sie ausführen möchten, wenn das Arbeitselement in einem beliebigen Schritt des Pfads abgelehnt wird:</p> 
      <ul> <li><strong>Problem erstellen</strong>: (Nur für Projekt- und Aufgabengenehmigungsprozesse verfügbar) Ein Problem wird in dem Projekt oder der Aufgabe erstellt, in dem/der der Genehmigungsprozess ausgeführt wird. Die der Aufgabe standardmäßig zugewiesene Ressource oder der Projektbesitzer wird dem Problem zugewiesen. Standardmäßig lautet der Name des erstellten Problems <strong>Genehmigung abgelehnt (Projekt- oder Aufgabenname)</strong>. Hierbei handelt es sich um ein Ablehnungsproblem, das je nach Genehmigungsprozess, in dem die Ablehnung stattfand, unter der Aufgabe oder dem Projekt eingegeben wird.</li> 
      <li> <p><strong>Status festlegen auf</strong>: Wählen Sie eine der folgenden Optionen:</p> 
      <ul> <li><strong>Vorheriger Status</strong>: Das abgelehnte Projekt, die abgelehnte Aufgabe oder das abgelehnte Problem wird auf den Status vor dem Status zurückgesetzt, der den Genehmigungsprozess aktiviert.</li> 
      <li> <p><strong>Beliebiger anderer Status in der Liste</strong>: Das abgelehnte Objekt wechselt in den ausgewählten Status, z. B. „Zurückgestellt“. Sie können einen der Standardstatus oder einen benutzerdefinierten Status auswählen, den Sie Ihrem Workfront-System hinzugefügt haben.</p> <p>Wenn Sie einen mit einem Genehmigungsprozess verknüpften Status als Ablehnungsstatus für einen Genehmigungspfad auswählen, wechselt das abgelehnte Objekt in den ausgewählten Status und erhält die Kennzeichnung „Genehmigung ausstehend“.</p>
      <p>Wenn Sie beispielsweise für den Ablehnungsstatus Halten auswählen und der Halten -Status mit einem Genehmigungsprozess verknüpft ist, wird das abgelehnte Objekt in den Status „Wird gehalten - Genehmigung ausstehend“ versetzt, was eine Genehmigung erfordert.</p>    <p>Für einen systemweiten Genehmigungsprozess sind nur systemweite Status verfügbar.</p> <p>Für einen gruppenspezifischen Genehmigungsprozess stehen alle Gruppenstatus zur Verfügung. Dazu gehören alle benutzerdefinierten Status, die der Gruppenadministrator speziell für die Gruppe erstellt hat, sowie alle systemweiten Status. </p> <p>Informationen zur Funktionsweise von Genehmigungsprozessen mit Status finden Sie im Abschnitt <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Wie Genehmigungsprozesse auf Status </a>) im Artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Übersicht über Genehmigungsprozesse</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie **Pfad hinzufügen**, um einen weiteren Pfad zum Genehmigungsprozess hinzuzufügen, der auf die Liste der Optionen im vorherigen Schritt verweist.

   Der neue Pfad muss mit einem anderen Status verknüpft sein. Der Pfad gibt Trigger, wenn das Element aktualisiert wird, um diesen Status anzuzeigen. Sie können nicht zwei Pfade für denselben Status haben.

1. Klicken Sie auf **Speichern**.
1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Ordnen Sie bestimmte Projekte, Aufgaben oder Probleme systemweit dem Genehmigungsprozess zu, wie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) beschrieben.
   * Benachrichtigen Sie Benutzende außerhalb von Workfront darüber, dass ihnen der Genehmigungsprozess zur Verfügung steht, um sie mit ihren Projekten, Aufgaben oder Problemen zu verknüpfen, wie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) beschrieben.
   * Erstellen Sie einen weiteren Genehmigungsprozess, der ausgelöst wird, wenn dieser Genehmigungsprozess abgelehnt wird und das Element einen anderen Status erhält. Auf diese Weise können Sie Genehmigungsprozesse miteinander verknüpfen.
