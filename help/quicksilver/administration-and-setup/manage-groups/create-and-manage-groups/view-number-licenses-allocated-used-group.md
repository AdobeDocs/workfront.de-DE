---
title: Anzahl der in einer Gruppe zugewiesenen und verwendeten Lizenzen anzeigen
description: Als Adobe Workfront-Administrator können Sie die Zählung der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und deren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Anzahl der in einer Gruppe zugewiesenen und verwendeten Lizenzen anzeigen

Als Adobe Workfront-Administrator können Sie die Zählung der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und deren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!IMPORTANT]
>
>Die Lizenz eines Benutzers wird nur dann in einer bestimmten Gruppe gezählt, wenn es sich bei der Gruppe um die Startseite des Benutzers handelt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

## Anzahl der in einer Gruppe verwendeten Lizenzen anzeigen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Rufen Sie auf der angezeigten Seite im Kopfzeilenbereich oben rechts den Bereich **Verwendete Lizenzen** auf, um die Anzahl der aktuell verwendeten Lizenzen für **Plan** und **Arbeit** anzuzeigen.

   Wenn Sie eine Gruppe der obersten Ebene anzeigen und der Workfront-Administrator eine Höchstzahl für jeden Lizenztyp für die Gruppe definiert hat, werden diese Zahlen ebenfalls angezeigt. In der unten stehenden Gruppe können beispielsweise maximal 10 Benutzer über eine Planlizenz und 15 über eine Work-Lizenz verfügen:

   ![](assets/licenses-used-allocated.png)

   Informationen dazu, wie ein Workfront-Administrator eine Höchstzahl zugewiesener Lizenzen für eine Gruppe definiert, finden Sie im Abschnitt [Festlegen der maximalen Lizenzanzahl für eine Home Group](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) im Artikel [Verwalten verfügbarer Lizenzen in Ihrem System](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Wenn es sich bei der Gruppe, die Sie betrachten, um eine Untergruppe handelt, können Sie nur die Anzahl der verwendeten Lizenzen anzeigen, nicht die maximale Anzahl der Lizenzen, die der Gruppe zugewiesen sind. Dies liegt daran, dass Workfront-Administratoren keine maximale Lizenzanzahl für eine Untergruppe definieren.
   >
   >![](assets/subgroup-used-licenses-only.png)
   >

1. Klicken Sie für separate Zählungen für jeden Lizenztyp, der derzeit in der Gruppe verwendet wird (einschließlich Überprüfung und Anforderung), auf den Textbereich direkt unter **Verwendete Lizenzen:**.

   ![](assets/click-text-to-see-more.png)

   Das angezeigte Feld enthält dieselben Informationen für alle vier Workfront-Lizenztypen: Plan, Arbeit, Überprüfung und Anforderung. Unten im Feld sehen Sie die Gesamtzahl der Lizenzen, die von Mitgliedern dieser Gruppe oder einer ihrer Untergruppen verwendet werden:

   ![](assets/more-license-info.png)

   Bei Review- und Anfragelektionen wird in der Spalte &quot;Maximal&quot;immer &quot;Unbegrenzt&quot;angezeigt.
