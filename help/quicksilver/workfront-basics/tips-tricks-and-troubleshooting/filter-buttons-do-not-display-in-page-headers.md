---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterschaltflächen werden nicht in Seitenüberschriften angezeigt
description: Lesen Sie diesen Artikel zur Fehlerbehebung bei Filterschaltflächen, die nicht in Seitenkopfzeilen angezeigt werden.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 3%

---

# Filterschaltflächen werden nicht in Seitenüberschriften angezeigt

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problem

Die folgenden Filterschaltflächen werden nicht in den entsprechenden Bereichen angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] Bereich</strong></td> 
   <td><strong>Filter-Schaltflächen</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL-Projekte] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projekte, an denen ich mitwirke]</p> </li> 
     <li> <p>[!UICONTROL Projekte in meinem Besitz]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Arbeitszeittabellen]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Meine Arbeitszeittabellen-Genehmigungen]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Meine Arbeitszeittabellen]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Die Filterschaltflächen im Bereich [!UICONTROL Projekte und Arbeitszeittabellen] werden nicht angezeigt, da die entsprechenden Filter nicht in der auf den Benutzer angewendeten Layout-Vorlage enthalten sind. Der [!DNL Workfront] muss eine Layoutvorlage zuweisen, die die Filter enthält.

>[!NOTE]
>
>Manchmal werden die Filter aus dem Bereich [!UICONTROL Listensteuerelemente] in [!UICONTROL Setup] entfernt. Der [!DNL Workfront] muss sie in die Listen in diesem Bereich aufnehmen, damit sie in den Layoutvorlagen verfügbar sind.

1. Stellen Sie sicher, dass die Layout-Vorlage die folgenden Filter anzeigt:

   * [!UICONTROL Projekte, an denen ich mitwirke] und [!UICONTROL Projekte, ] ich besitze) [!UICONTROL Projekte] Bereich
   * [!UICONTROL Meine Arbeitszeittabellen] und [!UICONTROL Meine Arbeitszeittabellen] im Bereich [!UICONTROL Arbeitszeittabelle]

   Gehen Sie dazu folgendermaßen vor:

   1. Zugriff auf die Layout-Vorlage.
   1. Wählen Sie **[!UICONTROL Listen]** unter **[!UICONTROL Anpassen, was Benutzer sehen]** aus.
   1. Wählen Sie **[!UICONTROL Projekte]** oder **[!UICONTROL Arbeitszeittabellen]** unter **[!UICONTROL Wählen Sie eine anzupassende Liste aus]**.
   1. Überprüfen Sie **[!UICONTROL Abschnitt]** Filter), ob **[!UICONTROL Projekte, an denen ich]** bin, **[!UICONTROL Projekte, deren Inhaber ich bin]** (für Projekte) und **[!UICONTROL Meine Arbeitszeittabellen-Genehmigungen]** und **[!UICONTROL Meine Arbeitszeittabellen]** (für Arbeitszeittabellen) ausgewählt sind.
   1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Weisen Sie die Layout-Vorlage den richtigen Benutzern, Aufgabengebieten, Teams oder Gruppen zu. Weitere Informationen finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
