---
product-area: requests
navigation-topic: create-requests
title: Ansichten im Bereich Anfragen erstellen
description: Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern.
author: Becky
feature: Work Management
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Erstellen oder Bearbeiten von Ansichten im Bereich Anfragen


Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern. Zu diesen Ansichten gehören Filter und Spaltenanordnungen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  <p>Sie müssen Workfront-Administrator sein, um Ansichten Layoutvorlagen hinzufügen zu können</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen Sie eine Ansicht im Bereich Anfragen .

{{step1-to-requests}}

1. (Optional und bedingt) Wählen Sie die Einstellung **Zu neuem Erlebnis wechseln** oben rechts im Bildschirm aus, wenn die folgenden Dinge auf Ihr Unternehmen und Ihre Workfront-Instanz zutreffen:

   * Ihr Unternehmen hat ein Workfront-Paket erworben
   * Ihr Unternehmen wurde in das einheitliche Adobe-Erlebnis integriert.
   * Ihr Administrator hat Ihnen Zugriff auf Workfront Planning gewährt
   * Sie haben zumindest Anzeigeberechtigungen für einen Workfront Planning-Arbeitsbereich

   Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)

1. Klicken Sie auf das **Ansichten** Dropdown-![Ansichten](assets/view-icon-requests.png) und wählen Sie **Neue Ansicht**.

   ![Neue Ansicht](assets/create-new-view.png)

1. Geben Sie einen Namen für die neue Ansicht ein und klicken Sie auf **Erstellen**.
1. Fahren Sie [Bearbeiten einer Ansicht im Bereich Anfragen](#edit-a-view-in-the-requests-area) fort.

## Bearbeiten einer Ansicht im Bereich „Anfragen“

Sie können vorhandene Ansichten bearbeiten, einschließlich der soeben erstellten Ansichten.

{{step1-to-requests}}

1. (Optional und bedingt) Wählen Sie die Einstellung **Zu neuem Erlebnis wechseln** oben rechts im Bildschirm aus, wenn die folgenden Dinge auf Ihr Unternehmen und Ihre Workfront-Instanz zutreffen:

   * Ihr Unternehmen hat ein Workfront-Paket erworben
   * Ihr Unternehmen wurde in das einheitliche Adobe-Erlebnis integriert.
   * Ihr Administrator hat Ihnen Zugriff auf Workfront Planning gewährt
   * Sie haben zumindest Anzeigeberechtigungen für einen Workfront Planning-Arbeitsbereich

   Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)1.

1. (Optional) Um eine Ansicht umzubenennen, klicken Sie auf das **Ansichten** Dropdown-Menü ![Ansichten](assets/view-icon-requests.png) und klicken Sie auf das Dreipunkt-Menü neben der Ansicht, wählen Sie **Umbenennen** aus und geben Sie dann den neuen Namen für die Ansicht ein.
1. Klicken Sie auf **Ansichten** Dropdown-![Ansichten](assets/view-icon-requests.png) und wählen Sie die Ansicht aus, die Sie bearbeiten möchten.
1. (Optional) Klicken Sie **Filter** und beginnen Sie mit dem Hinzufügen von Bedingungen für die Anfragen, die Sie auf der Registerkarte „Planung“ anzeigen möchten.

   ![Filter in der Registerkarte „Planungsanfragen“ bearbeiten](assets/filters-editing-box-in-requests-planning-tab.png)

   Sie können nach den folgenden Feldern filtern:

   * **Workspace**: Der Arbeitsbereich, mit dem das Anfrageformular verknüpft ist.
   * **Datensatztyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
   * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
   * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
   * **Status**: Der Status der Anfrage.
   * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anfrage von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.

   Es können mehrere Filter entweder durch „Und **oder** Oder **verbunden**.
Die Anfrageliste wird automatisch gefiltert, wenn Sie die Filterbedingungen hinzufügen.

1. (Optional) Klicken Sie auf **Spalten** und blenden Sie die Spalten in der Anfrageliste aus, anzeigen oder neu anordnen.

   ![Spalten-Feld](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Es können keine weiteren Spalten hinzugefügt werden.

>[!IMPORTANT]
>
> * Änderungen an Ansichten werden automatisch gespeichert.
> * Änderungen an Ansichten sind für alle sichtbar, die die Ansicht verwenden.

## Hinzufügen der Ansicht zu einer Layout-Vorlage.

Ein Workfront-Administrator kann die neue Ansicht Layoutvorlagen hinzufügen.

Anweisungen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).
