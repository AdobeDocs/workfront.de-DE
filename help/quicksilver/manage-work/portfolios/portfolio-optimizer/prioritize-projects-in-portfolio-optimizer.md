---
title: Priorisieren von Projekten in Portfolio Optimizer
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Sie können Ihre Portfolio Optimizer-Projekte priorisieren, um die Reihenfolge festzulegen, in der sie abgeschlossen werden sollen.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Priorisieren von Projekten im [!UICONTROL Portfolio Optimizer]

Sie können Ihre Portfolios im [!UICONTROL Projektoptimierer] priorisieren, um die Reihenfolge festzulegen, in der sie abgeschlossen werden sollen.

Beachten Sie Folgendes bei Verwendung von [!UICONTROL Portfolio Optimizer]:

* Die Projekte am oberen Rand des [!UICONTROL Portfolio Optimizer] werden als wichtiger angesehen als die am unteren Rand aufgelisteten. Sie müssen die Projekte in der Reihenfolge ihrer Priorität im [!UICONTROL Portfolio Optimizer] abschließen, damit das Portfolio optimiert werden kann.
* Die Priorität von Projekten im [!UICONTROL Projektoptimierung] ist nicht mit dem Feld [!UICONTROL Portfolio-Priorität] auf der Registerkarte [!UICONTROL Projektdetails] eines Projekts verbunden.

  Das Feld [!UICONTROL Priorität] auf der Registerkarte [!UICONTROL Projektdetails] ist eine visuelle Kennzeichnung, die Sie manuell angeben, um zu verstehen, wie wichtig ein Projekt sein sollte.

* Die Projektpriorität im Portfolio Optimizer ist in der [!DNL Resource Planner] sichtbar, sofern sie dort aktiviert ist. In der [!DNL Resource Planner] erhalten Projekte Ressourcen in der Reihenfolge ihrer Priorität [!UICONTROL Ressourcenplaner] und nicht die Priorität des [!UICONTROL Portfolios Priority].

  Informationen zum Priorisieren von Projekten im [!UICONTROL Ressourcenplaner] finden Sie im Artikel [Priorisieren von Projekten im [!UICONTROL Ressourcenplaner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Im Bereich **[!UICONTROL Projektpriorität]** von [!UICONTROL Portfolio Optimizer] werden standardmäßig Projekte in der Reihenfolge [!UICONTROL Geplante Startdaten] und [!UICONTROL Nettowert] angezeigt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>[!UICONTROL Business] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Zugriff auf Projekte und Portfolios bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Verwalten] Berechtigungen für das Portfolio</p> <p>Contribute oder höhere Berechtigungen für Projekte</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Projektpriorität im [!UICONTROL Portfolio Optimizer] ändern

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **[!UICONTROL Portfolio]**.
1. (Optional) Wählen Sie im Dropdown-Menü **[!UICONTROL Filter]** den richtigen Filter aus, um die richtige Liste der Portfolios anzuzeigen.
1. Klicken Sie auf den Namen eines Portfolios, um es zu öffnen.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Portfolio-Optimierung]** .
1. Ändern Sie im Bereich [!UICONTROL Projektoptimierung] die Priorität Ihrer Projekte, indem Sie die Projekte nach Priorität ziehen und dann an die gewünschte Anzeigeposition ziehen.

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Klicken Sie im Bereich zur Projektoptimierung auf **[!UICONTROL Priorität festlegen]** , wenn Sie die Neuanordnen Ihrer Projekte abgeschlossen haben. Die Projekte erhalten eine neue Nummer, die auf der neuen Bestellung basiert.

1. Klicken Sie auf **[!UICONTROL Speichern]** , um die neue Projektpriorität im [!UICONTROL Portfolio Optimizer] zu speichern. Die Priorität wird als Zahl in der Spalte mit der Zahl **#** aufgeführt.

   >[!TIP]
   >
   >Dies ändert nicht unbedingt die Reihenfolge der Portfolios im [!UICONTROL Projektoptimierer], da die Projektliste möglicherweise durch eine andere Spalte als die Spalte **#** sortiert wird. Klicken Sie auf die Spaltenüberschrift **#** , um die Liste nach Projektpriorität anzuordnen.

   Sie können die Projektpriorität so anzeigen, wie sie im [!UICONTROL Projektoptimierung] im Ressourcenplaner angezeigt wird, indem Sie die Einstellung **[!UICONTROL Portfolio-Prioritäten anzeigen]** im Ressourcenplaner aktivieren.

   Informationen zum Priorisieren von Projekten im [!UICONTROL Ressourcenplaner] finden Sie im Artikel [Priorisieren von Projekten im [!UICONTROL Ressourcenplaner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
