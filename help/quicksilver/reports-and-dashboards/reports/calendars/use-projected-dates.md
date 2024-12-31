---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Prognostiziertes Datum in einem Kalenderbericht verwenden
description: Ein Kalenderbericht ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können die Felder für das voraussichtliche Datum in einem Kalenderbericht für Aufgaben, Probleme und Projekte verwenden.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 1%

---

# Verwenden [!UICONTROL Voraussichtliche Termine] in einem Kalenderbericht

Ein Kalenderbericht ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können die Felder für das voraussichtliche Datum in einem Kalenderbericht für folgende Objekte verwenden:

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz*</strong></td> 
   <td> <p>[!UICONTROL-Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL ]Bearbeitungszugriff auf [!UICONTROL-Berichte], [!UICONTROL-Dashboards] und [!UICONTROL-Kalender]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Manage] Zugriff auf den Kalenderbericht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Elementgruppe einrichten

Sie können festlegen, wie die Gruppe von Elementen in Ihrem Kalender angezeigt werden soll.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **[!UICONTROL Kalender]**.

1. Wählen Sie den Kalender aus, dem Sie eine neue Gruppe von Elementen hinzufügen möchten.\
   Oder\
   Klicken Sie auf **[!UICONTROL + Neuer Kalender]** und geben Sie den Kalendernamen ein.

   >[!NOTE]
   >
   >Sie müssen [!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender] in Ihrer Zugriffsebene haben, um einen Kalenderbericht zu erstellen.

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
      <td><p>Wählen Sie <strong>[!UICONTROL Voraussichtliche Termine]</strong>. Weitere Informationen über geplante Termine finden Sie unter </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Übersicht über das voraussichtliche Startdatum des Projekts</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Im Kalender, anzeigen]</strong></td>
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

## Hinzufügen von Objekten zur Gruppe von Elementen

Nachdem Sie eingerichtet haben, wie Elemente angezeigt werden sollen, müssen Sie die Objekte, die im Kalender angezeigt werden sollen, zur Gruppierung hinzufügen.

1. Im **[!UICONTROL Was möchten Sie dem Kalender hinzufügen?]** Sie den Abschnitt aus.

   * **[!UICONTROL Aufgaben]**
   * **[!UICONTROL Projekte]**
   * **[!UICONTROL Probleme]**

1. Klicken Sie **[!UICONTROL Aufgaben hinzufügen]**, **[!UICONTROL Projekte hinzufügen]** oder **[!UICONTROL Probleme hinzufügen]** je nach dem Objekttyp, den Sie dem Kalender hinzufügen.\
   ![Objekt für Kalender auswählen](assets/field-name.png)

1. Geben Sie im Dropdown-Menü den Feldnamen ein und wählen Sie dann die Feldquelle des Objekts aus, das Sie im Kalender anzeigen möchten (z. B. **[!UICONTROL Aufgaben]**).
1. Eine Bedingungsanweisung für die Kalendergruppierung festlegen.

   ![Bedingungsanweisung](assets/condition-statement-calendar.png)

   Informationen zum Festlegen von Bedingungen finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Geben Sie zusätzliche Objekte für die Kalendergruppierung an, indem Sie die Schritte 1-4 wiederholen.
1. Wählen **[!UICONTROL im Feld Aufgaben/Projekte/Probleme als]** festlegen aus, wie die Objekte in dieser Kalendergruppierung im Kalender gekennzeichnet werden sollen.

   >[!NOTE]
   >
   >Wenn die standardmäßigen Beschriftungsoptionen für ein bestimmtes Objekt nicht verfügbar sind, wird stattdessen der Objektname angezeigt. Wenn beispielsweise die Beschriftung Übergeordnete Aufgabe ausgewählt ist und dem Objekt keine übergeordnete Aufgabe zugeordnet ist, zeigt [!DNL Adobe Workfront] den Objektnamen an, den Sie im Kalender anzeigen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
