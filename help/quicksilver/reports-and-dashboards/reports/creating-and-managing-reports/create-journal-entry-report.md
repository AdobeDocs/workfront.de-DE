---
title: Bericht zum Bereich "Updates"
description: Der Bericht Journaleintrag enthält Systemaktualisierungen aus dem Bereich Updates für Projekte, Aufgaben, Probleme und andere Objekte, die zuvor nur über die Adobe Workfront-API verfügbar waren. Obwohl es sich hierbei um einen erweiterten Bericht handelt, der für bestimmte Anwendungsfälle gedacht ist, erleichtert das besser lesbare Format die Berichterstellung über Projektaktivitäten und Systemaktualisierungen in Workfront.
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '2734'
ht-degree: 4%

---

# Bericht zum Bereich &quot;Updates&quot;

<!-- Audited: 11/2024 -->

Der Bericht Journaleintrag enthält Systemaktualisierungen aus dem Bereich Updates für Projekte, Aufgaben, Probleme und andere Objekte, die zuvor nur über die Adobe Workfront-API verfügbar waren. Obwohl es sich hierbei um einen erweiterten Bericht handelt, der für bestimmte Anwendungsfälle gedacht ist, erleichtert das besser lesbare Format die Berichterstellung über Projektaktivitäten und Systemaktualisierungen in Workfront.

>[!TIP]
>
>Der Bericht Journaleintrag enthält nur Systemaktualisierungen aus dem Bereich Updates der Objekte. Um über Kommentare zu berichten, die im Bereich Updates übrig geblieben sind, müssen Sie den Bericht Hinweis verwenden.\
>Weitere Informationen zum Bericht &quot;Hinweis&quot;finden Sie unter [Alle Aktualisierungen in einem Hinweis-Bericht anzeigen](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

Der Journaleintragsbericht kann Folgendes anzeigen:

* Anzahl der Statusänderungen
* Beim Löschen einer Aufgabe oder eines Problems
* Änderung der Werte in wichtigen benutzerdefinierten Feldern im Verlauf des Lebenszyklus eines Projekts
* Welche wichtigen Daten haben sich im Laufe des Lebenszyklus eines Projekts geändert?
* Wenn sich der Eigentümer eines Projekts geändert hat

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für Objekte, die die Journaleinträge enthalten, die im Bericht angezeigt werden</p> <p>Sie erhalten nach der Erstellung Verwaltungsberechtigungen für den Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie die in diesem Artikel beschriebenen Aktionen durchführen können, müssen Sie Folgendes sicherstellen:

* Alle Felder (einschließlich benutzerdefinierter Felder), für die Sie Berichte erstellen möchten, werden in Workfront nachverfolgt. Sie können nur Berichte zu Daten aus dem verfolgten Bereich Updates erstellen.

  Informationen zum Hinzufügen von Feldern, die von Workfront verfolgt werden sollen, finden Sie unter [Konfigurieren von Systemaktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

## Übersicht über den Journaleintrag

Da das Informationssystem für Journaleinträge aktualisiert wird, kann es zu einer erheblichen Anzahl von Ergebnissen führen. Aus diesem Grund empfehlen wir, bei der Erstellung des Berichts nach bestimmten Objekten wie Projekten, Programmen, Portfolios, Gruppen usw. zu filtern.

Weitere Informationen zu den verschiedenen Objekttypen in Workfront finden Sie unter [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Da der Journaleintragsbericht so viele Daten zurückgibt, werden der Export und die geplante Berichtbereitstellung nicht unterstützt.

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
   <td> <p><span style="font-weight: normal;">Der Name des betroffenen Felds. Je nachdem, wie Sie den Bericht einrichten, kann diese Spalte Status, Inhaber-ID, Aufgabenname, Geplantes Abschlussdatum oder andere Felder enthalten.</span> </p> <p><span style="font-weight: normal;">Wenn in dieser Spalte </span> <strong>DE</strong>:<span style="font-weight: normal;"> angezeigt wird, bedeutet dies, dass es sich bei dem aufgelisteten Feld um ein benutzerdefiniertes Feld handelt.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Änderungstyp</strong> </td> 
   <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde. Je nach den von Ihnen eingerichteten Filterregeln und den von Benutzern durchgeführten Aktionen kann in diesem Feld Folgendes angezeigt werden:</p> 
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
   <td><strong>Top objCode</strong> </td> 
   <td> <p>Das höchste übergeordnete Objekt in der Hierarchie.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Umfang</strong> </td> 
   <td> <p>Der Typ des geänderten Objekts.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Einstiegsdatum</strong> </td> 
   <td> <p>Das Datum der Änderung des Felds.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Bearbeitet nach Name</strong> </td> 
   <td> <p>Der Benutzer, der das Feld geändert hat.</p> </td> 
  </tr> 
 </tbody> 
</table>

Um die Informationen in diesem Bericht zu organisieren, können Sie die integrierte Gruppierung namens Projekt verwenden. Die Gruppierung des Projekts bietet eine primäre Gruppierung des Projektnamen und eine sekundäre Gruppierung des Entrypages. Sie können diese bestehende Gruppierung bei der Berichterstellung anwenden oder sie bei der Berichtanzeige anwenden.

Informationen zum Einrichten der für Ihren Bericht gewünschten Ansichten, Filter und Gruppierungen finden Sie im entsprechenden Abschnitt:

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Ermitteln Sie, welche Statusänderungen aufgetreten sind](#see-what-status-changes-occurred)
* [Ermitteln, wann eine Aufgabe oder ein Problem gelöscht wurde](#see-when-a-task-or-issue-was-deleted)
* [Erfahren Sie, wie sich benutzerdefinierte Felder im Laufe des Lebenszyklus eines Projekts änderten](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Erfahren Sie, wie sich das geplante Abschlussdatum im Laufe des Lebenszyklus eines Projekts geändert hat](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Überprüfen, ob der Eigentümer eines Projekts geändert hat](#see-if-the-owner-of-a-project-changed)

## Erfahren Sie, welche Statusänderungen aufgetreten sind {#see-what-status-changes-occurred}

Sie können den Journaleintragsbericht so einrichten, dass er Folgendes anzeigt:

* Anzahl der Statusänderungen an einem Projekt, einer Aufgabe oder einem Problem

* Was war der vorherige Status vor der Änderung?
* Wer hat den Status geändert
* Zeitpunkt der Statusänderung

Wenn Sie den Zustand eines Projekts anzeigen möchten, können Sie den Bericht auch so einrichten, dass dieselben Informationen über das Feld **Bedingung** des Projekts angezeigt werden.

Diese Informationen können verwendet werden, um bei der Prüfung zu helfen und zu veranschaulichen, wie gut Sie und Ihr Unternehmen planen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Wenn Sie den Unterschied in Tagen zwischen Bedingungsänderungen vergleichen möchten, können Sie die erweiterte Analyse verwenden.\
>Weitere Informationen zu erweiterten Analysen finden Sie unter [Überblick über erweiterte Analysen](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Journaleintrag** aus.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Die Berichterstellung wird geladen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die folgenden Spalten hinzu:

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
      <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde, z. B. <strong>Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet nach Name</p> </td> 
      <td> <p>Der Name des Benutzers, der den Status aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem der Status geändert wurde</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Alter Textwert</p> </td> 
      <td> <p>Der Schlüssel für den vorherigen Status. Im Folgenden finden Sie die Statusschlüssel für die standardmäßigen Projektstatus:</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: Aktuell</p> </li> 
        <li> <p><strong>DED</strong>: Dead</p> </li> 
        <li> <p><strong>ONH</strong>: Bei gedrückter Taste</p> </li> 
        <li> <p><strong>PLN</strong>: Planung</p> </li> 
        <li> <p><strong>CPL</strong>: Complete</p> </li> 
        <li> <p><strong>REQ</strong>: angefordert</p> </li> 
        <li> <p><strong>APR</strong>: Genehmigt</p> </li> 
        <li> <p><strong>REJ</strong>: Abgelehnt</p> </li> 
        <li> <p><strong>IDA</strong>: Idee</p> </li> 
       </ul> <p>Wenn Ihr Unternehmen benutzerdefinierte Status eingerichtet hat, werden möglicherweise andere Statusschlüssel in dieser Spalte angezeigt. Wenden Sie sich an Ihren Workfront-Administrator oder -Gruppenadministrator, um zu erfahren, welcher benutzerdefinierte Status mit einem Statusschlüssel verknüpft ist.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Neuer Textwert</p> </td> 
      <td> <p>Der Schlüssel für den aktualisierten Status.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Feld mit der Statusänderung.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Umfang</p> </td> 
      <td> <p>Der Typ des Objekts, für das die Statusänderung erfolgte.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Problemname<br> (optional)</p> </td> 
      <td> <p>Der Name des Problems, das eine Statusänderung aufweist.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aufgabenname<br>(optional)</p> </td> 
      <td> <p>Der Name der Aufgabe, deren Status geändert wurde.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf der Registerkarte **Filter** auf **Filterregel hinzufügen** und fügen Sie dann die Filterregel **Feldname** > **Gleich** > **Status** hinzu.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Um über Bedingungsänderungen zu berichten, können Sie stattdessen die Filterregel **Feldname** > **Gleich** > **Bedingung** hinzufügen.

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Um den Fokus des Berichts einzuschränken und die Ladezeiten zu reduzieren, fügen Sie eine Eingabeaufforderung hinzu.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeit tatsächlich erhöhen. Daher empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Equal** zu verwenden, um nach einer bestimmten Projekt- oder Objekt-ID einer höheren Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf der Registerkarte **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Ermitteln, wann eine Aufgabe oder ein Problem gelöscht wurde {#see-when-a-task-or-issue-was-deleted}

Sie können den Journaleintragsbericht so einrichten, dass er Folgendes anzeigt:

* Welche Aufgaben oder Probleme wurden gelöscht?
* Aufgabe oder Problem gelöscht haben

So sehen Sie, wann eine Aufgabe oder ein Problem gelöscht wurde:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Journaleintrag** aus.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Die Berichterstellung wird geladen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die folgenden Spalten hinzu:

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
      <td> <p>Die Art der Veränderung, die stattgefunden hat. Die Änderung <strong>Löschen</strong> wird in dieser Spalte angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem die Aufgabe oder das Problem gelöscht wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet nach Name</p> </td> 
      <td> <p>Der Name des Benutzers, der die Aufgabe oder das Problem gelöscht hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektname</p> </td> 
      <td> <p>Der Name des Projekts, für das Aufgaben oder Probleme gelöscht wurden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf der Registerkarte **Filter** auf **Filterregel hinzufügen** und fügen Sie dann die folgenden Filter hinzu:

   * **Änderungstyp** > **Equal** > **Delete**
   * **Projekt-ID** > **Equal** > **`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Um den Fokus des Berichts einzuschränken und die Ladezeiten zu reduzieren, fügen Sie eine Eingabeaufforderung hinzu.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeit tatsächlich erhöhen. Daher empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Equal** zu verwenden, um nach einer bestimmten Projekt- oder Objekt-ID einer höheren Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Optional) Klicken Sie auf der Registerkarte **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Erfahren Sie, wie sich benutzerdefinierte Felder im Laufe des Lebenszyklus eines Projekts verändert haben {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Sie können wichtige Feldänderungen im Laufe des Projekts verfolgen. Dazu können Sie den Journaleintrag einrichten, um Folgendes zu verfolgen:

* Wenn bestimmte benutzerdefinierte Felder hinzugefügt, aktualisiert oder bearbeitet wurden
* Wann diese Änderungen eingetreten sind
* Wer hat die Änderungen vorgenommen?

So sehen Sie, wie sich benutzerdefinierte Felder im Verlauf des Projektlebenszyklus verändert haben:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Journaleintrag** aus.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Die Berichterstellung wird geladen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die folgenden Spalten hinzu:

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
      <td> <p>Der Name des betroffenen benutzerdefinierten Felds.</p> <p><span style="font-weight: normal;">Wenn in dieser Spalte </span> <strong>DE</strong>:<span style="font-weight: normal;"> angezeigt wird, bedeutet dies, dass es sich bei dem aufgelisteten Feld um ein benutzerdefiniertes Feld handelt.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Die Art der Änderung, die am betroffenen Feld vorgenommen wurde, z. B. <strong>Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet nach Name</p> </td> 
      <td> <p>Der Name des Benutzers, der das benutzerdefinierte Feld aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum, an dem der Wert im benutzerdefinierten Feld geändert wurde.</p> <p>Sie sollten dieses Feld in absteigender Reihenfolge sortieren.</p> </td> 
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
      <td> <p>Der aktuelle Textwert im benutzerdefinierten Feld.</p> <p>Wenn das benutzerdefinierte Feld ein typeahead -Feld ist, zeigt die Spalte <strong>Neuer Textwert</strong> die Objekt-ID an.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf der Registerkarte **Filter** auf **Filterregel hinzufügen** und fügen Sie dann die folgenden Filter hinzu:

   * **Journal Entry Field Name** > **contains** > **DE**

     >[!TIP]
     >
     >Um diesen Bericht auf bestimmte benutzerdefinierte Felder zu beschränken, fügen Sie die Filterregel **Journal Entry Field Name** > **Equal** > **`<custom field>`** hinzu.

   * **Projekt-ID** > **Equal** > **`<project>`**

   ![](assets/qs-custom-form-changes-filter-350x92.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Um den Fokus des Berichts einzuschränken und die Ladezeiten zu reduzieren, fügen Sie eine Eingabeaufforderung hinzu.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeit tatsächlich erhöhen. Daher empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Equal** zu verwenden, um nach einer bestimmten Projekt- oder Objekt-ID einer höheren Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf der Registerkarte **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Erfahren Sie, wie sich das geplante Abschlussdatum im Laufe des Lebenszyklus eines Projekts geändert hat. {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Sie können den Journaleintragsbericht so einrichten, dass er anzeigt, wie oft sich das geplante Abschlussdatum im Laufe des Projektlebens ändert.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Journaleintrag** aus.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Die Berichterstellung wird geladen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die folgenden Spalten hinzu:

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
      <td> <p>Der Name des betroffenen Felds.</p> <p><span style="font-weight: normal;">Wenn in dieser Spalte </span> <strong>DE</strong>:<span style="font-weight: normal;"> angezeigt wird, bedeutet dies, dass es sich bei dem aufgelisteten Feld um ein benutzerdefiniertes Feld handelt.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td>Die Art der vorgenommenen Änderung, z. B. <strong>Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet nach Name</p> </td> 
      <td> <p>Der Name des Benutzers, der das geplante Abschlussdatum des Projekts aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td> <p>Das Datum der Änderung des geplanten Abschlussdatums des Projekts.</p> <p>Sie sollten dieses Feld in absteigender Reihenfolge sortieren.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Feld mit der Änderung des geplanten Abschlussdatums.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Umfang</p> </td> 
      <td> <p>Das Objekt, für das das geplante Abschlussdatum geändert wurde.</p> </td> 
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
      <td> <p>Der Name des Projekts mit dem geplanten Abschlussdatum.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Aufgabenname</p> <p>(Optional)</p> </td> 
      <td> <p>Der Name der Aufgaben im Projekt, für die das geplante Abschlussdatum geändert wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Name des Problems</p> <p>(Optional)</p> </td> 
      <td>Der Name der Probleme im Projekt, für die das geplante Abschlussdatum geändert wurde.</td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf der Registerkarte **Filter** auf **Filterregel hinzufügen** und fügen Sie dann Folgendes hinzu:

   * **Feldname** > **Equal** > **Datum**
   * **Projekt-ID** > **Equal** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Um den Fokus des Berichts einzuschränken und die Ladezeiten zu reduzieren, fügen Sie eine Eingabeaufforderung hinzu.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeit tatsächlich erhöhen. Daher empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Equal** zu verwenden, um nach einer bestimmten Projekt- oder Objekt-ID einer höheren Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf der Registerkarte **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.

## Überprüfen, ob der Eigentümer eines Projekts geändert hat {#see-if-the-owner-of-a-project-changed}

Sie können den Journaleintragsbericht so einrichten, dass er anzeigt, wie oft sich der Projektinhaber - oder Projektmanager - im Laufe der Lebensdauer eines Projekts ändert.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Journaleintrag** aus.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Die Berichterstellung wird geladen.

1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die folgenden Spalten hinzu:

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
      <td>Der Name des betroffenen Felds. In dieser Spalte wird die <strong>ownerID</strong> angezeigt.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Typ ändern</p> </td> 
      <td> <p>Die Art der vorgenommenen Änderung, z. B. <strong>Hinzufügen</strong>, <strong>Löschen</strong> oder <strong>Bearbeiten</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Top ObjCode</p> </td> 
      <td> <p>Das höchste übergeordnete Objekt für das Projekt, für das der Projekteigentümer aktualisiert wurde.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Eingabedatum</p> </td> 
      <td>Das Datum, an dem der Projektinhaber geändert wurde.<br>Sie sollten nach diesem Feld in absteigender Reihenfolge sortieren.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Bearbeitet nach Name</p> </td> 
      <td> <p>Der Name des Benutzers, der den Projektinhaber aktualisiert hat.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Zusatzinfo 1</p> </td> 
      <td> <p>Der aktuelle Projektinhaber im Projekt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Zusatzinfo 2</p> </td> 
      <td> <p>Der vorherige Projektinhaber im Projekt.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Projektname</p> </td> 
      <td> <p>Das Projekt, bei dem das Feld Projektinhaber aktualisiert wurde.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Weitere Informationen zum Hinzufügen von Spalten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Klicken Sie auf der Registerkarte **Filter** auf **Filterregel hinzufügen** und fügen Sie dann Folgendes hinzu:

   * **Feldname** > **Equal** > **ownerID**
   * **Projekt-ID** > **Equal** > **`<project name>`**

   ![](assets/qs-owner-changes-filter-350x94.png)

   Weitere Informationen zum Hinzufügen von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Um den Fokus des Berichts einzuschränken und die Ladezeiten zu reduzieren, fügen Sie eine Eingabeaufforderung hinzu.

   Oder

   Erstellen Sie zusätzliche Filterregeln, um bestimmte Projekte, Aufgaben oder Probleme einzubeziehen.

   >[!IMPORTANT]
   >
   >Das Erstellen einer Filterregel, die den Modifikator **Enthält** verwendet, kann die Ladezeit tatsächlich erhöhen. Daher empfehlen wir, nach Möglichkeit einen anderen Modifikator wie **Equal** zu verwenden, um nach einer bestimmten Projekt- oder Objekt-ID einer höheren Ebene zu filtern.

   Informationen zum Hinzufügen einer Eingabeaufforderung finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Optional) Klicken Sie auf der Registerkarte **Gruppierungen** auf **Vorhandene Gruppierung anwenden** und wählen Sie dann **Projekt** aus.

   Weitere Informationen zum Hinzufügen von Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ihr neuer Bericht wird geladen.
