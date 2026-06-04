---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filterschaltflächen werden in Seitenüberschriften nicht angezeigt
description: Lesen Sie diesen Artikel zur Fehlerbehebung bei Filterschaltflächen, die nicht in Seitenkopfzeilen angezeigt werden.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
TQID: https://experienceleague.adobe.com/36hMJKo4unpIxvUOmBk79XlhFvFL5TgqUaoQXxrPd7c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 20%

---

# Filterschaltflächen werden in Seitenüberschriften nicht angezeigt

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td>Beliebig</td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Abo</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
   <td> <p>[!UICONTROL Projekte] </p> </td> 
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
