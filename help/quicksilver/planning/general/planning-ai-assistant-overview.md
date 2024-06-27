---
title: "Übersicht über den Adobe Workfront Planning AI Assistant"
description: Sie können den KI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der aktuellen Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen. Die Befehle des Benutzers und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass von der KI vorgenommene Änderungen in Ihrer Umgebung korrekt widergespiegelt werden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---


# Übersicht über den Adobe Workfront Planning AI Assistant

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf die Adobe Workfront-Planung und den AI-Assistenten, bei denen es sich um neue Angebote von Adobe Workfront handelt.
>
>Workfront Planning und der AI Assistant befinden sich derzeit in einer frühen Zugriffsphase, die nur einer begrenzten Anzahl von Kunden zugänglich ist.
>
>Sie müssen Workfront-Kunde sein, um diese Funktionen nutzen zu können.
>
>Ihr Kundenbetreuer wird Sie darüber informieren, ob Sie Teil dieser Phase sind.
>
>Weitere Informationen finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md).

Sie können den KI-Assistenten verwenden, um Datensätze basierend auf dem aktuellen Seitenkontext und der aktuellen Datensatzstruktur zu generieren, zu aktualisieren oder zu entfernen.

Die Befehle des Benutzers und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass von der KI vorgenommene Änderungen in Ihrer Umgebung korrekt widergespiegelt werden.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent ist standardmäßig für Workfront-Administratoren verfügbar.

* Der Workfront-Administrator muss den KI-Assistenten für alle anderen Benutzer aktivieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des AI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der KI-Assistent arbeitet im Kontext jeder Seite. Die Anfragen, die Sie für den AI-Assistenten senden, müssen auf Funktionen verweisen, die auf der geöffneten Seite verfügbar sind.

* Die vom AI-Assistenten durchgeführten Aktionen beziehen sich auf Ihre Workfront Planning-Berechtigungen und Ihre Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die vom AI-Assistenten im Namen des Benutzers vorgenommen werden, werden im Verlaufsfenster des Datensatzes verfolgt.

* Sie können Befehle verwenden, um Ihre Aktionen rückgängig zu machen.

## Derzeit für den AI-Assistenten verfügbare Funktionen

Derzeit ist der AI-Assistent im Planungsbereich von Workfront für die folgenden Seiten verfügbar:

* Seite mit Datentyp
* Seite aufzeichnen

Sie können den AI-Assistenten verwenden, um zu diesem Zeitpunkt die folgenden Aktionen durchzuführen:

* Erstellen Sie Datensätze. Eine ID mit einem Link zum neuen Datensatz wird nach der Erstellung des Datensatzes angezeigt.
* Erstellen Sie Datensätze anhand eines hochgeladenen Dokuments. Workfront unterstützt die folgenden Dokumentenformate für den AI-Assistenten:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt und die meisten Bildformate
* Aktualisieren Sie die Felder für die Datensätze, die auf dem Bildschirm angezeigt werden
* Datensätze löschen
* Wiederherstellen von gerade gelöschten Datensätzen

## Zugriff auf den KI-Assistenten

1. Melden Sie sich bei Workfront an und wechseln Sie dann zum **Planung** Bereich.

1. Klicken Sie auf **Arbeitsfläche** > **Record Type Card**.

1. (Optional) Klicken Sie auf eine **record** , um den Datensatz zu öffnen **Details** Seite.

1. Klicken Sie auf **Symbol &quot;KI-Assistent&quot;** in der oberen rechten Ecke des Bildschirms in der globalen Navigationsleiste.

   ![](assets/ai-assistant-icon-highlighted.png)

1. Geben Sie in der vorgesehenen Platzierung Befehle für den AI-Assistenten ein und klicken Sie auf die Eingabetaste , wenn Sie fertig sind.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Sie können beispielsweise eine der folgenden eingeben:

   * Datensatz erstellen
   * Aktualisieren Sie das Feld Beschreibung des Datensatzes der Sommerkampagne mit dem noch festzulegenden Datum.
   * Letzten Datensatz löschen
   * Datensatz wiederherstellen

   Ein visueller Indikator wird angezeigt, während der AI-Assistent Befehle verarbeitet und Erwartungen für die Reaktionszeit festlegt.

   Nachdem Sie eine erfolgreiche Antwort erhalten haben, folgen Sie den angegebenen Links oder beachten Sie die Änderungen auf der linken Seite.
