---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Portfolios löschen und deaktivieren
description: Portfolios sind Sammlungen von Projekten oder Programmen in Adobe Workfront. Sie können ein Portfolio löschen oder deaktivieren, wenn Sie feststellen, dass es für Ihr System irrelevant ist.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 03c1f17504846fc4b8c4114ddc32df687281bc07
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 1%

---

# Portfolios löschen und deaktivieren

<!--Audited: 2/2024-->

Portfolios sind Sammlungen von Projekten oder Programmen in [!DNL Adobe Workfront]. Sie können ein Portfolio löschen oder deaktivieren, wenn Sie feststellen, dass es für Ihr System irrelevant ist.

Es wird empfohlen, ein Portfolio, das nicht mehr mit zukünftigen Projekten verknüpft werden muss, zu deaktivieren, anstatt es zu löschen, um die historischen Informationen über die Projekte zu behalten, die derzeit mit dem Portfolio und seinen Programmen verknüpft sind.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL -Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Projekte und Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für das Portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überblick über das Löschen und Deaktivieren von Portfolios

Beachten Sie bei der Entscheidung, ob Portfolios gelöscht oder deaktiviert werden sollen, Folgendes:

* Durch Löschen eines Portfolios werden die damit verbundenen Programme gelöscht.

  >[!IMPORTANT]
  >
  >Sie benötigen keine Berechtigungen für Programme, um das Portfolio löschen zu können.

* Beim Löschen eines Portfolios werden die damit verbundenen Projekte nicht gelöscht.
* Gelöschte Portfolios können nicht wiederhergestellt werden.
* Durch die Deaktivierung eines Portfolios wird sichergestellt, dass der Name des Portfolios und seiner Programme beim Erstellen eines Projekts nicht mehr Projekten zugewiesen werden kann.
* Wenn Sie ein Portfolio deaktivieren, das bereits an ein Projekt angehängt ist, wird es nicht aus dem Projekt entfernt. Wenn Sie ein deaktiviertes Portfolio aus einem Projekt entfernen, müssen Sie es erneut aktivieren, bevor Sie es erneut an das Projekt anhängen können.

## Löschen eines Portfolios

{{step1-to-portfolios}}

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie das Portfolio in der Liste aus und klicken Sie dann auf das **[!UICONTROL Löschen]**-Symbol ![Löschen](assets/delete.png).
   * Klicken Sie auf das Portfolio, um es zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Portfolionamen und dann auf **Portfolio löschen**.
1. Klicken Sie **[!UICONTROL Ja, löschen]** zur Bestätigung.

   Das Portfolio wurde gelöscht und kann nicht wiederhergestellt werden.

## Portfolio deaktivieren

Wenn Sie ein Portfolio deaktivieren, können Sie weiterhin über den Bereich [!UICONTROL Portfolios] darauf zugreifen. Wenn Benutzer versuchen, es zu einem Projekt hinzuzufügen, wird es jedoch nicht mehr in der Liste der Portfolios angezeigt.

>[!NOTE]
>
>Je nachdem, wie Ihr [!DNL Workfront]- oder Gruppenadministrator Ihre Layoutvorlage konfiguriert, wird der Bereich [!UICONTROL Portfolios] möglicherweise nicht im [!UICONTROL Hauptmenü] angezeigt. Weitere Informationen finden Sie unter [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Klicken Sie **[!UICONTROL Portfolios]** .
1. Klicken Sie auf den Namen des Portfolios.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Portfolionamen und klicken Sie dann auf **[!UICONTROL Portfolio deaktivieren]**.
Das Portfolio wird sofort deaktiviert.
1. (Optional) Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Portfolionamen und dann auf **[!UICONTROL Portfolio aktivieren]**, um es erneut zu aktivieren.


