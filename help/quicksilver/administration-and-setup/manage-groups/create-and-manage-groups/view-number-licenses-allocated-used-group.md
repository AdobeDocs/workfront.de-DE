---
title: Anzahl der zugeordneten und in einer Gruppe verwendeten Lizenzen anzeigen
description: Als Adobe Workfront-Administrator können Sie die Anzahl der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und ihren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Anzahl der zugeordneten und in einer Gruppe verwendeten Lizenzen anzeigen

Als Adobe Workfront-Administrator können Sie die Anzahl der einzelnen Lizenztypen anzeigen, die derzeit in Ihrer Gruppe und ihren Untergruppen verwendet werden. Dies ist nützlich, wenn Sie beurteilen müssen, ob Lizenzen neu verteilt werden sollen.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!IMPORTANT]
>
>Die Lizenz eines/r Benutzenden wird nur dann in einer bestimmten Gruppe gezählt, wenn es sich bei der Gruppe um die Hauptgruppe des/r Benutzenden handelt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzahl der in einer Gruppe verwendeten Lizenzen anzeigen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe.
1. Zeigen Sie auf der angezeigten Seite im Kopfzeilenbereich oben rechts den Bereich **Verwendete Lizenzen** an, um die Anzahl der **Plan** und **Work**-Lizenzen anzuzeigen.

   Wenn Sie eine Gruppe der obersten Ebene anzeigen und der Workfront-Administrator eine Höchstzahl jedes Lizenztyps für die Gruppe definiert hat, werden diese Zahlen ebenfalls angezeigt. In der folgenden Gruppe können beispielsweise maximal 10 Benutzende über eine Planlizenz und 15 über eine Arbeitslizenz verfügen:

   ![](assets/licenses-used-allocated.png)

   Informationen dazu, wie Workfront-Admins die maximale Anzahl zugewiesener Lizenzen für eine Gruppe definieren, finden Sie im Abschnitt [Festlegen der maximalen Lizenzanzahl für eine Hauptgruppe](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) im Artikel [Verwalten verfügbarer Lizenzen in Ihrem System](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Wenn es sich bei der gewünschten Gruppe um eine Untergruppe handelt, können Sie nur die Anzahl der verwendeten Lizenzen und nicht die maximale Anzahl der für die Gruppe zugewiesenen Lizenzen anzeigen. Dies liegt daran, dass Workfront-Admins keine maximale Lizenzanzahl für eine Untergruppe definieren.
   >
   >![](assets/subgroup-used-licenses-only.png)
   >

1. Für eine separate Zählung der einzelnen Lizenztypen, die derzeit in der Gruppe verwendet werden (einschließlich Überprüfung und Anfrage), klicken Sie auf den Textbereich direkt unter **Verwendete Lizenzen:**

   ![](assets/click-text-to-see-more.png)

   Das angezeigte Feld enthält dieselben Informationen für alle vier Workfront-Lizenztypen: Plan, Arbeit, Überprüfung und Anfrage. Unten im Feld sehen Sie die Gesamtzahl der Lizenzen, die von den Mitgliedern dieser Gruppe oder einer ihrer Untergruppen verwendet werden:

   ![](assets/more-license-info.png)

   Bei Prüfungs- und Anfragelizenzen wird in der Spalte Maximal immer Unbegrenzt angezeigt.
