---
title: Anzahl der zugeordneten und in einer Gruppe verwendeten Lizenzen anzeigen
description: Als Adobe Workfront-Administrator können Sie die Anzahl der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und ihren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
TQID: https://experienceleague.adobe.com/z7vh7rdkB40A2gzfSYddUAHF-nOGqVCgpVyu729gYgE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 469
ht-degree: 7%

---

# Anzahl der zugeordneten und in einer Gruppe verwendeten Lizenzen anzeigen

Als Adobe Workfront-Administrator können Sie die Anzahl der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und ihren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!IMPORTANT]
>
>Die Lizenz eines/r Benutzenden wird nur dann in einer bestimmten Gruppe gezählt, wenn es sich bei der Gruppe um die Hauptgruppe des/r Benutzenden handelt.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anzahl der in einer Gruppe verwendeten Lizenzen anzeigen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Zeigen Sie auf der angezeigten Seite im Kopfzeilenbereich oben rechts den Bereich **Verwendete Lizenzen** an, um die Anzahl der **Plan** und **Work**-Lizenzen anzuzeigen.

   Wenn Sie eine Gruppe der obersten Ebene anzeigen und der Workfront-Administrator eine Höchstzahl jedes Lizenztyps für die Gruppe definiert hat, werden diese Zahlen ebenfalls angezeigt. In der folgenden Gruppe können beispielsweise maximal 10 Benutzende über eine Planlizenz und 15 über eine Arbeitslizenz verfügen:

   ![Zugeordnete Lizenzen](assets/licenses-used-allocated.png)

   Informationen dazu, wie Workfront-Admins die maximale Anzahl zugewiesener Lizenzen für eine Gruppe definieren, finden Sie im Abschnitt [Festlegen der maximalen Lizenzanzahl für eine Hauptgruppe](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) im Artikel [Verwalten verfügbarer Lizenzen in Ihrem System](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Wenn es sich bei der gewünschten Gruppe um eine Untergruppe handelt, können Sie nur die Anzahl der verwendeten Lizenzen und nicht die maximale Anzahl der für die Gruppe zugewiesenen Lizenzen anzeigen. Dies liegt daran, dass Workfront-Admins keine maximale Lizenzanzahl für eine Untergruppe definieren.
   >
   >![Verwendete Lizenzen in Untergruppe](assets/subgroup-used-licenses-only.png)
   >

1. Für eine separate Zählung der einzelnen Lizenztypen, die derzeit in der Gruppe verwendet werden (einschließlich Überprüfung und Anfrage), klicken Sie auf den Textbereich direkt unter **Verwendete Lizenzen:**

   ![Hier klicken, um mehr zu sehen](assets/click-text-to-see-more.png)

   Das angezeigte Feld enthält dieselben Informationen für alle vier Workfront-Lizenztypen: Plan, Arbeit, Überprüfung und Anfrage. Unten im Feld sehen Sie die Gesamtzahl der Lizenzen, die von den Mitgliedern dieser Gruppe oder einer ihrer Untergruppen verwendet werden:

   ![Weitere Lizenzinformationen](assets/more-license-info.png)

   Bei Prüfungs- und Anfragelizenzen wird in der Spalte Maximal immer Unbegrenzt angezeigt.
