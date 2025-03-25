---
title: Adobe Workfront Planning AI Assistant - Übersicht
description: Sie können den KI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen. Die Benutzerbefehle und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass die von der KI vorgenommenen Änderungen genau in Ihrer Umgebung widergespiegelt werden.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant - Überblick

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Sie können den KI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen.

Die Benutzerbefehle und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass die von der KI vorgenommenen Änderungen genau in Ihrer Umgebung widergespiegelt werden.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent muss für Ihre Organisation aktiviert sein, damit er für Benutzende in Ihrer Firma verfügbar ist. Weitere Informationen finden Sie unter [Übersicht über den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Nachdem Workfront den KI-Assistenten für Ihr Unternehmen aktiviert hat, ist er für den Workfront-Hauptadministrator verfügbar. Weitere Informationen finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Der Workfront-Administrator muss den KI-Assistenten für alle anderen Benutzer aktivieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der KI-Assistent arbeitet im Kontext jeder Seite. Die Anfragen, die Sie für den KI-Assistenten senden, müssen auf Funktionen verweisen, die auf der geöffneten Seite verfügbar sind.

* Die vom KI-Assistenten im Bereich Planung durchgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die der KI-Assistent im Auftrag des Benutzers vornimmt, werden im Verlaufsfenster des Datensatzes erfasst.

* Sie können Befehle verwenden, um Ihre Aktionen rückgängig zu machen. Sie können beispielsweise „Letzte Änderung rückgängig machen“ eingeben, um Ihre Änderung rückgängig zu machen.

* <span class="preview"> Beim Erstellen, Aktualisieren oder Löschen eines Objekts über den KI-Assistenten zeigt der KI-Assistent die beabsichtigten Aktionen an und bittet um Bestätigung. Anschließend können Sie die Aktionen bestätigen oder abbrechen. </span>

## Derzeit für den KI-Assistenten verfügbare Funktionen

Derzeit ist der KI-Assistent im Planungsbereich von Workfront für die folgenden Seiten verfügbar:

* Workspace-Seite
* Seite des Datensatztyps
* Seite aufzeichnen

Sie können den KI-Assistenten verwenden, um zu diesem Zeitpunkt die folgenden Aktionen auszuführen:

* Nach Datensätzen suchen. Sie können nach Informationen suchen, die in beliebigen Datensatzfeldern enthalten sind.
* Einträge erstellen. Eine ID mit einem Link zum neuen Datensatz wird angezeigt, nachdem der Datensatz erstellt wurde. Sie können die Felder angeben, die Sie während des Erstellungsprozesses aktualisieren möchten, z. B. Datum oder Beschreibung.
* Erstellen Sie Datensätze basierend auf einem Dokument, das Sie hochladen. Workfront unterstützt die folgenden Dokumentformate für den KI-Assistenten:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT und die meisten Bildformate
* Aktualisieren Sie die Felder für die Datensätze, die Sie auf dem Bildschirm sehen
* Löschen von Datensätzen
* Wiederherstellen von soeben gelöschten Datensätzen


## Suchen des KI-Assistenten in Workfront Planning

Der KI-Assistent befindet sich in den folgenden Bereichen von Workfront Planning:

* Die Hauptnavigationsleiste in der oberen rechten Ecke des Bildschirms.
* Innerhalb des Detailbereichs eines Datensatzes, nachdem Sie den Datensatz in der Vorschau geöffnet oder nachdem Sie die Datensatzseite geöffnet haben.

## Zugriff auf den KI-Assistenten im Bereich Planung

1. Melden Sie sich bei Workfront an und klicken Sie dann auf **Hauptmenü** Symbol ![Punkte-](assets/dots-main-menu.png)) in der rechten oberen Ecke des Bildschirms oder auf das Symbol **Hauptmenü** ![Zeilen-Hauptmenü](assets/lines-main-menu.png) in der linken oberen Ecke, falls verfügbar.

. Klicken Sie **Planung**. Der Bereich Planung wird geöffnet.

1. Klicken Sie auf eine **Arbeitsbereichskarte**.

1. (Optional) Klicken Sie auf eine **Karte vom Typ „Datensatz**.

1. (Optional) Klicken Sie auf **Datensatz**, um die Seite **Details** des Datensatzes zu öffnen.

1. Klicken Sie auf **KI** Assistentensymbol) in der oberen rechten Ecke des Bildschirms in der globalen Navigationsleiste oder in der oberen rechten Ecke der Vorschau oder Seite des Datensatzes.

   ![KI-Assistenten-Symbol](assets/ai-assistant-icon-highlighted.png)

1. Beginnen Sie in dem dafür vorgesehenen Feld mit der Eingabe von Befehlen für den KI-Assistenten und klicken Sie abschließend auf die Eingabetaste .

   ![AI Assistant Panel mit leerem Befehlsfeld](assets/ai-assistant-panel-with-empty-command-box.png)

   Sie können beispielsweise einen der folgenden Typen eingeben:

   * Erstellen Sie eine Kampagne mit dem Startdatum 4. Juli und dem Enddatum 30. Juli
   * Aktualisieren Sie das Feld Beschreibung des Sommerkampagnendatensatzes mit dem zu bestimmenden Datum
   * Letzten Eintrag löschen
   * Datensatz wiederherstellen

   Während der Verarbeitung von Befehlen durch den KI-Assistenten wird ein visueller Indikator angezeigt, der Erwartungen für die Antwortzeit festlegt.

   Folgen Sie nach Erhalt einer erfolgreichen Antwort den angegebenen Links oder beachten Sie die Änderungen auf der linken Seite.



