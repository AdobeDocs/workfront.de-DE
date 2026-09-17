---
title: Adobe Workfront-Planung - CX Coworker - Übersicht
description: Sie können die CX Coworker in Workfront Planning verwenden, um ähnliche Aktionen wie Datensätze und andere Objekte in Planning auszuführen, die Sie normalerweise in der Benutzeroberfläche ausführen würden. Die Benutzerbefehle und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass die von der KI vorgenommenen Änderungen genau in Ihrer Umgebung widergespiegelt werden.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: d5f36e0c8dbd9749503de25b75e70bf18b1d187b
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 5%
---

# Übersicht über Adobe Workfront Planning CX Coworker


<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Die CX Coworker ist eine Gesprächsoberfläche, auf der Sie ein Ziel in einfacher Sprache beschreiben und dann die Arbeit in Ihrer Adobe und den verbundenen Systemen plant, ausführt und validiert, bevor Sie sie zur Genehmigung zurückbringen.

Der CX Coworker behält alles bei, was der KI-Assistent heute tut, und fügt gleichzeitig leistungsfähigere End-to-End-Funktionen hinzu, sowohl in einem neuen Vollbilderlebnis als auch in der rechten Leiste von Workfront.

Sie wird innerhalb der bestehenden Zugriffssteuerungen auf Produktebene Ihres Unternehmens ausgeführt, sodass Benutzende nur Aktionen ausführen können, zu denen sie bereits in Workfront berechtigt sind. Der schreibgeschützte Zugriff wird dabei standardmäßig von Workfront-Admins gesteuert.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Beliebige Workfront oder Workflows mit einem Planungspaket</p>
ODER
<p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td>  
   <p>Ihr Administrator muss Folgendes tun, um in Planning den Zugriff auf die CX Coworker zuzulassen:</p>
   <ul>
   <li><p>Fügen Sie Ihrer Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzu, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p></li>
   <li><p>Deaktivieren Sie die Option CX Coworker-Bedienfeld in Workfront deaktivieren in Ihrer Zugriffsebene. Er ist standardmäßig ausgewählt.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Systemeinstellungen</p></td> 
   <td>   <p>Ihr Workfront-Administrator muss die schreibgeschützten und schreibgeschützten MCP-Tools im Bereich „Systemeinstellungen“ des Setups auswählen. Die schreibgeschützten MCP-Tools sind standardmäßig ausgewählt.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Überlegungen zum CX Coworker

* Die CX Coworker muss für Ihr Unternehmen aktiviert sein, damit sie für Benutzende in Ihrem Unternehmen verfügbar ist.

  Weitere Informationen finden Sie unter [Übersicht über CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Nachdem Workfront den Agenten für Ihr Unternehmen aktiviert hat, ist er für den Workfront-Hauptadministrator verfügbar. Weitere Informationen finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Der Workfront-Administrator muss den KI-Assistenten für alle anderen Benutzer aktivieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der KI-Assistent arbeitet im Kontext jeder Seite. Die Anfragen, die Sie für den KI-Assistenten senden, müssen auf Funktionen verweisen, die auf der geöffneten Seite verfügbar sind.

* Die vom KI-Assistenten im Bereich Planung durchgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

  * [Überblick über das Freigeben von Berechtigungen in Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Überblick über die Lizenztypen bei Verwendung von Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die der KI-Assistent im Auftrag des Benutzers vornimmt, werden im Verlaufsfenster des Datensatzes erfasst.

* Die vom KI-Assistenten durchgeführten Aktionen sind dauerhaft und könnten unumkehrbar sein. Das Löschen eines Felds kann beispielsweise nicht rückgängig gemacht werden. Überprüfen Sie alle vom KI-Assistenten vorgeschlagenen Aktionen, bevor Sie sie akzeptieren.

* Beim Erstellen, Aktualisieren oder Löschen eines Objekts über den KI-Assistenten zeigt der KI-Assistent die beabsichtigten Aktionen an und bittet um Bestätigung. Anschließend können Sie die Aktionen bestätigen oder abbrechen.

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
* Löschen von Einträgen
* Wiederherstellen von soeben gelöschten Datensätzen


## Suchen des KI-Assistenten in Workfront Planning

Der KI-Assistent befindet sich in den folgenden Bereichen von Workfront Planning:

* Die Hauptnavigationsleiste in der oberen rechten Ecke des Bildschirms.
* Innerhalb des Detailbereichs eines Datensatzes, nachdem Sie den Datensatz in der Vorschau geöffnet oder nachdem Sie die Datensatzseite geöffnet haben.

## Zugriff auf den KI-Assistenten im Bereich Planung

1. Melden Sie sich bei Workfront an und klicken Sie dann oben links auf ****-Symbol ![Hauptmenü „Zeilen](assets/lines-main-menu.png) und dann auf **Planung**.

   Der Bereich Planung wird geöffnet.

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



