---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Für die direkte Installation verfügbare Kenntnisse
description: Workfront bietet einige Fähigkeiten, die Sie direkt in Ihr LLM installieren können.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Für die direkte Installation verfügbare Kenntnisse

Adobe Workfront bietet einige Fähigkeiten, die Sie direkt in Ihr LLM installieren können. Die Fähigkeiten zeigen, wie diese Tools für bestimmte Aufgaben verwendet werden, wobei die richtigen Schritte bereits integriert sind.

Diese Kenntnisse finden Sie als Dateien im Adobe Skills GitHub-Repository. Dieses Repository enthält Dateien für eine Vielzahl von Adobe-Produkten. Wenn Sie diese Dateien herunterladen und in Claude kopieren, kann Claude dann die in den Dateien beschriebenen Fähigkeiten verwenden.

Beispielsweise ermöglicht es die Fähigkeiten des Planning Solution Architect Claude, Fragen zu zu zu beantworten und einige Aktionen in Workfront Planning durchzuführen.

Sie müssen diese Kenntnisse nicht aufrufen oder Trigger machen, nachdem sie in das LLM kopiert wurden. Stattdessen können Sie wie gewohnt mit Ihrem LLM interagieren und Fragen in natürlicher Sprache stellen, und der LLM verwendet die Informationen und Aktionen, die in der Fähigkeit beschrieben sind, die für das Gespräch angemessen sind.

>[!NOTE]
>
>Derzeit sind diese Fähigkeiten nur für Claude verfügbar.
>Anweisungen zum Einrichten von Claude mit Adobe finden Sie unter [Erste Schritte](https://developer.adobe.com/adobe-for-creativity/getting-started/) in der Dokumentation zu Adobe Developer.

## Installieren einer Kenntnisse aus dem Workfront GitHub-Repository in Claude

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
