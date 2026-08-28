---
title: Konfigurieren von Geschäftsregeln für Datensatztypen
description: Sie können Geschäftsregeln für Datensatztypen konfigurieren, die festlegen, wie Datensätze dieses Typs in Adobe Workfront Planning verwaltet werden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 31db7a4ef190793558bcb2fa10beb2585e1068e4
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 1%

---


# Konfigurieren von Geschäftsregeln für Datensatztypen

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Sie können Geschäftsregeln für Datensatztypen konfigurieren, die festlegen, wie Datensätze dieses Typs in Adobe Workfront Planning verwaltet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen, um die Schritte in diesem Artikel auszuführen:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Workflow-Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Planungsstandard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und einen Datensatztyp</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Konfigurieren von Geschäftsregeln

* Sie können Regeln konfigurieren, nach denen Datensätze je nach definierten Bedingungen bearbeitet oder gelöscht werden können.

  Sie können beispielsweise Bedingungen erstellen, die verlangen, dass bestimmte Felder einen Wert enthalten. Wenn der Wert in diesen Feldern fehlt, können Benutzende diesen Datensatz nicht bearbeiten oder löschen.
* Sie können keine Geschäftsregeln zu globalen Datensatztypen in ihren primären oder sekundären Arbeitsbereichen hinzufügen.
* Regeln für den Zeitpunkt der Datensatzerstellung können nicht konfiguriert werden. Jeder, der über Verwaltungsberechtigungen für den Datensatztyp verfügt, kann Datensätze erstellen.
* Sie können eine Bedingung für Ihre Geschäftsregel erstellen, die auf alle Feldtypen mit Ausnahme der folgenden verweist:
  * Formelfelder
  * Suchfelder
  * Referenzfelder

## Geschäftsregeln konfigurieren

1. Zu einem Datensatztyp gehen.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf Geschäftsregeln.


**&#x200B;**&#x200B;**&#x200B;**&#x200B;*** VON CLAUDE - UNTEN - MUSS BEARBEITET WERDEN &#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;***

## Einrichten von Geschäftsregeln in Workfront Planning: Eine schrittweise Anleitung

Schon einmal eine Rekordverlagerung auf „Ready for Execution“ vorgenommen, nur um später herauszufinden, dass die Hälfte der erforderlichen Felder - Marke, Anzeige, Launch-Datum - nie ausgefüllt wurden? Wenn jemand das bemerkt, gibt es bereits ein nachgelagertes Projekt mit fehlenden Daten, und jemand muss die Details aufspüren und sie von Hand aufstocken.

Geschäftsregeln beheben das. Damit können Sie einen einfachen Checkpoint einrichten: **Bevor ein Datensatz einen bestimmten Status erreichen kann, müssen bestimmte Felder ausgefüllt werden.** Wenn dies nicht der Fall ist, sieht die Person, die die Änderung vornimmt, genau, was fehlt, und kann erst fortfahren, wenn das Problem behoben ist.

Dieses Handbuch erläutert, was Geschäftsregeln bewirken, wie Sie sie einrichten und was Ihr Team nach der Live-Schaltung erlebt.

### Was Geschäftsregeln tatsächlich bewirken

Geschäftsregeln fügen einer **Statusänderung“ eine Bedingung**. Anstatt vollständige Daten in dem Moment durchzusetzen, in dem jemand einen Datensatz erstellt (was alle verlangsamen würde), wird die Regel nur zu einem bestimmten, beabsichtigten Zeitpunkt eingeführt: wenn ein Status dabei ist, zu einem von Ihnen konfigurierten Status zu wechseln.

Eine Regel sieht in einfacher Sprache wie folgt aus:

> „Bevor ein Datensatz in „Bereit **Ausführung“ verschoben werden kann** muss **Feld „Marke** einen Wert aufweisen.“

Wenn das Feld leer ist, wird die Statusänderung blockiert und die Person erhält eine klare Meldung, die ihr mitteilt, was behoben werden soll. Sobald sie es ausfüllen und erneut versuchen, geht die Änderung durch.

Einige wichtige Dinge, die dies *nicht*:

* **Die Erstellung von Datensätzen wird nicht blockiert.** Man kann immer noch sofort einen neuen Eintrag erstellen und ihn mit der Zeit ausfüllen, genau wie heute.
* **Es füllt nichts automatisch aus oder ändert den Status nicht automatisch.** Eine Person muss die Statusänderung immer selbst vornehmen.
* **Alte Einträge werden nicht rückwirkend markiert.** Datensätze, die sich bereits im Zielstatus befinden, sind davon nicht betroffen. Die Prüfung wird nur ausgeführt, wenn das nächste Mal versucht wird, einen Datensatz in *Status* verschieben.



### Vorbereitung

Einige Dinge müssen zutreffen, bevor Sie Regeln konfigurieren können:

1. **Die Funktion muss für Ihre Organisation aktiviert sein.** Dies geschieht auf der Seite von Adobe (über ein Feature Flag), nicht etwas, das Sie selbst aktivieren. Wenn der unten beschriebene Abschnitt „Geschäftsregeln“ nicht angezeigt wird, überprüfen Sie bei Ihrem Adobe-Ansprechpartner, ob er für Ihren Mandanten aktiviert wurde.
2. **Sie benötigen Admin- oder Workspace-Konfigurator-Berechtigungen.** Reguläre Planer können keine Regeln erstellen oder bearbeiten - nur die Personen, die den Arbeitsbereich verwalten, können dies tun.

### Schritt 1: Konfigurationsbereich für Geschäftsregeln öffnen

Geschäftsregeln live neben Ihrem anderen Admin-Setup - Sie brauchen kein separates „Planning“-Panel zu suchen. Im Bereich für die Workflow-Einrichtung:

1. Wechseln Sie zum Hauptbereich **Workflow-Einrichtung/Admin** für Ihren Arbeitsbereich.
2. Suchen Sie **Abschnitt „Geschäftsregeln** für den Datensatztyp, den Sie konfigurieren möchten (z. B. „Materialien“ oder „Kampagnen„).


### Schritt 2: Auswählen des Datensatztyps

Regeln werden pro Datensatztyp konfiguriert. Wählen Sie daher die Regel aus, der Sie eine Regel hinzufügen möchten. Wenn Sie beispielsweise sicherstellen möchten, dass vor der Ausführung in jedem Materialdatensatz Schlüsselfelder ausgefüllt sind, wählen Sie **Materialien**.



### Schritt 3: Neue Regel erstellen

Für jede Regel geben Sie drei Dinge an:

| Was Sie festgelegt haben | Beispiel |
|---|---|
| **Datensatztyp** | Materialien |
| **Zielstatus** | Bereit zur Ausführung |
| **Erforderliches Feld** | Marke |

Mit anderen Worten: „Wenn der Status eines Materialdatensatzes in &quot;**zur Ausführung“ geändert wird** muss das Feld **Marke** einen Wert enthalten.“

Sie können für denselben Status mehr als eine Regel hinzufügen. Beispielsweise kann es erforderlich sein, dass alle Angaben zu Marke, Therapiebereich, Indikation und voraussichtlichem Startdatum ausgefüllt werden, bevor ein Datensatz in „Bereit zur Ausführung“ geändert werden kann. Dabei handelt es sich jeweils um eine eigene Regel, die alle gemeinsam überprüft werden.

**Welche Felder können benötigt werden?**
&#x200B;- Verbundene Datensatzfelder (z. B. ein verknüpfter Marken- oder Indikationsdatensatz) - Die Regel wird erfolgreich abgeschlossen, sobald mindestens ein Datensatz verknüpft ist.
&#x200B;- Standardtextfelder (einzeilig oder Absatz) - die Regel wird übergeben, sobald ein Wert vorhanden ist.
&#x200B;- Datumsfelder - Die Regel wird übergeben, sobald ein Datum festgelegt wird.

**Was Sie noch nicht verwenden können:** Formelfelder und Lookup-Felder werden in dieser Version nicht als Regelziele unterstützt, da sie im Hintergrund berechnet und nicht direkt von einer Person ausgefüllt werden.

### Schritt 4: Schreiben Sie die Nachricht, die die Benutzer sehen werden

Wenn Sie eine Regel erstellen, geben Sie auch die Meldung an, die angezeigt wird, wenn versucht wird, die Änderung vorzunehmen, ohne dass das Feld ausgefüllt ist. Halten Sie es spezifisch und umsetzbar - so etwas wie:

> „Marke ist erforderlich.“

Sie müssen sich keine Gedanken über die Formatierung eines ganzen Fehlerbanners machen - das System verarbeitet die Kombination von Nachrichten, wenn mehrere Regeln gleichzeitig verletzt werden (siehe unten).

### Schritt 5: Speichern der Regel

Nach dem Speichern wird die Regel **sofort** für alle Benutzer im Arbeitsbereich wirksam - sie müssen sich nicht abmelden, aktualisieren oder auf eine Bereitstellung warten. Wenn das nächste Mal versucht wird, einen Datensatz in diesen Status zu verschieben, wird die Regel überprüft.

### Was Ihr Team tatsächlich erleben wird

Für die Benutzer, die die tägliche Planung verwenden, ändert sich dies, sobald eine Regel live ist.

#### Wenn ein erforderliches Feld leer ist

1. Ein Planer öffnet einen Datensatz und ändert den Status in den abgeschlossenen Status (z. B. „Bereit zur Ausführung„).
2. Das System prüft alle Regeln, die mit diesem Status verknüpft sind.
3. Wenn ein erforderliches Feld leer ist, wird die Änderung **abgelehnt** - der Status wird auf den ursprünglichen Wert zurückgesetzt.
4. Es wird eine Popup-Meldung angezeigt, in der genau angegeben wird, welche Felder fehlen:
   > *Statusänderung blockiert: &#39;Marke&#39; und &#39;Geschätztes Launch-Datum&#39; müssen ausgefüllt werden, bevor der Wechsel zu &#39;Bereit zur Ausführung&#39; erfolgt*
5. Der Planer füllt die fehlenden Felder aus und versucht die Statusänderung erneut.
6. Dieses Mal vergeht die Regel, und der Status wird normal aktualisiert.

#### Wenn bereits alles ausgefüllt ist

Nichts ändert sich. Der Status wird sofort aktualisiert, ohne zusätzliche Schritte oder Popups. Geschäftsregeln sind unsichtbar, bis sie tatsächlich gebraucht werden.

#### Wenn mehrere Felder gleichzeitig fehlen

Alle verletzten Regeln werden zusammen überprüft und die Nachricht listet alle fehlenden Felder in einem Schritt auf - Planer müssen nicht ein Feld reparieren, es erneut versuchen, über das nächste informiert werden und dann wiederholen.

### Schritt 6: Später Regel bearbeiten oder entfernen

Regeln sind nicht in Stein gemeißelt. Änderungen vornehmen:

1. Kehren Sie zum Konfigurationsbereich für Geschäftsregeln für den Datensatztyp zurück.
2. Suchen Sie die Regel, die Sie ändern möchten.
3. Erforderliches Feld, Zielstatus oder Nachricht bearbeiten oder die Regel vollständig löschen.
4. Speichern Sie. Die Änderung gilt unmittelbar für zukünftige Statusänderungen.

Denken Sie daran: Das Bearbeiten oder Löschen einer Regel **wirkt sich nur auf künftige Transitionen aus.** Datensätze, die bereits vor der Änderung in den Zielstatus übergegangen sind, werden nicht neu ausgewertet.
3## Einige Dinge, die es wert sind, gewusst zu werden

* **Dies ist von der Sperrung von Datensätzen nach einer Statusänderung getrennt.** Geschäftsregeln (wie hier beschrieben) überprüfen nur die Vollständigkeit der Felder *bevor* eine Statusänderung durchläuft. Eine andere, damit zusammenhängende Funktion regelt, ob ein Datensatz vollständig von Bearbeitungen/Löschungen gesperrt wird, sobald er einen bestimmten Status erreicht - das wird hier nicht behandelt.
* **Massenstatusänderungen** (Änderung des Status in vielen Datensätzen gleichzeitig) sind noch nicht vollständig definiert für die Interaktion mit Geschäftsregeln. Wenn Ihr Team stark auf Massenaktionen angewiesen ist, sollten Sie sich bei Ihrem Adobe-Ansprechpartner über das aktuelle Verhalten erkundigen.
* **Wenn eine Regel aufgrund eines Systemfehlers nicht ausgewertet werden kann** wird die Transition blockiert und nicht stumm durchgelassen - aufgrund eines Backend-Hickups wird ein unvollständiger Datensatz nie über eine Regel hinausgereicht.
* **Beim Deaktivieren der Funktion** Ihre konfigurierten Regeln nicht gelöscht, sondern nur angehalten. Wenn Sie sie wieder aktivieren, werden sie genau so wiederhergestellt, wie sie waren. Es ist keine Neukonfiguration erforderlich.

### Kurzanleitung: Einrichten der ersten Regel

1. Bestätigen Sie, dass die Funktion für Ihren Mandanten aktiviert ist.
2. Gehen Sie zur Workflow-Einrichtung → Geschäftsregeln für Ihren Datensatztyp.
3. Wählen Sie den Datensatztyp aus (z. B. Material).
4. Erstellen Sie eine Regel: Zielstatus + erforderliches Feld.
5. Schreiben Sie eine eindeutige, spezifische Fehlermeldung.
6. Speichern - es ist sofort live.
7. Wiederholen Sie diesen Vorgang für jedes Feld, das Sie benötigen möchten.
8. Testen Sie es selbst: Versuchen Sie, den Status eines Datensatzes mit leerem Feld zu ändern, bestätigen Sie, dass Sie die erwartete Nachricht sehen, füllen Sie das Feld aus und bestätigen Sie, dass die Statusänderung jetzt durchgeführt wird.

Das war&#39;s. Von hier an bekommt jeder, der einen Datensatz nach vorn konvertiert, einen klaren Anstoß, wenn etwas fehlt, anstelle von einem nachgelagerten Projekt, das leise unvollständig erscheint.