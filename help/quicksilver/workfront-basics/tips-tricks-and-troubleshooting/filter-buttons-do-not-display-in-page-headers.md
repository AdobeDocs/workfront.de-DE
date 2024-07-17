---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterschaltflächen werden nicht in Seitenkopfzeilen angezeigt
description: Lesen Sie diesen Artikel, um Probleme mit Filterschaltflächen zu beheben, die nicht in Seitenkopfzeilen angezeigt werden.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
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
   <td> <p>Alle</p> </td> 
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

Die Filterschaltflächen im Bereich [!UICONTROL Projekte und Timesheets] werden nicht angezeigt, da die entsprechenden Filter nicht in der Layout-Vorlage enthalten sind, die auf den Benutzer angewendet wird. Der Administrator [!DNL Workfront] muss eine Layoutvorlage zuweisen, die die Filter enthält.

>[!NOTE]
>
>Manchmal werden die Filter aus dem Bereich [!UICONTROL Listen-Steuerelemente] in der [!UICONTROL Einrichtung] entfernt. Der Administrator [!DNL Workfront] muss sie in die Listen in diesem Bereich aufnehmen, damit sie in den Layoutvorlagen verfügbar sind.

1. Stellen Sie sicher, dass die Layoutvorlage die folgenden Filter anzeigt:

   * [!UICONTROL Projekte, die ich auf] und [!UICONTROL Projekte, deren Eigentümer ich bin] im Bereich [!UICONTROL Projekte] befinde
   * [!UICONTROL My Timesheet Approvals] und [!UICONTROL My Timesheets] im Bereich [!UICONTROL Timesheet]

   Gehen Sie dazu folgendermaßen vor:

   1. Greifen Sie auf die Layout-Vorlage zu.
   1. Wählen Sie **[!UICONTROL Listen]** unter **[!UICONTROL Anpassen, was Benutzer sehen]**.
   1. Wählen Sie **[!UICONTROL Projekte]** oder **[!UICONTROL Timesheets]** unter **[!UICONTROL Wählen Sie eine Liste zum Anpassen von]** aus.
   1. Überprüfen Sie im Abschnitt **[!UICONTROL Filter]** , ob die Optionen **[!UICONTROL Projekte, die ich verwende,]**, **[!UICONTROL Projekte, deren Eigentümer ich bin]** (für Projekte) und **[!UICONTROL Meine Timesheet-Genehmigungen]** und **[!UICONTROL Meine Timesheets]** (für Timesheets) ausgewählt sind.
   1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Weisen Sie die Layoutvorlage den richtigen Benutzern, Auftragsrollen, Teams oder Gruppen zu. Weitere Informationen finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
