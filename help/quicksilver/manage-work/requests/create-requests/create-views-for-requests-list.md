---
product-area: requests
navigation-topic: create-requests
title: Erstellen und Verwalten von Ansichten im Bereich „Anfragen“
description: Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: 78ad910e8d121dda38c9a7da27b0b338e0e1dcda
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 6%

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
>* Die Anforderungsliste im Bereich &quot;Anforderungen&quot; verwendet die verbesserte Liste in Workfront. Weitere Informationen finden Sie unter [Erweiterte Listen verwenden](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebiges Workfront- oder Workflow-Paket</p>

<p>Eine beliebige Workfront Planning-Lizenz, um Workfront Planning-Anfragen in Anfragelisten anzuzeigen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p>  <p>Sie müssen Workfront-Administrator sein, um Ansichten Layoutvorlagen hinzufügen zu können</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
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

Sie können bestehende Ansichten bearbeiten, einschließlich der Ansichten, die Sie gerade im Bereich &quot;Anforderungen&quot; von Workfront erstellt haben.

Wenn Sie eine Ansicht im Bereich &quot;Anforderungen&quot; bearbeiten, können Sie die folgenden Elemente der Ansicht ändern:

* Name
* Filter
* Spalten

Die Änderungen, die Sie an einer Ansicht vornehmen, sind für alle sichtbar, für die Sie die Ansicht freigeben.

1. Um auf eine Liste von Anfragen in zuzugreifen, gehen Sie folgendermaßen vor:

   {{step1-to-requests}}

1. Stellen Sie sicher **dass die Einstellung** Neues Erlebnis verwenden“ aktiviert ist.
1. Suchen Sie in der Liste **Anforderungen** die Ansicht, die Sie bearbeiten möchten, im Dropdown-Menü **Ansichten** ![Ansichten-Dropdown](assets/view-icon-requests.png).

1. Klicken Sie auf das Dropdown-Menü **Ansichten** ![Ansichten-Dropdown](assets/view-icon-requests.png), klicken Sie auf das Menü mit drei Punkten neben der Ansicht, wählen Sie **Umbenennen** aus, und geben Sie dann den neuen Namen für die Ansicht ein.
1. Drücken Sie die Eingabetaste, um den neuen Namen zu speichern.
1. Klicken Sie auf **Ansichten** Dropdown-![Ansichten](assets/view-icon-requests.png) und wählen Sie die Ansicht aus, die Sie bearbeiten möchten.
1. Um ein Feld als Spalte hinzuzufügen, klicken Sie auf das Symbol **Spalte hinzufügen** ![Spalte hinzufügen](assets/add-column.png) in der oberen rechten Ecke der Liste.

   Der **Spalten-Manager** wird geöffnet.
1. Klicken Sie auf das Pluszeichen neben dem Feld, das Sie als Spalte zur Ansicht hinzufügen möchten, und klicken Sie dann auf **Speichern**.

   Felder, die mit den Objekten in der Liste verknüpft sind, können als Spalten hinzugefügt werden. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Felder, die Sie den Spalten hinzufügen, müssen vorhanden sein, bevor sie im **Spalten-Manager“ verfügbar**.


1. (Optional) Klicken Sie auf **Spalten**, um das Feld F **Ergibt Sichtbarkeit und Reihenfolge** zu öffnen.
1. Aktivieren Sie die Einstellung für jedes Feld, das in der Liste angezeigt werden soll, deaktivieren Sie es, um es auszublenden, oder ziehen Sie die Felder in eine andere Reihenfolge.

1. (Optional) Klicken Sie auf **Filter** und fügen Sie Bedingungen für die Anforderungen hinzu, die Sie anzeigen möchten.

   Sie können nach folgenden Anfragefeldern filtern:

   * **Arbeitsbereich**: Der Arbeitsbereich, dem das Anfrageformular zugeordnet ist.
   * **Objekttyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
   * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
   * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
   * **Status**: Der Status der Anfrage.
   * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anforderung von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.

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

1. So greifen Sie auf eine Liste von Anforderungen in den Anforderungen zu:

   {{step1-to-requests}}

1. Stellen Sie sicher, dass die Einstellung **Neues Erlebnis verwenden** aktiviert ist.
1. Suchen Sie in der Liste **Anforderungen** die Ansicht, die Sie freigeben möchten.
1. Bewegen Sie den Mauszeiger über die Ansicht, die Sie freigeben möchten, klicken Sie dann auf das Menü mit den drei Punkten rechts neben dem Namen der Ansicht, und klicken Sie dann auf **Freigeben**.
1. Geben Sie im Feld &quot;**Freigeben**&quot; die Personen, Teams, Rollen, Gruppen oder Unternehmen ein, für die Sie die Ansicht freigeben möchten, und wählen Sie sie bei ihrer Anzeige aus der Liste aus.
1. Klicken Sie auf **Speichern**.

   Die Ansicht wird für die angegebenen Entitäten freigegeben. Sie können die aktualisierten Ansichtselemente anzeigen, die Sie für die Ansicht bearbeitet haben, bevor sie sie freigeben. <span class="preview">Wenn sie die Ansicht aktualisieren, sind ihre Änderungen für andere nicht sichtbar, es sei denn, sie erstellen eine Kopie derselben Ansicht und behalten ihre Änderungen bei, bevor sie die Kopie freigeben. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
