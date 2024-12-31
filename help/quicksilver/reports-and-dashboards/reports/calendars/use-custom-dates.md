---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht
description: Ein Kalenderbericht ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können benutzerdefinierte Datumsfelder in einem Kalenderbericht für Aufgaben, Probleme und Projekte verwenden.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 1%

---

# Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht

Ein [!UICONTROL Kalenderbericht] ist ein dynamischer Bericht, der Ihre Arbeit visuell darstellt. Sie können benutzerdefinierte Datumsfelder in einem Kalenderbericht für die folgenden Objekte verwenden:

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
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Manage] Zugriff auf den Kalenderbericht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

1. Sie müssen über benutzerdefinierte Datumsfelder und einen -Wert innerhalb des -Felds in Ihrer [!DNL Workfront] verfügen. Wenn Sie kein benutzerdefiniertes Formular mit benutzerdefinierten Datumsangaben eingerichtet haben, befolgen Sie die Anweisungen in [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Hängen Sie das benutzerdefinierte Formular an ein Projekt, eine Aufgabe oder ein Problem an, das/das Sie dem Kalender hinzufügen möchten, und geben Sie ein Datum an. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Elementgruppe einrichten

Sie können festlegen, wie die Gruppe von Elementen in Ihrem Kalender angezeigt werden soll.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Kalender]**.

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
      <td>Wählen Sie <strong>[!UICONTROL Benutzerdefinierte Daten]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Im Kalender, anzeigen]</strong></td>
      <td><p>Wählen Sie aus, wie die Daten angezeigt werden sollen:</p>
       <ul>
        <li><strong>[!UICONTROL Einzeldatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Duration] (Anfang bis Ende)</strong>: Der Kalender zeigt das Objekt über einen Zeitraum von Tagen an.<br><p>Hinweis: Wenn Sie <strong>[!UICONTROL Duration]</strong> auswählen, muss das angegebene Enddatum nach dem Startdatum liegen, da das Element sonst nicht im Kalender angezeigt wird.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Daten]</strong></td>
      <td><p>Geben Sie den benutzerdefinierten Datumnamen ein, der an das Objekt angehängt ist, das Sie verfolgen möchten.</p><p><strong>HINWEIS:</strong> Die Suche nach dem benutzerdefinierten Datumennamen ist auf 50 Ergebnisse beschränkt, um Leistungsprobleme zu vermeiden.</td>
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
   >Wenn die standardmäßigen Beschriftungsoptionen für ein bestimmtes Objekt nicht verfügbar sind, wird stattdessen der Objektname angezeigt. Wenn beispielsweise die Beschriftung [!UICONTROL Übergeordnete Aufgabe] ausgewählt ist und dem Objekt keine übergeordnete Aufgabe zugeordnet ist, zeigt [!DNL Adobe Workfront] den Objektnamen an, den Sie im Kalender anzeigen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
