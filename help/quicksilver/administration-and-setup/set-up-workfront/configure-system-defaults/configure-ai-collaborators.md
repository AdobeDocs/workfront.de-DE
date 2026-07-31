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
source-git-commit: dc6bfcd7d3431532c1227f6cd31f22445882143f
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 2%

---

# KI-Mitwirkende konfigurieren


<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>


KI-Mitwirkende sind eine Möglichkeit, KI-Agenten in Ihre Projekte und Aufgaben einzubinden. Sie können einen KI-Mitwirkenden konfigurieren und ihn dann wie einen Benutzer zuweisen.

Sie können beispielsweise einen KI-Mitarbeiter vom Typ „Prüfer“ mit Markenrichtlinien konfigurieren und diesen Mitarbeiter dann zuweisen, um ein Dokument zu überprüfen.

Zu den verfügbaren KI-Typen für Mitwirkende gehören:

* Reviewer: Erstellen Sie einen Mitarbeiter mit Brands oder Adobe Brand Intelligence und weisen Sie ihn dann als Reviewer für Assets zu.

  Weitere Informationen finden Sie unter [Erste Schritte mit dem Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Aufgabenmitarbeiter: Erstellen Sie einen Mitwirkenden mit Copilot oder Writer und weisen Sie dann den Mitwirkenden einer Aufgabe zu, um Arbeiten auf Aufgabenebene abzuschließen.

  Weitere Informationen finden Sie unter [Verwenden von ](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Standard, Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

### Für KI-Reviewer:

* Ihr Unternehmen muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.

  Weitere Informationen finden Sie unter [Unterschreiben des Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)Abkommens im Artikel KI-Assistent in Workfront.
* Sie müssen eine Marke in Workfront konfiguriert haben, bevor Sie sie für einen KI-Mitwirkenden vom Typ Prüfer verwenden können.

  Anweisungen finden Sie unter [Erstellen und Verwalten von Marken für den Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Um Adobe Brand Intelligence für einen Reviewer AI-Mitwirkenden verwenden zu können, muss Ihr Unternehmen das einheitliche Prüf- und Genehmigungs-Erlebnis in Workfront nutzen. </span>

  Weitere Informationen finden Sie unter [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

<div class="preview">

### Für Aufgaben-Mitwirkende

Sie müssen einen Agenten in Claude, Copilot Studio oder Writer konfigurieren, bevor Sie ihn als Task Collaborator verwenden können.

</div>

## Erstellen eines neuen KI-Mitarbeiters vom Typ „Prüfer“

Reviewer AI Collaborators können für die Verwendung von Workfront-Marken oder Adobe Brand Intelligence konfiguriert werden.

* **Marken**: Marken werden in Workfront erstellt. Sie können in Workfront Marken erstellen, indem Sie PDF-Dateien mit Ihren Markenrichtlinien hochladen oder manuell Markenelemente eingeben.
* **Adobe Brand Intelligence**: Wenn ein KI-Mitwirkender ein Asset mit Adobe Brand Intelligence überprüft, können Sie die Kommentare des Reviewers in Frame.io anzeigen.  </span>


{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Klicken Sie **Reviewer** und dann auf **Weiter**.
1. Geben Sie im Feld Name des Mitarbeiters einen Namen für den Mitarbeiter ein. Dies ist der Name, der in der Liste der verfügbaren Bevollmächtigten für eine Aufgabe angezeigt wird.
1. Wählen Sie aus, ob der Mitarbeiter eine Marke oder Adobe Brand Intelligence für seine Überprüfungen verwenden soll.
1. (Bedingt) Wenn der KI-Mitwirkende eine Marke verwenden wird, wählen Sie die Marke und die Markenrichtlinie aus, die er verwenden wird.
1. Klicken Sie auf **Speichern**.

<div class="preview">

## Aufgabe „Mitarbeiter“ konfigurieren

Aufgabenmitarbeiter sind MCP-Agenten, die Sie in Workfront Aufgaben zuweisen können. Sie konfigurieren den Task Collaborator mit einem Namen, einer Zugriffsebene und anderen Details und weisen ihn so zu, wie Sie es einem Benutzer zuweisen würden.

Da es sich bei den Aufgabenmitarbeitern um MCP-Agenten handelt, werden ihre Aktionen und Fähigkeiten dort konfiguriert, wo Sie Ihre Agenten konfigurieren. Derzeit können Agenten, die als Aufgabenmitarbeiter verwendet werden, in Copilot Studio, Claude oder Writer erstellt werden.

Eine Liste der Best Practices beim Erstellen eines Agenten für die Arbeit als Aufgabenmitarbeiter finden Sie unter [Best Practices zum Erstellen eines Agenten für einen Aufgabenmitarbeiter](#best-practices-for-creating-an-agent-for-a-task-collaborator).

### Konfigurieren eines AufgabenMitarbeiters in Workfront

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Wählen Sie **Aufgabenagenten** aus und klicken Sie dann auf **Weiter**.
1. Geben Sie im Feld Name des KI-Mitarbeiters einen Namen für den Mitarbeiter ein. Dies ist der Name, der in der Liste der verfügbaren Bevollmächtigten für eine Aufgabe angezeigt wird.
1. Geben Sie im Feld KI-Mitwirkende-Beschreibung eine Beschreibung des Zwecks des Mitwirkenden oder der von ihm durchgeführten Aktionen ein.
1. Wählen Sie im Feld Zugriffsebene eine Zugriffsebene für diesen Mitarbeiter aus. Diese Zugriffsebene steuert, was der Mitarbeiter tun kann, auf dieselbe Weise wie eine Zugriffsebene steuert, was ein Benutzer tun kann.
1. Wählen **im Bereich „Agent-Herkunft auswählen** aus, ob Sie einen Agenten verbinden möchten, der in einer gemeinsamen Plattform wie Copilot oder Writer erstellt wurde, oder einen benutzerdefinierten Agenten verwenden möchten.
1. (Bedingt) Wenn Sie einen Agenten von einer gemeinsamen Plattform verwenden, geben Sie Authentifizierungsdetails für die Plattform des Agenten ein:

   | Plattform | Erforderliche Authentifizierung |
   |---|---|
   | CoPilot Studio | Geheimnis für Web-Kanal |
   | Claude Managed Agents | Anthropische API-Schlüssel<br>Agent-ID<br>Umgebungs-ID |
   | Verfasser bzw. Verfasserin | API-Schlüssel<br>Anwendungs-ID |

1. Klicken Sie **Verbindung testen**. Auf diese Weise wissen Sie, ob die Verbindung korrekt eingerichtet wurde.
1. Im **Nachdem der Mitarbeiter seine Arbeit abgeschlossen hat, kann er im** die Aktionen umschalten, die der Mitarbeiter ausführen soll.
1. Klicken Sie auf **Speichern**.

Weitere Informationen zu „Aufgabenmitarbeiter“, einschließlich ihrer Zuweisung zu Aufgaben, finden Sie unter [Verwenden von Aufgabenmitarbeitern](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


### Best Practices zum Erstellen eines Agenten für einen Aufgabenmitarbeiter

Die folgenden Best Practices sind möglicherweise hilfreich, wenn Sie einen Agenten erstellen, der als Aufgabenmitarbeiter in Workfront verwendet werden soll. Um die Best Practices anzuzeigen, klicken Sie auf den Abschnitt für das Programm, in dem Sie den Agenten erstellen.

+++ Claude

1. Navigieren Sie zur Claude-Konsole unter [platform.claude.com](https://platform.claude.com/).
1. Erstellen Sie einen API-Schlüssel.
   1. Klicken Sie unter API-Schlüssel **Schlüssel erstellen** in der oberen rechten Ecke.
   1. Geben Sie einen Namen und ein Ablaufdatum an.
   1. Kopieren Sie den Schlüssel und speichern Sie ihn an einem sicheren Ort. Sie benötigen diesen Schlüssel, um den Task Collaborator in Workfront zu konfigurieren.

1. Erstellen Sie eine Umgebung.
   1. Klicken **unter** > **Umgebungen** oben rechts auf **Umgebung erstellen**.
   1. Geben Sie einen Namen und ggf. einen Hosttyp an.
   1. Konfigurieren Sie freigegebene Pakete und Metadaten nach Bedarf. Umgebungen können über mehrere Agenten hinweg wiederverwendet werden und ermöglichen gemeinsame Pakete und Metadaten.
      Die Umgebungs-ID wird unter dem Umgebungsnamen in der oberen linken Ecke angezeigt.

1. Erstellen Sie einen Agenten.
   1. Klicken Sie unter Managed Agents > Agents **Create Agent** in der oberen rechten Ecke.
   1. Geben Sie nach Bedarf einen Namen, ein Modell, eine Systemaufforderung, Kenntnisse und Tools an. Seien Sie beschreibend, da die Aufgabenmitarbeiter den Aufgabenkontext an diesen Agenten weitergeben, der dann die Arbeit ausführt.
      Die Agenten-ID wird unter dem Namen des Agenten in der oberen linken Ecke angezeigt.

1. Konfigurieren Sie den Task Collaborator in Workfront.
   1. Geben Sie Ihren API-Schlüssel, die Umgebungs-ID und die Agenten-ID ein
   1. Klicken Sie **Verbindung testen**, um sie zu überprüfen.

1. Weisen Sie den Aufgabenmitarbeiter einer Workfront-Aufgabe zu.
   1. Der Aufgaben-Collaborator wird ausgelöst, nachdem alle Vorgängeraufgaben abgeschlossen sind.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Verfasser bzw. Verfasserin

Beim Erstellen eines Agenten für die Verwendung als Aufgabenmitarbeiter in Writer empfehlen wir den folgenden Workflow.

Ausführlichere Informationen zum Erstellen von Agenten finden Sie in der [Writer-Dokumentation](https://dev.writer.com/no-code/introduction).

1. Erstellen Sie eine Nicht-Code-App in Writer AI Studio.
1. Ein einzelnes Texteingabefeld hinzufügen. Sie können den Standardnamen „Texteingabe“ verwenden.
1. `@TextInput` zu Ihrer Eingabeaufforderung hinzufügen. Stellen Sie im Abschnitt Eingabeaufforderungen Ihrer App-Konfiguration sicher, dass Ihre Eingabeaufforderungsvorlage auf die Eingabevariable verweist. Ohne dies sieht das Modell die Aufgabendaten nie.
1. Passen Sie Ihre Eingabeaufforderung an, um die Ausgabe sofort zu generieren. Entfernen Sie alle Anweisungen, die den Benutzer um Klarstellung oder zusätzlichen Kontext bitten, bevor Sie antworten. Beispiel: „Wenn Sie eine Eingabe erhalten, behandeln Sie sie als Anfrage zur Inhaltserstellung und erstellen Sie die Ausgabe sofort. Bitten Sie nicht um Klarstellung.“
1. Kopieren Sie Ihren API-Schlüssel und die Anwendungs-ID. Zum Konfigurieren des Task Collaborators in Workfront benötigen Sie Task Collaborator .

   * Anweisungen zum Einrichten eines API-Schlüssels in Writer finden Sie unter [Quickstart](https://dev.writer.com/home/quickstart) in der Writer-Dokumentation.
   * Anweisungen zum Einrichten einer Anwendungs-ID in Writer finden Sie unter [Aufrufen von Nicht-Code-Agenten über die API](https://dev.writer.com/home/applications) in der Writer-Dokumentation.

1. Konfigurieren Sie den Task Collaborator in Workfront. Geben Sie im Rahmen der Konfiguration Ihren API-Schlüssel und Ihre Anwendungs-ID ein und klicken Sie dann auf **Verbindung testen**, um sie zu überprüfen.
1. Weisen Sie den Aufgabenmitarbeiter einer Workfront-Aufgabe zu. Der Collaborator beginnt mit der Arbeit, wenn alle Vorgängeraufgaben der Aufgabe abgeschlossen sind.

+++

</div>

## KI-Mitwirkende verwalten

Sie können vorhandene KI-Mitwirkende bearbeiten, kopieren und löschen.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. (Bedingt) Um einen Mitarbeiter zu bearbeiten, klicken Sie auf den Namen des Mitarbeiters, den Sie bearbeiten möchten, nehmen Sie im Fenster „Mitarbeiter bearbeiten“ Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Mitwirkenden zu kopieren, klicken Sie auf das Kopiersymbol ![Kopiersymbol](assets/copy-ai-collaborator.png) in der Zeile des KI-Mitwirkenden, die Sie kopieren möchten, klicken Sie auf den Namen der Kopie, nehmen Sie im Fenster Mitwirkende bearbeiten Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Kollaborateur zu löschen, klicken Sie auf das Löschsymbol ![Löschsymbol](assets/delete-collaborator-icon.png) in der Zeile des KI-Mitarbeiters, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
