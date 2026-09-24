---
title: Share Planning Requests
description: Sie können eine Workfront-Planungsanfrage für andere freigeben, nachdem sie übermittelt wurde.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 4ee702aeded88e330ec456a0e6b5cf1813bfb64e
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 5%
---
# Share Planning Requests

<!--add to TOC, and miniTOC-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Nachdem eine Planungsanfrage übermittelt wurde, können Sie steuern, wer sie sieht, wer daran arbeiten kann und welche Aktionen jede Person oder jedes Team durchführen darf. Dadurch können sich die richtigen Mitarbeiter auf die richtigen Anfragen konzentrieren und nur die ihrer Rolle entsprechenden Maßnahmen ergreifen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebige Workfront oder Workflows mit einem Planungspaket</p> 
ODER
<p>Beliebige Workfront-Planung beim Kauf als eigenständiges Produkt</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Beliebig</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Anzeigen oder Erweitern der Berechtigungen für einen Arbeitsbereich und einen Datensatztyp, wenn Sie Workfront-Benutzer sind</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Anfragen

* Sie können Benutzern für eine Anfrage die folgenden Berechtigungen gewähren:

  * Anzeigen: Benutzende können nur die Anfrage sehen.
  * Beitragen: Benutzer können die Anfrage anzeigen, bearbeiten und kommentieren.
  * Verwalten: Benutzer können die Anfrage anzeigen, bearbeiten, kommentieren und löschen.

* Anfragenden wird automatisch Zugriff auf die von ihnen gesendeten Anfragen gewährt, es sei denn, ein Administrator hat einen anderen Standard konfiguriert.

  Weitere Informationen finden Sie unter [Anforderungsformular erstellen](/help/quicksilver/planning/requests/create-request-form.md).

* Workfront-Administratoren können auf alle Anfragen zugreifen und sie verwalten.
* Benutzer mit Zugriff auf „Verwalten“ für einen Datensatztyp erben den Verwaltungszugriff auf das Aufnahmeformular dieses Datensatztyps und auf jede über ihn gesendete Anfrage.
* Jeder, der über die Berechtigung für eine Anfrage verfügt, kann die Anfrage mit derselben Berechtigungsstufe oder einer niedrigeren Stufe als seiner eigenen freigeben.

  Benutzende mit der Berechtigung Beitragen können niemand anderem Berechtigungen zum Verwalten der Anfrage erteilen.

* Verschiedene Personen und Teams können unterschiedliche Zugriffsebenen für dieselbe Anfrage haben.
* Berechtigungen können über mehrere Entitäten zugewiesen werden. Wenn ein(e) Benutzende(r) die Berechtigung Beitragen für eine Anfrage hat, seine/ihre Gruppe oder Aufgabengebiet jedoch über Anzeigeberechtigungen verfügt, behält er/sie die höchste Berechtigungsstufe, die Beitragen lautet.

## Freigeben einer Anfrage

Stellen Sie sicher, dass Sie das neue Anfrageerlebnis verwenden.

1. {{step1-to-requests}}
1. Suchen Sie eine Planning-Anfrage und klicken Sie darauf, um sie zu öffnen.
1. Klicken Sie auf **Freigabe**.

   Das **Freigeben**-Feld wird für die ausgewählte Anfrage geöffnet.

   ![Feld für die Anforderungsfreigabe](assets/requests-sharing-box.png)

1. Geben **im Feld „Zugriff auf diese Anfrage gewähren** den Namen eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens ein und klicken Sie auf den Namen, wenn er/sie in der Liste angezeigt wird.

   In der Liste werden nur aktive Entitäten angezeigt.
1. Wählen Sie aus dem Dropdown-Menü rechts neben dem Namen jeder Entität eine der folgenden Berechtigungsebenen aus:

   * Verwalten
   * Mitwirken
   * Ansicht
1. (Optional) Klicken Sie für jede Berechtigungsstufe auf das Symbol für granulare Berechtigungen und wählen Sie granulare Berechtigungen wie **Bearbeiten**, **Kommentar**, **Freigeben** oder **Löschen** aus oder heben Sie die Auswahl auf.

   ![Detaillierte Berechtigungen für Anfragen](assets/granular-permissions-on-requests.png)
1. Klicken Sie auf **Speichern**.

   Die Anfrage wird für die ausgewählten Entitäten freigegeben.


