---
user-type: administrator
product-area: system-administration
keywords: Kickstart,Kickstart,Kickstarts,Kickstarts
navigation-topic: use-kick-starts
title: Importieren von Daten in Workfront mithilfe einer Kickstart-Vorlage
description: Kickstarts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kickstart-Vorlage, die Sie dazu verwenden können, wie unter Kickstarts-Datenimport beschrieben.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 4c80802c8e0084aa9e7be350caefc8929c9c4e2b
workflow-type: tm+mt
source-wordcount: '2785'
ht-degree: 6%

---

# Daten mithilfe einer Kickstart-Vorlage in Workfront importieren

<!--Audited: 12/2023-->

Kickstarts sind speziell formatierte Excel-Arbeitsmappen, die Sie mit Daten füllen können, die Sie in Workfront importieren möchten. Adobe Workfront bietet eine Kickstart-Vorlage, die Sie dazu verwenden können, wie unter [Kickstarts-Datenimportprogramm“ ](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Dieser Prozess ist in drei Hauptaufgaben unterteilt:

* Exportieren Sie zunächst eine Kickstart-Vorlage als Tabellendatei
* Zweitens füllen Sie die Tabelle mit Ihren Daten
* Schließlich importieren Sie die ausgefüllte Tabelle in Workfront

Jedes dieser Verfahren wird in der richtigen Reihenfolge in diesem Artikel beschrieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p> Neu: Standard</p>
   oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einschränkungen

Sie können mithilfe einer Kickstart-Vorlage eine große Anzahl von Objekten in Workfront importieren. Beachten Sie jedoch die folgenden Einschränkungen:

* Durch das Importieren von Daten auf diese Weise werden Informationen zu Datensätzen, die bereits in Workfront vorhanden sind, nicht aktualisiert.
* Sie können nur neue Datensätze und deren Informationen importieren.
* Importieren Sie maximal 2.000 Datensätze gleichzeitig, um sicherzustellen, dass beim Import keine Zeitüberschreitung auftritt

## Kickstart-Vorlage als Tabellendatei exportieren

Wenn Sie eine Kickstart-Vorlage exportieren, erhalten Sie eine leere Excel-Kalkulationstabellen-Arbeitsmappe. Nachdem die Tabelle auf Ihren Computer heruntergeladen wurde, können Sie sie verwenden, um Ihre Informationen einzutragen und sie dann wieder in Workfront zu importieren.

Kickstart-Vorlage exportieren:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. Klicken Sie **System** > **Daten importieren (Kickstarts)**.

1. Wählen Sie die Informationstypen aus, die Sie einbeziehen möchten.

   Jede von Ihnen ausgewählte Option stellt eine Sammlung mehrerer Registerkarten im exportierten Arbeitsblatt dar. Wenn Sie beispielsweise die Option **Bericht** auswählen, werden alle erforderlichen Objekte zum Erstellen eines Berichts in die Tabelle aufgenommen (Ansichten, Filter, Gruppierungen, Berichte).

   Sie können alle unten aufgeführten Objekttypen verwenden, um Daten in Workfront zu importieren. (Die einzige Ausnahme ist die Option Zugriffsebenen . Das Datenblatt „Zugriffsebenen“ in einem Export wird zu Referenzzwecken bereitgestellt - es ermöglicht Ihnen, einem neuen Benutzerkonto eine Zugriffsebene per ID zuzuweisen.)

   Die Vorlage für jeden Objekttyp kann in den folgenden Dateiformaten exportiert werden und enthält die folgenden Blätter:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objekt</strong> </p> </th> 
      <th> <p><strong>Exportiert als</strong> </p> </th> 
      <th> <p><strong>Tabellen in der exportierten Tabelle</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Dashboard</p> <p>Alle öffentlich freigegebenen Dashboards im System können exportiert werden. Dashboards, die nicht systemweit freigegeben sind, können nicht exportiert werden. Sie können in einem Export bis zu 100 spezifische Dashboards auswählen.</p> </td> 
      <td scope="col">Exportiert als ZIP-Datei</td> 
      <td scope="col"> <p>Parameter</p> <p>Beschreibender Text</p><p>Parameteroption</p> <p>Parametergruppe</p> <p>Kategorieparameter</p> <p>Kategorie</p> <p>Bericht</p> <p>Portal-Registerkarten-Abschnitt</p> <p>Dashboard</p> <p>Einstellungen</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Bericht</p> <p>Alle Berichte im System können exportiert werden. Sie können bis zu 100 spezifische Berichte in einem Export auswählen.</p> <p>Kickstarts unterstützen keine Textmodusfilter oder Gruppierungen. Für einen erfolgreichen Export müssen die Berichtsfilter und Gruppierungen in den Standardmodus umgeschaltet werden.</p> </td> 
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
      <td> <p> Kosten“</p> <p>Einstellungen </p> </td> 
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
      <td> <p> Aufgabengebiet</p> <p>Einstellungen </p> </td> 
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

1. Klicken Sie **Herunterladen**.
1. Fahren Sie mit [Kalkulationstabellenvorlage mit Ihren Daten füllen](#populate-the-spreadsheet-template-with-your-data) fort, um die leere Vorlagenkalkulationstabelle mit Ihren Informationen zu füllen.

## Füllen Sie die Tabellenvorlage mit Ihren Daten {#populate-the-spreadsheet-template-with-your-data}

* [Übersicht über die in der Tabelle enthaltenen Registerkarten (Datenblätter)](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Datensatz importieren](#import-a-record)
* [Daten einschließen](#include-dates)
* [Verwenden von Platzhaltern](#use-wildcards)
* [Ersetzung von IDs durch Attributnamen](#attribute-name-substitution-for-ids)

### Übersicht über die in der Tabelle enthaltenen Registerkarten (Datenblätter)

>[!TIP]
>
>Um besser zu verstehen, wie Sie die Informationen in den einzelnen Spalten formatieren müssen, wenn Sie die Kickstart-Vorlage ausfüllen, sollten Sie einen Übungslauf durchführen, indem Sie einen Kickstart mit den vorhandenen Workfront-Daten zu den Objekten exportieren, die Sie importieren möchten. Anweisungen finden Sie unter [Exportieren von Daten aus Adobe Workfront über Kickstarts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Wenn Sie eine leere Kick-Starts-Vorlage öffnen, stehen eine Reihe von Registerkarten (Datenblätter) zur Verfügung. Sie hängen von den Objekten ab, die Sie zum Herunterladen ausgewählt haben. Jede Komponente stellt ein Objekt in der Anwendung dar, z. B. Projekt, Aufgaben, Stunden, Dashboard und Benutzer:

Wenn Sie eine dieser Registerkarten öffnen, zeigt Zeile 2 die Felder für jedes Objekt an, das während eines Imports festgelegt werden kann. In einer Spaltenüberschrift wird nach dem Wort „set“ der Name des Felds so angezeigt, wie er in der Datenbank angezeigt wird. Diese Felder dienen als Spaltenüberschriften.

>[!IMPORTANT]
>
>Um Fehler zu vermeiden, stellen Sie Folgendes sicher:
>
>* Löschen Sie nicht die leere erste Zeile einer Kickstart-Tabelle.
>* Diese Felder (Spaltenüberschriften) dürfen in keiner Weise gelöscht, geändert oder neu angeordnet werden. Ändern Sie beispielsweise weder ihre Reihenfolge noch ihren Namen.
>* Fügen Sie Werte zu jedem Feld hinzu, das in der Spaltenüberschrift fett dargestellt wird. Diese stellen Pflichtfelder dar.
>
>     Wenn ein Pflichtfeld jedoch einen in den Systemeinstellungen festgelegten Standardwert enthält, müssen Sie ihn nicht ausfüllen.
>
>     Auf der Registerkarte **PROJ-Projekt** können beispielsweise die Felder **setCondition** und **setConditionType** leer gelassen werden, die Spalten **setGroupID** und **setName** jedoch nicht.
>
>* Bestimmte Felder, einschließlich **setResourceRevenue** und **setEnteredByID**, werden automatisch vom System generiert. Wenn Sie Daten für diese Felder in das Arbeitsblatt eingeben, wird der Kickstart-Prozess diese Daten beim Hochladen des Arbeitsblatts überschreiben.

### Datensatz importieren  {#import-a-record}

Jede Zeile des Blatts entspricht einem eindeutigen Objekt.

1. Fügen Sie Informationen in der Spalte **isNew** hinzu:

   * Wenn das zu importierende Objekt neu ist, geben Sie **TRUE** ein, um die Daten in die Zeile zu importieren. Bei diesem Wert wird zwischen Groß- und Kleinschreibung unterschieden. Er muss immer in Großbuchstaben geschrieben werden
   * Wenn sich das Objekt bereits in Workfront befindet, geben Sie **FALSE** in die Spalte **isNew** ein, um die Zeile zu ignorieren. Bei diesem Wert wird zwischen Groß- und Kleinschreibung unterschieden. Er muss immer in Großbuchstaben geschrieben werden

      * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
      * Wenn Sie eine Vorlage mit Daten aus Workfront heruntergeladen haben, sind vorhandene Objekte bereits mit &quot;**&quot;**.
      * Wenn Sie eine leere Vorlage heruntergeladen haben, müssen Sie keine neuen Zeilen für vorhandene Objekte hinzufügen.

1. Fügen Sie Informationen in der Spalte **ID** auf eine der folgenden Arten hinzu:

   * Wenn das zu importierende Objekt neu ist (und Sie **„TRUE** in der Spalte **isNew** eingegeben haben), geben Sie eine beliebige Zahl für die ID ein. Diese Zahl muss in der Tabelle eindeutig sein. Wenn Sie beispielsweise drei Objekte importieren, können Sie ihnen die ID 1, 2 bzw. 3 zuweisen.

   * Wenn das Objekt bereits in Workfront vorhanden ist (und **FALSE** sich in der Spalte **isNew** befindet) und Sie neue Informationen über vorhandene Objekte importieren, muss die ID die alphanumerische GUID sein, die in Workfront für dieses Objekt vorhanden ist.

   >[!TIP]
   >
   > Um die eindeutige GUID eines Objekts in Workfront zu ermitteln, können Sie einen Bericht für dieses Objekt erstellen und die ID-Spalte zum Bericht hinzufügen. Der Wert für jedes Objekt in dieser Spalte ist die GUID des -Objekts.

   * Datensätze, die bereits in Workfront vorhanden sind, werden nicht aktualisiert.
   * Wenn Sie eine Vorlage mit Daten heruntergeladen haben, enthalten vorhandene Objekte bereits die GUID als ID.
   * Sie können ein neues Objekt importieren, das auf einem vorhandenen Objekt basiert, indem Sie **FALSE** in der Spalte **isNew** in **TRUE** ändern, die ID ändern und vor dem Import die erforderlichen Datenanpassungen vornehmen.

   ![Beispiel-ID für eine Gruppe](assets/kick-start-group-example.png)

   * Beim Importieren eines Projekts müssen Sie eine Gruppen-ID angeben.

      * Wenn die Gruppe bereits in Workfront vorhanden ist, müssen Sie ihre eindeutige ID zum Feld **setGroupID** für das Projekt hinzufügen.
      * Wenn die Gruppe in Workfront nicht vorhanden ist, können Sie das Blatt **GROUP** zu Ihrer Importdatei hinzufügen, das Feld **isNew** auf **TRUE** auf dem Gruppenblatt festlegen und in der Spalte **ID** eine numerische ID für die neue Gruppe angeben. Das Feld **setGroupID** für das neue Projekt muss mit der numerischen **ID** für die neue Gruppe übereinstimmen.

     **Beispiel** Für ein Projekt muss der in der Spalte **setGroupID** angezeigte Wert einer der folgenden sein:

      * Die GUID für eine bestehende Gruppe in Ihrer Workfront-Instanz
      * Der Wert (Zahl) in der Spalte ID auf dem Blatt **Gruppe**, wenn Sie beim Import eine neue Gruppe erstellen

1. Geben Sie Werte für die erforderlichen Felder und alle anderen Felder ein, die Sie während des Imports ausfüllen möchten.
1. (Optional) So fügen Sie benutzerdefinierte Daten hinzu:

   * Erstellen Sie für jedes benutzerdefinierte Feld, das Sie in den Importprozess einbeziehen möchten, eine neue Spalte.
   * Benennen Sie jede neue Spalte für das entsprechende benutzerdefinierte Feld wie folgt: **DE:[Name des benutzerdefinierten Felds, wie es in Workfront angezeigt wird]**. Sie können beispielsweise das folgende benutzerdefinierte Feld erstellen: „DE: Departments“.
   * Geben Sie in die Spalte **setCategoryID** die GUID des vorhandenen benutzerdefinierten Formulars ein, in dem sich dieses benutzerdefinierte Feld befindet. Dieses Feld ist beim Import von benutzerdefinierten Daten erforderlich.
   * Wenn Sie mehrere Datenwerte in dem benutzerdefinierten Feld hinzufügen müssen (z. B. Optionsfelder, Kontrollkästchen oder Listen), verwenden Sie das vertikale Balken-Trennzeichen für benutzerdefinierte Daten &quot;|&quot;, das auf der Registerkarte „Voreinstellungen“ aufgeführt ist, um die Werte zu trennen.

     **Beispiel:** Geben Sie A|D unter der Spalte DE:Departments ein, um Abteilung A und Abteilung D in Ihrem benutzerdefinierten Formular auszufüllen.

     >[!NOTE]
     >
     >Verwenden Sie nur das Trennzeichen &quot;|&quot;, um benutzerdefinierte Feldwerte zu trennen. Sie können sie in keiner der anderen Tabellenspalten verwenden, einschließlich **setCategoryID**.

### Daten einschließen  {#include-dates}

Workfront kann die meisten Datumsformate verarbeiten. Sie müssen jedoch sicherstellen, dass die Datumsspalte in der Tabelle als Datum formatiert ist. Der Import schlägt fehl, wenn die Spalte als Allgemein, Zahl oder Text formatiert ist.

>[!TIP]
>
>Das beliebteste Format ist das Format MM/TT/JJJJ.
>
>Beispiel: 07/10/2023.

Workfront akzeptiert auch Zeitwerte als Teil des Datums.

Beispiel: 07/10/2022 13:30 oder 07/10/2022 13:00 Uhr.

Wenn Sie eine Uhrzeit im Datum auslassen, führt Workfront einen der folgenden Schritte aus:

* Angenommen, die Zeit ist um 00:00 Uhr. Um das erwartete Datumsergebnis sehen zu können, muss die Systemzeitzone mit Ihrer Zeitzone übereinstimmen.
* Wenn er sich auf einem Objekt befindet, das mit einem Zeitplan verknüpft ist, bezieht sich die Zeit auf die früheste Zeit, die der Zeitplan zulässt.

>[!NOTE]
>
>Bei Verwendung eines UNIX-Zeitstempels müssen Sie drei zusätzliche Nullen am Ende des Werts angeben.
>
>Wenn Ihr Zeitstempel beispielsweise 7336899000 ist, geben Sie 7336899000000 in die Zelle ein.

### Platzhalter verwenden {#use-wildcards}

Sie können beim Ausfüllen Ihrer Kickstart-Vorlage die folgenden Platzhalter verwenden:

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
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Bei Verwendung in einem <strong>setDate</strong>-Feld legt dieser Platzhalter das Datum als Mitternacht am Tag des Kickstarts fest.</p> <p>Sie können den Platzhalter mit der Standardsyntax ändern, die mit dem Platzhalter für einen Filter zulässig ist.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn ein Projekt am Montag der Woche starten soll, an der es importiert wird, können Sie <strong>$$TODAYbw verwenden, unabhängig davon, an welchem Tag Sie den Import tatsächlich durchführen</strong>. Damit wird das geplante Startdatum Ihres Projekts auf Sonntag, 12:00 Uhr festgelegt. Da der Zeitplan für das Projekt zu diesem Zeitpunkt wahrscheinlich keine Arbeit zulässt, wird es um 9:00 Uhr Montagmorgen beginnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Bei Verwendung in einem <strong>setDate</strong>-Feld legt dieser Platzhalter das Datum entsprechend dem Zeitpunkt fest, zu dem Sie den Datensatz während des Kickstart-Imports erstellen.</p> <p>Sie können den Platzhalter mit der Standardsyntax ändern, die mit dem Platzhalter für einen Filter zulässig ist.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn ein Projekt 3 Stunden nach dem Import gestartet werden soll, können Sie <strong>$$NOW+3h verwenden</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Bei Verwendung in einem <strong>setAssignedToID</strong> oder einem anderen auf userID basierenden Feld weist dieser Platzhalter die Arbeit zu oder verknüpft den Datensatz anderweitig mit der Person, die den Import durchführt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Dieser Platzhalter wurde speziell für Kickstart-Benutzerimporte hinzugefügt. Beim Erstellen eines Workfront-Kontos wird ein Benutzer mit der Zugriffsebene „Systemadministrator“ erstellt. Der dem Standardadministrator zugewiesene Benutzername kann beim Erstellen anderer Benutzer im Konto als Präfix verwendet werden.</p> <p>Da Benutzernamen für alle Kunden eindeutig sein müssen, ist dies nützlich, wenn Sie mehrere Personen mit sehr gängigen Benutzernamen wie John Smith haben, die möglicherweise den Benutzernamen „jsmith“ haben. Indem Sie der Benutzernamenzuweisung den standardmäßigen Administrator-Benutzernamen voranstellen, garantieren Sie, dass jeder Benutzername eindeutig ist (z. B.: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Tipp: Eine elegantere Methode, um sicherzustellen, dass Benutzernamen systemweit eindeutig sind, besteht darin, die E-Mail-Adresse des Kontakts in das Feld <strong>setUsername</strong> einzugeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ersetzung von IDs durch Attributnamen  {#attribute-name-substitution-for-ids}

Obwohl es sich als Best Practice empfiehlt, nach Möglichkeit immer IDs zu verwenden, ist es manchmal unpraktisch, IDs von einem Blatt zum anderen zu vergleichen, wenn ein Wert **setAttributeID** festgelegt wird. Sie können Werte anhand des Namens referenzieren, indem Sie einfach die Spaltenüberschrift ändern.

**Beispiele:**

* **Projektimport**

  Legen Sie beim Importieren von Projekten die **setGroupID** der Projekte fest, indem Sie zum Blatt **GROUP** wechseln, die entsprechenden Gruppen-IDs notieren und sie in die richtigen Zellen (Spalte **setGroupID**) in das Blatt **PROJ Project** einfügen.

  Dies ist möglich, wenn Sie nur mit wenigen Gruppen und Projekten arbeiten, aber wenn Sie mit mehreren von jedem arbeiten, ist dies nicht praktisch.

  Um die Ersetzung durch den Attributnamen für das oben beschriebene Beispiel durchzuführen, ändern Sie die Spaltenüberschrift **setGroupID** in **#setGroupIDGRUPPENNAME**. Sie können dann nach Namen auf die Gruppe der einzelnen Projekte verweisen.

  >[!NOTE]
  >
  >Die Option zur Verwendung der Attributnamensersetzung ist auf Verweise für vorhandene Datensätze beschränkt. Sie können keine Namensersetzung für Objekte verwenden, die Sie im selben Import erstellen.

* **Benutzerimport**

  Füllen Sie beim Importieren von Benutzenden **setRoleID** auf der Registerkarte **ROLE** aus einer Liste von Rollen aus.

  Einige der Rollen-IDs sind für Datensätze vorgesehen, die bereits im Konto vorhanden sind, andere werden während des Imports erstellt.

  Für neue Benutzerdatensätze, die vorhandenen Rollen zugewiesen sind, können Sie die Namensersetzung verwenden. Für die neuen Benutzerdatensätze, die neu importierten Rollen zugewiesen wurden, ist dies nicht möglich.

  So können Sie beide Methoden für dieselbe Importdatei verwenden:

   * Fügen Sie in der Tabelle links neben der Spalte **setRoleID“ eine Spalte**.
   * Benennen Sie die neue Spalte mit dem Namen &lbrace;0#setRoleIDROLE **.**
   * Für Rollenzuweisungen zu vorhandenen Datensätzen geben Sie die Rollennamen in die Spalte **#setRoleID** ein.

     Für Rollenzuweisungen zu neuen Rollendatensätzen geben Sie die ID ein, die Sie auf dem Funktionsblatt in der setRoleID zugewiesen haben.

     ![Rollen-ID für Benutzer](assets/set-role-id.png)

## Importieren der Tabellendaten in Workfront

Nachdem Sie die Excel-Vorlage mit Ihren Daten gefüllt haben, können Sie deren Daten in Workfront hochladen.

Der Kickstart-Import unterstützt die folgenden Dateitypen:

* Excel (.xls oder .xlsx)
* ZIP-Datei (die nur XLSX- oder XLS-Dateien enthält)

  >[!NOTE]
  >
  >Sie müssen beim Importieren von Excel-Tabellen, die auf die folgenden Objekte verweisen, eine ZIP-Datei verwenden:
  >
  >* Berichte
  >* Dokumente
  >* Avatare
  >* Anzeigen, Filtern oder Gruppieren von Eigenschaftendateien
  >
  >Bei Verwendung einer komprimierten Importdatei muss die ZIP-Datei denselben Namen haben wie die XLSX- oder XLS-Datei, und alle Dateien müssen sich auf derselben Strukturebene befinden (keine Ordner).

So importieren Sie die Tabellenkalkulationsvorlagendaten in Workfront:

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Klicken Sie **System** > **Daten importieren (Kickstarts)**.

1. Klicken Sie **Abschnitt Daten mit Kickstart-** hochladen auf **Datei auswählen** navigieren Sie dann zu und wählen Sie das ausgefüllte Arbeitsblatt aus.

1. Klicken Sie auf **Hochladen.**

   Wenn das Hochladen der Excel-Datei in Workfront länger als 5 Minuten dauert, tritt ein Timeout der Anwendung auf, und Workfront kann die Datei nicht hochladen.

   Importieren Sie Ihre Daten in kleinere Objektstapel.

1. (Bedingt) Wenn Sie Workfront Fusion verwenden, können Sie jetzt Ihre FLOs oder Szenarien aktivieren.
