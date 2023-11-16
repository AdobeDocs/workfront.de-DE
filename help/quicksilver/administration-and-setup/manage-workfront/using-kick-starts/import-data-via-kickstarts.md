---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren
description: Kick-Starts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kick-Start-Vorlage, die Sie dazu verwenden können, wie unter Kick-Starts-Daten-Importer beschrieben.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 81a9f33f5707e37a62a81546b9249410ded23ab5
workflow-type: tm+mt
source-wordcount: '2642'
ht-degree: 6%

---

# Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren

Kick-Starts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kick-Start-Vorlage, die Sie dazu verwenden können, wie unter [Kick-Starts-Daten-Importer](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Dieser Prozess ist in drei Hauptaufgaben unterteilt:

* Exportieren Sie zunächst eine Kick-Start-Vorlage als Tabellendatei
* Als zweites füllen Sie die Tabelle mit Ihren Daten
* Schließlich importieren Sie die ausgefüllte Tabelle in Workfront

Jedes dieser Verfahren wird in der richtigen Reihenfolge in diesem Artikel beschrieben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTIZ</b>:</p> 
   <p> Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Einschränkungen

Mit einer Kick-Start-Vorlage können Sie eine große Anzahl von Objekten in Workfront importieren. Beachten Sie jedoch die folgenden Einschränkungen:

* Beim Datenimport auf diese Weise werden Informationen zu Datensätzen, die bereits in Workfront vorhanden sind, nicht aktualisiert
* Sie können nur neue Datensätze und deren Informationen importieren
* Importieren Sie nicht mehr als 2.000 Datensätze gleichzeitig, um sicherzustellen, dass beim Import keine Zeitüberschreitung auftritt

## Kick-Start-Vorlage als Tabellendatei exportieren

Wenn Sie eine Kick-Start-Vorlage exportieren, erhalten Sie eine leere Excel-Arbeitsmappe. In nachfolgenden Verfahren in diesem Artikel füllen Sie die Arbeitsmappe mit Ihren Informationen aus und importieren sie dann wieder in Workfront.

So exportieren Sie eine Kick-Start-Vorlage:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **System** > **Daten exportieren (Kick-Starts)**.

1. Klicks **Weitere Optionen** und wählen Sie dann die Informationstypen aus, die Sie einbeziehen möchten.

   Jede ausgewählte Option stellt eine Sammlung mehrerer Registerkarten im exportierten Arbeitsblatt dar. Wenn Sie beispielsweise die Option Bericht auswählen, werden alle zum Erstellen eines Berichts erforderlichen Objekte (Ansichten, Filter, Gruppierungen, Berichte) in die Tabelle aufgenommen.

   Sie können alle unten aufgeführten Objekttypen verwenden, um Daten in Workfront zu importieren. (Die einzige Ausnahme ist die Option Zugriffsebenen . Das Datenblatt Zugriffsebenen in einem Export wird zu Referenzzwecken bereitgestellt. Es ermöglicht Ihnen, einem neuen Benutzerkonto anhand der Kennung eine Zugriffsstufe zuzuweisen.)

   Die Vorlage für jeden Objekttyp kann in die folgenden Dateiformate exportiert werden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objekt</strong> </p> </th> 
      <th> <p><strong>Exportiert als</strong> </p> </th> 
      <th> <p><strong>Blätter im exportierten Arbeitsblatt</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Dashboard</p> <p>Alle Dashboards im System können exportiert werden. Sie können bis zu 100 spezifische Dashboards in einem Export auswählen.</p> </td> 
      <td scope="col">Exportiert als ZIP-Datei</td> 
      <td scope="col"> <p>Parameter</p> <p>Parameteroption</p> <p>Parametergruppe</p> <p>Kategorieparameter</p> <p>Kategorie</p> <p>Bericht</p> <p>Portal-Registerkarten-Abschnitt</p> <p>Dashboard</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Bericht</p> <p>Alle Berichte im System können exportiert werden. Sie können bis zu 100 spezifische Berichte in einem Export auswählen.</p> </td> 
      <td scope="col">Exportiert als ZIP-Datei </td> 
      <td scope="col"> <p scope="col">Parameter</p> <p scope="col">Parameteroption</p> <p scope="col">Parametergruppe</p> <p scope="col">Kategorieparameter</p> <p scope="col">Kategorie</p> <p scope="col">Bericht</p> <p scope="col">Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Genehmigung</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td scope="col"> <p>Schritt-Genehmiger</p> <p>Validierungsschritt</p> <p>Genehmigung</p> <p>Genehmigungsprozess</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Benutzerdefinierte Daten</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td scope="col"> <p>Parameter</p> <p>Parameteroption</p> <p>Parametergruppe</p> <p>Kategorieparameter</p> <p>Kategorie</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Ausgabentyp</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td> <p>Ausgabentyp</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Stundentyp</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td> <p>Stundentyp</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Team</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td> <p> Teammitglied</p> <p>Team</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Benutzerin oder Benutzer</p> </td> 
      <td> <p>Exportiert als Excel-Datei. Um die vollständige Liste der Optionen anzuzeigen, klicken Sie auf <strong>Weitere Optionen</strong>.</p> </td> 
      <td> <p>Benutzerin oder Benutzer</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td>Zugriffsebene</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p>Zugriffsebene</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td>Zuweisung</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p>Zuweisung</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td>Firma</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Firma</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>E-Mail-Vorlage</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p>E-Mail-Vorlage</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Ausgabe</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Ausgabe'</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Externe Seite</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Externe Seite</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Filter</td> 
      <td>Exportiert als ZIP-Datei</td> 
      <td> <p> Filter</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Gruppe</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Gruppe</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Gruppierung</td> 
      <td>Exportiert als ZIP-Datei</td> 
      <td> <p> Gruppierung</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Stunde</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Stunde</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Problem</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Problem</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Aufgabengebiet</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Auftragsrolle</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Meilensteinpfad</td> 
      <td> Exportiert als Excel-Datei</td> 
      <td> <p> Meilenstein</p> <p>Meilensteinpfad</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Notiz</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Notiz</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Portfolio</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Warteschlange</p> <p>Projekt</p> <p>Routingregel</p> <p>Warteschlangenthema</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Ressourcenkalkulation</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Ressourcenkalkulation</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Ressourcenpool</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Ressourcenpool</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Risiko</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Risiko</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Risikotyp</td> 
      <td> Exportiert als Excel-Datei</td> 
      <td> <p> Risikotyp</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p>Scorecard-Fragen</p> <p>Scorecard-Option</p> <p>Scorecard</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Aufgabe</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Aufgabe</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Vorlage</td> 
      <td> Exportiert als Excel-Datei</td> 
      <td> <p> Warteschlange</p> <p>Vorlage</p> <p>Routingregel</p> <p>Warteschlangenthema</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Vorlagenzuweisung</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Vorlagenzuweisung</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Vorlagenaufgabe</td> 
      <td>Exportiert als Excel-Datei</td> 
      <td> <p> Vorlagenaufgabe</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Arbeitszeittabelle</td> 
      <td> Exportiert als Excel-Datei</td> 
      <td> <p> Arbeitszeittabellen-Profil</p> <p>Arbeitszeittabelle</p> <p>Einstellungen </p> </td> 
     </tr> 
     <tr> 
      <td>Anzeigen </td> 
      <td> <p>Exportiert als ZIP-Datei</p> </td> 
      <td> <p> Anzeigen</p> <p>Einstellungen </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Herunterladen**.
1. Fahren Sie mit [Füllen Sie die Tabellenvorlage mit Ihren Daten](#populate-the-spreadsheet-template-with-your-data) , um die Vorlage mit Ihren Daten zu füllen.

## Füllen Sie die Tabellenvorlage mit Ihren Daten {#populate-the-spreadsheet-template-with-your-data}

* [Über die im Arbeitsblatt enthaltenen Registerkarten (Datenblätter)](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Datensatz importieren](#import-a-record)
* [Datum einschließen](#include-dates)
* [Verwenden von Platzhaltern](#use-wildcards)
* [Wertersetzung für IDs durch Attributnamen](#attribute-name-substitution-for-ids)

### Über die im Arbeitsblatt enthaltenen Registerkarten (Datenblätter) {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Um besser zu verstehen, wie Sie die Informationen in den einzelnen Spalten formatieren müssen, wenn Sie die Kick-Start-Vorlage füllen, sollten Sie eine Übung durchführen, indem Sie einen Kick-Start mit vorhandenen Workfront-Daten zu den Objekten exportieren, die Sie importieren möchten. Anweisungen finden Sie unter [Exportieren von Daten aus Adobe Workfront über Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Wenn Sie eine leere Kick-Starts-Vorlage öffnen, sind verschiedene Registerkarten (Datenblätter) verfügbar. Sie hängen von den Objekten ab, die Sie zum Herunterladen ausgewählt haben. Jedes Objekt stellt ein Objekt in der Anwendung dar, z. B. Projekt, Aufgaben, Stunden, Dashboard und Benutzer:

Wenn Sie eine dieser Registerkarten öffnen, zeigt Zeile 2 die Felder für jedes Objekt an, das während eines Imports festgelegt werden kann. In einer Spaltenüberschrift wird nach dem Wort &quot;set&quot;der Name des Felds so angezeigt, wie er in der Datenbank angezeigt wird. Diese Felder dienen als Spaltenüberschriften.

>[!IMPORTANT]
>
>Um Fehler zu vermeiden, stellen Sie Folgendes sicher:
>
>* Löschen oder ändern Sie diese Felder in keiner Weise. Ändern Sie beispielsweise nicht die Reihenfolge oder den Namen.
>* Füllen Sie jedes Feld mit einer fett gedruckten Spaltenüberschrift. Diese stellen erforderliche Felder dar.
>
>  Wenn ein erforderliches Feld jedoch einen in den Systemvoreinstellungen festgelegten Standardwert enthält, müssen Sie ihn nicht ausfüllen.
>
>  Beispiel: auf der **PROJ Project** Registerkarte, die **setCondition** und **setConditionType** -Felder können leer bleiben, aber die **setGroupID** und **setName** kann nicht verwendet werden.
>
>* Bestimmte Felder, darunter **setResourceRevenue** und **setEnteredByID**, werden automatisch vom System generiert. Wenn Sie Daten für diese Felder in das Arbeitsblatt eingeben, werden diese beim Hochladen des Arbeitsblatts durch den Kick-Start-Prozess überschrieben.

### Datensatz importieren  {#import-a-record}

Jede Tabellenzeile entspricht einem eindeutigen Objekt.

1. Füllen Sie die Zelle im **isNew** column:

   * Wenn das zu importierende Objekt neu ist, geben Sie **TRUE** um die Daten in die Zeile zu importieren.
   * Wenn sich das Objekt bereits in Workfront befindet, **FALSE** muss sich in der Spalte befinden, um die Zeile zu ignorieren.

      * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
      * Wenn Sie eine Vorlage mit Daten heruntergeladen haben, sind vorhandene Objekte bereits mit **FALSE**.
      * Wenn Sie eine leere Vorlage heruntergeladen haben, müssen Sie keine neuen Zeilen für vorhandene Objekte hinzufügen.

1. Füllen Sie die Zelle im **ID** auf eine der folgenden Arten:

   * Wenn das zu importierende Objekt neu ist (und Sie eingegeben haben) **TRUE** im **isNew** Spalte), geben Sie eine beliebige Zahl für die ID ein. Diese Nummer muss im Arbeitsblatt eindeutig sein.

   * Wenn das Objekt bereits in Workfront (und **FALSE** im **isNew** ), muss die ID die alphanumerische GUID sein, die in Workfront für dieses Objekt vorhanden ist.

      * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
      * Wenn Sie eine Vorlage mit Daten heruntergeladen haben, enthalten vorhandene Objekte bereits die GUID als ID.
      * Sie können ein neues Objekt auf Grundlage eines vorhandenen Objekts importieren, indem Sie **FALSE** nach **TRUE** im **isNew** -Spalte, indem Sie die ID ändern und die erforderlichen Datenanpassungen vor dem Import vornehmen.

     ![Beispiel-ID für eine Gruppe](assets/kick-start-group-example.png)

   * Beim Importieren eines Projekts müssen Sie eine Gruppen-ID angeben.

      * Wenn die Gruppe bereits in Workfront vorhanden ist, müssen Sie ihre eindeutige ID der **setGroupID** -Feld für das Projekt.
      * Wenn die Gruppe nicht in Workfront vorhanden ist, können Sie die **GRUPPENgruppe** in Ihre Importdatei eintragen, legen Sie die **isNew** -Feld zu **TRUE** im Gruppenblatt und geben Sie eine numerische ID für die neue Gruppe in der **ID** Spalte. Die **setGroupID** -Feld für das neue Projekt muss mit der numerischen **ID** für die neue Gruppe.

     **Beispiel:** Bei einem Projekt wird der Wert angezeigt, der im **setGroupID** -Spalte muss eine der folgenden Eigenschaften aufweisen:

      * Die GUID für eine bestehende Gruppe in Ihrer Workfront-Instanz
      * Der Wert (Zahl) in der Spalte ID auf der **GRUPPENgruppe** Blatt, wenn Sie während des Imports eine neue Gruppe erstellen

1. Geben Sie Werte für die erforderlichen Felder und alle anderen Felder ein, die während des Imports ausgefüllt werden sollen.
1. (Optional) So fügen Sie benutzerdefinierte Daten hinzu:

   * Erstellen Sie für jedes benutzerdefinierte Feld, das Sie in den Importprozess einbeziehen möchten, eine neue Spalte.
   * Benennen Sie jede neue Spalte für das entsprechende benutzerdefinierte Feld wie folgt: **DE:[Name des benutzerdefinierten Felds wie in Workfront angezeigt]**.
   * In der Spalte **setCategoryID** Geben Sie die GUID des vorhandenen benutzerdefinierten Formulars ein, in dem sich dieses benutzerdefinierte Feld befindet. Dieses Feld ist beim Import benutzerdefinierter Daten erforderlich.
   * Wenn Sie mehrere Datenwerte in das benutzerdefinierte Feld hinzufügen müssen (z. B. Optionsfelder, Kontrollkästchen oder Listen), verwenden Sie das auf der Registerkarte Voreinstellungen aufgelistete benutzerdefinierte Trennzeichen für die vertikale Leiste &quot;|&quot;, um die Werte zu trennen.

     **Beispiel:** Geben Sie A|D unter der Spalte DE:Departments ein, um Abteilung A und Abteilung D in Ihr benutzerdefiniertes Formular einzutragen.

### Datum einschließen  {#include-dates}

Workfront kann die meisten Datumsformate verarbeiten. Sie müssen jedoch sicherstellen, dass die Datumsspalte im Arbeitsblatt als Datum formatiert ist. Der Import schlägt fehl, wenn die Spalte als Allgemein, Zahl oder Text formatiert ist.

>[!TIP]
>
>Für die meisten Benutzer ist es am einfachsten, das Format MM/TT/JJJJ zu verwenden (z. B. 07/10/2022).

Workfront akzeptiert auch Zeitwerte als Teil des Datums (z. B. 07/10/2022 01:30 oder 07/10/2022 1:00 PM).

Wenn Sie einen Zeitpunkt im Datum weglassen, führt Workfront einen der folgenden Schritte aus:

* Es wird von 12:00 Uhr angenommen. Um das erwartete Datumsergebnis zu sehen, muss die Systemzeitzone mit Ihrer Zeitzone übereinstimmen.
* Wenn es sich um ein Objekt handelt, das mit einem Zeitplan verknüpft ist, verschiebt sich die Zeit auf den frühesten Zeitpunkt, den der Zeitplan zulässt.

>[!NOTE]
>
>Bei Verwendung eines UNIX-Zeitstempels müssen Sie drei weitere Nullen am Ende des Werts einfügen.
>
>Wenn Ihr Zeitstempel beispielsweise 7336899000 ist, geben Sie 7336899000000 in die Zelle ein.

### Verwenden von Platzhaltern {#use-wildcards}

Sie können die folgenden Platzhalterzeichen verwenden, wenn Sie Ihre Kick-Start-Vorlagenspreadsheet ausfüllen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Platzhalter</strong> </p> </th> 
   <th> <p><strong>Verhalten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$HEUTE</p> </td> 
   <td> <p>Bei Verwendung in <strong>setDate</strong> festgelegt, setzt dieser Platzhalter das Datum auf Mitternacht am Tag, an dem Sie den Kick-Start importieren.</p> <p>Sie können den Platzhalter mit der in einem Filter zulässigen Standardsyntax ändern.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie möchten, dass ein Projekt am Montag der Woche beginnt, an der es importiert wird, können Sie Folgendes verwenden: <strong>$$HEUTEbw</strong>. Dadurch wird das geplante Startdatum Ihres Projekts auf Sonntag um 12:00 Uhr festgelegt. Da der Zeitplan für das Projekt zu diesem Zeitpunkt wahrscheinlich keine Arbeit zulässt, wird er um 9:00 Uhr morgens beginnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Bei Verwendung in <strong>setDate</strong> festgelegt, setzt dieser Platzhalter das Datum entsprechend dem Zeitpunkt, zu dem Sie den Datensatz während des Kick-Start-Imports erstellen.</p> <p>Sie können den Platzhalter mit der in einem Filter zulässigen Standardsyntax ändern.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie möchten, dass ein Projekt drei Stunden nach dem Import gestartet wird, können Sie <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Bei Verwendung in <strong>setAssignedToID</strong> oder einem anderen auf der Benutzer-ID basierenden Feld, weist dieser Platzhalter das Werk zu oder ordnet den Datensatz anderweitig der Person zu, die den Import durchführt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Dieser Platzhalter wurde speziell für Kick-Start-Benutzerimporte hinzugefügt. Wenn ein Workfront-Konto erstellt wird, wird ein Benutzer mit der Zugriffsebene "Systemadministrator"erstellt. Der dem Standardadministrator zugewiesene Benutzername kann beim Erstellen anderer Benutzer in dem Konto als Präfix verwendet werden.</p> <p>Da Benutzernamen für alle Kunden eindeutig sein müssen, ist dies nützlich, wenn Sie mehrere Personen mit sehr häufigen Benutzernamen haben, z. B. John Smith, der den Benutzernamen "jsmith"haben könnte. Indem Sie der Zuweisung des Benutzernamens den standardmäßigen Administrator-Benutzernamen voranstellen, garantieren Sie, dass jeder Benutzername eindeutig ist (z. B.: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Tipp: Eine elegantere Möglichkeit, sicherzustellen, dass Benutzernamen systemweit eindeutig sind, besteht darin, die E-Mail-Adresse des Kontakts in die <strong>setUsername</strong> -Feld.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Wertersetzung für IDs durch Attributnamen  {#attribute-name-substitution-for-ids}

Obwohl es sich nach Möglichkeit empfiehlt, IDs zu verwenden, ist es manchmal nicht praktisch, beim Festlegen einer **setAttributeID** -Wert. Sie können Werte nach Namen referenzieren, indem Sie einfach die Spaltenüberschrift ändern.

**Beispiele:**

* **(Projektimport)**

  Legen Sie beim Importieren von Projekten die **setGroupID** der Projekte, indem sie **GRUPPENgruppe** , wobei die jeweiligen Gruppen-IDs notiert und in die richtigen Zellen eingefügt werden (**setGroupID** -Spalte) **PROJ Project** Blatt.

  Dies ist möglich, wenn man nur mit wenigen Gruppen und Projekten arbeitet, aber wenn man mit mehreren von ihnen arbeitet, ist es nicht praktisch.

  Um die Ersetzung des Attributnamens für das oben beschriebene Beispiel durchzuführen, ändern Sie die **setGroupID** Spaltenüberschrift zu **#setGroupID GROUP***name**. Anschließend können Sie die Gruppe jedes Projekts nach Namen referenzieren.

  >[!NOTE]
  >
  >Die Option zur Verwendung der Attributnamenersetzung ist auf Verweise nur für vorhandene Datensätze beschränkt. Sie können die Namensersetzung nicht für Objekte verwenden, die Sie im selben Import erstellen.

* **(Benutzerimport)**

  Wenn Sie Benutzer importieren, füllen Sie die **setRoleID** aus einer Liste von Rollen auf der **ROLLROLLE** Registerkarte.

  Einige Rollen-IDs sind für Datensätze bestimmt, die bereits im Konto vorhanden sind, andere werden während des Imports erstellt.

  Für die neuen Benutzerdatensätze, die vorhandenen Rollen zugewiesen sind, können Sie die Namensersetzung verwenden. Für die neuen Benutzerdatensätze, die neu importierten Rollen zugewiesen sind, ist dies nicht möglich.

  So können Sie beide Methoden für dieselbe Importdatei verwenden:

   * Fügen Sie links im Arbeitsblatt eine Spalte hinzu **setRoleID** Spalte.
   * Benennen Sie die neue Spalte **#setRoleID ROLE name**.
   * Geben Sie für Rollenzuweisungen an vorhandene Datensätze die Rollennamen in die **#setRoleID ROLE name** Spalte.

     Geben Sie für Rollenzuweisungen an neue Rollendatensätze die ID ein, die Sie im Rollenblatt in setRoleID zugewiesen haben.

     ![Rolle-ID für Benutzer](assets/set-role-id.png)

## Importieren der Tabellenkalkulationsdaten in Workfront

Nachdem Sie die Excel-Vorlage mit Ihren Daten gefüllt haben, können Sie die Daten in Workfront hochladen.

Der Kick-Start-Import unterstützt die folgenden Dateitypen:

* XML-basiertes Excel (.xlsx)
* Ältere Excel-Dateien (.xls)
* Zip-Datei (.ZIP) (die nur .xlsx- oder .xls-Dateien enthält)

  >[!NOTE]
  >
  >Sie müssen beim Import von Excel-Arbeitsblättern, die auf die folgenden Objekte verweisen, eine ZIP-Datei verwenden:
  >
  >* Berichte
  >* Dokumente
  >* Avatare
  >* Eigenschaftendateien anzeigen, filtern oder gruppieren.
  >
  >Bei Verwendung einer komprimierten Importdatei muss die .ZIP-Datei denselben Namen wie die .xlsx- oder .xls-Datei haben und alle Dateien müssen sich auf derselben Strukturebene befinden (keine Ordner).

So importieren Sie die Tabellenkalkulationsvorlagen-Daten in Workfront:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **System** >**Daten importieren (Kick-Starts)**.

1. Im **Hochladen von Daten mit der Kick-Start-Tabelle** Abschnitt, klicken Sie auf **Datei auswählen**, suchen Sie dann die ausgefüllte Tabelle und wählen Sie sie aus.

1. Klicks **Hochladen.**

   Wenn das Hochladen der Excel-Datei in Workfront länger als 5 Minuten dauert, wird das Programm mit einem Timeout beendet und die Datei kann nicht hochgeladen werden.

   Versuchen Sie, Ihre Daten in kleineren Objektstapeln zu importieren.

1. (Bedingt) Wenn Sie Workfront Fusion verwenden, können Sie jetzt Ihre FLOs oder Szenarien aktivieren.
