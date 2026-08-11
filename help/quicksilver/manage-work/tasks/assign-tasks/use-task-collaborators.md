---
title: Aufgaben-Mitwirkende verwenden
content-type: reference
description: Erfahren Sie, wie Sie Aufgabenkollaboratoren verwenden, KI-Collaboratoren, die Workfront-Aufgaben zugewiesen werden können.
author: Becky
feature: Work Management, Tasks
source-git-commit: 72921e4a1cb9ca564a5c8b4a7a587e37f6a90cc5
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 3%

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

## Trigger für den Start des Aufgabenmitarbeiters

Wenn eine Aufgabe einem Mitarbeiter zugewiesen wird, beginnt die Arbeit, wenn eine der folgenden Situationen eintritt:

* Der Aufgabenkollaborator wurde einer Aufgabe zugewiesen, die startbereit ist. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Die Aufgabe „Mitarbeiter“ und ein Benutzer werden einer Aufgabe zugewiesen und die Aufgabe „Mitarbeiter“ wird zuerst zugewiesen.
* Eine Aufgabe, der bereits ein Aufgabenmitarbeiter zugewiesen wurde, wird startbereit und der Aufgabenmitarbeiter ist der einzige oder primäre Zugewiesene. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Eine Aufgabe, der bereits ein Aufgabenmitarbeiter und ein Benutzer zugewiesen sind, ist startbereit, und der Aufgabenmitarbeiter wurde zuerst zugewiesen oder ist der primäre Zugewiesene. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Ein(e) Benutzende(r) und ein Mitarbeiter(in) für eine Aufgabe werden einer Aufgabe zugewiesen und der/die Benutzende wird entfernt.
* Ein Benutzer und ein Aufgabenmitarbeiter werden einer Aufgabe zugewiesen und der Aufgabenmitarbeiter wird als Primärer Bearbeiter für die Aufgabe festgelegt.

Die folgenden Situationen führen nicht dazu, dass der Mitarbeiter der Aufgabe mit der Arbeit an der Aufgabe beginnt:

* Einem Aufgabenmitarbeiter wird eine Aufgabe zugewiesen, der bereits ein Benutzer zugewiesen ist.
* In einer Aufgabe wird ein Aufgabenmitarbeiter @mentioned.
* Ein Aufgabenmitarbeiter wird einer Aufgabe zugewiesen, der bereits ein Aufgabenmitarbeiter zugewiesen ist. In diesem Fall hat der erste zugewiesene Aufgabenmitarbeiter bereits mit der Arbeit begonnen, und der zweite Aufgabenmitarbeiter unternimmt nichts.
* Einem Aufgabenmitarbeiter wird eine Aufgabe zugewiesen, die noch nicht startbereit ist. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger noch nicht abgeschlossen.)

## Aufgabe einem Mitarbeiter zuweisen

Aufgabenmitarbeiter werden Aufgaben auf die gleiche Weise zugewiesen wie Benutzern.

Wenn Sie in der Liste der verfügbaren Bevollmächtigten nach einem Aufgabenmitarbeiter suchen, ist der Name des Aufgabenmitarbeiters nur ein Vorname.

Anweisungen finden Sie unter [Aufgaben zuweisen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).
