---
product-area: requests
navigation-topic: create-requests
title: Ansichten im Bereich Anfragen erstellen und verwalten
description: Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern.
author: Becky
feature: Work Management
source-git-commit: 4061163b8b761bc3922bfb95da6c0110b6ee5871
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 3%

---

# Ansichten im Bereich Anfragen erstellen und verwalten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>

Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern. Zu diesen Ansichten gehören Filter und Spaltenanordnungen.

Ansichten können im Bereich Anfragen von Workfront erstellt und verwaltet werden.

>[!IMPORTANT]
>
>* Diese Funktion ist nur in der neuen anfragenden -Version verfügbar.
>* Anzeigeeinstellungen sind im Widget Meine Anfragen auf der Startseite nicht verfügbar.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


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

Sie können eine Ansicht im Bereich Anfragen von Workfront erstellen.

1. So greifen Sie auf die Anfragenliste zu:

   {{step1-to-requests}}

1. Klicken Sie in der Liste Anfragen auf das Dropdown **** Dropdown-Menü ![Ansichten](assets/view-icon-requests.png) und wählen Sie **Neue Ansicht**.

   ![Neue Ansicht](assets/create-new-view.png)

1. Geben Sie einen Namen für die neue Ansicht ein und klicken Sie auf **Erstellen**.
1. Fahren Sie [Bearbeiten einer Ansicht im Bereich Anfragen](#edit-a-view-in-the-requests-area) fort.

## Bearbeiten einer Ansicht im Bereich „Anfragen“

Sie können vorhandene Ansichten bearbeiten, einschließlich der soeben erstellten Ansichten.

1. So greifen Sie auf die Anfragenliste zu:

   {{step1-to-requests}}
1. Suchen Sie in der Anfragenliste die Ansicht, die Sie bearbeiten möchten.

1. (Optional) Um eine Ansicht umzubenennen, klicken Sie auf das **Ansichten** Dropdown-Menü ![Ansichten](assets/view-icon-requests.png) und klicken Sie auf das Dreipunkt-Menü neben der Ansicht, wählen Sie **Umbenennen** aus und geben Sie dann den neuen Namen für die Ansicht ein.
1. Klicken Sie auf **Ansichten** Dropdown-![Ansichten](assets/view-icon-requests.png) und wählen Sie die Ansicht aus, die Sie bearbeiten möchten.
1. <span class="preview">Um ein benutzerdefiniertes Feld als Spalte hinzuzufügen, klicken Sie auf das Symbol **Spalte hinzufügen** ![Spalte hinzufügen](assets/add-column.png) rechts im Bildschirm und klicken Sie auf das Pluszeichen neben dem benutzerdefinierten Formularfeld, das Sie der Ansicht als Spalte hinzufügen möchten.</span>

   <span class="preview">Benutzerdefinierte Felder in Formularen, die an das Objekt in der Liste angehängt sind, können als Spalten hinzugefügt werden.</span>

   >[!TIP]
   >
   >Es ist derzeit nicht möglich, Spalten in der Produktionsumgebung hinzuzufügen.
1. (Optional) Klicken Sie auf **Spalten** und blenden Sie die Spalten in der Anfrageliste aus, anzeigen oder neu anordnen.

   ![Spalten-Feld](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Es können derzeit keine weiteren Spalten in der Produktionsumgebung hinzugefügt werden.

1. (Optional) Klicken Sie **Filter** und beginnen Sie mit dem Hinzufügen von Bedingungen für die Anfragen, die Sie auf der Registerkarte „Planung“ anzeigen möchten.

   ![Filter in der Registerkarte „Planungsanfragen“ bearbeiten](assets/filters-editing-box-in-requests-planning-tab.png)

   Sie können nach den folgenden Feldern filtern:

   * **Workspace**: Der Arbeitsbereich, mit dem das Anfrageformular verknüpft ist.
   * **Datensatztyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
   * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
   * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
   * **Status**: Der Status der Anfrage.
   * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anfrage von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.

   <span class="preview">In der Vorschau -Umgebung können Sie auch nach beliebigen benutzerdefinierten Feldern filtern, die der Ansicht hinzugefügt wurden.</span>

   Es können mehrere Filter entweder durch „Und **oder** Oder **verbunden**.
Die Anfrageliste wird automatisch gefiltert, wenn Sie die Filterbedingungen hinzufügen.



>[!IMPORTANT]
>
> * Änderungen an Ansichten werden automatisch gespeichert.
> * Änderungen an Ansichten sind für alle sichtbar, die die Ansicht verwenden.

## Hinzufügen der Ansicht zu einer Layout-Vorlage.

Ein Workfront-Administrator kann die neue Ansicht zu Layout-Vorlagen hinzufügen.

Anweisungen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Ansicht freigeben

Sie können Ansichten, die Sie erstellen, für andere Benutzer, Teams oder Gruppen freigeben.

1. So greifen Sie auf die Anfragenliste zu:

   {{step1-to-requests}}

1. Suchen Sie in der Anfragenliste die Ansicht, die Sie freigeben möchten.
1. Bewegen Sie den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie dann auf das Dreipunkt-Menü, wenn es angezeigt wird.
1. Wählen Sie **Freigeben** aus.
1. Geben Sie in dem daraufhin angezeigten Dialogfeld die Namen der Benutzer, Teams oder Gruppen ein, für die Sie die Ansicht freigeben möchten, und wählen Sie sie dann aus der Liste aus.
1. Klicken Sie auf **Speichern**.

