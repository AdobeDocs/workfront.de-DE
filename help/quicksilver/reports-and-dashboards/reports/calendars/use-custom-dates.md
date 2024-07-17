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
source-wordcount: '699'
ht-degree: 1%

---

# Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht

Ein [!UICONTROL Kalender] -Bericht ist ein dynamischer Bericht, der eine visuelle Darstellung Ihrer Arbeit bietet. Sie können benutzerdefinierte Datumsfelder in einem Kalenderbericht für die folgenden Objekte verwenden:

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender] bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf den Kalenderbericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

1. Sie müssen über benutzerdefinierte Datumsfelder und einen Wert im Feld verfügen, die in Ihrer [!DNL Workfront] -Instanz verfügbar sind. Wenn Sie kein benutzerdefiniertes Formular mit benutzerdefinierten Datumsangaben eingerichtet haben, befolgen Sie die Anweisungen in den ersten beiden Abschnitten unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Hängen Sie das benutzerdefinierte Formular an ein Projekt, eine Aufgabe oder ein Problem an, das Sie dem Kalender hinzufügen möchten, und geben Sie ein Datum an. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Einrichten der Gruppe von Elementen

Sie können auswählen, wie die Gruppe von Elementen im Kalender angezeigt werden soll.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Kalender]**.![](assets/main-menu-icon.png)

1. Wählen Sie den Kalender aus, dem Sie eine neue Gruppe von Elementen hinzufügen möchten.\
   Oder\
   Klicken Sie auf **[!UICONTROL + Neuer Kalender]** und geben Sie den Kalendernamen ein.

   >[!NOTE]
   >
   >Sie müssen auf Ihrer Zugriffsebene über den Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender] verfügen, um einen Kalenderbericht zu erstellen.

1. Klicken Sie links auf **[!UICONTROL Zum Kalender hinzufügen]** und dann auf **[!UICONTROL Erweiterte Elemente hinzufügen]**.

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
      <td>Wählen Sie <strong>[!UICONTROL Benutzerdefinierte Datumswerte]</strong> aus.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Im Kalender anzeigen]</strong></td>
      <td><p>Legen Sie fest, wie die Daten angezeigt werden sollen:</p>
       <ul>
        <li><strong>[!UICONTROL Einzeldatum]</strong>: Der Kalender zeigt das Objekt an einem einzelnen Datum an.</li>
        <li><strong>[!UICONTROL Dauer] (Start bis Ende)</strong>: Der Kalender zeigt das Objekt über einen Zeitraum von Tagen an.<br><p>Hinweis: Wenn Sie "<strong>[!UICONTROL Duration]</strong>"auswählen, muss das angegebene Enddatum nach dem Startdatum liegen, da sonst das Element nicht im Kalender angezeigt wird.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Datumswerte]</strong></td>
      <td><p>Geben Sie den benutzerdefinierten Datumnamen ein, der an das Objekt angehängt ist, das Sie verfolgen möchten.</p><p><strong>HINWEIS:</strong> Die Suche nach dem benutzerdefinierten Datumsnamen ist auf 50 Ergebnisse beschränkt, um Leistungsprobleme zu vermeiden.</td>
     </tr>
    </tbody>
   </table>

1. Fahren Sie mit dem folgenden Abschnitt fort.

## Objekte zur Gruppe von Elementen hinzufügen

Nachdem Sie eingerichtet haben, wie Elemente angezeigt werden sollen, müssen Sie die Objekte, die Sie im Kalender sehen möchten, zur Gruppierung hinzufügen.

1. Was möchten Sie im **[!UICONTROL Kalender zum Kalender hinzufügen?Abschnitt]** auswählen

   * **[!UICONTROL Aufgaben]**
   * **[!UICONTROL Projekte]**
   * **[!UICONTROL Probleme]**

1. Klicken Sie je nach dem Objekttyp, den Sie zum Kalender hinzufügen, auf **[!UICONTROL Aufgaben hinzufügen]**, **[!UICONTROL Projekte hinzufügen]** oder **[!UICONTROL Probleme hinzufügen]**.\
   ![Objekt für Kalender auswählen](assets/field-name.png)

1. Geben Sie im Dropdown-Menü den Feldnamen ein und wählen Sie dann die Feldquelle des Objekts aus, das im Kalender angezeigt werden soll (z. B. **[!UICONTROL Verspätete Aufgaben]**).
1. Legen Sie eine Bedingungsanweisung für die Kalendergruppierung fest.

   ![Bedingungsanweisung](assets/condition-statement-calendar.png)

   Weitere Informationen zum Festlegen von Bedingungen finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Geben Sie zusätzliche Objekte für die Kalendergruppierung an, indem Sie die Schritte 1 bis 4 wiederholen.
1. Wählen Sie im Feld **[!UICONTROL Aufgaben/Projekte/Probleme als Titel festlegen...]** aus, wie die Objekte in dieser Kalendergruppierung im Kalender beschriftet werden sollen.

   >[!NOTE]
   >
   >Wenn die standardmäßigen Beschriftungsoptionen für ein bestimmtes Objekt nicht verfügbar sind, wird stattdessen der Objektname angezeigt. Wenn beispielsweise die Bezeichnung [!UICONTROL Übergeordnete Aufgabe] ausgewählt ist und dem Objekt keine übergeordnete Aufgabe zugeordnet ist, zeigt [!DNL Adobe Workfront] den Objektnamen an, den Sie im Kalender anzeigen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
