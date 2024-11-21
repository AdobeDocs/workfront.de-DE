---
title: Übersicht über den Adobe Workfront Planning AI Assistant - Überblick
description: Sie können den KI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der aktuellen Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen. Die Befehle des Benutzers und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass von der KI vorgenommene Änderungen in Ihrer Umgebung korrekt widergespiegelt werden.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 170edee352f1219986057dbb7d77228f84d855b1
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# Übersicht über den Adobe Workfront Planning AI Assistant

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 
-->

{{planning-important-intro}}

Sie können den AI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der aktuellen Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen.

Die Befehle des Benutzers und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass von der KI vorgenommene Änderungen in Ihrer Umgebung korrekt widergespiegelt werden.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent muss für Ihre Organisation aktiviert werden, bevor er für Benutzer in Ihrem Unternehmen verfügbar ist. Weitere Informationen finden Sie unter [AI Assistant Overview](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Nachdem Workfront den KI-Assistenten für Ihr Unternehmen aktiviert hat, steht er dem Hauptadministrator von Workfront zur Verfügung. Weitere Informationen finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Der Workfront-Administrator muss den KI-Assistenten für alle anderen Benutzer aktivieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des AI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der KI-Assistent arbeitet im Kontext jeder Seite. Die Anfragen, die Sie für den AI-Assistenten senden, müssen auf Funktionen verweisen, die auf der geöffneten Seite verfügbar sind.

* Die vom AI-Assistenten im Planungsbereich durchgeführten Aktionen beziehen sich auf Ihre Workfront Planning-Berechtigungen und Ihre Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die vom AI-Assistenten im Namen des Benutzers vorgenommen werden, werden im Verlaufsfenster des Datensatzes verfolgt.

* Sie können Befehle verwenden, um Ihre Aktionen rückgängig zu machen. Sie können beispielsweise &quot;Letzte Änderung rückgängig machen&quot;eingeben, um Ihre Änderung wiederherzustellen.

## Derzeit für den AI-Assistenten verfügbare Funktionen

Derzeit ist der AI-Assistent im Planungsbereich von Workfront für die folgenden Seiten verfügbar:

* Workspace-Seite
* Seite mit Datentyp
* Seite aufzeichnen

Sie können den AI-Assistenten verwenden, um zu diesem Zeitpunkt die folgenden Aktionen durchzuführen:

* Suchen Sie nach Datensätzen. Sie können nach Informationen in beliebigen Datensatzfeldern suchen.
* Erstellen Sie Datensätze. Eine ID mit einem Link zum neuen Datensatz wird nach der Erstellung des Datensatzes angezeigt. Sie können die Felder angeben, die Sie während des Erstellungsprozesses aktualisieren möchten, z. B. Datumsangaben oder Beschreibungen.
* Erstellen Sie Datensätze anhand eines hochgeladenen Dokuments. Workfront unterstützt die folgenden Dokumentenformate für den AI-Assistenten:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt und die meisten Bildformate
* Aktualisieren Sie die Felder für die Datensätze, die auf dem Bildschirm angezeigt werden
* Datensätze löschen
* Wiederherstellen von gerade gelöschten Datensätzen


<!-- ## Locate the AI Assistant in Workfront Planning

You can locate the AI Assistant in the following areas of Workfront Planning:

* The main navigation bar, in the upper-right corner of the screen.
* Inside the details area of a record, after you opened the record in the preview or after you opened the record's page. 

-->

## Zugriff auf die KI-Assistenzkraft im Planungsbereich

1. Melden Sie sich bei Workfront an und klicken Sie dann oben rechts im Bildschirm auf das Symbol **Hauptmenü** ![](assets/dots-main-menu.png) oder, falls verfügbar, auf das Symbol **Hauptmenü** ![](assets/lines-main-menu.png) oben links.

. Klicken Sie auf **Planung**. Der Planungsbereich wird geöffnet.

1. Klicken Sie auf eine **Workspace-Karte**.

1. (Optional) Klicken Sie auf eine Karte vom Typ **record type**.

1. (Optional) Klicken Sie auf einen **Datensatz** , um die Seite **Details** des Datensatzes zu öffnen.

1. Klicken Sie in der oberen rechten Ecke des Bildschirms in der globalen Navigationsleiste auf das Symbol **AI-Assistent** .<!--or in the upper-right corner of the record's preview or page.-->

   ![](assets/ai-assistant-icon-highlighted.png)

1. Geben Sie in der vorgesehenen Platzierung Befehle für den AI-Assistenten ein und klicken Sie auf die Eingabetaste , wenn Sie fertig sind.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Sie können beispielsweise eine der folgenden eingeben:

   * Erstellen Sie eine Kampagne mit dem Startdatum 4. Juli und dem Enddatum 30. Juli.
   * Aktualisieren Sie das Feld Beschreibung des Datensatzes der Sommerkampagne mit dem noch festzulegenden Datum.
   * Letzten Datensatz löschen
   * Datensatz wiederherstellen

   Ein visueller Indikator wird angezeigt, während der AI-Assistent Befehle verarbeitet und Erwartungen für die Reaktionszeit festlegt.

   Nachdem Sie eine erfolgreiche Antwort erhalten haben, folgen Sie den angegebenen Links oder beachten Sie die Änderungen auf der linken Seite.



