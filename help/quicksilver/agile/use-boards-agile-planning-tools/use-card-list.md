---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Verwenden der Kartenliste
description: Sie können in einem Arbeitsablauf eine Kartenliste erstellen und die Karten zu Iterationen hinzufügen.
author: Courtney
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 9%

---

# Verwenden der Kartenliste

>[!IMPORTANT]
>
>Arbeitsabläufe sind nicht für alle Kunden verfügbar.

Sie können in einem Arbeitsablauf eine Kartenliste erstellen und die Karten zu Iterationen hinzufügen.

Die Kartenliste kann als Auftragsbestand für den Arbeitsablauf dienen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Karten zur Kartenliste hinzufügen

{{step1-to-boards}}

1. Um einen Arbeitsablauf zu öffnen, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**].
1. Klicken Sie auf die Registerkarte [!UICONTROL **Kartenliste**].
1. Klicken Sie auf [!UICONTROL **Karte hinzufügen**].
1. Fügen Sie im Dialogfeld [!UICONTROL **Karte erstellen/bearbeiten**] die folgenden Informationen hinzu:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Der Name der Karte.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Beschreibung]</strong></td> 
      <td>Eine Beschreibung der Karte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Schätzung]</strong></td> 
      <td>Die geschätzte Anzahl der Stunden für die auszufüllende Karte. Dies ist nur eine manuelle Eingabe.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Wählen Sie einen Status für die Karte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterationen]</strong></td> 
      <td>Wählen Sie eine Iteration aus, der die Karte zugewiesen werden soll.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Bevollmächtigte]</strong></td> 
      <td><p>Um die Karte zuzuweisen, geben Sie zunächst einen Namen in das Suchfeld ein und wählen Sie diese aus, wenn sie in der Liste angezeigt wird. Sie können sowohl Einzelpersonen als auch Teams hinzufügen und einer Karte mehr als eine Person oder ein Team zuweisen.</p><p>Zugewiesene Teilnehmer müssen Mitglieder im Arbeitsablauf sein, andernfalls werden sie nicht in der Auswahlliste angezeigt.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf [!UICONTROL **Speichern**].
1. Fügen Sie weitere Karten hinzu, bis Sie die Kartenliste erstellt haben.

## Karten anzeigen

Um alle Karten für den Arbeitsablauf in einer Liste anzuzeigen, klicken Sie auf [!UICONTROL **Listenansicht**] auf der Registerkarte Kartenliste .

Um alle Karten für den Arbeitsablauf nach Iteration gruppiert anzuzeigen, klicken Sie auf [!UICONTROL **Iterationsansicht**]. Nicht geplante Karten werden in einer eigenen Gruppe angezeigt.

Um eine vorhandene Karte zu bearbeiten, wählen Sie sie in der Liste aus und klicken auf [!UICONTROL **Bearbeiten**].

Um eine Karte zu löschen, wählen Sie sie in der Liste aus und klicken auf [!UICONTROL **Löschen**].

### Filterkarten

Karten können nur vom Iterationsboard aus archiviert werden. Wenn eine Karte archiviert ist, wird sie nicht in der Kartenliste angezeigt, es sei denn, Sie filtern, um archivierte Karten anzuzeigen. Informationen zum Archivieren einer Karte finden Sie unter [Löschen oder Archivieren einer Karte aus einem Board](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Rufen Sie die Kartenliste für den Arbeitsablauf auf.
1. Klicken Sie [!UICONTROL **Filtern**] und wählen Sie [!UICONTROL **Alle**], [!UICONTROL **Aktive Karten**] oder [!UICONTROL **Archivierte Karten**].

   Wenn ein anderer Filter als der Standard auf die Kartenliste angewendet wird, wird eine Anzeige auf dem Filtersymbol ![Filter angewendet](assets/boards-filterapplied-30x30.png) angezeigt.

### In der Kartenliste suchen

1. Rufen Sie die Kartenliste für den Arbeitsablauf auf.
1. Klicken Sie [!UICONTROL **Suchen**] und geben Sie einen Suchbegriff ein. Drücken Sie dann die Eingabetaste.

   Alle Karten, die den Suchbegriff enthalten, werden angezeigt.
Klicken Sie auf das X, um die Suche zu löschen.

   ![Karten in einem Board suchen](assets/boards-searchbox.png)

## Karten zu einer Iteration hinzufügen

>[!NOTE]
>
>Sie müssen eine Iteration erstellen, bevor Sie Karten hinzufügen können. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Greifen Sie auf die Kartenliste für den Arbeitsablauf zu.
1. Wählen Sie die [!UICONTROL **Iterationsansicht**] aus, um anzuzeigen, welche Karten einer Iteration zugewiesen sind und welche nicht geplant sind.
1. Wählen Sie eine ungeplante Karte in der Liste aus und klicken Sie auf [!UICONTROL **Bearbeiten**].
1. Wählen Sie im Feld [!UICONTROL **Iterationen**] eine Iteration aus.
1. Wenn Sie Textabschnittspunkte verwenden, geben Sie einen Wert in das Feld [!UICONTROL **Schätzung**] ein.
1. Klicken Sie auf [!UICONTROL **Speichern**].

   Die Karte wird in die Iteration verschoben, und die Iterationsmetriken spiegeln die Anzahl der Karten und Punkte wider.

   Sie können auch eine Karte aus der Gruppe „Ungeplante Karten“ in die Iteration ziehen und dort ablegen oder auf [!UICONTROL **Karte hinzufügen**] klicken, um der Iteration eine neue Karte hinzuzufügen.

>[!TIP]
>
>Wenn Sie eine Pinnwand für den Iterationsprozess erstellt haben, werden alle nicht geplanten Karten auf der Kartenliste in der Spalte [!UICONTROL Auftragsbestand] angezeigt. Wenn eine Karte in eine andere Spalte verschoben wird, wird sie Teil der aktiven Iteration. Karten, die Sie der Iteration in der Kartenliste hinzufügen, werden einer Spalte basierend auf ihrem Status hinzugefügt.
