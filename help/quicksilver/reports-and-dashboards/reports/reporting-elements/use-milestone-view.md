---
product-area: reporting
navigation-topic: reporting-elements
title: Meilenstein-Ansicht verwenden
description: Sie können die Meilenstein -Ansicht auf eine Projektliste oder einen Bericht anwenden. In der Ansicht Meilenstein können Sie alle Meilensteine anzeigen, die mit Aufgaben innerhalb der angezeigten Projekte verknüpft sind.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 1%

---

# Meilenstein-Ansicht verwenden

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen sind ab einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Sie können die Meilenstein -Ansicht auf eine Projektliste oder einen Bericht anwenden. In der Ansicht Meilenstein können Sie alle Meilensteine anzeigen, die mit Aufgaben innerhalb der angezeigten Projekte verknüpft sind.

Bevor Sie die Meilenstein -Ansicht verwenden können, müssen die folgenden Elemente vorhanden sein:

* Meilensteinpfade werden konfiguriert. Weitere Informationen finden Sie unter [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Meilensteinpfade müssen Projekten hinzugefügt werden. Weitere Informationen finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* Meilensteine sind mit Aufgaben verbunden. Weitere Informationen finden Sie unter [Zuordnen von Meilensteinen zu Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

Die Meilenstein -Ansicht ist beim Anzeigen einer Projektliste oder eines Projektberichts verfügbar. In den folgenden Abschnitten wird beschrieben, wie Sie die Meilenstein -Ansicht anzeigen und verwenden.

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
   <td role="rowheader">Adobe Workfront-Lizenz</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Arbeit oder höher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Berichte, Dashboards, Kalender</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
    <td> <p>Anzeigen von Berechtigungen für einen Projektbericht, um die Meilenstein -Ansicht auf einen Bericht anzuwenden</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zur Ansicht Meilenstein wechseln {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Klicken Sie auf **Dropdown** Menü „Ansicht“ und dann auf **Meilenstein**.

   Die Liste oder der Bericht wird in einer Meilenstein -Ansicht angezeigt.

   Weitere Informationen zur Meilenstein-Ansicht finden Sie im Abschnitt [Meilenstein-Ansicht - Übersicht](#milestone-view-overview) in diesem Artikel.

## Meilenstein-Ansicht - Übersicht {#milestone-view-overview}

<div class="preview">

Die Meilenstein -Ansicht ist in Projektlisten und Projektberichten verfügbar. Sie können schnell alle Meilensteine anzeigen, die mit Aufgaben innerhalb der angezeigten Projekte verknüpft sind.

![Projekt mit Meilenstein-Ansicht](assets/project-with-milestone-view-with-complete.png)

</div>

>[!NOTE]
>
>Die Ansicht Meilenstein ist in den folgenden Bereichen nicht verfügbar:
>
>* Arbeitszeittabellen, in der Projektliste beim Hinzufügen eines Projekts.

Informationen zum Wechseln zur Meilenstein -Ansicht finden Sie im Abschnitt [Wechseln zur Meilenstein -](#switch-to-the-milestone-view) in diesem Artikel.


### Meilenstein-Ansichtsabschnitte

Beim Anwenden der Meilenstein -Ansicht auf eine Liste von Projekten werden die Projekte in den folgenden Abschnitten angezeigt:

* Die Projekte, die mit einem Meilensteinpfad verknüpft sind, werden zuerst angezeigt und unter dem Namen des jeweiligen Meilensteinpfads aufgeführt.

  Workfront sortiert die Projekte im ersten Abschnitt anhand der folgenden Kriterien in der folgenden Reihenfolge:

   1. Meilensteinpfad-ID. Sie können die Meilensteinpfad-ID in einem Meilensteinpfadbericht anzeigen.

   2. Das als erstes Sortierfeld für die Projektliste ausgewählte Feld in der Ansicht, die zuvor auf die Projektliste angewendet wurde, bevor Sie die Meilenstein -Ansicht ausgewählt haben.

* Die Projekte, die keinem Meilensteinpfad zugeordnet sind, werden als Nächstes im Abschnitt Nicht zugewiesen angezeigt. Workfront sortiert die Projekte im Bereich Nicht zugewiesen nach dem Feld, das als erstes Sortierfeld für die Projektliste in der Ansicht ausgewählt wurde, die zuvor auf die Projektliste angewendet wurde, bevor Sie die Meilenstein -Ansicht ausgewählt haben.

### Projektinformationen in der Meilenstein -Ansicht

Beim Anzeigen einer Projektliste oder eines Projektberichts in der Meilenstein -Ansicht sind die folgenden Informationen verfügbar:

* **Geplante Termine oder Voraussichtliche Termine:** Geben Sie an, ob Sie geplante Termine oder Voraussichtliche Termine in der Ansicht „Meilenstein“ anzeigen möchten.\
  Im Meilensteinpfad werden Datumsangaben für das Start- und Abschlussdatum des Projekts sowie für den Abschluss jeder Meilensteinaufgabe angezeigt.

  Wenn Sie ein voraussichtliches Datum anzeigen, können die Daten nicht bearbeitet werden. Voraussichtliche Termine werden von Workfront berechnet und können nicht manuell geändert werden.

  Wenn Sie geplante Termine anzeigen und auch Zugriff auf das Projekt verwalten haben, können Sie die folgenden Termine direkt in der Ansicht Meilenstein bearbeiten:

   * **Projektstartdaten:** Wenn ein Projekt ab dem Startdatum geplant wird, können Sie das geplante Startdatum des Projekts manuell ändern. Anschließend wird das geplante Abschlussdatum berechnet.
   * **Projektabschlussdaten:** ein Projekt ab dem geplanten Abschlussdatum geplant wird, können Sie das geplante Abschlussdatum des Projekts manuell ändern. Anschließend wird das geplante Startdatum berechnet.
   * **Abschlussdaten von Aufgaben:** Sie können das geplante Abschlussdatum für Aufgaben direkt in der Ansicht Meilenstein manuell aktualisieren.

* **Prozent abgeschlossen:** Zeigt den Prozentsatz der Fertigstellung jeder Aufgabe und jedes Projekts an.

  Sie können die Anzeige des Prozentsatzes der Fertigstellung deaktivieren, wie im Abschnitt [Konfigurieren der in der Meilenstein-Ansicht angezeigten Informationen](#configure-what-information-displays-in-the-milestone-view) in diesem Artikel beschrieben.

  Sie können den Prozentsatz der Fertigstellung direkt in der Ansicht Meilenstein anpassen, wie im Abschnitt [Anpassen des Prozentsatzes der Fertigstellung für Aufgaben in der Ansicht Meilenstein](#adjust-percent-complete-for-tasks-in-the-milestone-view) in diesem Artikel beschrieben.

* **Symbole für den Aufgabenstatus:** Je nach Umgebung, in der Sie die Meilenstein -Ansicht anzeigen, zeigen die folgenden Symbole den Fortschrittsstatus der Aufgabe an:

   * In der Produktionsumgebung werden die folgenden Statussymbole neben jedem Projekt und jeder Aufgabe in der Meilenstein -Ansicht angezeigt:

      * Im Zeitplan\
        ![Symbol „Einschaltzeit“](assets/gantt-ontime.png)

      * In Verzug\
        ![Hinter-Symbol](assets/gantt-behind.png)

      * Gefährdet\
        ![Risiko-Symbol](assets/gantt-atrisk.png)

      * Verspätet\
        ![Spätsymbol](assets/gantt-late.png)

     <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <div class="preview">

   * In der Vorschau -Umgebung werden die folgenden farbigen Kreise neben jedem Projekt und jeder Aufgabe in der Meilenstein -Ansicht angezeigt:

      * Einschaltzeit - grün
      * Hinten - gelb
      * Gefährdet - blau
      * Spät - rot

  </div>

  Sie können die Anzeige dieser Statussymbole deaktivieren, wie im Abschnitt [Konfigurieren, welche Informationen in der Meilenstein-Ansicht angezeigt werden](#configure-what-information-displays-in-the-milestone-view) in diesem Artikel beschrieben.

  Weitere Informationen zu den einzelnen Statustypen finden Sie im Artikel [Übersicht über den Aufgabenstatus](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Aufgabenstatusschattierung für abgeschlossene Aufgaben**: Nachdem eine Aufgabe als „Abgeschlossen“ markiert wurde, wird der Hintergrund der Aufgabe in der Meilenstein -Ansicht schattiert, um anzugeben, ob die Aufgabe termingerecht oder zu spät abgeschlossen wurde:

   * **Rote Schattierung für**: Der Hintergrund einer Aufgabe ist rot, wenn der Fortschrittsstatus &quot;**&quot;**.

   * **Grüne Schattierung für Aufgabenspalte**: Der Hintergrund einer Aufgabe ist grün, wenn der Fortschrittsstatus &quot;**&quot;**.

* **Projektstatusschattierung für die Spalten Projektstart und Projektabschluss**:

   * **Spalte Projektstart**: Der Hintergrund der Spalte Projektstart ist nur dann rot oder grün, wenn das tatsächliche Startdatum angegeben wird:

      * **Rote Schattierung für Projektstartspalte**: Der Hintergrund der Projektstartspalte ist rot, wenn der Fortschrittsstatus des Projekts &quot;**&quot;**.

      * **Grüne Schattierung für Projektstartspalte**: Der Hintergrund der Projektstartspalte ist grün, wenn der Fortschrittsstatus des Projekts &quot;**&quot;**.

     >[!TIP]
     >
     >Sie müssen zur Seite mit den Projektdetails gehen, um das tatsächliche Startdatum des Projekts anzuzeigen.

   * **Spalte für den Projektabschluss**: Der Hintergrund der Spalte für den Projektabschluss ist nur dann rot oder grün, wenn das tatsächliche Abschlussdatum angegeben wird:

      * **Rote Schattierung für**: Der Hintergrund der Spalte „Projektabschluss“ ist rot, wenn der Fortschrittsstatus des Projekts &quot;**&quot;**.

      * **Grüne Schattierung für die Spalte Projektabschluss**: Der Hintergrund der Spalte Projektabschluss ist grün, wenn der Fortschrittsstatus des Projekts &quot;**&quot;**.

     >[!TIP]
     >
     >Sie müssen zur Seite mit den Projektdetails gehen, um das tatsächliche Abschlussdatum des Projekts anzuzeigen.

   * Den Spalten Start und Abschluss wird keine Farbschattierung zugewiesen, wenn die Aufgaben den Verlaufsstatus Gefährdet oder Hinten aufweisen.

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![Meilensteinansicht mit Schattierung](assets/milestone-view-with-shading.png)

* **Projektname**: Der Projektname wird mit einem Link zum Projekt angezeigt.
* **Projektbedingungssymbol**: Je nach Umgebung greifen Sie über die folgenden Indikatoren auf die Meilenstein -Ansicht zu und zeigen die Projektbedingung an:

   * In der Produktionsumgebung wird neben dem Projektnamen ein Symbol angezeigt, das den Zustand des Projekts angibt. Die Bedingung des Projekts kann eine der folgenden sein:

      * Im Zielbereich
      * Gefährdet
      * In Schwierigkeiten

  <div class="preview">

   * In der Vorschau -Umgebung wird neben jedem Projekt ein Bedingungssymbol in Form eines farbigen Kreises angezeigt. Mögliche Projektbedingungen und Kreisfarben sind:

      * On Target - grün
      * Gefährdet - gelb
      * In Schwierigkeiten - rot

     </div>


## Konfigurieren, welche Informationen in der Meilenstein -Ansicht angezeigt werden {#configure-what-information-displays-in-the-milestone-view}

Sie können konfigurieren, ob die folgenden Elemente in der Ansicht Meilenstein angezeigt werden:

* Symbole für den Fortschrittsstatus
* Prozent abgeschlossen von Projekten und Aufgaben

Standardmäßig werden Fortschrittsstatus-Symbole und Prozent abgeschlossen von Projekten und Aufgaben angezeigt.

Alle Änderungen, die Sie an diesen Optionen vornehmen, gelten nur für Sie. Andere Benutzende sind davon nicht betroffen. Die von Ihnen vorgenommenen Änderungen werden beibehalten, wenn Sie sich das nächste Mal bei Workfront anmelden.

So konfigurieren Sie, ob Projektstatussymbole und der Prozentsatz der Projektabschlüsse angezeigt werden:

{{step1-to-projects}}

1. Klicken Sie auf **Dropdown** Menü „Ansicht“ und dann auf **Meilenstein**.

1. Klicken Sie in der Produktionsumgebung in **rechten oberen Ecke** Ansicht Meilenstein auf Optionen und wählen Sie dann im nächsten Schritt eine der Optionen aus.

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

   <div class="preview">Wählen Sie in der Vorschau -Umgebung aus den Optionen im nächsten Schritt rechts oben in der Meilenstein -Ansicht.</div>

   <!--at Production release, replace this screen shot and adjust the Production/ Preview text above-->


1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fortschrittsstatus</td> 
      <td> <p>Wählen Sie diese Option, um Fortschrittsstatus-Symbole neben jedem Projekt und jeder Aufgabe anzuzeigen.</p> <p>Standardmäßig ist diese Option aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Wählen Sie diese Option, um den Prozentsatz der Fertigstellung neben jedem Projekt und jeder Aufgabe anzuzeigen.</p> <p>Standardmäßig ist diese Option aktiviert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Anpassen des Prozentsatzes für abgeschlossene Aufgaben in der Ansicht Meilenstein {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Sie können den abgeschlossenen Prozentsatz für Aufgaben in der Ansicht Meilenstein anpassen. Sie können den abgeschlossenen Prozentsatz nicht für eine übergeordnete Aufgabe (eine Aufgabe, die Teilaufgaben enthält) oder für ein Projekt anpassen.

So passen Sie den abgeschlossenen Prozentsatz für eine Aufgabe in der Ansicht Meilenstein an:

{{step1-to-projects}}

1. Klicken Sie auf **Dropdown** Menü „Ansicht“ und dann auf **Meilenstein**.

1. (Bedingt) Wenn die Abschlussprozentsätze in der Meilenstein -Ansicht nicht aktuell sind, aktivieren Sie die Anzeige des Prozentsatzes der abgeschlossenen Aufgaben und Projekte, wie im Abschnitt [Konfigurieren der Informationen, die in der Meilenstein -Ansicht angezeigt werden](#configure-what-information-displays-in-the-milestone-view) in diesem Artikel beschrieben.

1. Klicken Sie in der Produktionsumgebung unter einer Aufgabe auf den Fertigstellungsprozentsatz, geben Sie einen neuen Prozentsatz an und drücken Sie dann die Eingabetaste.

   <div class="preview">Verschieben Sie in der Vorschau-Umgebung die Folie Prozent abgeschlossen auf den neuen Prozentsatz abgeschlossen, um sie zu aktualisieren. </div>
