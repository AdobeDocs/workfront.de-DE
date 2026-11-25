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
source-git-commit: ee344fe88ba7e4fb78a6d80ccbfe5cfa1ecbec47
workflow-type: tm+mt
source-wordcount: '1961'
ht-degree: 2%
---
# KI-Mitwirkende konfigurieren

KI-Mitwirkende sind eine Möglichkeit, KI-Agenten in Ihre Projekte, Aufgaben und Probleme einzubinden. Sie können einen KI-Mitwirkenden konfigurieren und ihn dann wie einen Benutzer zuweisen.

Sie können beispielsweise einen KI-Mitarbeiter vom Typ „Prüfer“ mit Markenrichtlinien konfigurieren und diesen Mitarbeiter dann zuweisen, um ein Dokument zu überprüfen.

Zu den verfügbaren KI-Typen für Mitwirkende gehören:

* KI-Reviewer: Erstellen Sie einen Mitarbeiter mit Marken oder Adobe Brand Intelligence und weisen Sie ihn dann als Reviewer für Assets zu.

  Weitere Informationen finden Sie unter [Erste Schritte mit dem Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Arbeitsagent : Erstellen Sie einen auf Adobe CX Coworker basierenden Mitarbeiter, verwenden Sie einen vordefinierten Mitarbeiter oder verbinden Sie einen Agenten von einer unterstützten externen Plattform, weisen Sie dann den Mitarbeiter einer Aufgabe oder einem Problem zu, um Arbeitselemente abzuschließen.

  Weitere Informationen finden Sie unter [Verwenden von Arbeitsagenten](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

  Weitere Informationen zu Adobe CX Enterprise Coworker finden Sie unter [Übersicht über CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

Von KI-Mitwirkenden verwendete Lizenzen werden nicht in Rechnung gestellt. Wenn Ihr Unternehmen über 200 Workfront-Lizenzen verfügt und einen KI-Mitwirkenden erstellt, werden 201 Lizenzen verwendet, aber nur 200 in Rechnung gestellt.

* Projektkoordinator: Ein vorkonfigurierter Mitarbeiter, der den Projektstatus überwacht und Projektaktualisierungen sendet, ohne einen externen Agenten konfigurieren zu müssen.

  Weitere Informationen finden Sie unter [Verwenden des Projektkoordinators](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).


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

Die Voraussetzungen hängen von der Herkunft des Agenten ab:

* Nativ in Adobe: Um CX Enterprise Coworker Collaborator verwenden zu können, muss Adobe CX Enterprise Coworker in Ihrem Unternehmen aktiviert sein. Sie müssen keinen Agenten in einer externen Plattform konfigurieren oder Anmeldeinformationen für eine externe Plattform angeben.
* Externe Plattform oder benutzerdefinierter Agent: Konfigurieren Sie den Agenten auf der Plattform, mit der Sie eine Verbindung herstellen möchten, bevor Sie den Arbeitsagenten in Workfront erstellen.

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

Da Arbeitsagenten Agenten sind, werden ihre Aktionen und Fähigkeiten dort konfiguriert, wo Sie Ihre Agenten konfigurieren. Arbeitsagenten können vorgefertigte Arbeitsagenten oder Agenten sein, die einen Kollegen verwenden, oder sie können von einer unterstützten externen Plattform wie Copilot Studio, Claude, OpenAI und IBM stammen.

>Arbeitsagenten können Aufgaben oder Problemen zugewiesen werden.

Von Arbeitsagenten verwendete Lizenzen werden nicht in Rechnung gestellt. Wenn Ihr Unternehmen über 200 Workfront-Lizenzen verfügt und einen Arbeitsagenten erstellt, werden 201 Lizenzen verwendet, aber nur 200 in Rechnung gestellt.

Eine Liste der Best Practices beim Erstellen eines Agenten für die Arbeit als Arbeitsagent finden Sie unter [Best Practices zum Erstellen eines Agenten für einen Arbeitsagenten](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Konfigurieren eines Arbeitsagenten in Workfront](#configure-a-work-agent-in-workfront)
* [Best Practices für die Erstellung eines Agenten für einen Arbeitsagenten](#best-practices-for-creating-an-agent-for-a-work-agent)

### Konfigurieren eines Arbeitsagenten in Workfront

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

1. Wählen **im Bereich &quot;** des Agenten auswählen“ aus, ob Sie nativ Adobe verwenden, einen in einer gemeinsamen Plattform wie Copilot erstellten Agenten verbinden oder einen benutzerdefinierten Agenten verwenden möchten.
1. (Bedingt) Wenn Sie Nativ in Adobe auswählen, wählen Sie den zu verwendenden Collaborator aus: den CX Enterprise Coworker-Collaborator oder einen vordefinierten KI-Collaborator wie „Aufnahmekoordinator“. Weitere Informationen zu vordefinierten Kollaborateuren, einschließlich Beschreibungen, finden Sie unter [Konfigurieren von vordefinierten KI-Kollaborateuren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-prebuilt-ai-collaborators.md).

   >[!NOTE]
   >
   >Nachdem Sie einen vordefinierten KI-Mitwirkenden aktiviert haben, dauert es etwa 30 Sekunden, bis er bereitgestellt wird. Ein Spinner wird angezeigt, bis der Collaborator bereit ist.

1. (Bedingt) Wenn Sie einen Agenten von einer gemeinsamen Plattform verwenden, geben Sie Authentifizierungsdetails für die Plattform des Agenten ein:

   | Plattform | Erforderliche Authentifizierung |
   |---|---|
   | Claude Managed Agents | Anthropische API-Schlüssel<br>Agent-ID<br>Umgebungs-ID |
   | CoPilot Studio | Geheimnis für Web-Kanal |
   | IBM watsonx Orchestrate | Service-URL<br>API-Schlüssel<br> Agent-ID |
   | OpenAI-Agents | API-Schlüssel <br>Agent-ID |
   | Playbooks schreiben | API-Schlüssel </br>Playbook-ID |

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

## Konfigurieren eines Projektkoordinators

Der Projektkoordinator ist ein vorkonfigurierter Mitarbeiter, der den Projektstatus überwacht und dabei hilft, die Arbeit auf Kurs zu halten. Im Gegensatz zu Arbeitsagenten erfordert der Projektkoordinator nicht die Konfiguration eines externen Agenten.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Wählen Sie **Projektkoordinator** aus und klicken Sie dann auf **Weiter**.
1. Geben Sie im Feld **Name des KI** Mitarbeiters“ einen Namen für den Projektkoordinator ein. Dies ist der Name, der als Mitwirkender an Ihrem Projekt angezeigt wird.
1. (Optional) Geben Sie im Feld **KI-Mitwirkende-Beschreibung** eine Beschreibung dessen ein, was der Projektkoordinator tut oder wozu er dient.
1. Wählen **Feld „Zugriffsebene** eine Zugriffsebene für den Projektkoordinator aus. Diese Zugriffsebene steuert, was die beteiligten Personen an Projekten tun können, ebenso wie eine Zugriffsebene steuert, was Benutzende tun können.
1. (Optional) Wählen Sie im Feld **Gruppen** die Gruppen aus, mit denen der Projektkoordinator verknüpft werden soll.

   >[!NOTE]
   >
   >Wenn Sie Gruppenadministrator sind, werden in diesem Feld nur Gruppen angezeigt, für die Sie Administrator sind. Gruppenadministratoren müssen mindestens eine Gruppe auswählen.

1. Geben Sie im Bereich **Koordinatoraktionen** an, wie der Projektkoordinator Projektaktualisierungen sendet. Der Projektkoordinator muss über die Berechtigung zum Ausführen dieser Aktionen verfügen. Ein Projektkoordinator kann sich auch zu dem Projekt und seinen Aufgaben äußern.

   Projektaktualisierungen können eine Zusammenfassung des Fortschritts, des Projektzustands, überfällige oder gefährdete Aufgaben oder Genehmigungen sowie fehlende Felder oder Zuweisungen enthalten.

   * Wählen **im Feld** aus, ob der Projektkoordinator täglich oder wöchentlich Aktualisierungen sendet.
   * (Bedingt) Wenn Sie „Wöchentlich“ im Feld **Tag** ausgewählt haben, wählen Sie den Wochentag aus, an den Aktualisierungen gesendet werden.
   * Wählen Sie **Feld &quot;**&quot; die Zeit aus, zu der Aktualisierungen gesendet werden.
   * Wählen Sie **Feld** die Zeitzone für die Zeitaktualisierung aus.
   * Wählen Sie im Feld **Wer erhält die Aktualisierung** aus, ob die Aktualisierung an den Projektbesitzer oder an Projektbeteiligte gesendet werden soll. Die Standardeinstellung ist der Projektbesitzer.

1. Klicken Sie auf **Speichern**.

Fügen Sie nach dem Speichern des Projektkoordinators das Feld **Projektkoordinator** zur Projektkopfzeile in den von Ihren Benutzern verwendeten Layout-Vorlagen hinzu. Benutzende können einem Projekt keinen Projektkoordinator zuweisen, bis das Feld in der Kopfzeile verfügbar ist.

Anweisungen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Weitere Informationen zum Projektkoordinator, einschließlich seiner Zuweisung zu Projekten, finden Sie unter [Verwenden des Projektkoordinators](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).

## KI-Mitwirkende verwalten

Sie können vorhandene KI-Mitwirkende bearbeiten, kopieren und löschen.

>[!NOTE]
>
>Gruppenadministratoren können nur KI-Kollaborateure anzeigen und mit ihnen interagieren, die Gruppen zugeordnet sind, für die sie Administratoren sind. Wenn andere Gruppen ebenfalls mit einem bestimmten KI-Mitwirkenden verknüpft sind, kann ein Gruppenadministrator sie anzeigen, aber nicht bearbeiten.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. (Bedingt) Um einen Mitarbeiter zu bearbeiten, klicken Sie auf den Namen des Mitarbeiters, den Sie bearbeiten möchten, nehmen Sie im Fenster „Mitarbeiter bearbeiten“ Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Kollaborateur zu löschen, klicken Sie auf das Löschsymbol ![Löschsymbol](assets/delete-collaborator-icon.png) in der Zeile des KI-Mitarbeiters, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
