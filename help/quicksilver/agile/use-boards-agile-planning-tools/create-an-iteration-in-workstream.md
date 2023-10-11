---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Erstellen einer Iteration in einem Workstream
description: Eine Iteration ist eine bestimmte Zeitdauer, die für den Abschluss der Arbeit reserviert ist. Einige agile Teams können eine Iteration als Sprint bezeichnen.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# Erstellen einer Iteration in einem Workstream

>[!IMPORTANT]
>
>Workflows stehen nur einer bestimmten Kundengruppe zur Verfügung.

Eine Iteration ist eine bestimmte Zeitdauer, die für den Abschluss der Arbeit reserviert ist. Einige agile Teams können eine Iteration als Sprint bezeichnen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

## Erstellen einer Iteration in einem Workstream

{{step1-to-boards}}

1. Öffnen Sie den Workflow, in dem Sie die Iteration hinzufügen möchten. Um einen Workflow zu öffnen, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**].
1. Erstellen Sie eine Iteration mit einer der folgenden Methoden:

   * Klicken Sie auf der Registerkarte Kartenliste in der Ansicht &quot;Iteration&quot;auf [!UICONTROL **Iteration erstellen**].
   * Klicken Sie auf der Registerkarte Kartenliste in der Listenansicht auf [!UICONTROL **Iteration erstellen**].
   * Klicken Sie auf der Registerkarte &quot;Pinnwände&quot;auf [!UICONTROL **Pinnwand hinzufügen**] und wählen [!UICONTROL **Iterationsvorgang**] als Pinnwandvorlage. Öffnen Sie dann die Iterationsfläche und klicken Sie auf [!UICONTROL **Iterationen konfigurieren**].

1. Fügen Sie im Dialogfeld Iterationsdetails die folgenden Informationen hinzu:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>Der Name der Iteration, z. B. "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Iterationslänge]</strong></td> 
      <td>Die Länge der Iteration in Tagen, Wochen oder Monaten.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Startdatum]</strong></td> 
      <td>Das Datum, an dem die Iteration beginnt. Das Enddatum wird automatisch auf Basis der Iterationslänge angegeben.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf [!UICONTROL **Speichern**].

   Die Iteration wird jetzt in der Iterationsansicht der Kartenliste und im Metrikbereich auf der Iterationsfläche angezeigt.

   Informationen zum Hinzufügen von Karten zu einer Iteration finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Vorhandene Iteration bearbeiten

1. Um einen Workflow zu öffnen, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**].
1. Öffnen Sie die Iteration mit einer der folgenden Methoden:

   * Klicken Sie auf der Registerkarte Kartenliste in der Ansicht &quot;iteration&quot;auf die [!UICONTROL **Iterationsdetails**] icon ![Iterationsdetails](assets/iteration-details-button.png).
   * Klicken Sie auf der Iterationsfläche auf die [!UICONTROL **Iterationsdetails**] icon ![Iterationsdetails](assets/iteration-details-button.png) im Metrikbereich oben rechts.

1. Im [!UICONTROL Iterationskonfiguration] bearbeiten Sie die Iteration nach Bedarf.
1. Erweitern Sie zum Ändern des Iterationsnamens [!UICONTROL **Iterationsdetails**].

   Nachdem eine Iteration gestartet wurde, können Sie nur den Iterationsnamen und nicht die Daten oder die Iterationslänge ändern.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Iteration löschen

1. Klicken Sie auf [!UICONTROL **Kartenliste**] im Workflow-Stream und öffnen Sie die Iterationsansicht.
1. Klicken Sie auf **Löschen** icon ![Löschsymbol](assets/delete.png) neben der Iteration.
1. Klicks [!UICONTROL **Iteration löschen**] in der Bestätigungsnachricht angezeigt.
