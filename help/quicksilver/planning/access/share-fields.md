---
title: Workfront-Planungsfelder freigeben
description: Sie können das Feld eines Workfront-Planungsdatensatzes für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac94936cc4dc9dc4f2d56b3f1221f71a405c5c65
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 2%
---

# Workfront-Planungsfelder freigeben

{{planning-important-intro}}

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
* Sie können nur Felder aus der Tabellenansicht eines Datensatztyps freigeben.
* Die folgenden Typen von Feldern können nicht freigegeben werden:

  * Systemfelder (z. B. Erstellt von, Datensatz-ID)
  * Primäre Felder
  * Nachschlagefelder. Sie übernehmen immer die Berechtigungen ihrer Quellobjektfelder.
* Der Zugriff auf ein Feld erfolgt durch die Kombination der folgenden Einstellungen:

  * **Geerbte Berechtigungen**: Standardmäßig erbt ein Feld den gleichen Zugriff, den jemand auf den Datensatztyp hat. Sie können geerbte Berechtigungen deaktivieren und Benutzern einen geringeren Zugriff auf das Feld gewähren, als sie ihn für den Datensatztyp haben.
  * Die Auswahl **Alle mit Zugriff auf den Datensatztyp können anzeigen** oder **Nur eingeladene Personen können zugreifen**. Sie können entweder zulassen, dass jeder Benutzer mit Berechtigungen für den Arbeitsbereich das Feld anzeigen kann, oder Berechtigungen nur für einzelne Entitäten erteilen.

  Wenn mehrere Regeln für dieselbe Person gelten, erhalten sie die höchste Berechtigung, die ihnen von einer der Regeln zur Verfügung steht.

* Damit ein Feld für alle Benutzer in einem Arbeitsbereich schreibgeschützt ist, müssen Sie sicherstellen, dass die folgende Einrichtung vorhanden ist:

  * Übernommene Berechtigungen deaktivieren
  * Beibehalten der Einstellung **Jeder Benutzer mit Zugriff auf den Datensatztyp kann anzeigen**
  * Fügen Sie keine einzelnen Entitäten hinzu.

* Je nach den Berechtigungen des Datensatztyps können Benutzende die folgenden Feldberechtigungen erhalten:

  * Berechtigungen für den Datensatztyp anzeigen erteilen einem Benutzer die Berechtigung zum Anzeigen von Feldwerten
  * Berechtigungen zum Beitragen oder Verwalten von Datensatztypen erteilen Benutzenden die Berechtigung zum Verwalten von Feldwerten

* Nur Workspace-Besitzer und -Manager können Feldberechtigungen anpassen. Workspace-Manager behalten immer den Verwaltungszugriff auf alle Felder bei und dieser kann nicht verringert werden.
* Die Feldfreigabe steuert den Zugriff auf Werte, nicht auf Feldeinstellungen. Nur Workspace-Manager können die Konfiguration eines Felds ändern.
* Wenn Sie jemanden zur Freigabeliste eines Felds hinzufügen, erhält er keinen Zugriff auf Arbeitsbereiche oder Datensatztypen. Wenn diese Zugriffsrechte nicht verfügbar sind, wird die Berechtigung erst wirksam, nachdem sie zum Datensatztyp hinzugefügt wurden.
* Felder mit eingeschränkten Berechtigungen werden überall dort durchgesetzt, wo das Feld angezeigt wird. Dazu gehören alle Ansichten, Datensatzdetailseiten, Anfrageformulare, Verbindungen und Lookup-Felder, Canvas-Dashboards, die API und MCP-Tools.
* Öffentliche Ansichten bleiben für alle, die darauf zugreifen können, vollständig sichtbar und schreibgeschützt.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* Eingeschränkte Feldwertänderungen werden nicht im Verlauf eines Datensatzes aufgezeichnet.
* Bei Berechtigungsänderungen für Felder werden keine Trigger-Benachrichtigungen erstellt.
* Für globale Datensatztypen gelten Feldberechtigungen für alle sekundären Arbeitsbereiche und können nicht lokal angepasst werden.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Freigeben von Feldern

Als Workspace-Manager können Sie Berechtigungen an einzelne Felder anpassen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich und dann den Datensatztyp, dessen Felder Sie freigeben möchten.

1. Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen der Spaltenüberschrift eines Felds und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Feld freigeben**.

   Das Feld **Freigeben** wird geöffnet.

1. (Optional) Im Bereich **Zugriff gewähren** ist die Option **Jeder, der Zugriff auf den Datensatztyp hat, kann** anzeigen) standardmäßig ausgewählt. Alle Benutzer mit **Anzeigen** oder höheren Berechtigungen für den Arbeitsbereich und den Datensatztyp haben dieselben Berechtigungen für das Feld.

1. (Optional) Klicken Sie unter der Option **Vererbte Berechtigungen von** auf die Avatare von Benutzern, um Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete anzuzeigen, die Berechtigungen vom Arbeitsbereich erben.

   Die Berechtigungen des Benutzers für den Datensatztyp werden angezeigt, wenn Sie die geerbten Berechtigungen erweitern.

   >[!TIP]
   >
   >Sie können keine einzelnen Entitäten aus der Liste der geerbten Berechtigungen entfernen. Die Benutzer aus Teams, Gruppen, Unternehmen oder Aufgabengebieten werden anstelle der Entitäten aufgelistet, mit denen sie verknüpft waren, als der Arbeitsbereich und der Datensatztyp für sie freigegeben wurden.

1. (Optional und bedingt) Wenn Sie das Feld für bestimmte Entitäten freigeben und ihnen einen anderen Zugriff auf das Feld gewähren möchten, als sie bereits für den Datensatztyp haben, gehen Sie wie folgt vor:

   1. Deaktivieren Sie die **Aktiviert** unter **Vererbte Berechtigungen**. Er ist standardmäßig ausgewählt.

      Die Option ändert sich in **Deaktiviert**.

      >[!TIP]
      >
      >Workspace-Manager verfügen weiterhin über Verwaltungsberechtigungen für den Datensatztyp und das Feld.

   1. (Optional) Klicken Sie auf das **Alle Personen mit Zugriff auf den Datensatztyp können anzeigen** Dropdown-Menü und wählen Sie **Nur eingeladene Personen können darauf zugreifen**.

      >[!IMPORTANT]
      >
      >Diese Änderung in Verbindung mit dem Deaktivieren **Vererbte Berechtigungen** entfernt den Zugriff für alle Personen, die den Datensatztyp anzeigen können und nur bestimmten Personen Zugriff gewähren. Workspace-Manager und -Administratoren haben immer Zugriff auf alle Felder.


   1. Fügen Sie im Feld **Zugriff gewähren** die Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzu, denen Sie eine andere Berechtigungsstufe gewähren möchten als für den Arbeitsbereich oder den Datensatztyp.

      Wenn Sie ein Feld für einen Benutzer freigeben, werden dessen primäres Aufgabengebiet und dessen E-Mail-Adresse ebenfalls im Feld angezeigt. Damit Sie die E-Mail-Adresse des Benutzers anzeigen können, muss für das Benutzerobjekt in Ihrer Zugriffsebene die Einstellung „Kontaktinformationen anzeigen“ aktiviert sein.

   1. Wählen Sie eine der folgenden Berechtigungsebenen aus:

      * Feldwerte anzeigen
      * Feldwerte verwalten

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* Es ist nicht möglich, Benutzenden eine geringere Berechtigung für das Feld zu erteilen, wenn diese mindestens über die Eigenschaft Beitragen für den Datensatztyp verfügen.
      >
      >* Benutzern, die sich nicht im Arbeitsbereich befinden, können keine Berechtigungen erteilt werden. Benutzende, die keine Berechtigungen für den Arbeitsbereich und den Datensatztyp haben, können auf keines der Felder zugreifen. Sie können auf die Felder zugreifen, wenn sie Berechtigungen für den Arbeitsbereich und die Datensatztypen erhalten.

1. Klicken Sie auf **Speichern**.

   Das Feld wird jetzt für andere Benutzer freigegeben.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## Entfernen von Berechtigungen für ein Feld

Sie können Benutzerberechtigungen aus einem Feld entfernen. Sie behalten jedoch mindestens die Berechtigung Anzeigen für den Arbeitsbereich und den Datensatztyp bei, wodurch sie mindestens die Berechtigung Anzeigen für das Feld erhalten.

Sie müssen ihren Zugriff aus dem Arbeitsbereich entfernen, wenn sie keine Berechtigungen für die Datensatztypen oder Felder im Arbeitsbereich haben sollen.

Sie können einen Benutzer nicht aus geerbten Berechtigungen entfernen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Felder Sie nicht mehr freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz . Dadurch wird die Seite „Datensatztyp“ geöffnet.
1. Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen der Spaltenüberschrift eines Felds und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Feld freigeben**.

   Das Feld **Freigeben** wird geöffnet.
1. Suchen Sie die Person, Gruppe, Team, Firma oder Aufgabengebiet, deren Berechtigungen Sie entfernen möchten, erweitern Sie das Dropdown-Menü Berechtigungen rechts neben ihrem Namen und klicken Sie auf **Entfernen**.

1. Klicken Sie auf **Speichern**.

   Die Personen verfügen nicht mehr über die angegebenen Berechtigungen für das Feld. Sie haben jedoch weiterhin Berechtigungen für den Datensatztyp und den Arbeitsbereich, es sei denn, Sie entfernen sie auch aus diesen Berechtigungen.

   Die Benutzer, die vom Zugriff auf das Feld entfernt wurden, erhalten keine Benachrichtigung, dass sie nicht mehr über diese Berechtigungen verfügen.
