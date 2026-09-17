---
title: Adobe Workfront-Planung - CX Coworker - Übersicht
description: Sie können die CX Coworker in Workfront Planning verwenden, um ähnliche Aktionen wie Datensätze und andere Objekte in Planning auszuführen, die Sie normalerweise in der Benutzeroberfläche ausführen würden. Die Benutzerbefehle und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass die von der KI vorgenommenen Änderungen genau in Ihrer Umgebung widergespiegelt werden.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 3%
---

# Übersicht über Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Die CX Coworker ist eine Gesprächsoberfläche, auf der Sie ein Ziel in einfacher Sprache beschreiben. Anschließend plant, führt und validiert sie die Arbeit in Ihrem Workfront Planning- und anderen verbundenen Adobe-Systemen, bevor sie zur Genehmigung zurückgebracht wird.

Der CX Coworker behält alles bei, was der KI-Assistent heute tut, und fügt gleichzeitig leistungsfähigere End-to-End-Funktionen hinzu, sowohl in einem neuen Vollbilderlebnis als auch in der rechten Leiste von Workfront.

Sie wird innerhalb der bestehenden Zugriffssteuerungen auf Produktebene Ihres Unternehmens ausgeführt, sodass Benutzende nur Aktionen ausführen können, zu denen sie bereits in Workfront berechtigt sind. Der schreibgeschützte Zugriff wird dabei standardmäßig von Workfront-Admins gesteuert.

>[!IMPORTANT]
>
>CX Coworker steht derzeit Organisationen im Gesundheitswesen, im Finanzwesen oder in einigen anderen Branchen mit sensiblen Daten nicht zur Verfügung. KI-Assistent steht diesen Organisationen zur Verfügung.
>
>Weitere Informationen finden Sie unter [Übersicht über den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


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

* Nachdem Workfront den Agenten für Ihre Workfront-Instanz aktiviert hat, ist er für den Workfront-Hauptadministrator verfügbar und er kann ihn für Ihr Unternehmen aktivieren. Weitere Informationen finden Sie [Konfigurieren von Systemvoreinstellungen](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Der Workfront-Administrator muss für Sie auch CX Coworker in Ihrer Zugriffsebene aktivieren. Weitere Informationen finden Sie [Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Die CX Coworker arbeitet mit Informationen und Objekten, die sich in Workfront oder Workfront Planning befinden und für die Sie über Zugriffsberechtigungen verfügen. In der rechten Leiste „Planung“ kann das Bedienfeld „Mitarbeiter“ im Kontext des Arbeitsbereichs, des Datensatztyps oder der Datensatzseite, den bzw. die Sie geöffnet haben, verwendet werden.

* Die von CX Coworker im Bereich Planung durchgeführten Aktionen stehen im Zusammenhang mit Ihren Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

  * [Überblick über das Freigeben von Berechtigungen in Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Überblick über die Lizenztypen bei Verwendung von Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die von der CX Coworker im Auftrag des Benutzers vorgenommen werden, werden im Bedienfeld Verlauf des Datensatzes nachverfolgt.

* Die von der CX Coworker ergriffenen Maßnahmen sind dauerhaft und könnten unumkehrbar sein. Das Löschen eines Felds kann beispielsweise nicht rückgängig gemacht werden. Überprüfen Sie alle von CX Coworker vorgeschlagenen Aktionen, bevor Sie sie akzeptieren.

* Beim Erstellen, Aktualisieren oder Löschen eines Objekts über die CX Coworker zeigt die CX Coworker die beabsichtigten Aktionen an und bittet um Bestätigung. Anschließend können Sie die Aktionen bestätigen oder abbrechen.

## Derzeit für CX Coworker verfügbare Funktionen

Derzeit ist die CX Coworker im Planungsbereich von Workfront verfügbar und nutzt verschiedene Fähigkeiten, um auf Informationen für Planning-Objekte zuzugreifen und sie zu bearbeiten. Weitere Informationen finden Sie unter [CX Coworker-Kenntnisse](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Mit der CX Coworker können Sie die folgenden Aktionen durchführen:

* Nach Datensätzen suchen. Sie können nach Informationen suchen, die in beliebigen Datensatzfeldern enthalten sind.
* Einträge erstellen. Eine ID mit einem Link zum neuen Datensatz wird angezeigt, nachdem der Datensatz erstellt wurde. Sie können die Felder angeben, die Sie während des Erstellungsprozesses aktualisieren möchten, z. B. Datum oder Beschreibung.
* Erstellen Sie Datensätze basierend auf einem Dokument, das Sie hochladen. Workfront unterstützt die folgenden Dokumentenformate für CX Coworker:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT und die meisten Bildformate
* Aktualisieren Sie die Felder für die Datensätze, die Sie auf dem Bildschirm sehen
* Löschen, Duplizieren oder Wiederherstellen von Datensätzen
* Datensätze mit anderen Datensätzen verknüpfen
* Anzeigen des Änderungsverlaufs eines Datensatzes


## Suchen der CX Coworker in Workfront Planning

Sie finden die CX Coworker in den folgenden Bereichen von Workfront Planning:

* Die Hauptnavigationsleiste in der oberen rechten Ecke des Bildschirms.
* Innerhalb des Detailbereichs eines Datensatzes, wenn Sie ihn in einer neuen Registerkarte öffnen.

## Zugriff auf die CX Coworker im Planungsbereich


1. Melden Sie sich bei Workfront an und klicken Sie dann oben links auf ****-Symbol ![Hauptmenü „Zeilen](assets/lines-main-menu.png) und dann auf **Planung**.

   Der Bereich Planung wird geöffnet.

   Suchen Sie das **KI** Symbol ![KI](assets/ai-icon.png)Symbol oben rechts auf der Seite oder fahren Sie mit den folgenden Schritten fort.

1. Klicken Sie auf eine **Arbeitsbereichskarte**.

1. Klicken Sie auf **Karte vom Typ Datensatz**.

1. Klicken Sie auf **Datensatz**, um die Seite **Details** des Datensatzes zu öffnen, und klicken Sie dann auf In öffnen .

1. Klicken Sie oben rechts **Bildschirm auf das Symbol** CX Coworker .

1. Beginnen Sie im vorgesehenen Feld mit der Eingabe von Befehlen für die CX Coworker und klicken Sie abschließend auf die Eingabetaste .

   ![CX Coworker-Bedienfeld mit leerem Befehlsfeld](assets/cx-coworker-right-rail.png)

   Sie können beispielsweise einen der folgenden Typen eingeben:

   * Erstellen Sie einen neuen Kampagnendatensatz mit dem Namen Summer Sale 2026
   * Aktualisieren Sie das Budgetfeld im Sommerkampagnendatensatz auf 75.000 $
   * Löschen Sie den Kampagnendatensatz mit dem Namen „Alte Promotion“.
   * Die versehentlich gelöschte Kampagne wiederherstellen

   >[!TIP]
   >
   >Stellen Sie sicher, dass der Workfront-Administrator die schreibgeschützten MCP-Tools in den Systemeinstellungen aktiviert hat, bevor Sie den CX Coworker auffordern, Bearbeitungsaktionen für Objekte durchzuführen.

   Während die CX Coworker -Befehle verarbeitet, wird ein visueller Indikator angezeigt, der die Erwartungen für die Antwortzeit festlegt.

   Folgen Sie nach Erhalt einer erfolgreichen Antwort den angegebenen Links oder beachten Sie die Änderungen auf der linken Seite.


1. (Optional) Klicken Sie auf das **Vollbildsymbol erweitern**-Symbol ![Vollbildsymbol erweitern](assets/expand-full-screen-icon.png), um das Chat-Feld „Mitarbeiter“ in einer Browser-Registerkarte im Vollbildmodus zu öffnen.


