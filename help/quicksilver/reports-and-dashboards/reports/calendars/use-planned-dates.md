---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Verwenden geplanter Datumswerte in einem Kalenderbericht
description: Ein Kalenderbericht ist ein dynamischer Bericht, der eine visuelle Darstellung Ihrer Arbeit bietet. Sie können die Felder für das geplante Datum in einem Kalenderbericht für Aufgaben, Probleme und Projekte verwenden.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 2%

---

# Verwendung [!UICONTROL Geplante Datumswerte] in einem Kalenderbericht

Ein Kalenderbericht ist ein dynamischer Bericht, der eine visuelle Darstellung Ihrer Arbeit bietet. Sie können [!UICONTROL Geplantes Datum] -Felder in einem Kalenderbericht für die folgenden Objekte:

* Aufgaben
* Probleme
* Projekte

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender] bearbeiten</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf den Kalenderbericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Einrichten der Gruppe von Elementen

Sie können auswählen, wie die Gruppe von Elementen im Kalender angezeigt werden soll.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Kalender]**.

1. Wählen Sie den Kalender aus, dem Sie eine neue Gruppe von Elementen hinzufügen möchten.\
   Oder\
   Klicken **[!UICONTROL + Neuer Kalender]** und geben Sie den Kalendernamen ein.

   >[!NOTE]
   >
   >Sie müssen Zugriff auf Berichte, Dashboards und Kalender bearbeiten haben, um einen Kalenderbericht zu erstellen.

1. Klicken Sie links auf **[!UICONTROL Zum Kalender hinzufügen]** Klicken Sie auf **[!UICONTROL Erweiterte Elemente hinzufügen]**.

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
      <td role="rowheader"><strong>[!UICONTROL Farbe]</strong></td>
      <td>Wählen Sie eine Farbe für die Gruppe von Elementen aus. Alle Elemente werden im Kalenderbericht in der ausgewählten Farbe angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Datumsfeld]</strong></td>
      <td><p>Auswählen <strong>[!UICONTROL Geplante Daten]</strong>. Weitere Informationen über geplante Termine finden Sie unter </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Übersicht über das geplante Projektstartdatum</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Übersicht über die geplante Aufgabe - Startdatum</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über die geplante Aufgabe - Abschlussdatum</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Festlegen des geplanten Abschlussdatums des Projekts</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Im Kalender anzeigen</strong></td>
      <td><p>Legen Sie fest, wie die Daten angezeigt werden sollen:</p>
       <ul>
        <li><strong>[!UICONTROL Startdatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Enddatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Dauer] (Start bis Ende)</strong>: Der Kalender zeigt das Objekt über einen Zeitraum von Tagen an.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Wechseln zu den tatsächlichen Daten, falls verfügbar]</strong></td>
      <td><p>Der Kalender wechselt automatisch zu den tatsächlichen Daten, sobald sie verfügbar sind. <br>Auswählen <strong>[!UICONTROL Ja]</strong> oder <strong>[!UICONTROL Nein]</strong> , um zu den tatsächlichen Daten zu wechseln, sofern verfügbar. Weitere Informationen zu den tatsächlichen Daten finden Sie unter</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Übersicht über das tatsächliche Projektstartdatum </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Übersicht über das tatsächliche Abschlussdatum des Projekts </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Fahren Sie mit dem folgenden Abschnitt fort.

## Objekte zur Gruppe von Elementen hinzufügen

Nachdem Sie eingerichtet haben, wie Elemente angezeigt werden sollen, müssen Sie die Objekte, die Sie im Kalender sehen möchten, zur Gruppierung hinzufügen.

1. Im **[!UICONTROL Was möchten Sie zum Kalender hinzufügen?]** Bereich, wählen Sie

   * **[!UICONTROL Aufgaben]**
   * **[!UICONTROL Projekte]**
   * **[!UICONTROL Probleme]**

1. Klicken **[!UICONTROL Aufgaben hinzufügen]**, **[!UICONTROL Projekte hinzufügen]** oder **[!UICONTROL Hinzufügen von Problemen]**- abhängig vom Objekttyp, den Sie dem Kalender hinzufügen.\
   ![Objekt für Kalender auswählen](assets/field-name.png)

1. Geben Sie im Dropdown-Menü den Feldnamen ein und wählen Sie dann die Feldquelle des Objekts aus, das im Kalender angezeigt werden soll (z. B. **[!UICONTROL Verspätete Aufgaben]**).
1. Legen Sie eine Bedingungsanweisung für die Kalendergruppierung fest.

   ![Bedingungsanweisung](assets/condition-statement-calendar.png)

   Weitere Informationen zum Festlegen von Bedingungen finden Sie unter [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Geben Sie zusätzliche Objekte für die Kalendergruppierung an, indem Sie die Schritte 1 bis 4 wiederholen.
1. Im **[!UICONTROL Legen Sie für die Beschriftungen Aufgaben/Projekte/Probleme fest, dass ...]** auswählen, wie die Objekte in dieser Kalendergruppierung im Kalender beschriftet werden.

   >[!NOTE]
   >
   >Wenn die standardmäßigen Beschriftungsoptionen für ein bestimmtes Objekt nicht verfügbar sind, wird stattdessen der Objektname angezeigt. Beispiel: Wenn die Variable [!UICONTROL Übergeordnete Aufgabe] &quot;label&quot;ausgewählt ist und keine übergeordnete Aufgabe mit dem Objekt verknüpft ist, [!DNL Adobe Workfront] zeigt den Objektnamen an, den Sie im Kalender anzeigen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
