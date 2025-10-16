---
title: Bericht zum Bereich „Aktualisierungen“ mit einem Journaleintragsbericht
description: Systemaktualisierungen für Journaleinträge werden im Bereich Aktualisierungen von Projekten, Aufgaben, Problemen und anderen Objekten angezeigt, die zuvor nur über die Adobe Workfront-API verfügbar waren. Dies ist zwar ein erweiterter Bericht, der für bestimmte Anwendungsfälle gedacht ist, aber das besser verdauliche Format erleichtert Ihnen die Berichterstellung über Projektaktivität und Systemaktualisierungen in Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2763'
ht-degree: 4%

---

# Bericht im Bereich Aktualisierungen mit einem Journaleintragsbericht

<!-- Audited: 11/2024 -->

Systemaktualisierungen für Journaleinträge werden im Bereich Aktualisierungen von Projekten, Aufgaben, Problemen und anderen Objekten angezeigt, die zuvor nur über die Adobe Workfront-API verfügbar waren. Dies ist zwar ein erweiterter Bericht, der für bestimmte Anwendungsfälle gedacht ist, aber das besser verdauliche Format erleichtert Ihnen die Berichterstellung über Projektaktivität und Systemaktualisierungen in Workfront.

>[!TIP]
>
>Der Journaleintragsbericht enthält nur Systemaktualisierungen aus dem Bereich Aktualisierungen der Objekte. Um über die im Bereich Aktualisierungen verbliebenen Kommentare zu berichten, müssen Sie den Notizbericht verwenden.\
>Weitere Informationen zum Notizbericht finden Sie unter [Alle Aktualisierungen in einem Notizbericht anzeigen](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md).

Der Journaleintragsbericht kann Folgendes anzeigen:

* Anzahl der Statusänderungen
* Wenn eine Aufgabe oder ein Problem gelöscht wurde
* Wie sich Werte in wichtigen benutzerdefinierten Feldern im Laufe des Lebenszyklus eines Projekts geändert haben
* Welche wichtigen Daten haben sich im Laufe des Lebenszyklus eines Projekts geändert?
* Wenn der Eigentümer eines Projekts geändert wurde

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Objekte anzeigen, die die im Bericht angezeigten Journaleinträge enthalten</p> <p>Sie erhalten Verwaltungsberechtigungen für den Bericht, nachdem Sie ihn erstellt haben</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie die in diesem Artikel beschriebenen Aktionen durchführen können, müssen Sie Folgendes sicherstellen:

* Alle Felder (einschließlich benutzerdefinierter Felder), über die Sie einen Bericht erstellen möchten, werden in Workfront verfolgt. Sie können nur Berichte zu Daten aus dem Bereich Aktualisierungen erstellen, die verfolgt werden.

  Informationen zum Hinzufügen von Feldern, die von Workfront verfolgt werden sollen, finden Sie unter [Konfigurieren von Systemaktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Journaleintragsbericht - Übersicht

Da das Journaleintragsbericht-System aktualisiert wird, kann es eine erhebliche Anzahl von Ergebnissen zurückgeben. Daher empfehlen wir, bei der Erstellung des Berichts nach bestimmten Objekten zu filtern, z. B. nach Projekten, Programmen, Portfolios, Gruppen usw.

Weitere Informationen zu den verschiedenen Objekttypen in Workfront finden Sie unter [Grundlegendes zu Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Da der Journaleintragsbericht so viele Daten zurückgibt, werden der Export und die geplante Berichtlieferung nicht unterstützt.

Die Standardansicht für diesen Bericht enthält die folgenden Spalten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feld</th> 
   <th>Erklärung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Feldname</strong> </td> 
   <td> <p><span style="font-weight: normal;">Der Name des betroffenen Felds. Je nach Einrichtung des Berichts kann diese Spalte Status, Eigentümer-ID, Aufgabennamen, geplantes Abschlussdatum oder andere Felder enthalten.</span> </p> <p><span style="font-weight: normal;">Wenn</span> <strong>DE</strong>:<span style="font-weight: normal;"> in dieser Spalte angezeigt wird, bedeutet dies, dass das aufgelistete Feld ein benutzerdefiniertes Feld ist.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Typ ändern</strong> </td> 
   <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde. Je nach den von Ihnen eingerichteten Filterregeln und den von den Benutzenden durchgeführten Aktionen kann in diesem Feld Folgendes angezeigt werden:</p> 
    <ul> 
     <li> <p>Hinzufügen</p> </li> 
     <li> <p>Prüfung</p> </li> 
     <li> <p>Löschen</p> </li> 
     <li> <p>Digest</p> </li> 
     <li> <p>Bearbeiten</p> </li> 
     <li> <p>Wiederherstellen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Top ObjCode</strong> </td> 
   <td> <p>Das höchste übergeordnete Objekt in der Hierarchie.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Umfang</strong> </td> 
   <td> <p>Der Typ des geänderten Objekts.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Eingabedatum</strong> </td> 
   <td> <p>Das Datum der Änderung des Felds.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Bearbeitet nach Name</strong> </td> 
   <td> <p>Der Benutzer, der das Feld geändert hat.</p> </td> 
  </tr> 
 </tbody> 
</table>

Um die Informationen in diesem Bericht zu organisieren, können Sie die integrierte Gruppierung Projekt verwenden. Mit der Projektgruppierung erhalten Sie eine primäre Gruppierung des Projektnamens und eine sekundäre Gruppierung des Eingabedatums. Sie können diese bestehende Gruppierung bei der Erstellung eines Berichts anwenden oder sie beim Anzeigen des Berichts anwenden.

Informationen zum Einrichten der Ansichten, Filter und Gruppierungen, die Sie für Ihren Bericht benötigen, finden Sie im entsprechenden Abschnitt:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Ermitteln Sie, welche Statusänderungen aufgetreten sind](#see-what-status-changes-occurred)
* [Anzeigen, wann eine Aufgabe oder ein Problem gelöscht wurde](#see-when-a-task-or-issue-was-deleted)
* [Erfahren Sie, wie sich benutzerdefinierte Felder im Laufe des Lebenszyklus eines Projekts geändert haben](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Hier erfahren Sie, wie sich das geplante Abschlussdatum im Laufe des Lebenszyklus eines Projekts geändert hat](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Überprüfen, ob der Eigentümer eines Projekts geändert wurde](#see-if-the-owner-of-a-project-changed)

## Ermitteln, welche Statusänderungen aufgetreten sind {#see-what-status-changes-occurred}

Sie können festlegen, dass die Auswertung „Journaleinträge“ Folgendes anzeigt:

* Wie viele Statusänderungen wurden an einem Projekt, einer Aufgabe oder einem Problem vorgenommen

* Der vorherige Status vor der Änderung
* Wer hat den Status geändert
* Zeitpunkt der Statusänderung

Wenn Sie den Zustand eines Projekts überprüfen möchten, können Sie auch den Bericht so einrichten, dass dieselben Informationen über das Feld „Bedingung **des Projekts angezeigt**.

Diese Informationen können beim Auditing hilfreich sein und veranschaulichen, wie gut Sie und Ihr Unternehmen planen.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie **Journaleintrag**.

   ![Journaleintrag auswählen](assets/nwe-select-journal-entry-350x273.png)

   Report Builder wird geladen.

1. Fügen Sie auf der **Spalten (Ansicht)** die folgenden Spalten hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Spalte</th> 
      <th>Erklärung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Feldname</p> </td> 
      <td> <p>Der Name des betroffenen Felds. In diesem Fall sollte <strong>status</strong> in dieser Spalte angezeigt werden.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde, z. B<strong> „Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet von Name</p> </td> 
      <td> <p>Der Name des Benutzers, der den Status aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum der Statusänderung.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Textwert</p> </td> 
      <td> <p>Der Schlüssel für den vorherigen Status. Im Folgenden finden Sie die Statusschlüssel für die standardmäßigen Projektstatus:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Aktuell</p> </li> 
        <li> <p><strong>DED</strong>: Dead</p> </li> 
        <li> <p><strong>ONH</strong>: Halten</p> </li> 
        <li> <p><strong>PLN</strong>: Planung</p> </li> 
        <li> <p><strong>CPL</strong>: Abgeschlossen</p> </li> 
        <li> <p><strong>REQ</strong>: angefordert</p> </li> 
        <li> <p><strong>APR</strong>: Genehmigt</p> </li> 
        <li> <p><strong>REJ</strong>: Abgelehnt</p> </li> 
        <li> <p><strong>IDA</strong>: Idee</p> </li> 
       </ul> <p>Wenn Ihr Unternehmen benutzerdefinierte Status eingerichtet hat, werden möglicherweise weitere Statusschlüssel in dieser Spalte angezeigt. Wenden Sie sich an Ihren Workfront-Administrator oder Gruppenadministrator, um zu erfahren, welcher benutzerdefinierte Status mit einem Statusschlüssel verbunden ist.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Textwert</p> </td> 
      <td> <p>Der Schlüssel für den aktualisierten Status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Feld, das die Statusänderung hatte.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Umfang</p> </td> 
      <td> <p>Der Typ des Objekts, das die Statusänderung hatte.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Name des Problems<br>(optional)</p> </td> 
      <td> <p>Der Name des Problems, das eine Statusänderung hatte.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aufgabenname<br>(optional)</p> </td> 
      <td> <p>Der Name der Aufgabe, die eine Statusänderung hatte.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf **Registerkarte** Filter **auf Filterregel hinzufügen** und fügen Sie dann die Filterregel hinzu **Feldname** > **Gleich** > **Status**.

   ![Journaleintragsstatus-Filter](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Um über Bedingungsänderungen zu berichten, können Sie stattdessen die Filterregel **Feldname** > **Gleich** > **Bedingung** hinzufügen.

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Fügen Sie eine Eingabeaufforderung hinzu, um den Berichtfokus einzugrenzen und Ladezeiten zu reduzieren.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeiten tatsächlich erhöhen. Aus diesem Grund empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Gleich** zu verwenden, um nach einem bestimmten Projekt oder einer Objekt-ID auf höherer Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Registerkarte** Gruppierungen“ auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Anzeigen, wann eine Aufgabe oder ein Problem gelöscht wurde {#see-when-a-task-or-issue-was-deleted}

Sie können festlegen, dass die Auswertung „Journaleinträge“ Folgendes anzeigt:

* Welche Aufgaben oder Probleme gelöscht wurden
* Wer hat eine Aufgabe oder ein Problem gelöscht?

So sehen Sie, wann eine Aufgabe oder ein Problem gelöscht wurde:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie **Journaleintrag**.

   ![Journaleintrag auswählen](assets/nwe-select-journal-entry-350x273.png)

   Report Builder wird geladen.

1. Fügen Sie auf der **Spalten (Ansicht)** die folgenden Spalten hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Spalte</th> 
      <th>Erklärung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Umfang</p> </td> 
      <td> <p>Der Typ des gelöschten Objekts.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Die Art der Änderung, die stattgefunden hat. In <strong> Spalte wird </strong> Änderung „Löschen“ angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem die Aufgabe oder das Problem gelöscht wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet von Name</p> </td> 
      <td> <p>Der Name des Benutzers, der die Aufgabe oder das Problem gelöscht hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektname</p> </td> 
      <td> <p>Der Name des Projekts, das Aufgaben oder Probleme gelöscht hat.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken **auf** Registerkarte Filter **Filterregel hinzufügen** und fügen Sie dann die folgenden Filter hinzu:

   * **Typ ändern** > **Gleich** > **Löschen**
   * **Projekt-ID** > **Gleich** > **&lt; Projektname >**

     <!--WRITER check link; this png file has spaces
     [![Task or issue deleted](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Fügen Sie eine Eingabeaufforderung hinzu, um den Berichtfokus einzugrenzen und Ladezeiten zu reduzieren.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeiten tatsächlich erhöhen. Aus diesem Grund empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Gleich** zu verwenden, um nach einem bestimmten Projekt oder einer Objekt-ID auf höherer Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Optional) Klicken Sie auf der **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Erfahren Sie, wie sich benutzerdefinierte Felder im Laufe des Lebenszyklus eines Projekts geändert haben {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Sie können wichtige Feldänderungen im Laufe des Projekts verfolgen. Dazu können Sie den Journaleintrag einrichten, um Folgendes zu verfolgen:

* Wenn bestimmte benutzerdefinierte Felder hinzugefügt, aktualisiert oder bearbeitet wurden
* Wann diese Änderungen vorgenommen wurden
* Wer die Änderungen vorgenommen hat

So zeigen Sie, wie sich benutzerdefinierte Felder im Laufe des Lebenszyklus eines Projekts geändert haben:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie **Journaleintrag**.

   ![Journaleintrag auswählen](assets/nwe-select-journal-entry-350x273.png)

   Report Builder wird geladen.

1. Stellen Sie auf der Registerkarte **Spalten (Ansicht** sicher, dass Sie **Spalte hinzufügen** haben oder klicken, um die folgenden Spalten hinzuzufügen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Spalte</th> 
      <th>Erklärung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Feldname</p> </td> 
      <td> <p>Der Name des betroffenen benutzerdefinierten Feldes.</p> <p><span style="font-weight: normal;">Wenn</span> <strong>DE</strong>:<span style="font-weight: normal;"> in dieser Spalte angezeigt wird, bedeutet dies, dass das aufgelistete Feld ein benutzerdefiniertes Feld ist.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde, z. B<strong> „Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet von Name</p> </td> 
      <td> <p>Der Name des Benutzers, der das benutzerdefinierte Feld aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem der Wert im benutzerdefinierten Feld geändert wurde.</p> <p>Sortieren Sie in absteigender Reihenfolge nach diesem Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Zahlenwert</p> </td> 
      <td> <p>Der vorherige Zahlenwert im benutzerdefinierten Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Zahlenwert</p> </td> 
      <td> <p>Der aktuelle Zahlenwert im benutzerdefinierten Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Datumswert</p> </td> 
      <td> <p>Der vorherige Datumswert im benutzerdefinierten Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Datumswert</p> </td> 
      <td> <p>Der aktuelle Datumswert im benutzerdefinierten Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Textwert</p> </td> 
      <td> <p>Der vorherige Textwert im benutzerdefinierten Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Textwert</p> </td> 
      <td> <p>Der aktuelle Textwert im benutzerdefinierten Feld.</p> <p>Wenn das benutzerdefinierte Feld ein Feld mit automatischer Textvervollständigung ist, zeigt die Spalte <strong>Neuer </strong>" die Objekt-ID an.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken **auf** Registerkarte Filter **Filterregel hinzufügen** und fügen Sie dann die folgenden Filter hinzu:

   * **Feldname des Journaleintrags** > **Enthält** > **DE**

     >[!TIP]
     >
     >Um diesen Bericht auf bestimmte benutzerdefinierte Felder zu beschränken, fügen Sie die Filterregel **Journaleintragsfeldname** > **Gleich** > **&lt; benutzerdefinierter Feldname>** hinzu.

   * **Projekt-** > **Gleich** > **&lt; Projekt >**.

   ![Filter für benutzerdefinierte Formularänderungen](assets/qs-custom-form-changes-filter-350x92.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Fügen Sie eine Eingabeaufforderung hinzu, um den Berichtfokus einzugrenzen und Ladezeiten zu reduzieren.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeiten tatsächlich erhöhen. Aus diesem Grund empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Gleich** zu verwenden, um nach einem bestimmten Projekt oder einer Objekt-ID auf höherer Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Registerkarte** Gruppierungen“ auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Hier erfahren Sie, wie sich das geplante Abschlussdatum im Laufe des Lebenszyklus eines Projekts geändert hat {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Sie können die Auswertung „Journaleintrag“ so einrichten, dass sie anzeigt, wie oft sich das geplante Abschlussdatum im Laufe der Lebensdauer eines Projekts ändert.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie **Journaleintrag**.

   ![Journaleintrag auswählen](assets/nwe-select-journal-entry-350x273.png)

   Report Builder wird geladen.

1. Fügen Sie auf der **Spalten (Ansicht)** die folgenden Spalten hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Spalte</th> 
      <th>Erklärung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Feldname</p> </td> 
      <td> <p>Der Name des betroffenen Felds.</p> <p><span style="font-weight: normal;">Wenn</span> <strong>DE</strong>:<span style="font-weight: normal;"> in dieser Spalte angezeigt wird, bedeutet dies, dass das aufgelistete Feld ein benutzerdefiniertes Feld ist.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td>Der Typ der vorgenommenen Änderung, z. B<strong> „Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet von Name</p> </td> 
      <td> <p>Der Name des Benutzers, der das geplante Abschlussdatum des Projekts aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem das geplante Abschlussdatum des Projekts geändert wurde.</p> <p>Sortieren Sie in absteigender Reihenfolge nach diesem Feld.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Feld, in dem die Änderung des geplanten Abschlussdatums vorgenommen wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Umfang</p> </td> 
      <td> <p>Das Objekt mit der Änderung des geplanten Abschlussdatums.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Datumswert</p> </td> 
      <td> <p>Der vorherige Wert für das geplante Abschlussdatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Datumswert</p> </td> 
      <td> <p>Der aktuelle Wert für das geplante Abschlussdatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektname</p> <p>(Optional)</p> </td> 
      <td> <p>Der Name des Projekts, bei dem die Änderung des geplanten Abschlussdatums vorgenommen wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aufgabenname</p> <p>(Optional)</p> </td> 
      <td> <p>Der Name der Aufgaben im Projekt, bei denen die Änderung des geplanten Abschlussdatums vorgenommen wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Name des Problems</p> <p>(Optional)</p> </td> 
      <td>Der Name der Probleme im Projekt, bei denen die Änderung des geplanten Abschlussdatums vorgenommen wurde.</td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf **Registerkarte** Filter **auf „Filterregel hinzufügen** und fügen Sie dann Folgendes hinzu:

   * **Feldname** > **Gleich** > **Datum**
   * **Projekt-** > **Gleich** > **&lt; Projektname >**.

   ![Filter für Änderung des geplanten Abschlussdatums](assets/qs-planned-completion-date-change-filter-350x91.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Fügen Sie eine Eingabeaufforderung hinzu, um den Berichtfokus einzugrenzen und Ladezeiten zu reduzieren.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeiten tatsächlich erhöhen. Aus diesem Grund empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Gleich** zu verwenden, um nach einem bestimmten Projekt oder einer Objekt-ID auf höherer Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Registerkarte** Gruppierungen“ auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Überprüfen, ob der Eigentümer eines Projekts geändert wurde {#see-if-the-owner-of-a-project-changed}

Sie können die Auswertung „Journaleintrag“ so einrichten, dass sie anzeigt, wie oft sich der Projektbesitzer oder Projektmanager im Laufe der Lebensdauer eines Projekts ändert.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie **Journaleintrag**.

   ![Journaleintrag auswählen](assets/nwe-select-journal-entry-350x273.png)

   Report Builder wird geladen.

1. Fügen Sie auf der **Spalten (Ansicht)** die folgenden Spalten hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Spalte</th> 
      <th>Erklärung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Feldname</p> </td> 
      <td>Der Name des betroffenen Felds. In <strong> Spalte wird </strong>ownerID“ angezeigt.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Der Typ der vorgenommenen Änderung, z. B<strong> „Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Projekt, das vom Projektbesitzer aktualisiert wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td>Das Datum, an dem der Projektbesitzer geändert wurde.<br>Sortieren Sie in absteigender Reihenfolge nach diesem Feld.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet von Name</p> </td> 
      <td> <p>Der Name des Benutzers, der den Projektbesitzer aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Zusatzinfo 1</p> </td> 
      <td> <p>Der aktuelle Projektbesitzer für das Projekt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Zusatzinfo 2</p> </td> 
      <td> <p>Der vorherige Projektbesitzer im Projekt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektname</p> </td> 
      <td> <p>Das Projekt, bei dem das Feld „Projektbesitzer“ aktualisiert wurde.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf **Registerkarte** Filter **auf „Filterregel hinzufügen** und fügen Sie dann Folgendes hinzu:

   * **Feldname** > **Gleich** > **EigentümerID**
   * **Projekt-** > **Gleich** > **&lt; Projektname >**.

   ![Filter für Besitzer-Änderung](assets/qs-owner-changes-filter-350x94.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Fügen Sie eine Eingabeaufforderung hinzu, um den Berichtfokus einzugrenzen und Ladezeiten zu reduzieren.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeiten tatsächlich erhöhen. Aus diesem Grund empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Gleich** zu verwenden, um nach einem bestimmten Projekt oder einer Objekt-ID auf höherer Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Optional) Klicken Sie auf der **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Der neue Journaleintragsbericht wird angezeigt.
