---
title: Workfront-Planungsfelder freigeben
description: Sie können das Feld eines Workfront-Planungsdatensatzes für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 3%

---


# Workfront-Planungsfelder freigeben

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Sie können das Feld eines Workfront-Planungsdatensatzes für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.

Mit der gemeinsamen Nutzung von Feldern können Workspace-Admins den Zugriff auf ein einzelnes Feld steuern. Jedes Feld in einem Datensatztyp verfügt über ein eigenes Freigabedialogfeld, in dem der Zugriff auf „Kein Zugriff“, „Feldwerte anzeigen“ oder „Feldwerte verwalten“ festgelegt werden kann.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebige Workfront oder Workflows mit einem Planungspaket</p> 
ODER
<p>Beliebige Workfront-Planung als eigenständiges Produktpaket</p> 
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
   <td><p>Verwalten von Berechtigungen für ein Feld, um Werte für das Feld zu ändern</p>  
   <p>Tragen Sie oder höhere Berechtigungen zu einem Datensatztyp bei, um Berechtigungen für das Feld zu erben oder zu verwalten</p>  
   </td> 
  </tr>
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Feldern

* Sie können Felder für Benutzer, Aufgabengebiete, Gruppen, Teams oder Unternehmen freigeben.
* Der Zugriff auf ein Feld erfolgt durch die Kombination der folgenden Einstellungen:

  * **Geerbte Berechtigungen**: Standardmäßig erbt ein Feld den gleichen Zugriff, den jemand auf den Datensatztyp hat (Berechtigungen für den Datensatztyp anzeigen geben einem Benutzer die Berechtigung zum Anzeigen von Feldwerten; Berechtigungen für den Datensatztyp „Beitragen“ oder „Verwalten“ geben einem Benutzer die Berechtigung zum Verwalten von Feldwerten). Sie können geerbte Berechtigungen deaktivieren und Benutzern einen geringeren Zugriff auf das Feld gewähren, als sie ihn für den Datensatztyp haben.
  * Die Auswahl **Jeder Benutzer im Arbeitsbereich kann anzeigen** oder **Nur eingeladene Personen können darauf zugreifen**. Sie können entweder zulassen, dass jeder Benutzer mit Berechtigungen für den Arbeitsbereich das Feld anzeigen kann, oder Berechtigungen nur für einzelne Entitäten erteilen.

  Wenn mehrere Regeln für dieselbe Person gelten, erhalten sie die höchste Berechtigung, die ihnen von einer der Regeln zur Verfügung steht.

* Nur Workspace-Besitzer und -Manager können Feldberechtigungen anpassen. Workspace-Manager behalten immer den Verwaltungszugriff auf alle Felder bei und dieser kann nicht verringert werden.
* Die Feldfreigabe steuert den Zugriff auf Werte, nicht auf Feldeinstellungen. Nur Workspace-Manager können die Konfiguration eines Felds ändern.
* Wenn Sie jemanden zur Freigabeliste eines Felds hinzufügen, erhält er keinen Zugriff auf Arbeitsbereiche oder Datensatztypen. Wenn diese Zugriffsrechte nicht verfügbar sind, wird die Berechtigung erst wirksam, nachdem sie zum Datensatztyp hinzugefügt wurden.
* Systemfelder (z. B. Erstellt von, Datensatz-ID) und primäre Felder können keine eingeschränkte Freigabe haben.
* Eingeschränkte Felder werden überall dort durchgesetzt, wo das Feld angezeigt wird. Dazu gehören alle Ansichten, Datensatzdetailseiten, Anfrageformulare, Verbindungen und Lookup-Felder, Canvas-Dashboards, die API und MCP-Tools.
* Suchfelder übernehmen die Berechtigungen ihres Quellfelds.
* Öffentliche Ansichten bleiben für alle, die darauf zugreifen können, vollständig sichtbar und schreibgeschützt.
* Beim Duplizieren eines Datensatzes werden die eingeschränkten Werte nicht in die neuen Datensätze kopiert.
* Eingeschränkte Feldwertänderungen werden nicht im Verlauf eines Datensatzes aufgezeichnet.
* Bei Berechtigungsänderungen für Felder werden keine Trigger-Benachrichtigungen erstellt.
* Für globale Datensatztypen gelten Feldberechtigungen für alle sekundären Arbeitsbereiche und können nicht lokal angepasst werden.


Von Claude:
Zusätzliche Berechtigungen für Felder - fügen Sie dies möglicherweise zum Übersichtsartikel für die gesamte Freigabe hinzu?? - help/quicksilver/planning/access/sharing-permissions-overview.md

Hier erfahren Sie, wie der Datensatztyp-/Arbeitsbereichszugriff dem Zugriff auf Feldebene im Dokument zugeordnet wird:

Berechtigungsebenen für Felder (nur zwei, plus keine):

Kein Zugriff - Feld ist vollständig ausgeblendet
Feldwerte anzeigen : Der Wert kann angezeigt werden, aber nicht bearbeitet werden
Verwalten von Feldwerten - Kann anzeigen und bearbeiten

Standardmäßige Vererbung von Datensatztyp-Rollen

Datensatztyp/Arbeitsbereich-Zugriff Standardfeldberechtigung
Anzeigen von Feldwerten
Verwalten von Feldwerten
Verwalten (Workspace Manager) Verwalten von Feldwerten (gesperrt, nicht reduzierbar)

Standardmäßig spiegelt ein Feld einfach die Rolle wider, die eine Person auf dem Datensatztyp spielt - Zuschauer erhalten schreibgeschützt, Mitwirkende und Manager erhalten Bearbeitungsrechte. Workspace-Manager sind ein Sonderfall: Wenn sie zur Freigabeliste eines Felds hinzugefügt werden, ist „Feldwerte verwalten“ vorausgewählt und die Option „Feldwerte anzeigen“ ist deaktiviert, da ihr Bearbeitungszugriff nie entfernt werden kann.

Einstellung für Platzhalter (Fallback)
Neben der Vererbung verfügt jedes Feld über einen standardmäßigen Platzhalter:

Jeder Benutzer im Arbeitsbereich kann Folgendes anzeigen (Standard)
Nur eingeladene Personen haben Zugriff

Wie die endgültige Berechtigung berechnet wird

Wenn geerbte Berechtigungen aktiviert sind: der Zugriff einer Person = der höchste der folgenden Werte (geerbt von Datensatztyp, Platzhalter, einzeln erteilte Berechtigung).
Wenn geerbte Berechtigungen deaktiviert sind: Der Zugriff einer Person = der höchste Wert von (Platzhalter, einzeln erteilte Berechtigung) — Die Rolle des Datensatztyps spielt keine Rolle mehr.
Wenn die Vererbung deaktiviert ist, lautet der Platzhalter „Nur eingeladene Personen können zugreifen“ und die Person wird nicht einzeln hinzugefügt, → sie keinen Zugriff erhält.

Weitere Hinweise zu Berechtigungen

Wenn Sie jemandem Zugriff gewähren, wird ihm kein Zugriff auf Arbeitsbereich/Datensatztyp gewährt. Er bleibt einfach inaktiv (mit einem Warnsymbol), bis er separat zum Arbeitsbereich hinzugefügt wird.
Für globale Datensatztypen werden Feldberechtigungen nur einmal festgelegt und gelten für alle sekundären Arbeitsbereiche. Sekundäre/Team Workspace-Manager können sie nicht lokal überschreiben.

## Freigeben von Feldern

