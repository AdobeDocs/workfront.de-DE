---
content-type: overview
title: Überblick über Breadcrumbs
description: Breadcrumbs zeigen die vollständige Navigationshierarchie für alle Objekttypen an.
feature: Get Started with Workfront
exl-id: c4103f8e-4c3f-4d4d-a0eb-628c60735ab7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VryLEVTqJFgAxlm-al5y0hqxVQ71zFPi8YG1oAlox8k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 8771d66f6b7ecae9ac439456822889d4fe438649
workflow-type: tm+mt
source-wordcount: 334
ht-degree: 1%

---

# Überblick über Breadcrumbs

Breadcrumbs zeigen die vollständige Navigationshierarchie für alle Objekttypen an. Jedes Objekt im Breadcrumb-Pfad verfügt über eine Beschriftung, die den Objekttyp anzeigt. Die Seite, auf der Sie sich derzeit befinden, wird sowohl in der Kopfzeile der Seite als auch am Ende des Breadcrumb-Pfads kursiv angezeigt. Im folgenden Beispiel ist dies die Aufgabe &quot;[!UICONTROL &#x200B; für das Brand Team].

![Reduzierter Breadcrumb](assets/collapsed-breadcrumb-2026.png)

Wenn im Breadcrumb-Pfad zu viele Objekte vorhanden sind oder die Bildschirmbreite die Anzeige der vollständigen Navigationshierarchie verhindert, reduziert der Pfad einige der Breadcrumbs und gruppiert diese Objekte am Anfang des Breadcrumb-Pfads. Sowohl das Projekt als auch die aktuelle Objektseite sind immer im Breadcrumb-Pfad sichtbar.

Beispielsweise zeigt „3 more“ in der obigen Abbildung an, dass 3 Objekte nicht angezeigt werden. Diese Elemente können sich über der Projektebene oder zwischen dem Projekt und der aktuellen Seite befinden.

Wenn Sie auf &quot;[!UICONTROL mehr] klicken, können Sie die gesamte Hierarchie erweitern. Sie können auf &quot;[!UICONTROL Less] klicken, um den Breadcrumb-Pfad erneut zu reduzieren.

![Reduzierter Breadcrumb](assets/expanded-breadcrumb-2026.png)

Sie können auch die folgenden Tasten verwenden, um durch die Breadcrumbs zu navigieren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>tab</strong> </td> 
   <td> <p>Zu jedem Element in den Breadcrumbs navigieren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Eingeben</strong> </td> 
   <td> <p>Erweitern Sie einen reduzierten Breadcrumb-Pfad, reduzieren Sie einen erweiterten Breadcrumb-Pfad und öffnen Sie eine neue Seite, wenn Sie auf einen Objekt-Link klicken</p> </td> 
  </tr> 
 </tbody> 
</table>



<!--
drafted: this is no longer possible, since we removed Campaigns, but it might come back as part of Maestro: 

## Multi-object breadcrumbs

>[!NOTE]
>
>The information in this article is available only in the Preview environment when you participate in the [!UICONTROL Campaigns] beta program. The functionality described here might not be fully available yet. For more information about current available features and how to enroll, see [Campaigns beta].

Some objects can belong to multiple parent objects. For example, a project can belong to multiple campaigns. In this case, all the campaigns that the project belongs to display in the breadcrumb.

The multi-object listing in the breadcrumb (for example, the campaigns) displays the number of parent objects which expands into a list to display all the campaigns that the project is associated with. For more information, see [Add objects to a campaign](../../manage-work/campaigns/add-objects-to-a-campaign.md).


![Project with multiple campaigns in the breadcrumb](assets/project-with-multiple-campaigns-in-breadcrumb.png)

-->

## Zugreifen auf ein übergeordnetes Objekt über die Breadcrumbs

Informationen zu übergeordneten Objekten in [!DNL Workfront] finden Sie unter [Grundlegendes zu Objekten in [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Bedingt) Wenn das Objekt, zu dem Sie in einem reduzierten Breadcrumb-Pfad navigieren möchten, nicht angezeigt wird, klicken Sie auf **[!UICONTROL Mehr]** und suchen Sie dann nach dem Objekt.

   >[!NOTE]
   >
   >Wenn Sie keine Berechtigung für ein Objekt haben, ist es nicht in den Breadcrumbs sichtbar.

1. Klicken Sie auf ein beliebiges Objekt im Breadcrumb-Pfad, um auf dieses Objekt zuzugreifen.

   Die Objektseite wird geöffnet.

   Wenn Sie ein Projekt betrachten, das mit einem Objekt in Workfront Planning verbunden ist (z. B. eine Kampagne), können Sie über den Breadcrumb zwischen den Objekttypen Planning und Workfront wechseln. Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
