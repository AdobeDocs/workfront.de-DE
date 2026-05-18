---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Konfigurieren des Adobe Workfront MCP-Servers
description: Konfigurieren Sie Ihre Workfront-Instanz und Ihren KI-Assistenten, damit Sie über Konversationen in natürlicher Sprache mit Workfront arbeiten können.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 5%

---


# Konfigurieren des Adobe Workfront MCP-Servers

Mit dem [!DNL Adobe Workfront] MCP-Server können Sie mit Ihren Workfront-Daten durch Gespräche in natürlicher Sprache in einem unterstützten KI-Assistenten wie Claude oder ChatGPT arbeiten.

Bevor Sie einen KI-Assistenten mit Workfront verbinden können, muss ein Workfront-Administrator den MCP-Serverzugriff in Ihrer Workfront-Instanz aktivieren. Die genauen Schritte zum Verbinden eines KI-Assistenten sind für jeden unterstützten KI-Assistenten unterschiedlich.

Weitere Informationen zum Workfront MCP-Server finden Sie unter [Übersicht über den Adobe Workfront MCP-Server](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Unterstützte KI-Assistenten

Der Workfront MCP-Server unterstützt derzeit die folgenden KI-Assistenten:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Bevor Sie Workfront mit einem KI-Assistenten verbinden können, müssen Sie:

* Sie verfügen über ein aktives [!DNL Adobe Workfront]-Konto mit der Berechtigung zum Zugriff auf die Daten, mit denen Sie arbeiten möchten.
* Zugriff auf einen KI-Assistenten wie [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Voraussetzungen für Admin

Der Zugriff auf MCP-Server wird von zwei separaten Administratoren gesteuert. Beide müssen den Zugriff aktivieren, bevor Sie eine Verbindung herstellen können.

* **Ihr Workfront-Administrator** muss den MCP-Serverzugriff in Ihrer Workfront-Instanz aktivieren.

* Wenn Sie eine Unternehmensversion eines KI-Assistenten verwenden, muss die Administratorin bzw. der Administrator des KI-Assistenten den [!DNL Adobe Workfront]-Connector für Ihr Unternehmen aktivieren.


## Workfront mit Claude verbinden

Sie stellen eine Verbindung zu Workfront einmal pro [!DNL Claude] her. Die Verbindung authentifiziert Sie für eine bestimmte Workfront-Instanz, und Sie bleiben in Verbindung, bis Sie die Verbindung trennen.


>[!IMPORTANT]
>
>Wenn Sie [!DNL Claude] Enterprise verwenden, **Ihr [!DNL Claude] Enterprise-**) den [!DNL Adobe Workfront]-Connector für Ihr Unternehmen aktivieren. Bis dahin wird der [!DNL Adobe Workfront]-Connector nicht angezeigt, wenn Sie in [!DNL Claude] danach suchen. Wenden Sie sich zuerst an Ihren [!DNL Claude].


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

### Verbindung überprüfen

Um zu bestätigen, [!DNL Claude] mit Workfront verbunden ist, bitten Sie [!DNL Claude], die Aktionen aufzulisten, die der Workfront MCP-Server zur Verfügung stellt. Beispiel:

* *Welche Workfront-Aktionen können Sie durchführen?*
* *Listen Sie die Workfront-Tools auf, auf die Sie Zugriff haben.*

[!DNL Claude] gibt die Liste der verfügbaren Aktionen zurück.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Zu einer anderen Workfront-Instanz wechseln

Jede Verbindung authentifiziert sich [!DNL Claude] einer einzelnen Workfront-Instanz. Um eine andere Instanz zu verwenden, trennen Sie die Verbindung und stellen Sie erneut eine Verbindung her.

So stellen Sie eine Verbindung zu einer anderen Workfront-Instanz her:

1. Trennen Sie [!DNL Claude] den [!DNL Adobe Workfront].
1. Schließen Sie den Connector wieder an.
1. Authentifizierung bei der neuen Workfront-Instanz.

>[!NOTE]
>
>Durch die Abmeldung von [!DNL Claude] allein wird die Workfront-Instanz nicht gewechselt. Sie müssen den Stecker trennen und erneut anschließen.

## Claude-Verhalten mit Fähigkeiten anpassen

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] unterstützt benutzerdefinierte Befehlssätze, die als „Skills“ bezeichnet werden. Sie können eine Kenntnis verwenden, um anzupassen, wie [!DNL Claude] sich bei Workfront verhält. Sie können beispielsweise eine Fähigkeit erstellen, die [!DNL Claude] anweist, immer neue Daten aus Workfront abzurufen, anstatt sich auf frühere Ergebnisse zu verlassen.

## Fehlerbehebung bei Setup und Authentifizierung

| Problem | Wahrscheinliche Ursache | Korrigieren |
|---|---|---|
| Der [!DNL Adobe Workfront]-Connector wurde nicht in [!DNL Claude] gefunden. | Ihr [!DNL Claude] hat sie nicht aktiviert. | Wenden Sie sich an Ihren [!DNL Claude]-Administrator (nicht an Ihren Workfront-Administrator) und bitten Sie ihn, den [!DNL Adobe Workfront] Connector zu aktivieren. |
| Sie haben verbunden, aber Sie können Ihre Daten nicht sehen. | Sie haben sich bei der falschen Workfront-Instanz authentifiziert. | Trennen Sie den Connector, stellen Sie erneut eine Verbindung her, und authentifizieren Sie sich bei der richtigen Instanz. |
| Die Authentifizierung ist fehlgeschlagen, oder die Verbindung funktioniert nicht mehr. | Ihre Authentifizierungssitzung ist abgelaufen oder es liegt ein Verbindungsfehler vor. | Den Stecker abziehen und wieder anschließen. |
| Sie möchten zu einer anderen Workfront-Instanz wechseln. | Eine einzige Verbindung verbindet Sie mit einer Instanz. | Trennen Sie die Verbindung zur neuen Instanz und stellen Sie erneut eine Verbindung her, und authentifizieren Sie sich für sie. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Eine tägliche Fehlerbehebung nach der Verbindung (z. B. veraltete Ergebnisse oder unerwartetes Verhalten) finden Sie unter [Verwenden des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

## Häufig gestellte Fragen zum Setup

### Kann ich gleichzeitig eine Verbindung zu mehreren Workfront-Instanzen herstellen?

Nein. Jede Verbindung verknüpft einen KI-Assistenten mit einer einzelnen Workfront-Instanz. Um zu wechseln, die Verbindung zu trennen und erneut herzustellen, authentifizieren Sie sich bei der neuen Instanz.

### Funktioniert das mit Claude Pro oder Claude Team oder nur Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Welcher Administrator aktiviert dies?

Sowohl Ihr Workfront-Administrator als auch Ihr KI-Assistentenadministrator. Ihr Workfront-Administrator aktiviert den MCP-Serverzugriff auf der Workfront-Seite. Der Administrator Ihres KI-Assistenten aktiviert den Workfront-Zugriff auf der Seite des KI-Assistenten. Der [!DNL Claude] Enterprise-Administrator aktiviert [!DNL Claude] den [!DNL Adobe Workfront]-Connector.
