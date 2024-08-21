---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Importieren von Daten in Workfront mithilfe einer Kick-Start-Vorlage
description: Kick-Starts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kick-Start-Vorlage, die Sie dazu verwenden können, wie unter Kick-Starts-Daten-Importer beschrieben.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '2753'
ht-degree: 6%

---

# Daten mithilfe einer Kick-Start-Vorlage in Workfront importieren

<!--Audited: 12/2023-->

Kick-Starts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kick-Start-Vorlage, die Sie dazu verwenden können, wie unter [Kick-Starts-Datenimport](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md) beschrieben.

Dieser Prozess ist in drei Hauptaufgaben unterteilt:

* Exportieren Sie zunächst eine Kick-Start-Vorlage als Tabellendatei
* Als zweites füllen Sie die Tabelle mit Ihren Daten
* Schließlich importieren Sie die ausgefüllte Tabelle in Workfront

Jedes dieser Verfahren wird in der richtigen Reihenfolge in diesem Artikel beschrieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p> Neu: Standard</p>
   oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einschränkungen

Mit einer Kick-Start-Vorlage können Sie eine große Anzahl von Objekten in Workfront importieren. Beachten Sie jedoch die folgenden Einschränkungen:

* Beim Datenimport auf diese Weise werden Informationen zu Datensätzen, die bereits in Workfront vorhanden sind, nicht aktualisiert.
* Sie können nur neue Datensätze und deren Informationen importieren.
* Importieren Sie nicht mehr als 2.000 Datensätze gleichzeitig, um sicherzustellen, dass beim Import keine Zeitüberschreitung auftritt

## Kick-Start-Vorlage als Tabellendatei exportieren

Wenn Sie eine Kick-Start-Vorlage exportieren, erhalten Sie eine leere Excel-Arbeitsmappe. Nachdem das Arbeitsblatt auf Ihren Computer heruntergeladen wurde, können Sie es verwenden, um Ihre Informationen einzutragen und sie dann wieder in Workfront zu importieren.

So exportieren Sie eine Kick-Start-Vorlage:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  -->

1. Klicken Sie auf **System** > **Daten importieren (Kick-Starts)**.

1. Wählen Sie die Informationstypen aus, die Sie einbeziehen möchten.

   Jede ausgewählte Option stellt eine Sammlung mehrerer Registerkarten im exportierten Arbeitsblatt dar. Wenn Sie beispielsweise die Option **Bericht** auswählen, werden alle zum Erstellen eines Berichts erforderlichen Objekte (Ansichten, Filter, Gruppierungen, Berichte) in die Tabelle aufgenommen.

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
      <td scope="col"> <p>Parameter</p> <p>Beschreibender Text</p><p>Parameteroption</p> <p>Parametergruppe</p> <p>Kategorieparameter</p> <p>Kategorie</p> <p>Bericht</p> <p>Portal-Registerkarten-Abschnitt</p> <p>Dashboard</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Bericht</p> <p>Alle Berichte im System können exportiert werden. Sie können bis zu 100 spezifische Berichte in einem Export auswählen.</p> <p>Kick-Starts unterstützt keine Textmodus-Filter. Für einen erfolgreichen Export müssen die Berichtsfilter in den Standardmodus umgestellt werden.</p> </td> 
      <td scope="col">Exportiert als ZIP-Datei </td> 
      <td scope="col"> <p scope="col">Parameter</p> <p scope="col">Beschreibender Text</p> <p scope="col">Parameteroption</p> <p scope="col">Parametergruppe</p> <p scope="col">Kategorieparameter</p> <p scope="col">Kategorie</p> <p scope="col">Bericht</p> <p scope="col">Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Genehmigung</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td scope="col"> <p>Genehmigende Person für Phase</p> <p>Genehmigungsphase</p> <p>Genehmigung</p> <p>Genehmigungsprozess</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Benutzerdefinierte Daten</p> </td> 
      <td scope="col"> <p>Exportiert als Excel-Datei</p> </td> 
      <td scope="col"> <p>Parameter</p> <p>Beschreibender Text</p>  <p>Parameteroption</p> <p>Parametergruppe</p> <p>Kategorieparameter</p> <p>Kategorie</p> <p>Einstellungen</p> </td> 
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
      <td> <p>Exportiert als Excel-Datei. Um die vollständige Liste der Optionen anzuzeigen, klicken Sie auf <strong>Mehr Optionen</strong>.</p> </td> 
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
      <td> <p> Ausgaben'</p> <p>Einstellungen </p> </td> 
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
      <td> <p>Scorecard-Frage</p> <p>Scorecard-Option</p> <p>Scorecard</p> <p>Einstellungen </p> </td> 
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

1. Klicken Sie auf **Herunterladen**.
1. Fahren Sie mit [Füllen Sie die Tabellenvorlage mit Ihren Daten](#populate-the-spreadsheet-template-with-your-data) fort, um das leere Vorlagensatzblatt mit Ihren Daten zu füllen.

## Füllen Sie die Tabellenvorlage mit Ihren Daten {#populate-the-spreadsheet-template-with-your-data}

* [Übersicht über die im Arbeitsblatt enthaltenen Registerkarten (Datenblätter)](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Import a record](#import-a-record)
* [Datum einschließen](#include-dates)
* [Verwenden Sie Platzhalter](#use-wildcards)
* [Wertersetzung für IDs durch Attributnamen](#attribute-name-substitution-for-ids)

### Übersicht über die im Arbeitsblatt enthaltenen Registerkarten (Datenblätter)

>[!TIP]
>
>Um besser zu verstehen, wie Sie die Informationen in den einzelnen Spalten formatieren müssen, wenn Sie die Kick-Start-Vorlage füllen, sollten Sie eine Übung durchführen, indem Sie einen Kick-Start mit vorhandenen Workfront-Daten zu den Objekten exportieren, die Sie importieren möchten. Anweisungen finden Sie unter [Exportieren von Daten aus Adobe Workfront über Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Wenn Sie eine leere Kick-Starts-Vorlage öffnen, sind verschiedene Registerkarten (Datenblätter) verfügbar. Sie hängen von den Objekten ab, die Sie zum Herunterladen ausgewählt haben. Jedes Objekt stellt ein Objekt in der Anwendung dar, z. B. Projekt, Aufgaben, Stunden, Dashboard und Benutzer:

Wenn Sie eine dieser Registerkarten öffnen, zeigt Zeile 2 die Felder für jedes Objekt an, das während eines Imports festgelegt werden kann. In einer Spaltenüberschrift wird nach dem Wort &quot;set&quot;der Name des Felds so angezeigt, wie er in der Datenbank angezeigt wird. Diese Felder dienen als Spaltenüberschriften.

>[!IMPORTANT]
>
>Um Fehler zu vermeiden, stellen Sie Folgendes sicher:
>
>* Löschen Sie nicht die leere erste Zeile einer Kick-Start-Tabelle.
>* Löschen, ändern oder ordnen Sie diese Felder (Spaltenüberschriften) nicht neu an. Ändern Sie beispielsweise nicht die Reihenfolge oder den Namen.
>* Fügen Sie jedem Feld, das in der Spaltenüberschrift fett dargestellt wird, Werte hinzu. Diese stellen erforderliche Felder dar.
>
>     Wenn ein erforderliches Feld jedoch einen in den Systemvoreinstellungen festgelegten Standardwert enthält, müssen Sie ihn nicht ausfüllen.
>
>     Auf der Registerkarte **PROJ-Projekt** können beispielsweise die Felder **setCondition** und **setConditionType** leer gelassen werden, die Spalten **setGroupID** und **setName** jedoch nicht.
>
>* Bestimmte Felder, einschließlich **setResourceRevenue** und **setEnteredByID**, werden automatisch vom System generiert. Wenn Sie Daten für diese Felder in das Arbeitsblatt eingeben, werden diese beim Hochladen des Arbeitsblatts durch den Kick-Start-Prozess überschrieben.

### Datensatz importieren  {#import-a-record}

Jede Tabellenzeile entspricht einem eindeutigen Objekt.

1. Fügen Sie Informationen in die Spalte **isNew** ein:

   * Wenn das Objekt, das Sie importieren, neu ist, geben Sie **TRUE** ein, um die Daten in die Zeile zu importieren. Bei diesem Wert wird zwischen Groß- und Kleinschreibung unterschieden. Dabei muss es sich immer um Großbuchstaben handeln
   * Wenn sich das Objekt bereits in Workfront befindet, geben Sie **FALSE** in die Spalte **isNew** ein, um die Zeile zu ignorieren. Bei diesem Wert wird zwischen Groß- und Kleinschreibung unterschieden. Dabei muss es sich immer um Großbuchstaben handeln

      * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
      * Wenn Sie eine Vorlage mit Daten aus Workfront heruntergeladen haben, sind vorhandene Objekte bereits mit **FALSE** markiert.
      * Wenn Sie eine leere Vorlage heruntergeladen haben, müssen Sie keine neuen Zeilen für vorhandene Objekte hinzufügen.

1. Fügen Sie Informationen in der Spalte **ID** auf eine der folgenden Arten hinzu:

   * Wenn das Objekt, das Sie importieren, neu ist (und Sie **TRUE** in die Spalte **isNew** eingegeben haben), geben Sie eine beliebige Zahl für die ID ein. Diese Nummer muss im Arbeitsblatt eindeutig sein. Wenn Sie beispielsweise drei Objekte importieren, können Sie ihnen die Kennung 1, 2, 3 zuweisen.

   * Wenn das Objekt bereits in Workfront vorhanden ist (und sich **FALSE** in der Spalte **isNew** befindet) und Sie neue Informationen über vorhandene Objekte importieren, muss die ID die alphanumerische GUID sein, die in Workfront für dieses Objekt vorhanden ist.

   >[!TIP]
   >
   > Um die eindeutige GUID eines Objekts in Workfront zu ermitteln, können Sie einen Bericht für dieses Objekt erstellen und die Spalte ID zum Bericht hinzufügen. Der Wert für jedes Objekt in dieser Spalte ist die GUID des Objekts.

   * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
   * Wenn Sie eine Vorlage mit Daten heruntergeladen haben, enthalten vorhandene Objekte bereits die GUID als ID.
   * Sie können ein neues Objekt importieren, das auf einem vorhandenen Objekt basiert, indem Sie **FALSE** in **TRUE** in der Spalte **isNew** ändern, die ID ändern und die erforderlichen Datenanpassungen vor dem Import vornehmen.

   ![Beispiel-ID für eine Gruppe](assets/kick-start-group-example.png)

   * Beim Importieren eines Projekts müssen Sie eine Gruppen-ID angeben.

      * Wenn die Gruppe bereits in Workfront vorhanden ist, müssen Sie ihre eindeutige ID dem Feld **setGroupID** für das Projekt hinzufügen.
      * Wenn die Gruppe nicht in Workfront vorhanden ist, können Sie das Blatt **GRUPPENgruppe** zu Ihrer Importdatei hinzufügen, das Feld **isNew** auf **TRUE** im Gruppenblatt setzen und eine numerische ID für die neue Gruppe in der Spalte **ID** angeben. Das Feld **setGroupID** für das neue Projekt muss mit der numerischen **ID** für die neue Gruppe übereinstimmen.

     **Beispiel:** Für ein Projekt muss der in der Spalte **setGroupID** angezeigte Wert einer der folgenden sein:

      * Die GUID für eine bestehende Gruppe in Ihrer Workfront-Instanz
      * Der Wert (Zahl) in der Spalte &quot;ID&quot;im Blatt **GRUPPENgruppe** , wenn Sie beim Import eine neue Gruppe erstellen

1. Geben Sie Werte für die erforderlichen Felder und alle anderen Felder ein, die während des Imports ausgefüllt werden sollen.
1. (Optional) So fügen Sie benutzerdefinierte Daten hinzu:

   * Erstellen Sie für jedes benutzerdefinierte Feld, das Sie in den Importprozess einbeziehen möchten, eine neue Spalte.
   * Benennen Sie jede neue Spalte für das entsprechende benutzerdefinierte Feld wie folgt: **DE:[Name des benutzerdefinierten Felds, wie es in Workfront]** angezeigt wird. Sie können beispielsweise das folgende benutzerdefinierte Feld erstellen: &quot;DE: Departments&quot;.
   * Geben Sie in die Spalte **setCategoryID** die GUID des vorhandenen benutzerdefinierten Formulars ein, in dem sich dieses benutzerdefinierte Feld befindet. Dieses Feld ist beim Import benutzerdefinierter Daten erforderlich.
   * Wenn Sie mehrere Datenwerte in das benutzerdefinierte Feld hinzufügen müssen (z. B. Optionsfelder, Kontrollkästchen oder Listen), verwenden Sie das auf der Registerkarte Voreinstellungen aufgelistete benutzerdefinierte Trennzeichen für die vertikale Leiste &quot;|&quot;, um die Werte zu trennen.

     **Beispiel:** Geben Sie A|D unter der Spalte DE:Departments ein, um Abteilung A und Abteilung D in Ihr benutzerdefiniertes Formular einzutragen.

### Datum einschließen  {#include-dates}

Workfront kann die meisten Datumsformate verarbeiten. Sie müssen jedoch sicherstellen, dass die Datumsspalte im Arbeitsblatt als Datum formatiert ist. Der Import schlägt fehl, wenn die Spalte als Allgemein, Zahl oder Text formatiert ist.

>[!TIP]
>
>Das beliebteste Format ist das Format MM/TT/JJJJ.
>
>Beispiel: 10.07.2023.

Workfront akzeptiert auch Zeitwerte als Teil des Datums.

Beispiel: 07/10/2022 01:30 oder 07/10/2022 1:00 PM.

Wenn Sie einen Zeitpunkt im Datum weglassen, führt Workfront einen der folgenden Schritte aus:

* Es wird angenommen, dass die Zeit 12:00 Uhr ist. Um das erwartete Datumsergebnis zu sehen, muss die Systemzeitzone mit Ihrer Zeitzone übereinstimmen.
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
   <td> <p>Bei Verwendung in einem <strong>setDate</strong> -Feld legt dieser Platzhalter das Datum an dem Tag, an dem Sie den Kick-Start importieren, als Mitternacht fest.</p> <p>Sie können den Platzhalter mit der in einem Filter zulässigen Standardsyntax ändern.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie möchten, dass ein Projekt am Montag der Woche beginnt, an dem es importiert wird, können Sie <strong>$$TODAYbw</strong> verwenden, unabhängig vom Tag, an dem Sie den Import tatsächlich durchführen. Dadurch wird das geplante Startdatum Ihres Projekts auf Sonntag um 12:00 Uhr festgelegt. Da der Zeitplan für das Projekt zu diesem Zeitpunkt wahrscheinlich keine Arbeit zulässt, wird er um 9:00 Uhr morgens beginnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Bei Verwendung in einem Feld <strong>setDate</strong> legt dieser Platzhalter das Datum entsprechend dem Zeitpunkt fest, zu dem Sie den Datensatz während des Kick-Start-Imports erstellen.</p> <p>Sie können den Platzhalter mit der in einem Filter zulässigen Standardsyntax ändern.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie möchten, dass ein Projekt drei Stunden nach dem Import gestartet wird, können Sie <strong>$$NOW+3h</strong> verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Bei Verwendung in einem <strong>setAssignedToID</strong>- oder einem anderen auf der Benutzer-ID basierenden Feld weist dieser Platzhalter die Arbeit zu oder ordnet den Datensatz anderweitig der Person zu, die den Import durchführt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Dieser Platzhalter wurde speziell für Kick-Start-Benutzerimporte hinzugefügt. Wenn ein Workfront-Konto erstellt wird, wird ein Benutzer mit der Zugriffsebene "Systemadministrator"erstellt. Der dem Standardadministrator zugewiesene Benutzername kann beim Erstellen anderer Benutzer in dem Konto als Präfix verwendet werden.</p> <p>Da Benutzernamen für alle Kunden eindeutig sein müssen, ist dies nützlich, wenn Sie mehrere Personen mit sehr häufigen Benutzernamen haben, z. B. John Smith, der den Benutzernamen "jsmith"haben könnte. Indem Sie der Zuweisung des Benutzernamens den standardmäßigen Administrator-Benutzernamen voranstellen, garantieren Sie, dass jeder Benutzername eindeutig ist (z. B.: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Tipp: Eine elegantere Möglichkeit, sicherzustellen, dass Benutzernamen systemweit eindeutig sind, besteht darin, die E-Mail-Adresse des Kontakts in das Feld <strong>setUsername</strong> einzugeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Wertersetzung für IDs durch Attributnamen  {#attribute-name-substitution-for-ids}

Obwohl es sich nach Möglichkeit empfiehlt, IDs zu verwenden, ist es manchmal nicht praktisch, beim Festlegen eines **setAttributeID** -Werts zwischen den Tabellenblättern zu verweisen. Sie können Werte nach Namen referenzieren, indem Sie einfach die Spaltenüberschrift ändern.

**Beispiele:**

* **Projektimport**

  Legen Sie beim Importieren von Projekten die **setGroupID** der Projekte fest, indem Sie das Blatt **GROUP Group** aufrufen, die entsprechenden Gruppen-IDs notieren und sie in die richtigen Zellen (**setGroupID** -Spalte) auf dem Blatt **PROJ Project** einfügen.

  Dies ist möglich, wenn man nur mit wenigen Gruppen und Projekten arbeitet, aber wenn man mit mehreren von ihnen arbeitet, ist es nicht praktisch.

  Um die Ersetzung des Attributnamens für das oben beschriebene Beispiel durchzuführen, ändern Sie die Spaltenüberschrift **setGroupID** in die Spaltenüberschrift **#setGroupID GROUP name**. Anschließend können Sie die Gruppe jedes Projekts nach Namen referenzieren.

  >[!NOTE]
  >
  >Die Option zur Verwendung der Attributnamenersetzung ist auf Verweise nur für vorhandene Datensätze beschränkt. Sie können die Namensersetzung nicht für Objekte verwenden, die Sie im selben Import erstellen.

* **Benutzerimport**

  Füllen Sie beim Importieren von Benutzern die Variable **setRoleID** aus einer Liste von Rollen auf der Registerkarte **ROLE Role** aus.

  Einige Rollen-IDs sind für Datensätze bestimmt, die bereits im Konto vorhanden sind, andere werden während des Imports erstellt.

  Für die neuen Benutzerdatensätze, die vorhandenen Rollen zugewiesen sind, können Sie die Namensersetzung verwenden. Für die neuen Benutzerdatensätze, die neu importierten Rollen zugewiesen sind, ist dies nicht möglich.

  So können Sie beide Methoden für dieselbe Importdatei verwenden:

   * Fügen Sie links neben der Spalte **setRoleID** eine Spalte im Arbeitsblatt hinzu.
   * Nennen Sie die neue Spalte &quot;**#setRoleID ROLE name**&quot;.
   * Geben Sie für Rollenzuweisungen zu vorhandenen Datensätzen die Rollennamen in die Spalte **#setRoleID ROLE name** ein.

     Geben Sie für Rollenzuweisungen an neue Rollendatensätze die ID ein, die Sie im Rollenblatt in setRoleID zugewiesen haben.

     ![Rollen-ID für Benutzer](assets/set-role-id.png)

## Importieren der Tabellenkalkulationsdaten in Workfront

Nachdem Sie die Excel-Vorlage mit Ihren Daten ausgefüllt haben, können Sie deren Daten in Workfront hochladen.

Der Kick-Start-Import unterstützt die folgenden Dateitypen:

* Excel (.xls oder .xlsx)
* Zip-Datei (.ZIP) (die nur .xlsx- oder .xls-Dateien enthält)

  >[!NOTE]
  >
  >Sie müssen beim Import von Excel-Arbeitsblättern, die auf die folgenden Objekte verweisen, eine ZIP-Datei verwenden:
  >
  >* Berichte
  >* Dokumente
  >* Avatare
  >* Eigenschaftendateien anzeigen, filtern oder gruppieren
  >
  >Bei Verwendung einer komprimierten Importdatei muss die .ZIP-Datei denselben Namen wie die .xlsx- oder .xls-Datei haben und alle Dateien müssen sich auf derselben Strukturebene befinden (keine Ordner).

So importieren Sie die Tabellenkalkulationsvorlagen-Daten in Workfront:

<!--1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Daten importieren (Kick-Starts)**.

1. Klicken Sie im Abschnitt **Daten mit Kick-Start-Tabelle hochladen** auf **Datei auswählen** und suchen Sie dann nach der ausgefüllten Tabelle und wählen Sie sie aus.

1. Klicken Sie auf **Hochladen.**

   Wenn das Hochladen der Excel-Datei in Workfront länger als 5 Minuten dauert, wird das Programm mit einer Zeitüberschreitung beendet und Workfront kann die Datei nicht hochladen.

   Versuchen Sie, Ihre Daten in kleineren Objektstapeln zu importieren.

1. (Bedingt) Wenn Sie Workfront Fusion verwenden, können Sie jetzt Ihre FLOs oder Szenarien aktivieren.
