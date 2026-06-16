---
product-area: programs
navigation-topic: create and manage programs
title: Hinzufügen eines vorhandenen Programms zu einer Portfolio
description: Sie können einem Portfolio vorhandene Programme hinzufügen. Da Programme nicht in zwei verschiedenen Portfolios vorhanden sein können, wird sie beim Hinzufügen eines vorhandenen Programms dauerhaft von einem Portfolio in ein anderes verschoben.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LkyWuPHqv0muTinWZT1PMKPGUNErWulIIxHmXVtPIVg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 12%

---

# Hinzufügen eines vorhandenen Programms zu einem Portfolio

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Sie können einem Portfolio vorhandene Programme hinzufügen. Da Programme nicht in zwei verschiedenen Portfolios vorhanden sein können, wird sie beim Hinzufügen eines vorhandenen Programms dauerhaft von einem Portfolio in ein anderes verschoben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Portfolios] und [!UICONTROL Programme] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für das Portfolio und das Programm</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Hinzufügen eines vorhandenen Programms zu einem Portfolio

>[!NOTE]
>
>Wenn Ihr Unternehmen sowohl den alten Workfront- als auch den Adobe-Cloud-Speicher für Dokumente verwendet, können Sie kein Adobe-Cloud-Speicherprogramm zu einem alten Speicherportfolio oder kein Legacy-Programm zu einem Adobe-Cloud-Speicherportfolio hinzufügen.
>Ihre Workfront-Instanz verfügt möglicherweise nicht über beide Arten von Dokumentspeicher.
>Weitere Informationen finden Sie unter [Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
>

So fügen Sie ein vorhandenes Programm einem anderen Portfolio hinzu:

1. Gehen Sie zu einem Portfolio und klicken Sie **[!UICONTROL linken Bereich]** Programme“.
1. Klicken Sie auf **[!UICONTROL Neues Programm]**.
1. Klicken Sie auf **[!UICONTROL Vorhandenes Programm]**.

   Das **„Programme hinzufügen** wird geöffnet. <!--check screen shot - I logged changes for this casing-->

   ![Feld „Programm hinzufügen“](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >Durch Hinzufügen eines vorhandenen Programms werden alle mit diesem Programm verknüpften Projekte in das Portfolio übernommen. Achten Sie darauf, Projekte nicht unbeabsichtigt auf diese Weise zu verschieben.

1. Geben **[!UICONTROL in das Feld]** Programme zu diesem Portfolio hinzufügen“ den Namen eines Programms ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. <!--see the name of this field, I suggested changes here-->

   Sie können mehr als ein Programm hinzufügen.

1. (Optional) Klicken Sie auf das **Löschen**-Symbol ![Löschen](assets/delete-icon.png) neben dem Namen eines Programms, wenn Sie es nicht zum Portfolio hinzufügen möchten.

1. Klicken Sie **[!UICONTROL Programme hinzufügen]**.

   Das Programm wird auf der Registerkarte **[!UICONTROL Programme]** des ausgewählten Portfolios angezeigt.

