---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterschaltflächen werden nicht in Seitenkopfzeilen angezeigt
description: Lesen Sie diesen Artikel, um Probleme mit Filterschaltflächen zu beheben, die nicht in Seitenkopfzeilen angezeigt werden.
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Filterschaltflächen werden nicht in Seitenkopfzeilen angezeigt

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Die folgenden Filterschaltflächen werden in den jeweiligen Bereichen nicht angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Filterschaltflächen</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projekte] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte, an denen ich arbeite]</p> </li> 
     <li> <p>[!UICONTROL Projekte, deren Eigentümer ich bin]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Die Filterschaltflächen im [!UICONTROL Projekte und Timesheets] -Bereich wird nicht angezeigt, da die entsprechenden Filter nicht in der Layout-Vorlage enthalten sind, die auf den Benutzer angewendet wird. Die [!DNL Workfront] -Administrator muss eine Layoutvorlage zuweisen, die die Filter enthält.

>[!NOTE]
>
>Manchmal werden die Filter aus dem [!UICONTROL Listenelemente] Gebiet in [!UICONTROL Einrichtung]. Die [!DNL Workfront] -Administrator muss sie in die Listen in diesem Bereich aufnehmen, damit sie in den Layoutvorlagen verfügbar sind.

1. Stellen Sie sicher, dass die Layoutvorlage die folgenden Filter anzeigt:

   * [!UICONTROL Projekte, an denen ich arbeite] und [!UICONTROL Eigene Projekte] im [!UICONTROL Projekte] area
   * [!UICONTROL Meine Datenblatt-Genehmigungen] und [!UICONTROL Meine Timesheets] im [!UICONTROL Datenblatt] area

   Gehen Sie dazu folgendermaßen vor:

   1. Greifen Sie auf die Layout-Vorlage zu.
   1. Auswählen **[!UICONTROL Listen]** under **[!UICONTROL Anpassen der Ansicht von Benutzern]**.
   1. Auswählen **[!UICONTROL Projekte]** oder **[!UICONTROL Timesheets]** under **[!UICONTROL Liste zum Anpassen auswählen]**.
   1. Im **[!UICONTROL Filter]** überprüfen Sie, ob **[!UICONTROL Projekte, an denen ich arbeite]**, **[!UICONTROL Eigene Projekte]** (für Projekte) und **[!UICONTROL Meine Datenblatt-Genehmigungen]** und **[!UICONTROL Meine Timesheets]** (für Timesheets) ausgewählt sind.
   1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Weisen Sie die Layoutvorlage den richtigen Benutzern, Auftragsrollen, Teams oder Gruppen zu. Weitere Informationen finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
