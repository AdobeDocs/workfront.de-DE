---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene
description: Bei der Erstellung einer Auftragsrolle haben Sie die Möglichkeit, einen Stundensatz für die Abrechnung dieser Rolle auszuwählen. Sie können eine unternehmensspezifische Abrechnungsrate erstellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene

Bei der Erstellung einer Auftragsrolle haben Sie die Möglichkeit, einen Stundensatz für die Abrechnung dieser Rolle auszuwählen. Sie können eine unternehmensspezifische Abrechnungsrate erstellen.

Auf Projektebene können Sie eine Option aktivieren, mit der die Abrechnungsraten auf Unternehmensebene außer Kraft gesetzt werden können. Weitere Informationen finden Sie unter [Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf Unternehmen, wenn Sie kein Systemadministrator sind</p> <p>[!UICONTROL Zugriff auf Finanzdaten bearbeiten</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Feste Abrechnungsrate für eine bestimmte Stellenrolle überschreiben oder ändern

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Unternehmen]**.
1. Suchen Sie das Unternehmen, dem die Auftragsrolle zugewiesen ist.
1. Klicken **[!UICONTROL Unternehmen bearbeiten]** in der oberen rechten Ecke.
1. Im **[!UICONTROL Abrechnungssätze]** , wählen Sie die Auftragsrolle aus, die Sie bearbeiten möchten, und geben Sie den neuen Abrechnungskurs für diese Auftragsrolle im **[!UICONTROL Abrechnungsrate des Unternehmens]** ankreuzen.

   >[!NOTE]
   >
   >Die auf dem Projekt geänderten Job-Rollenraten wirken sich nur auf dieses Projekt aus. Die auf Unternehmensebene geänderten Tarife wirken sich auf alle Projekte aus. Weitere Informationen finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
