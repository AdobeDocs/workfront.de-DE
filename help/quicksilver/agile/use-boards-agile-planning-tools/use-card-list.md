---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Verwenden der Kartenliste
description: Sie können eine Kartenliste in einem Workflow erstellen und die Karten zu Iterationen hinzufügen.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Kartenliste verwenden

>[!IMPORTANT]
>
>Workflows sind nicht für alle Kunden verfügbar.

Sie können eine Kartenliste in einem Workflow erstellen und die Karten zu Iterationen hinzufügen.

Die Kartenliste kann als Arbeitsrückstand für den Workflow dienen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL Anforderung] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Karten zur Kartenliste hinzufügen

{{step1-to-boards}}

1. Um einen Workstream zu öffnen, klicken Sie auf [!UICONTROL **Workflow anzeigen**].
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
      <td>Die geschätzte Anzahl der Stunden, die für das Ausfüllen der Karte benötigt werden. Dies ist nur ein manueller Eintrag.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Wählen Sie einen Status für die Karte aus.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterationen]</strong></td> 
      <td>Wählen Sie eine Iteration aus, der die Karte zugewiesen werden soll.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Zuweisung]</strong></td> 
      <td><p>Um die Karte zuzuweisen, geben Sie einen Namen in das Suchfeld ein und wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird. Sie können sowohl Einzelpersonen als auch Teams hinzufügen und einer Karte mehrere Personen oder Teams zuweisen.</p><p>Zugewiesene Benutzer müssen Mitglieder im Workflow-Stream sein oder sie werden nicht in der Auswahlliste angezeigt.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf [!UICONTROL **Speichern**].
1. Fügen Sie weitere Karten hinzu, bis Sie die Kartenliste erstellt haben.

## Karten anzeigen

Um alle Karten für den Workflow in einer Liste anzuzeigen, klicken Sie auf der Registerkarte &quot;Kartenliste&quot;auf [!UICONTROL **Listenansicht**] .

Um alle Karten für den Workstream, gruppiert nach Iteration, anzuzeigen, klicken Sie auf [!UICONTROL **Iterationsansicht**]. Ungeplante Karten werden in ihrer eigenen Gruppe angezeigt.

Um eine vorhandene Karte zu bearbeiten, wählen Sie sie in der Liste aus und klicken Sie auf [!UICONTROL **Bearbeiten**].

Um eine Karte zu löschen, wählen Sie sie in der Liste aus und klicken Sie auf [!UICONTROL **Löschen**].

### Filterkarten

Karten können nur über die Iterationskarte archiviert werden. Wenn eine Karte archiviert wird, wird sie nicht in der Kartenliste angezeigt, es sei denn, Sie filtern nach archivierten Karten. Informationen zum Archivieren einer Karte finden Sie unter [Löschen oder Archivieren einer Karte aus einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Greifen Sie auf die Kartenliste für den Workstream zu.
1. Klicken Sie auf [!UICONTROL **Filter**] und wählen Sie [!UICONTROL **Alle**], [!UICONTROL **Aktive Karten**] oder [!UICONTROL **Archivierte Karten**] aus.

   Wenn ein anderer Filter als der Standard auf die Kartenliste angewendet wird, wird auf dem Filtersymbol ![Angewendeter Filter](assets/boards-filterapplied-30x30.png) ein Indikator angezeigt.

### In der Kartenliste suchen

1. Greifen Sie auf die Kartenliste für den Workstream zu.
1. Klicken Sie auf [!UICONTROL **Suchen**] und geben Sie einen Suchbegriff ein. Drücken Sie dann die Eingabetaste.

   Alle Karten, die den Suchbegriff enthalten, werden angezeigt.
Klicken Sie auf das X, um die Suche zu löschen.

   ![Suche nach Karten in einer Pinnwand](assets/boards-searchbox.png)

## Hinzufügen von Karten zu einer Iteration

>[!NOTE]
>
>Sie müssen eine Iteration erstellen, bevor Sie ihr Karten hinzufügen können. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Greifen Sie auf die Kartenliste für den Workstream zu.
1. Wählen Sie die [!UICONTROL **Iterationsansicht**] aus, um zu sehen, welche Karten einer Iteration zugewiesen sind und welche nicht geplant sind.
1. Wählen Sie eine nicht geplante Karte in der Liste aus und klicken Sie auf [!UICONTROL **Bearbeiten**].
1. Wählen Sie im Feld [!UICONTROL **Iterationen**] eine Iteration aus.
1. Wenn Sie Story-Punkte verwenden, geben Sie einen Wert in das Feld [!UICONTROL **Schätzung**] ein.
1. Klicken Sie auf [!UICONTROL **Speichern**].

   Die Karte wird in die Iteration verschoben und die Iterationsmetriken spiegeln die Anzahl der Karten und Punkte wider.

   Sie können auch eine Karte aus der Gruppe Ungeplante Karten in die Iteration ziehen oder auf [!UICONTROL **Karte hinzufügen**] klicken, um der Iteration eine neue Karte hinzuzufügen.

>[!TIP]
>
>Wenn Sie eine Iterationsprozessplatine erstellt haben, werden alle ungeplanten Karten auf der Kartenliste in der Spalte [!UICONTROL Rückprotokoll] angezeigt. Wenn eine Karte in eine andere Spalte verschoben wird, wird sie Teil der aktiven Iteration. Karten, die Sie der Iteration in der Kartenliste hinzufügen, werden einer Spalte entsprechend ihrem Status hinzugefügt.
