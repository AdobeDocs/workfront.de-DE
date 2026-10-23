---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: KI-Mitwirkende konfigurieren
description: Als Adobe Workfront-Administrator können Sie KI-Mitwirkende konfigurieren und sie Projekten und Aufgaben zuweisen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 1a1e8fab8f8ef5c0c9dae032ed0eb5b24c3f364d
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 3%
---
# KI-Mitwirkende konfigurieren

KI-Mitwirkende sind eine Möglichkeit, KI-Agenten in Ihre Projekte, Aufgaben und Probleme einzubinden. Sie können einen KI-Mitwirkenden konfigurieren und ihn dann wie einen Benutzer zuweisen.

Sie können beispielsweise einen KI-Mitarbeiter vom Typ „Prüfer“ mit Markenrichtlinien konfigurieren und diesen Mitarbeiter dann zuweisen, um ein Dokument zu überprüfen.

Zu den verfügbaren KI-Typen für Mitwirkende gehören:

* KI-Reviewer: Erstellen Sie einen Mitarbeiter mit Marken oder Adobe Brand Intelligence und weisen Sie ihn dann als Reviewer für Assets zu.

  Weitere Informationen finden Sie unter [Erste Schritte mit dem Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Arbeitsagent : Erstellen Sie einen Mitarbeiter mit einer standardmäßigen KI-Plattform wie Claude, OpenAI oder Copilot und weisen Sie dann den Mitarbeiter einer Aufgabe oder einem Problem zu, um Arbeitselemente abzuschließen.

  Weitere Informationen finden Sie unter [Verwenden von Arbeitsagenten](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Auswählen von, Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator] oder Gruppenadministrator</span></td> 
  </tr> 
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

* [Für KI-Reviewer](#for-ai-reviewers)
* [Für Arbeitsagenten](#for-work-agents)

### Für KI-Reviewer:

* Ihr Unternehmen muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.

  Weitere Informationen finden Sie unter [Unterschreiben des Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)Abkommens im Artikel KI-Assistent in Workfront.
* Sie müssen eine Marke in Workfront konfiguriert haben, bevor Sie sie für einen KI-Reviewer verwenden können.

  Anweisungen finden Sie unter [Erstellen und Verwalten von Marken für den KI-Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Um Adobe Brand Intelligence für einen KI-Prüfer verwenden zu können, muss Ihr Unternehmen das einheitliche Prüf- und Genehmigungs-Erlebnis in Workfront verwenden.

  Weitere Informationen finden Sie unter [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Für Arbeitsagenten

Sie müssen einen Agenten in Claude, Copilot Studio, OpenAI oder IBM konfigurieren, bevor Sie ihn als Arbeitsagenten verwenden können.

>[!NOTE]
>
>Wir sind bestrebt, uns mit einem beliebigen Agentenanbieter zu verbinden. Wenn der von Ihnen verwendete Anbieter daher derzeit nicht mit Work Agents kompatibel ist, wenden Sie sich bitte an Ihr Account-Team, um Hilfe zu erhalten.

## Erstellen eines neuen KI-Reviewers

KI-Reviewer können so konfiguriert werden, dass sie Workfront-Marken oder Adobe Brand Intelligence verwenden.

* **Marken**: Marken werden in Workfront erstellt. Sie können in Workfront Marken erstellen, indem Sie PDF-Dateien mit Ihren Markenrichtlinien hochladen oder manuell Markenelemente eingeben.
* **Adobe Brand Intelligence**: Wenn ein KI-Mitwirkender ein Asset mit Adobe Brand Intelligence überprüft, können Sie in Frame.io Kommentare des KI-Reviewers anzeigen.


{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Klicken Sie **Reviewer** und dann auf **Weiter**.
1. Geben Sie im Feld Name des Mitarbeiters einen Namen für den Mitarbeiter ein. Dies ist der Name, der in der Liste der verfügbaren Bevollmächtigten für eine Aufgabe angezeigt wird.
1. Wählen Sie aus, ob der Mitarbeiter eine Marke oder Adobe Brand Intelligence für seine Überprüfungen verwenden soll.
1. (Bedingt) Wenn der KI-Mitwirkende eine Marke verwenden wird, wählen Sie die Marke und die Markenrichtlinie aus, die er verwenden wird.
1. Klicken Sie auf **Speichern**.

## Konfigurieren eines Arbeitsagenten

Arbeitsagenten sind Agenten, die Sie in Workfront Aufgaben oder Problemen zuweisen können. Sie konfigurieren den Arbeitsagenten mit einem Namen, einer Zugriffsebene und anderen Details und weisen ihn einer Aufgabe zu, wie Sie es bei der Zuweisung von Benutzenden tun würden.

Da Arbeitsagenten Agenten sind, werden ihre Aktionen und Fähigkeiten dort konfiguriert, wo Sie Ihre Agenten konfigurieren. Derzeit können als Arbeitsagenten verwendete Agenten in Copilot Studio, Claude, OpenAI und IBM erstellt werden.

Arbeitsagenten können Aufgaben oder Problemen zugewiesen werden.

Eine Liste der Best Practices beim Erstellen eines Agenten für die Arbeit als Arbeitsagent finden Sie unter [Best Practices zum Erstellen eines Agenten für einen Arbeitsagenten](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Konfigurieren eines Arbeitsagenten in Workfront](#configure-a-work-agent-in-workfront)
* [Best Practices für die Erstellung eines Agenten für einen Arbeitsagenten](#best-practices-for-creating-an-agent-for-a-work-agent)

### Konfigurieren eines Arbeitsagenten in Workfront

>[!NOTE]
>
>Von Arbeitsagenten verwendete Lizenzen werden nicht in Rechnung gestellt. Wenn Ihr Unternehmen über 200 Workfront-Lizenzen verfügt und einen Arbeitsagenten erstellt, werden 201 Lizenzen verwendet, aber nur 200 in Rechnung gestellt.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Wählen Sie **Arbeitsagenten** aus und klicken Sie dann auf **Weiter**.
1. Geben Sie im Feld Name des KI-Mitarbeiters einen Namen für den Mitarbeiter ein. Dies ist der Name, der in der Liste der verfügbaren Bevollmächtigten für eine Aufgabe angezeigt wird.
1. Geben Sie im Feld KI-Mitwirkende-Beschreibung eine Beschreibung des Zwecks des Mitwirkenden oder der von ihm durchgeführten Aktionen ein.
1. Wählen Sie im Feld Zugriffsebene eine Zugriffsebene für diesen Mitarbeiter aus. Diese Zugriffsebene steuert, was der Mitarbeiter tun kann, auf dieselbe Weise wie eine Zugriffsebene steuert, was ein Benutzer tun kann.
1. (Optional) Wählen Sie im Feld Gruppen die Gruppen aus, mit denen der Arbeitsagent verknüpft werden soll.

   >[!NOTE]
   >
   >Wenn Sie Gruppenadministrator sind, werden in diesem Feld nur Gruppen angezeigt, für die Sie Administrator sind. Gruppenadministratoren müssen mindestens eine Gruppe auswählen.

1. Wählen **im Bereich „Ursprung des Agenten**&quot; aus, ob Sie einen in einer gemeinsamen Plattform wie Copilot erstellten Agenten verbinden oder einen benutzerdefinierten Agenten verwenden möchten.
1. (Bedingt) Wenn Sie einen Agenten von einer gemeinsamen Plattform verwenden, geben Sie Authentifizierungsdetails für die Plattform des Agenten ein:

   | Plattform | Erforderliche Authentifizierung |
   |---|---|
   | CoPilot Studio | Geheimnis für Web-Kanal |
   | Claude Managed Agents | Anthropische API-Schlüssel<br>Agent-ID<br>Umgebungs-ID |
   | OpenAI-Agents | API-Schlüssel <br>Agent-ID |
   | IBM watsonx Orchestrate | Service-URL<br>API-Schlüssel<br> Agent-ID |

1. Klicken Sie **Verbindung testen**. Auf diese Weise wissen Sie, ob die Verbindung korrekt eingerichtet wurde.
1. Im **Nachdem der Mitarbeiter seine Arbeit abgeschlossen hat, kann er im** die Aktionen umschalten, die der Mitarbeiter ausführen soll.

   * Benachrichtigung senden: Der Agent gibt einen Kommentar im Aktualisierungsverlauf ab und markiert den Benutzer, der die Arbeit angefordert hat, dem Agenten zugewiesen hat oder dem das Projekt gehört.
   * Hochladen textbasierter Dokumente
   * Aufgabe als abgeschlossen kennzeichnen
   * Aufgabenfelder schreiben: Wählen Sie die Formulare und Felder aus, in die der Agent schreiben kann.
   * Projektfelder schreiben: Wählen Sie die Formulare und Felder aus, in die der Agent schreiben kann.

1. Klicken Sie auf **Speichern**.

Weitere Informationen zu Arbeitsagenten, einschließlich ihrer Zuweisung zu Aufgaben, finden Sie unter [Verwenden von Arbeitsagenten](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

### Best Practices für die Erstellung eines Agenten für einen Arbeitsagenten

Die folgenden Best Practices sind möglicherweise hilfreich, wenn Sie einen Agenten für die Verwendung als Arbeitsagent in Workfront erstellen. Um die Best Practices anzuzeigen, klicken Sie auf den Abschnitt für das Programm, in dem Sie den Agenten erstellen.

+++ Claude

1. Navigieren Sie zur Claude-Konsole unter [platform.claude.com](https://platform.claude.com/).
1. Erstellen Sie einen API-Schlüssel.
   1. Klicken Sie unter API-Schlüssel **Schlüssel erstellen** in der oberen rechten Ecke.
   1. Geben Sie einen Namen und ein Ablaufdatum an.
   1. Kopieren Sie den Schlüssel und speichern Sie ihn an einem sicheren Ort. Sie benötigen diesen Schlüssel, um den Arbeitsagenten in Workfront zu konfigurieren.

1. Erstellen Sie eine Umgebung.
   1. Klicken **unter** > **Umgebungen** oben rechts auf **Umgebung erstellen**.
   1. Geben Sie einen Namen und ggf. einen Hosttyp an.
   1. Konfigurieren Sie freigegebene Pakete und Metadaten nach Bedarf. Umgebungen können über mehrere Agenten hinweg wiederverwendet werden und ermöglichen gemeinsame Pakete und Metadaten.
      Die Umgebungs-ID wird unter dem Umgebungsnamen in der oberen linken Ecke angezeigt.

1. Erstellen Sie einen Agenten.
   1. Klicken Sie unter Managed Agents > Agents **Create Agent** in der oberen rechten Ecke.
   1. Geben Sie nach Bedarf einen Namen, ein Modell, eine Systemaufforderung, Kenntnisse und Tools an. Seien Sie beschreibend, da Arbeitsagenten den Aufgabenkontext an diesen Agenten weitergeben, der dann die Arbeit ausführt.
      Die Agenten-ID wird unter dem Namen des Agenten in der oberen linken Ecke angezeigt.

1. Konfigurieren Sie den Arbeitsagenten in Workfront.
   1. Geben Sie Ihren API-Schlüssel, die Umgebungs-ID und die Agenten-ID ein
   1. Klicken Sie **Verbindung testen**, um sie zu überprüfen.

1. Weisen Sie den Arbeitsagenten einer Workfront-Aufgabe zu.
   1. Der Arbeitsagent wird ausgelöst, nachdem alle Vorgängeraufgaben abgeschlossen sind.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Verfasser bzw. Verfasserin



>[!IMPORTANT]
>
>Writer hat die Verwendung von Agenten abgelehnt. Mit Writer-Agenten konfigurierte Arbeitsagenten funktionieren nach dem 9. Oktober nicht mehr. 2026.
>
>Weitere Informationen zur Einstellung finden Sie unter [Migration und Einstellung von Agentenbibliotheken](https://support.writer.com/articles/8335689949-migrating-no-code-agents) in der Writer-Dokumentation.


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## KI-Mitwirkende verwalten

Sie können vorhandene KI-Mitwirkende bearbeiten, kopieren und löschen.

>[!NOTE]
>
>Gruppenadministratoren können nur KI-Kollaborateure anzeigen und mit ihnen interagieren, die Gruppen zugeordnet sind, für die sie Administratoren sind. Wenn andere Gruppen ebenfalls mit einem bestimmten KI-Mitwirkenden verknüpft sind, kann ein Gruppenadministrator sie anzeigen, aber nicht bearbeiten.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. (Bedingt) Um einen Mitarbeiter zu bearbeiten, klicken Sie auf den Namen des Mitarbeiters, den Sie bearbeiten möchten, nehmen Sie im Fenster „Mitarbeiter bearbeiten“ Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Kollaborateur zu löschen, klicken Sie auf das Löschsymbol ![Löschsymbol](assets/delete-collaborator-icon.png) in der Zeile des KI-Mitarbeiters, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
