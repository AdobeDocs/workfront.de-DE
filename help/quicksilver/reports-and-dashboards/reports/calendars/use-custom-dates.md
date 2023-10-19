---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht
description: Ein Kalenderbericht ist ein dynamischer Bericht, der eine visuelle Darstellung Ihrer Arbeit bietet. Sie können benutzerdefinierte Datumsfelder in einem Kalenderbericht für Aufgaben, Probleme und Projekte verwenden.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht

A [!UICONTROL calendar] ist ein dynamischer Bericht, der eine visuelle Darstellung Ihrer Arbeit bietet. Sie können benutzerdefinierte Datumsfelder in einem Kalenderbericht für die folgenden Objekte verwenden:

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
   <td> <p>Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender] bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf den Kalenderbericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

1. Sie müssen über benutzerdefinierte Datumsfelder und einen Wert im Feld verfügen, die in Ihrer [!DNL Workfront] -Instanz. Wenn Sie kein benutzerdefiniertes Formular mit benutzerdefinierten Datumsangaben eingerichtet haben, folgen Sie den Anweisungen in den ersten beiden Abschnitten unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Hängen Sie das benutzerdefinierte Formular an ein Projekt, eine Aufgabe oder ein Problem an, das Sie dem Kalender hinzufügen möchten, und geben Sie ein Datum an. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Einrichten der Gruppe von Elementen

Sie können auswählen, wie die Gruppe von Elementen im Kalender angezeigt werden soll.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Kalender]**.

1. Wählen Sie den Kalender aus, dem Sie eine neue Gruppe von Elementen hinzufügen möchten.\
   Oder\
   Klicks **[!UICONTROL + Neuer Kalender]** und geben Sie den Kalendernamen ein.

   >[!NOTE]
   >
   >Sie müssen [!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards], und [!UICONTROL Kalender] in Ihrer Zugriffsebene, um einen Kalenderbericht zu erstellen.

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
      <td>Auswählen <strong>[!UICONTROL Benutzerdefinierte Datumswerte]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Im Kalender anzeigen]</strong></td>
      <td><p>Legen Sie fest, wie die Daten angezeigt werden sollen:</p>
       <ul>
        <li><strong>[!UICONTROL Einzeldatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Dauer] (Start bis Ende)</strong>: Der Kalender zeigt das Objekt über einen Zeitraum von Tagen an.<br><p>Hinweis: Wenn Sie <strong>[!UICONTROL Dauer]</strong>muss das angegebene Enddatum nach dem Startdatum liegen oder das Element wird nicht im Kalender angezeigt.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Datumswerte]</strong></td>
      <td><p>Geben Sie den benutzerdefinierten Datumnamen ein, der an das Objekt angehängt ist, das Sie verfolgen möchten.</p><p><strong>NOTE:</strong> Die Suche nach dem benutzerdefinierten Datumsnamen ist auf 50 Ergebnisse beschränkt, um Leistungsprobleme zu vermeiden.</td>
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

1. Klicks **[!UICONTROL Aufgaben hinzufügen]**, **[!UICONTROL Projekte hinzufügen]** oder **[!UICONTROL Hinzufügen von Problemen]**- abhängig vom Objekttyp, den Sie dem Kalender hinzufügen.\
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
