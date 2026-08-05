---
title: Aufgaben-Mitwirkende verwenden
content-type: reference
description: Erfahren Sie, wie Sie Aufgabenkollaboratoren verwenden, KI-Collaboratoren, die Workfront-Aufgaben zugewiesen werden können.
author: Becky
feature: Work Management, Tasks
source-git-commit: 2070a27e18d768dd14ce4f5c681ab08669c81766
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 6%

---

# Aufgaben-Mitwirkende verwenden

{{highlighted-preview-article-level}}

Aufgabenmitarbeiter sind KI-Mitwirkende, die zusätzlich zu dem bestehenden KI-Mitwirkenden des Typs „Prüfer“, der für Dokument- und Asset-Überprüfungen verwendet wird, direkt Workfront-Aufgaben zugewiesen werden können. Wie andere KI-Mitwirkende werden die Aufgaben-Mitwirkenden im Bereich „Setup“ konfiguriert und Aufgaben wie Benutzenden zugewiesen.

Die Mitarbeiter von Aufgaben stellen eine Verbindung zu den von Ihnen konfigurierten Agenten her, ähnlich wie bei einem MCP-Server.

Informationen und Anweisungen zum Erstellen eines Task Collaborators in Workfront finden Sie unter [Konfigurieren eines Task Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) im Artikel Konfigurieren von KI-Collaboratoren.

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
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

* Sie müssen einen Agenten in Copilot, Claude oder Writer.ai konfigurieren, bevor Sie ihn als Aufgabenmitarbeiter verwenden können.

## Übersicht über den Aufgabenmitarbeiter

Aufgabenkollaborateure sind eine Möglichkeit, MCP-Agenten bestimmten Aufgaben in Workfront zuzuweisen. Sie konfigurieren den Agenten in einer App wie Copilot Studio, Claude oder Writer.ai und verbinden diesen Agenten dann mit Workfront als Aufgabenmitarbeiter. Anschließend können Sie sie wie eine Benutzerin bzw. einen Benutzer Aufgaben zuweisen.

Beispiele für Workflows:

* Erkennen von Bildern, die in eine Aufgabe hochgeladen wurden, Generieren von Varianten basierend auf den dem Agenten gegebenen Kriterien und Hochladen der neuen Bilder in die Aufgabe.
* Erstellen einer Kopie aus einer Aufgabenbeschreibung, Überprüfen der Kopie anhand der im Agenten konfigurierten Richtlinien und Senden einer Kopie an den Aktualisierungsverlauf.
* Lesen der Details eines Ereignisses, Identifizieren fehlender Details und Posten von Fragen zu fehlenden Details im Aktualisierungsverlauf.

>[!NOTE]
>
>* Spezifische Details zu den Zuständigkeiten und Fähigkeiten eines Agenten werden in der Anwendung konfiguriert, in der der Agent erstellt wird, nicht in Workfront.
>* Mitarbeiter von Aufgaben unterstützen derzeit in Copilot Studio, Claude und Writer.ai erstellte Agenten.
>* Beim Konfigurieren eines Agenten in Copilot Studio müssen Sie die Sicherheit auf &quot;**Authentifizierung“**.
>* Informationen und Anweisungen zum Erstellen eines Task Collaborators in Workfront finden Sie unter [Konfigurieren eines Task Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator) im Artikel Konfigurieren von KI-Collaboratoren.

## Aufgabe einem Mitarbeiter zuweisen

Aufgabenmitarbeiter werden Aufgaben auf die gleiche Weise zugewiesen wie Benutzern.

Anweisungen finden Sie unter [Aufgaben zuweisen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
