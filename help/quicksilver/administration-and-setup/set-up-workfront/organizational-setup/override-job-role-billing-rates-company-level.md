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
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene

{{highlighted-preview}}

Bei der Erstellung einer Auftragsrolle haben Sie die Möglichkeit, einen Stundensatz für die Abrechnung dieser Rolle auszuwählen. <span class="preview">Sie können mehrere unternehmensspezifische Abrechnungsraten pro Stunde erstellen. Jede Abrechnungsrate ist für einen bestimmten Datumsbereich wirksam.</span>

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
1. <span class="preview">Klicken Sie auf den Unternehmensnamen in der Liste.</span>
1. <span class="preview">Klicken **[!UICONTROL Abrechnungssätze]** im linken Bereich.</span>
1. <span class="preview">Klicken **[!UICONTROL Abrechnungsrate hinzufügen] > [!UICONTROL Neuer Abrechnungskurs]** oder wählen Sie eine vorhandene Rate aus, die bearbeitet werden soll.</span>
1. <span class="preview">Im [!UICONTROL Neuer Abrechnungskurs] ein Dialogfeld, wählen Sie eine [!UICONTROL **Auftragsrolle**] , um den Abrechnungskurs für festzulegen.</span>

   <span class="preview">Die [!UICONTROL **Standardabrechnungsrate**] zeigt die Rate auf Systemebene für diese Auftragsrolle an.</span>

   <span class="preview">![Dialogfeld &quot;Neue Abrechnungsrate&quot;](assets/date-effective-billing-rates-for-company.png)</span>

1. <span class="preview">Im [!DNL **Abrechnungssätze 1**] Geben Sie den Abrechnungskurs ein. Klicken Sie anschließend auf [!UICONTROL **Speichern**] um die Abrechnungsrate einmal zu überschreiben.</span>

   <span class="preview">Oder</span>

   <span class="preview">Klicken [!UICONTROL **Rate hinzufügen**] , um weitere Abrechnungssätze mit effektiven Daten hinzuzufügen.</span>

1. <span class="preview">(Bedingt) Wenn Sie mehr als eine Abrechnungsrate hinzufügen, geben Sie die folgenden Informationen ein:</span>

   * <span class="preview">**[!UICONTROL Abrechnungssätze 1], 2 usw.**: Der Wert des Abrechnungskurses für den Zeitraum.</span>
   * <span class="preview">**[!UICONTROL Startdatum ]**: Das Datum, an dem die Rate wirksam wird.</span>
   * <span class="preview">**[!UICONTROL Enddatum ]**: Das Datum, an dem die Rate endet.</span>

     <span class="preview">Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum. Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie Abrechnungsrate 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird zum Abrechnungskurs 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.</span>

1. <span class="preview">Klicken Sie auf [!UICONTROL **Speichern**].</span>

   >[!NOTE]
   >
   >Die auf dem Projekt geänderten Job-Rollenraten wirken sich nur auf dieses Projekt aus. Die auf Unternehmensebene geänderten Tarife wirken sich auf alle Projekte aus. Weitere Informationen finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
