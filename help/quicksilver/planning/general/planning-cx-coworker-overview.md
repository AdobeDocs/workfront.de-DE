---
title: Adobe Workfront-Planung - CX Coworker - Übersicht
description: Sie können CX Coworker in Workfront Planning verwenden, um ähnliche Aktionen wie Datensätze und andere Objekte in Planning auszuführen, die Sie normalerweise in der Benutzeroberfläche ausführen würden. Die Benutzerbefehle und die Ausführung dieser Befehle durch die KI arbeiten zusammen, um sicherzustellen, dass die von der KI vorgenommenen Änderungen genau in Ihrer Umgebung widergespiegelt werden.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 5a341c85166860ce88cbda7dff17efbadcafaddb
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 3%
---

# Übersicht über Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

CX Coworker ist eine Gesprächsoberfläche, auf der Sie ein Ziel in einfacher Sprache beschreiben und dann die Arbeit in Ihrer Workfront-Planung und anderen verbundenen Adobe-Systemen plant, ausführt und validiert, bevor Sie sie zur Genehmigung zurückbringen.

Coworker behält alles, was AI Assistant heute tut, und fügt leistungsfähigere End-to-End-Funktionen sowohl in einem neuen Vollbilderlebnis als auch in der rechten Leiste von Workfront hinzu.

Sie wird innerhalb der bestehenden Zugriffssteuerungen auf Produktebene Ihres Unternehmens ausgeführt, sodass Benutzende nur Aktionen ausführen können, zu denen sie bereits in Workfront berechtigt sind. Der schreibgeschützte Zugriff wird dabei standardmäßig von Workfront-Admins gesteuert.

>[!IMPORTANT]
>
>Coworker steht derzeit Organisationen im Gesundheitswesen, im Finanzwesen oder in einigen anderen Branchen mit sensiblen Daten nicht zur Verfügung. KI-Assistent steht diesen Organisationen zur Verfügung.
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
  <p>Ihr Administrator muss folgende Schritte ausführen, um den Zugriff auf Mitarbeiter in Planung zuzulassen:</p>
   <ul>
   <li><p>Fügen Sie Ihrer Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzu, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p></li>
  <li><p>Deaktivieren Sie in Ihrer Zugriffsebene die Option Bedienfeld für Kollegen in Workfront deaktivieren . Er ist standardmäßig ausgewählt.</p></li></ul>
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

## Überlegungen für Kollegen

* Worker müssen für Ihre Organisation aktiviert sein, damit sie für Benutzer in Ihrer Firma verfügbar ist.

  Weitere Informationen finden Sie unter [Übersicht über CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Nachdem Workfront den Agenten für Ihre Workfront-Instanz aktiviert hat, ist er für den Workfront-Hauptadministrator verfügbar und er kann ihn für Ihr Unternehmen aktivieren. Weitere Informationen finden Sie [Konfigurieren von Systemvoreinstellungen](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Die Workfront-Administratorin bzw. der-Administrator muss auch Coworker für Sie in Ihrer Zugriffsebene aktivieren. Weitere Informationen finden Sie [Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Ein Mitarbeiter arbeitet mit Informationen und Objekten, die sich in Workfront oder Workfront Planning befinden und für die Sie über Zugriffsberechtigungen verfügen. In der rechten Leiste „Planung“ kann das Bedienfeld „Mitarbeiter“ im Kontext des Arbeitsbereichs, des Datensatztyps oder der Datensatzseite, den bzw. die Sie geöffnet haben, verwendet werden.

* Die von einem Mitarbeiter im Bereich Planung durchgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

  * [Überblick über das Freigeben von Berechtigungen in Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Überblick über die Lizenztypen bei Verwendung von Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die von einem Mitarbeiter im Auftrag des Benutzers vorgenommen werden, werden im Verlaufsfenster des Datensatzes erfasst.

* Von Kollegen durchgeführte Aktionen sind dauerhaft und können irreversibel sein. Das Löschen eines Felds kann beispielsweise nicht rückgängig gemacht werden. Überprüfen Sie alle von einem Kollegen vorgeschlagenen Aktionen, bevor Sie sie akzeptieren.

* Beim Erstellen, Aktualisieren oder Löschen eines Objekts durch einen Kollegen zeigt der Mitarbeiter die beabsichtigten Aktionen an und bittet um Bestätigung. Anschließend können Sie die Aktionen bestätigen oder abbrechen.

## Derzeit für Kollegen verfügbare Funktion

Derzeit ist Coworker im Planungsbereich von Workfront verfügbar und verwendet eine Reihe von Kenntnissen, um auf Informationen für Planning-Objekte zuzugreifen und diese zu bearbeiten. Weitere Informationen finden Sie unter [CX Coworker-Kenntnisse](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Sie können Coworker verwenden, um die folgenden Aktionen auszuführen:

* Nach Datensätzen suchen. Sie können nach Informationen suchen, die in beliebigen Datensatzfeldern enthalten sind.
* Einträge erstellen. Eine ID mit einem Link zum neuen Datensatz wird angezeigt, nachdem der Datensatz erstellt wurde. Sie können die Felder angeben, die Sie während des Erstellungsprozesses aktualisieren möchten, z. B. Datum oder Beschreibung.
* Erstellen Sie Datensätze basierend auf einem Dokument, das Sie hochladen. Workfront unterstützt die folgenden Dokumentenformate für den Coworker:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT und die meisten Bildformate
* Aktualisieren Sie die Felder für die Datensätze, die Sie auf dem Bildschirm sehen
* Löschen, Duplizieren oder Wiederherstellen von Datensätzen
* Datensätze mit anderen Datensätzen verknüpfen
* Anzeigen des Änderungsverlaufs eines Datensatzes


## Kollegen in Workfront-Planung suchen

Sie können Coworker in den folgenden Bereichen von Workfront Planning platzieren:

* Die Hauptnavigationsleiste in der oberen rechten Ecke des Bildschirms.
* Innerhalb des Detailbereichs eines Datensatzes, wenn Sie ihn in einer neuen Registerkarte öffnen.

## Zugriff auf Mitarbeiter im Planungsbereich

1. Melden Sie sich bei Workfront an und klicken Sie dann oben links auf ****-Symbol ![Hauptmenü „Zeilen](assets/lines-main-menu.png) und dann auf **Planung**.

   Der Bereich Planung wird geöffnet.

   Suchen Sie das Symbol **Mitarbeiter** ![Mitarbeiter-Symbol](assets/coworker-icon.png) in der rechten oberen Ecke der Seite oder fahren Sie mit den folgenden Schritten fort.

1. Klicken Sie auf eine **Arbeitsbereichskarte**.

1. Klicken Sie auf **Karte vom Typ Datensatz**.

1. Klicken Sie auf **Datensatz**, um die Seite **Details** des Datensatzes zu öffnen, und klicken Sie dann auf das Symbol **In neuer Registerkarte öffnen** ![In neuer Registerkarte öffnen](assets/open-workspace-on-new-tab-icon.png) .

1. Klicken Sie auf **Symbol &quot;**&quot; ![Symbol „Kollege](assets/coworker-icon.png) in der rechten oberen Ecke des Bildschirms.

1. Beginnen Sie im vorgesehenen Feld mit der Eingabe von Befehlen für einen Kollegen, und klicken Sie anschließend auf die Eingabetaste.

   ![Bedienfeld „Mitarbeiter“ mit leerem Befehlsfeld](assets/cx-coworker-right-rail.png)

   Sie können beispielsweise einen der folgenden Typen eingeben:

   * Erstellen Sie einen neuen Kampagnendatensatz mit dem Namen Summer Sale 2026
   * Aktualisieren Sie das Budgetfeld im Sommerkampagnendatensatz auf 75.000 $
   * Löschen Sie den Kampagnendatensatz mit dem Namen „Alte Promotion“.
   * Die versehentlich gelöschte Kampagne wiederherstellen

   >[!TIP]
   >
   >Stellen Sie sicher, dass der Workfront-Administrator die schreibgeschützten MCP-Tools in den Systemeinstellungen aktiviert hat, bevor Sie einen Mitarbeiter auffordern, Bearbeitungsaktionen für Objekte durchzuführen.

   Ein visueller Indikator wird angezeigt, während Coworker Befehle verarbeitet und Erwartungen für die Antwortzeit festlegt.

   Folgen Sie nach Erhalt einer erfolgreichen Antwort den angegebenen Links oder beachten Sie die Änderungen auf der linken Seite.


1. (Optional) Klicken Sie auf das **Vollbildsymbol erweitern**-Symbol ![Vollbildsymbol erweitern](assets/expand-full-screen-icon.png), um das Chat-Feld „Mitarbeiter“ in einer Browser-Registerkarte im Vollbildmodus zu öffnen.


