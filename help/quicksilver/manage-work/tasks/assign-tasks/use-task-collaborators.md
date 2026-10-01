---
title: Verwenden von Arbeitsagenten
content-type: reference
description: Erfahren Sie, wie Sie Arbeitsagenten und KI-Mitarbeiter verwenden, die Workfront-Aufgaben zugewiesen werden können.
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: a4dfe29c0cf85f6029fd5f4398942c60bd3d6b5a
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 2%
---
# Verwenden von Arbeitsagenten

{{preview-fast-release-general}}

Arbeitsagenten sind KI-Mitwirkende, die Workfront-Aufgaben und -Problemen direkt zugewiesen werden können. Wie andere KI-Mitwirkende werden Arbeitsagenten im Bereich „Setup“ konfiguriert und Aufgaben wie Benutzenden zugewiesen.

Arbeitsagenten stellen eine Verbindung zu Agenten her, die Sie in Copilot Studio, Claude, Writer, <span class="preview">OpenAI oder IBM konfiguriert haben. </span>

>[!IMPORTANT]
>
>Der Autor verwirft die Verwendung von Agenten. Mit Writer-Agenten konfigurierte Arbeitsagenten funktionieren nach dem 9. Oktober nicht mehr. 2026.
>
>Weitere Informationen zur Einstellung finden Sie unter [Migration und Einstellung von Agentenbibliotheken](https://support.writer.com/articles/8335689949-migrating-no-code-agents) in der Writer-Dokumentation.

Informationen und Anweisungen zum Erstellen eines Arbeitsagenten in Workfront finden Sie unter [Konfigurieren eines ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)) im Artikel Konfigurieren von KI-Mitwirkenden.

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

* Sie müssen einen Agenten in Copilot, Claude, Writer.ai, OpenAI oder IBM konfigurieren, bevor Sie ihn als Arbeitsagenten in Workfront verwenden können.

## Arbeitsagenten - Übersicht

Arbeitsagenten sind eine Möglichkeit, Agenten bestimmten Aufgaben in Workfront zuzuweisen. Sie konfigurieren den Agenten in einer App wie Copilot Studio, Claude oder Writer.ai und verbinden diesen Agenten dann mit Workfront als Arbeitsagenten. Anschließend können Sie sie wie eine Benutzerin bzw. einen Benutzer Aufgaben zuweisen.

Beispiele für Workflows:

* Erkennen von Bildern, die in eine Aufgabe hochgeladen wurden, Generieren von Varianten basierend auf den dem Agenten gegebenen Kriterien und Hochladen der neuen Bilder in die Aufgabe.
* Erstellen einer Kopie aus einer Aufgabenbeschreibung, Überprüfen der Kopie anhand der im Agenten konfigurierten Richtlinien und Senden einer Kopie an den Aktualisierungsverlauf.
* Lesen der Details eines Ereignisses, Identifizieren fehlender Details und Posten von Fragen zu fehlenden Details im Aktualisierungsverlauf.

>[!NOTE]
>
>* Spezifische Details zu den Zuständigkeiten und Fähigkeiten eines Agenten werden in der Anwendung konfiguriert, in der der Agent erstellt wird, nicht in Workfront.
>* Der Workfront MCP-Server muss nicht zu dem als Arbeitsagent verwendeten Agenten hinzugefügt werden und muss nicht verbunden sein, damit der Arbeitsagent funktioniert.
>* Arbeitsagenten unterstützen derzeit in Copilot Studio, Claude und Writer.ai, <span class="preview">OpenAI und IBM erstellte Agenten</span>
>* Beim Konfigurieren eines Agenten in Copilot Studio müssen Sie die Sicherheit auf &quot;**Authentifizierung“**.
>* Informationen und Anweisungen zum Erstellen eines Arbeitsagenten in Workfront finden Sie unter [Konfigurieren eines ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)) im Artikel Konfigurieren von KI-Mitwirkenden.

## Informationen, die ein Arbeitsagent liest

Wenn ein Arbeitsagent mit der Arbeit an einer Aufgabe beginnt, liest er automatisch die folgenden Aufgabeninformationen als Kontext:

* Aufgabentitel
* Aufgabenbeschreibung
* Kommentare im Aktualisierungsverlauf der Aufgabe
* Informationen in jedem benutzerdefinierten Formular, das an die Aufgabe angehängt ist
* <span class="preview"> Dokumente</span>

Diese Informationen werden immer gelesen und können nicht in Workfront konfiguriert werden.

>[!TIP]
>
>Für optimale Ergebnisse empfehlen wir Folgendes:
>
>* Einschließlich Hintergrundinformationen, die vom Agenten direkt in der Aufgabenbeschreibung oder einem relevanten benutzerdefinierten Formularfeld verwendet werden sollen.
>* Sicherstellen, dass die Aufgabe mit den Aufgaben übereinstimmt, für die Ihr Agent beauftragt wurde. Wenn Ihr Agent beispielsweise angewiesen wird, Text aus dem Englischen ins Französische zu übersetzen, fügen Sie den Text, den Sie übersetzen möchten, in die Aufgabenbeschreibung ein.

## Trigger zum Starten des Arbeitsagenten

Wenn ein Arbeitsagent einer Aufgabe (<span class="preview"> einem Problem) zugewiesen </span>, beginnt seine Arbeit, wenn eine der folgenden Situationen eintritt:

<!--update wording to include issues when this goes to production-->

* Der Arbeitsagent ist einer Aufgabe zugewiesen, die startbereit ist. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Der Arbeitsagent und ein Benutzer werden einer Aufgabe zugewiesen, und der Arbeitsagent wird zuerst zugewiesen.
* Eine Aufgabe, der bereits ein Arbeitsagent als zugewiesen wurde, ist startbereit und der Arbeitsagent ist der einzige oder primäre Zugewiesene. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Eine Aufgabe, der bereits ein Arbeitsagent und ein Benutzer zugewiesen sind, ist startbereit, und der Arbeitsagent wurde zuerst zugewiesen oder ist der primäre Zugewiesene. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger abgeschlossen.)
* Ein Benutzer und ein Arbeitsagent werden einer Aufgabe zugewiesen und der Benutzer wird entfernt.
* Ein(e) Benutzende(r) und ein Arbeitsagent werden einer Aufgabe zugewiesen und der Arbeitsagent wird als der Primäre Beauftragte für die Aufgabe festgelegt.

Die folgenden Situationen führen nicht dazu, dass der Arbeitsagent mit der Arbeit an der Aufgabe beginnt:

* Ein Arbeitsagent ist einer Aufgabe zugewiesen, der bereits ein Benutzer zugewiesen ist.
* Ein Arbeitsagent wird in einer Aufgabe @mentioned.
* Ein Arbeitsagent wird einer Aufgabe zugewiesen, der bereits ein Arbeitsagent zugewiesen ist. In diesem Fall hat der erste zugewiesene Arbeitsagent bereits mit der Arbeit begonnen, und der zweite Arbeitsagent unternimmt nichts.
* Ein Arbeitsagent ist einer Aufgabe zugewiesen, die noch nicht startbereit ist. (Wenn die Aufgabe beispielsweise Vorgänger hat, sind die Vorgänger noch nicht abgeschlossen.)

## Zuweisen eines Arbeitsagenten zu einer Aufgabe (<span class="preview"> Problem</span>

Arbeitsagenten werden Aufgaben (<span class="preview"> Problemen) auf </span> Weise zugewiesen.

Wenn Sie in der Liste der verfügbaren Bevollmächtigten nach einem Arbeitsagenten suchen, ist der Name des Arbeitsagenten nur ein Vorname.

Anweisungen finden Sie unter [Aufgaben zuweisen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md).

>[!NOTE]
>
>Arbeitsagenten können nicht zur Überprüfung oder Genehmigung eines Dokuments zugewiesen werden.

## Fehlerbehebung bei Arbeitsagenten

Wenn Ihr Arbeitsagent keine Antwort oder Ausgabe zurückgibt, überprüfen Sie Folgendes:

* Stellen Sie sicher, dass der Agent auf der Seite des KI-Plattformanbieters veröffentlicht wird.
* Stellen Sie sicher, dass Sie über ausreichende KI-Credits für die Plattform Ihres Agenten verfügen.
* Stellen Sie sicher, dass für die in der Aufgabe ausgeführte Aktion keine bestimmte Zugriffsebene erforderlich ist.
* Wenn Sie Copilot als Agentenanbieter verwenden, stellen Sie sicher, dass Sie die Einstellung „Keine Authentifizierung“ verwenden.
* Wenn Sie Copilot verwenden, stellen Sie sicher, dass Ihr Agent in einer globalen Umgebung konfiguriert ist. Die Funktion für Arbeitsagenten unterstützt derzeit keine regionalen Versionen von Copilot Studio.
* Stellen Sie sicher, dass der Mitarbeiter der primäre Zugewiesene für die Aufgabe ist.
* Stellen Sie sicher, dass die Aufgabe, der der Arbeitsagent zugewiesen ist, gestartet werden kann. Überprüfen Sie beispielsweise, ob alle Aufgabenvorgänger dieser Aufgabe abgeschlossen sind.

>[!TIP]
>
>Sie können auch zur Plattform des Agentenanbieters gehen und den Agenten bitten, die Aufgabe innerhalb der Plattform auszuführen. Wenn der Agent die Aufgabe nicht innerhalb der Plattform ausführen kann, treten beim Arbeitsagenten auch Probleme in Workfront auf.
