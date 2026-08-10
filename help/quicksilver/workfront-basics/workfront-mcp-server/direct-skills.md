---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Für die direkte Installation verfügbare Kenntnisse
description: Workfront bietet einige Fähigkeiten, die Sie direkt in Ihr LLM installieren können.
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---


# Für die direkte Installation verfügbare Kenntnisse

Workfront bietet einige Fähigkeiten, die Sie direkt in Ihr LLM installieren können. Die Fähigkeiten zeigen, wie diese Tools für bestimmte Aufgaben verwendet werden, wobei die richtigen Schritte bereits integriert sind.

Diese Kenntnisse finden Sie im GitHub-Repository zu Adobe Skills.

>[!NOTE]
>
>Derzeit sind diese Fähigkeiten nur für Claude verfügbar.
>Anweisungen zum Einrichten von Claude mit Adobe finden Sie unter [Erste Schritte](https://developer.adobe.com/adobe-for-creativity/getting-started/) in der Dokumentation zu Adobe Developer.

## Installieren Sie eine Qualifikation aus dem Workfront GitHub-Repository in Claude.

1. Navigieren Sie zum [Adobe Workfront Skills Repository](https://github.com/adobe/skills/tree/main/plugins/workfront) auf GitHub.
1. Laden Sie den Ordner für Kenntnisse herunter, den Sie verwenden möchten.
1. Kopieren Sie den Ordner in Ihre Claude-Kompetenzbibliothek.

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` (macOS) oder gleichwertig.
   * Claude-Code: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Derzeit verfügbare Kenntnisse

| Kenntnisse/Link zum Ordner | Beschreibung der Kenntnisse | Verfügbar für |
|---|---|---|
| [Planning Solution Architect](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Konfigurieren Sie einen Workfront Planning-Arbeitsbereich, um Ihren Anforderungen gerecht zu werden, und beantworten Sie Fragen zu Workfront Planning. | Claude |
