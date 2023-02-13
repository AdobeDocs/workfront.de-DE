---
title: Anzahl der in einer Gruppe zugewiesenen und verwendeten Lizenzen anzeigen
description: Als Adobe Workfront-Administrator können Sie die Zählung der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und deren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
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
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront-Abo</a>*</td> 
   <td> <p>Team oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront-Lizenz</a>*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Anzahl der in einer Gruppe verwendeten Lizenzen anzeigen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Zeigen Sie auf der angezeigten Seite im Kopfzeilenbereich in der Nähe der oberen rechten Ecke die **Verwendete Lizenzen** -Bereich, um die Anzahl der **Plan** und **Arbeit** Lizenzen, die derzeit verwendet werden.

   Wenn Sie eine Gruppe der obersten Ebene anzeigen und der Workfront-Administrator eine Höchstzahl für jeden Lizenztyp für die Gruppe definiert hat, werden diese Zahlen ebenfalls angezeigt. In der unten stehenden Gruppe können beispielsweise maximal 10 Benutzer über eine Planlizenz und 15 über eine Work-Lizenz verfügen:

   ![](assets/licenses-used-allocated.png)

   Informationen dazu, wie ein Workfront-Administrator eine Höchstzahl zugewiesener Lizenzen für eine Gruppe definiert, finden Sie im Abschnitt [Maximale Lizenzanzahl für eine Home Group festlegen](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) im Artikel [Verwalten der verfügbaren Lizenzen in Ihrem System](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Wenn es sich bei der Gruppe, die Sie betrachten, um eine Untergruppe handelt, können Sie nur die Anzahl der verwendeten Lizenzen anzeigen, nicht die maximale Anzahl der Lizenzen, die der Gruppe zugewiesen sind. Dies liegt daran, dass Workfront-Administratoren keine maximale Lizenzanzahl für eine Untergruppe definieren.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Klicken Sie für separate Zählungen für jeden Lizenztyp, der derzeit in der Gruppe verwendet wird (einschließlich Review und Anforderung), auf den Textbereich direkt unten. **Verwendete Lizenzen:**

   ![](assets/click-text-to-see-more.png)

   Das angezeigte Feld enthält dieselben Informationen für alle vier Workfront-Lizenztypen: Planen, Arbeiten, Überprüfen und Anfordern. Unten im Feld sehen Sie die Gesamtzahl der Lizenzen, die von Mitgliedern dieser Gruppe oder einer ihrer Untergruppen verwendet werden:

   ![](assets/more-license-info.png)

   Bei Review- und Anfragelektionen wird in der Spalte &quot;Maximal&quot;immer &quot;Unbegrenzt&quot;angezeigt.
