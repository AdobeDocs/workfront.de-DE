---
title: Erstellen von App Builder-Apps mit Claude Code-Kenntnissen
description: Verwenden Sie eine Reihe von Claude-Code-Fähigkeiten, um benutzerdefinierte Adobe Workfront App Builder-Apps zu erstellen, indem Sie beschreiben, was Sie möchten, anstatt die Einrichtungs- und Bereitstellungsschritte selbst auszuführen.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Erstellen von App Builder-Apps mit Claude Code-Kenntnissen

Mit einem Skill-Paket können [!DNL Claude] (oder beliebige KI-Codierungs-Kabelbäume, die Claude-formatierte Fähigkeiten wie [!DNL Claude Code] oder [!DNL OpenAI Codex] unterstützen) benutzerdefinierte [!DNL Adobe App Builder]-Apps für [!DNL Workfront] erstellen. Wenn Sie Zugriff auf eines dieser Tools haben, können Sie eine Benutzeroberflächenerweiterung erstellen, indem Sie beschreiben, was Sie möchten, in einfachem Englisch, ohne Entwicklererfahrung oder manuelle Einrichtungsschritte.

Benutzeroberflächenerweiterungen für Workfront auf Basis von Adobe App Builder ermöglichen es Kundinnen und Kunden sowie Partnern, benutzerdefinierte Benutzererlebnisse zu erstellen. Benutzeroberflächenerweiterungen ermöglichen es Ihnen, das Workfront-Erlebnis Ihres Unternehmens zu ändern, um es besser an die Anforderungen des Unternehmens anzupassen. Dies kann die Effizienz verbessern, nahtlose, vernetzte Erlebnisse bereitstellen und die Benutzerzufriedenheit erheblich verbessern und Ihrem Unternehmen dabei helfen, seine einzigartige Vision zu verwirklichen.

Weitere Informationen zu Workfront-Benutzeroberflächenerweiterungen finden Sie unter [Erstellen benutzerdefinierter Programme für Workfront mit Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Benutzeroberflächen-Erweiterbarkeitsfähigkeiten

Die Erweiterbarkeitsfähigkeiten der Benutzeroberfläche ermöglichen es einem KI-Codierungs-Kabelbaum, die Erstellung von Benutzeroberflächenerweiterungen in Workfront zu verwalten. Sie beschreiben die gewünschte Funktion und erledigen die praktischen Aufgaben, z. B. das Einrichten der Tools, das Erstellen Ihres Projekts in [!DNL Adobe App Builder], das Erstellen der App, die Bereitstellung in der Cloud von Adobe und die Ausführung in Workfront. Sie sind nur dann am Prozess beteiligt, wenn eine Entscheidung oder Anmeldung vorliegt, die eine Aktion von Ihnen erfordert. In diesem Artikel wird [!DNL Claude] als Beispiel verwendet, die Anweisungen gelten jedoch für alle KI-Codierungs-Kabelbäume mit Unterstützung von Claude Skills.

## Voraussetzungen

Bevor Sie beginnen, stellen Sie Folgendes sicher:

* **Ein KI-Codierungs-Kabelbaum, der Claude Skills unterstützt** z. B. [!DNL Claude Code].

  Weitere Informationen zu Claude Skills finden Sie unter [Was sind Fähigkeiten?](https://support.claude.com/en/articles/12512176-what-are-skills) in der Claude-Dokumentation.

* **Zugang zu den Kenntnissen**.

  * Die Qualifikationen finden Sie unter [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Wenn sich dieser Link nicht für Sie öffnet, bitten Sie Ihren Administrator, Ihnen Zugriff zu gewähren.
  * Die Qualifikationen werden auf dem Adobe-Markt für öffentliche Kompetenzen veröffentlicht ([adobe/skills](https://github.com/adobe/skills)). Führen Sie in [!DNL Claude Code] Folgendes aus:

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* **[!DNL Adobe App Builder]Zugriff mit der Rolle Entwickler**. Ihr Adobe-Unternehmen benötigt eine App Builder-Lizenz, und Sie müssen darin als Entwickler hinzugefügt werden. Dadurch können [!DNL Claude] die Adobe Developer Console öffnen und Ihr Projekt erstellen.

  So überprüfen Sie, ob diese Voraussetzung erfüllt ist:

  1. Öffnen Sie die [Adobe Developer Console](https://developer.adobe.com/console).
  1. Bestätigen Sie, dass die oben rechts angezeigte Organisation korrekt ist.
  1. Klicken Sie **Neues Projekt erstellen** > **Projekt aus Vorlage erstellen**.
  1. Überprüfen, ob **App Builder** in der Liste angezeigt wird.

     * Wenn **App Builder** in der Liste angezeigt wird, haben Sie Zugriff.
     * Wenn es keine Option **Projekt aus Vorlage erstellen** oder keine Option **App Builder** gibt, haben Sie noch keinen Zugriff. Bitten Sie Ihren Workfront- oder Adobe-Administrator, Sie als Entwickler hinzuzufügen (in der Adobe Admin Console > Benutzer > Entwickler), und bestätigen Sie, dass Ihr Unternehmen über eine App Builder-Lizenz verfügt.
* **Der Workfront-MCP-Server ist**, sodass [!DNL Claude] die echte Workfront-API verwendet, anstatt Datentypen, Felder und Befehle zu erraten.

  Um zu überprüfen, ob der Workfront MCP-Server bereits verbunden ist, fragen Sie [!DNL Claude]: *„Können Sie die Workfront MCP-Ressourcen sehen?“*

  Weitere Informationen und Anweisungen finden Sie unter [Workfront mit Claude verbinden](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude) im Artikel Konfigurieren des Adobe Workfront MCP-Servers.
