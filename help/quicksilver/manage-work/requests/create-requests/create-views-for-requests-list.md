---
product-area: requests
navigation-topic: create-requests
title: Erstellen und Verwalten von Ansichten im Bereich „Anfragen“
description: Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 7%

---


# Erstellen und Verwalten von Ansichten im Bereich „Anfragen“

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>





Wenn Sie das neue anfragende Erlebnis in Adobe Workfront verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern. Zu diesen Ansichten gehören Filter und Spaltenanordnungen.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Diese Funktion ist nur in der neuen anfragenden -Version im Bereich Anfragen verfügbar.
>* Anzeigeeinstellungen sind auch im Widget Meine Anfragen auf der Startseite verfügbar. Die Ansichten aus dem Bereich Anfragen sind jedoch von denen aus dem Widget Meine Anfragen getrennt.
>* Die Anfragenliste im Bereich Anfragen verwendet die erweiterte Liste in Workfront. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

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
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ansicht für Anfragen erstellen

Sie können eine Ansicht im Bereich Anfragen von Workfront erstellen, wenn Sie das neue Anfrageerlebnis verwenden.

1. So greifen Sie auf die Anfragenliste zu:

   {{step1-to-requests}}

1. Stellen Sie sicher **dass die Einstellung** Neues Erlebnis verwenden“ aktiviert ist.

1. Klicken Sie in der **Anfragen**-Liste auf das **Ansichten** Dropdown-Menü ![Ansichten](assets/view-icon-requests.png) und klicken Sie auf **Neue Ansicht**.

   ![Neue Ansicht](assets/create-new-view.png)

1. Geben Sie einen Namen für die neue Ansicht ein und klicken Sie auf **Erstellen**.
1. Fahren Sie [Bearbeiten einer Ansicht im Bereich Anfragen](#edit-a-view-in-the-requests-area) fort.

## Ansicht für Anfragen bearbeiten

Sie können bestehende Ansichten bearbeiten, einschließlich der Ansichten, die Sie gerade im Bereich Anfragen von Workfront erstellt haben.

Durch Bearbeiten einer Ansicht im Bereich Anfragen können Sie die folgenden Elemente der Ansicht ändern:

* Name
* Filter
* Spalten

Die Änderungen, die Sie an einer Ansicht vornehmen, sind für alle sichtbar, für die Sie die Ansicht freigeben.

1. Um auf eine Liste von Anfragen in zuzugreifen, gehen Sie folgendermaßen vor:

   {{step1-to-requests}}

1. Stellen Sie sicher **dass die Einstellung** Neues Erlebnis verwenden“ aktiviert ist.
1. Suchen Sie in der **Anfragen**-Liste die Ansicht, die Sie bearbeiten möchten, aus dem Dropdown-Menü **Ansichten** (![-Dropdown](assets/view-icon-requests.png).

1. Klicken Sie auf **Ansichten** Dropdown![Ansichten](assets/view-icon-requests.png) und klicken Sie auf das Dreipunkt-Menü neben der Ansicht, wählen Sie **Umbenennen** aus und geben Sie dann den neuen Namen für die Ansicht ein.
1. Drücken Sie die Eingabetaste, um den neuen Namen zu speichern.
1. Klicken Sie auf **Ansichten** Dropdown-![Ansichten](assets/view-icon-requests.png) und wählen Sie die Ansicht aus, die Sie bearbeiten möchten.
1. Um ein Feld als Spalte hinzuzufügen, klicken Sie auf das Symbol **Spalte hinzufügen** ![Spalte hinzufügen](assets/add-column.png) in der oberen rechten Ecke der Liste.

   Der **Spalten-Manager** wird geöffnet.
1. Klicken Sie auf das Pluszeichen neben dem Feld, das Sie als Spalte zur Ansicht hinzufügen möchten, und klicken Sie dann auf **Speichern**.

   Felder, die mit den Objekten in der Liste verknüpft sind, können als Spalten hinzugefügt werden. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Felder, die Sie den Spalten hinzufügen, müssen vorhanden sein, bevor sie im **Spalten-Manager“ verfügbar**.


1. (Optional) Klicken Sie auf **Spalten**, um das Feld **Sichtbarkeit und Reihenfolge** zu öffnen.
1. Aktivieren Sie die Einstellung für jedes Feld, das in der Liste angezeigt werden soll, deaktivieren Sie sie, um sie auszublenden, oder ziehen Sie die Felder in eine andere Reihenfolge.

1. (Optional) Klicken Sie **Filter** und fügen Sie Bedingungen für die Anforderungen hinzu, die Sie anzeigen möchten.

   Sie können nach den folgenden Anfragefeldern filtern:

   * **Workspace**: Der Arbeitsbereich, mit dem das Anfrageformular verknüpft ist.
   * **Objekttyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
   * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
   * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
   * **Status**: Der Status der Anfrage.
   * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anfrage von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.

   Sie können auch nach allen Feldern filtern, die der Ansicht für ein in der Ansicht sichtbares Objekt hinzugefügt wurden.

   Es können mehrere Filter entweder durch „Und **oder** Oder **verbunden**.
Die Anfrageliste wird automatisch gefiltert, wenn Sie die Filterbedingungen hinzufügen.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Änderungen an Ansichten werden automatisch gespeichert.
> * Änderungen an Ansichten sind für alle sichtbar, die die Ansicht verwenden.
> * Verwenden Sie den **Me (angemeldeter Benutzer),** den Platzhalter in jedem Feld zu filtern, das Benutzer als Wert enthält.

## Fügen Sie die Anfrageansicht zu einer Layout-Vorlage hinzu.

Ein Workfront-Administrator kann die neue Ansicht zu Layout-Vorlagen hinzufügen.

Anweisungen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Ansicht freigeben

Sie können Ansichten, die Sie erstellen, für andere Benutzer, Teams oder Gruppen freigeben.

1. Um auf eine Liste von Anfragen in zuzugreifen, gehen Sie folgendermaßen vor:

   {{step1-to-requests}}

1. Stellen Sie sicher **dass die Einstellung** Neues Erlebnis verwenden“ aktiviert ist.
1. Suchen Sie in **Liste** Anfragen“ die Ansicht, die Sie freigeben möchten.
1. Bewegen Sie den Mauszeiger über die Ansicht, die Sie freigeben möchten, klicken Sie dann auf das Dreipunkt-Menü rechts neben dem Ansichtsnamen und dann auf **Freigeben**.
1. Geben **im Feld** die Personen, Teams, Rollen, Gruppen oder Unternehmen ein, für die Sie die Ansicht freigeben möchten, und wählen Sie sie dann aus der Liste aus, wenn sie angezeigt werden.
1. Klicken Sie auf **Speichern**.

   Die Ansicht wird für die angegebenen Entitäten freigegeben. Sie können die aktualisierten Ansichtselemente anzeigen, die Sie für die Ansicht bearbeitet haben, bevor sie sie freigeben. <span class="preview">Wenn sie die Ansicht aktualisieren, sind ihre Änderungen für andere nicht sichtbar, es sei denn, sie erstellen eine Kopie derselben Ansicht und behalten ihre Änderungen bei, bevor sie die Kopie freigeben. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
