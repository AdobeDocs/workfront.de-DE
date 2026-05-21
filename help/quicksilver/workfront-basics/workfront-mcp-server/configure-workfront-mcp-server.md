---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Konfigurieren des Adobe Workfront MCP-Servers
description: Konfigurieren Sie Ihre Workfront-Instanz und Ihre KI-Agentenplattform, damit Sie über Konversationen in natürlicher Sprache mit Workfront arbeiten können.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Konfigurieren des Adobe Workfront MCP-Servers

Mit dem [!DNL Adobe Workfront] MCP-Server können Sie mit Ihren Workfront-Daten durch Gespräche in natürlicher Sprache auf einer unterstützten KI-Agentenplattform wie Claude oder ChatGPT arbeiten.

Bevor Sie eine KI-Agentenplattform mit Workfront verbinden können, muss ein Workfront-Administrator den MCP-Serverzugriff in Ihrer Workfront-Instanz aktivieren. Die genauen Schritte zum Verbinden einer KI-Agent-Plattform unterscheiden sich für jede unterstützte KI-Agent-Plattform.

Weitere Informationen zum Workfront MCP-Server finden Sie unter [Übersicht über den Adobe Workfront MCP-Server](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Unterstützte KI-Agentenplattformen

Der Workfront MCP-Server unterstützt derzeit die folgenden KI-Agentenplattformen:

* [!DNL Claude]
* [!DNL ChatGPT]

## Voraussetzungen

Bevor Sie Workfront mit einer KI-Agentenplattform verbinden können, müssen Sie Folgendes tun:

* Sie verfügen über ein aktives [!DNL Adobe Workfront]-Konto mit der Berechtigung zum Zugriff auf die Daten, mit denen Sie arbeiten möchten.
* Zugriff auf eine KI-Agentenplattform wie [!DNL Claude] haben.

### Voraussetzungen für Admin

Der Zugriff auf MCP-Server wird von zwei separaten Administratoren gesteuert.

* **Ihr Workfront-Administrator** steuert den MCP-Serverzugriff für Ihre Workfront-Instanz. Der Zugriff ist in den Systemeinstellungen standardmäßig aktiviert. Daher ist keine Aktion erforderlich, es sei denn, der Administrator hat sie deaktiviert. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* Wenn Sie eine Unternehmensversion einer KI-Agentenplattform verwenden, muss der Administrator für diese Plattform den [!DNL Adobe Workfront]-Connector für Ihr Unternehmen aktivieren.


## Workfront mit Claude verbinden

Sie stellen eine Verbindung zu Workfront einmal pro [!DNL Claude] her. Die Verbindung authentifiziert Sie für eine bestimmte Workfront-Instanz, und Sie bleiben in Verbindung, bis Sie die Verbindung trennen.

### Verbinden über das Connector-Verzeichnis

+++ Erweitern Sie , um eine schrittweise Anleitung zum Verbinden von Workfront mit [!DNL Claude] anzuzeigen.

So verbinden Sie Workfront mit [!DNL Claude]:

1. Öffnen Sie [!DNL Claude].

1. Navigieren Sie zum Bereich Connectoren .

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Suchen Sie **[!DNL Adobe Workfront]** in der Connector-Liste.

   Falls Sie sie nicht sehen, lesen Sie [Admin-Voraussetzungen](#admin-prerequisites) in diesem Artikel.

1. Klicken Sie auf **Verbinden**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. Melden Sie sich bei Aufforderung bei Ihrer Workfront-Instanz an.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. Nach Abschluss der Authentifizierung besteht eine Verbindung.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Verbindung mit einer URL herstellen

+++ Erweitern Sie , um eine schrittweise Anleitung zum Verbinden von Workfront mit [!DNL Claude] mit einer URL zu erhalten.

So verbinden Sie Workfront mit [!DNL Claude] über eine URL:

1. Melden Sie sich mit Ihren [ bei ](https://claude.ai)Claude“ an.
1. Wählen Sie im linken Menü das Symbol **Anpassen** aus.
1. Wählen Sie **Connectoren** und klicken Sie dann auf das Symbol **+** , um einen Connector hinzuzufügen.
1. Klicken Sie auf **Schaltfläche „App**&quot;.
1. Geben Sie dem Connector einen gewünschten Namen (z. B. &quot;Workfront„) und die gewünschte MCP-Server-URL ein: `https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. Nachdem der Connector erstellt wurde, wird ein Anmeldefenster angezeigt. Authentifizieren Sie sich mit Ihren Adobe ID-Anmeldeinformationen. Stellen Sie sicher, dass Sie die gewünschte Workfront-Instanz auswählen, wenn Sie zu mehreren gehören.

+++

### Claude-Verhalten mit Fähigkeiten anpassen

[!DNL Claude] unterstützt benutzerdefinierte Befehlssätze, die als „Skills“ bezeichnet werden. Sie können eine Kenntnis verwenden, um anzupassen, wie [!DNL Claude] sich bei Workfront verhält. Sie können beispielsweise eine Fähigkeit erstellen, die [!DNL Claude] anweist, immer neue Daten aus Workfront abzurufen, anstatt sich auf frühere Ergebnisse zu verlassen.

Um mehr über [!DNL Claude] Fähigkeiten zu erfahren, lesen Sie die [Claude-Benutzerdokumentation](https://code.claude.com/docs/en/skills) oder bitten Sie Claude um Hilfe bei den Fähigkeiten.

## Mit ChatGPT verbinden

1. Melden Sie sich mit Ihren [ bei ](https://chatgpt.com)ChatGPT) an.
1. Wählen Sie unten links &quot;**&quot;** → **Einstellungen**.
1. Wählen Sie **Apps** aus und aktivieren Sie dann **Entwicklermodus**.
1. Klicken Sie auf **Schaltfläche „App**&quot;.
1. Geben Sie der App einen gewünschten Namen (z. B. &quot;Workfront„) und die gewünschte MCP-Server-URL ein: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Stellen Sie sicher, dass die Authentifizierung auf **OAuth** (standardmäßig festgelegt) eingestellt ist, und aktivieren Sie das Kontrollkästchen Akzeptanz , um fortzufahren.
1. Nachdem die App erstellt wurde, wird ein Anmeldefenster angezeigt. Authentifizieren Sie sich mit Ihren Adobe ID-Anmeldeinformationen. Stellen Sie sicher, dass Sie die gewünschte Workfront-Instanz auswählen, wenn Sie zu mehreren gehören.

### Anpassen des ChatGPT-Verhaltens mit benutzerdefinierten GPTs

ChatGPT unterstützt von Benutzern erstellte Assistenten, die als benutzerdefinierte GPTs bezeichnet werden. Sie können ein benutzerdefiniertes GPT verwenden, um anzupassen, wie sich ChatGPT mit Ihrem Connector verhält. Sie können beispielsweise ein benutzerdefiniertes GPT erstellen, das ChatGPT anweist, immer neue Daten von Ihrem verbundenen Service abzurufen, anstatt sich auf frühere Ergebnisse zu verlassen.

Weitere Informationen zu benutzerdefinierten GPTs finden Sie in der [ChatGPT-Benutzerdokumentation](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) oder wenden Sie sich an ChatGPT, um Hilfe zu benutzerdefinierten GPTs zu erhalten.

## Verbindung überprüfen

Um zu bestätigen, dass die KI-Agentenplattform mit Workfront verbunden ist, bitten Sie die KI-Agentenplattform, die Aktionen aufzulisten, die der Workfront-MCP-Server zur Verfügung stellt. Beispiel:

* *Welche Workfront-Aktionen können Sie durchführen?*
* *Listen Sie die Workfront-Tools auf, auf die Sie Zugriff haben.*

Sie können auch die vollständige Liste der Tools in [Adobe Workfront MCP Server Tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md) anzeigen.

## Verfügbare Tools

Der Workfront MCP-Server stellt eine Reihe von Tools bereit, die die verbundene KI-Agentenplattform in Ihrem Namen aufruft, z. B. Tools zum Durchsuchen von Workfront, Erstellen von Elementen, Aktualisieren von Feldern und Verwalten von Genehmigungen. Die vollständige Referenzliste, gruppiert nach Workfront-Bereich, finden Sie unter [Adobe Workfront MCP Server Tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Zu einer anderen Workfront-Instanz wechseln

Jede Verbindung authentifiziert die KI-Agent-Plattform für eine einzelne Workfront-Instanz. Um eine andere Instanz zu verwenden, trennen Sie die Verbindung und stellen Sie erneut eine Verbindung her.

So stellen Sie eine Verbindung zu einer anderen Workfront-Instanz her:

1. Trennen Sie in der KI-Agentenplattform den Workfront MCP-Server.
1. Schließen Sie den Connector wieder an.
1. Authentifizierung bei der neuen Workfront-Instanz.

>[!NOTE]
>
>Durch die Abmeldung allein wird die Workfront-Instanz nicht gewechselt. Sie müssen den Stecker trennen und erneut anschließen.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Fehlerbehebung bei Setup und Authentifizierung

+++ Erweitern Sie , um Tipps zur Fehlerbehebung bei der Einrichtung und Authentifizierung des Workfront MCP-Servers zu erhalten.

| Problem | Wahrscheinliche Ursache | Korrigieren |
|---|---|---|
| Der [!DNL Adobe Workfront]-Connector wurde nicht in [!DNL Claude] gefunden. | Ihr [!DNL Claude] hat sie nicht aktiviert. | Wenden Sie sich an Ihren [!DNL Claude]-Administrator (nicht an Ihren Workfront-Administrator) und bitten Sie ihn, den [!DNL Adobe Workfront] Connector zu aktivieren. |
| Sie haben verbunden, aber Sie können Ihre Daten nicht sehen. | Sie haben sich bei der falschen Workfront-Instanz authentifiziert. | Trennen Sie den Connector, stellen Sie erneut eine Verbindung her, und authentifizieren Sie sich bei der richtigen Instanz. |
| Die Authentifizierung ist fehlgeschlagen, oder die Verbindung funktioniert nicht mehr. | Ihre Authentifizierungssitzung ist abgelaufen oder es liegt ein Verbindungsfehler vor. | Den Stecker abziehen und wieder anschließen. |
| Sie möchten zu einer anderen Workfront-Instanz wechseln. | Eine einzige Verbindung verbindet Sie mit einer Instanz. | Trennen Sie die Verbindung zur neuen Instanz und stellen Sie erneut eine Verbindung her, und authentifizieren Sie sich für sie. |
| Sie können keine Verbindung zu Workfront herstellen, oder es wird eine Meldung angezeigt, dass der Zugriff auf den MCP-Server deaktiviert ist. | Ihr Workfront-Administrator hat den MCP-Serverzugriff für Ihre Instanz deaktiviert. | Wenden Sie sich an Ihren Workfront-Administrator und bitten Sie ihn, den MCP-Serverzugriff in den Systemeinstellungen zu aktivieren. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Eine tägliche Fehlerbehebung nach der Verbindung (z. B. veraltete Ergebnisse oder unerwartetes Verhalten) finden Sie unter [Verwenden des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->