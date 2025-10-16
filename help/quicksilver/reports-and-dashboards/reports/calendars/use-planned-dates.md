---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Verwenden von geplanten Terminen in Kalenderberichten
description: Ein Kalenderbericht ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können die Felder für das geplante Datum in einem Kalenderbericht für Aufgaben, Probleme und Projekte verwenden.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 2%

---

# Verwenden [!UICONTROL &#x200B; „Geplante &#x200B;]&quot; in einem Kalenderbericht

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

Ein Kalenderbericht ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können [!UICONTROL Geplantes Datum] Felder in einem Kalenderbericht für die folgenden Objekte verwenden:

* Aufgaben
* Probleme
* Projekte

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf den Kalenderbericht verwalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elementgruppe einrichten

Sie können festlegen, wie die Gruppe von Elementen in Ihrem Kalender angezeigt werden soll.

{{step1-to-calendars}}

1. Wählen Sie den Kalender aus, dem Sie eine neue Gruppe von Elementen hinzufügen möchten.
oder
Klicken Sie auf **[!UICONTROL + Neuer Kalender]** und geben Sie den Kalendernamen ein.

   >[!NOTE]
   >
   >Sie müssen Bearbeitungszugriff auf Berichte, Dashboards und Kalender in Ihrer Zugriffsebene haben, um einen Kalenderbericht zu erstellen.

1. Klicken Sie links auf **[!UICONTROL Zum Kalender hinzufügen]** und anschließend auf **[!UICONTROL Erweiterte Elemente hinzufügen]**.

1. Geben Sie Folgendes an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Diese Gruppe von Elementen benennen]</strong></td>
      <td>Geben Sie einen Namen für die Gruppe von Elementen ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL color]</strong></td>
      <td>Wählen Sie eine Farbe für die Gruppe von Elementen. Alle Elemente werden im Kalenderbericht in der ausgewählten Farbe angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Datumsfeld]</strong></td>
      <td><p>Wählen Sie <strong>[!UICONTROL Geplante Termine]</strong>. Weitere Informationen über geplante Termine finden Sie unter </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Übersicht über das geplante Startdatum des Projekts</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Übersicht über das geplante Startdatum der Aufgabe</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über das geplante Abschlussdatum der Aufgabe</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Geplantes Abschlussdatum für das Projekt festlegen</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Im Kalender anzeigen</strong></td>
      <td><p>Wählen Sie aus, wie die Daten angezeigt werden sollen:</p>
       <ul>
        <li><strong>[!UICONTROL Nur Startdatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Nur Enddatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Duration] (Anfang bis Ende)</strong>: Der Kalender zeigt das Objekt über einen Zeitraum von Tagen an.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Zu tatsächlichen Daten wechseln, falls verfügbar]</strong></td>
      <td><p>Der Kalender wechselt automatisch zu tatsächlichen Daten, wenn sie verfügbar sind. <br>Wählen Sie <strong>[!UICONTROL Yes]</strong> oder <strong>[!UICONTROL No]</strong>, um zu den tatsächlichen Daten zu wechseln, sofern verfügbar. Weitere Informationen über tatsächliche Termine finden Sie unter</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Übersicht über das tatsächliche Startdatum des Projekts </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Übersicht über das tatsächliche Abschlussdatum des Projekts </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Fahren Sie mit dem folgenden Abschnitt fort.

## Hinzufügen von Objekten zur Gruppe von Elementen in der Vorschau

Nachdem Sie eingerichtet haben, wie Elemente angezeigt werden sollen, müssen Sie die Objekte, die im Kalender angezeigt werden sollen, zur Gruppierung hinzufügen.

1. Im **[!UICONTROL Was möchten Sie dem Kalender hinzufügen?]** Sie den Abschnitt aus.

   * **[!UICONTROL Aufgaben]**
   * **[!UICONTROL Projekte]**
   * **[!UICONTROL Probleme]**


1. Klicken Sie **[!UICONTROL Aufgaben hinzufügen]**, **[!UICONTROL Projekte hinzufügen]** oder **[!UICONTROL Probleme hinzufügen]** je nach dem Objekttyp, den Sie dem Kalender hinzufügen.

1. Geben Sie im Dropdown-Menü den Feldnamen ein und wählen Sie dann die Feldquelle des Objekts aus, das Sie im Kalender anzeigen möchten (z. B. **[!UICONTROL Aufgaben]**).
1. Eine Bedingungsanweisung für die Kalendergruppierung festlegen.


   ![Objekt für Kalender auswählen](assets/calendar-field-name.png)

   Informationen zum Festlegen von Bedingungen finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Geben Sie zusätzliche Objekte für die Kalendergruppierung an, indem Sie die Schritte 1-4 wiederholen.

1. Wählen **[!UICONTROL im Feld Aufgaben/Projekte/Probleme als]** festlegen aus, wie die Objekte in dieser Kalendergruppierung im Kalender gekennzeichnet werden sollen.

   >[!NOTE]
   >
   >Wenn die standardmäßigen Beschriftungsoptionen für ein bestimmtes Objekt nicht verfügbar sind, wird stattdessen der Objektname angezeigt. Wenn beispielsweise die Beschriftung [!UICONTROL Übergeordnete Aufgabe] ausgewählt ist und dem Objekt keine übergeordnete Aufgabe zugeordnet ist, zeigt [!DNL Adobe Workfront] den Objektnamen an, den Sie im Kalender anzeigen.

   ![Festlegen von Aufgabenbeschriftungen](assets/set-task-labels.png)
1. Klicken Sie auf **[!UICONTROL Speichern]**.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

