---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Unternehmensebene
description: Bei der Erstellung einer Auftragsrolle haben Sie die Möglichkeit, einen Stundensatz für die Abrechnung dieser Rolle auszuwählen. Sie können eine unternehmensspezifische Abrechnungsrate erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene

Bei der Erstellung einer Auftragsrolle haben Sie die Möglichkeit, einen Stundensatz für die Abrechnung dieser Rolle auszuwählen. Sie können mehrere unternehmensspezifische Abrechnungsraten pro Stunde erstellen. Jede Abrechnungsrate ist für einen bestimmten Datumsbereich wirksam.

Auf Projektebene können Sie eine Option aktivieren, mit der die Abrechnungsraten auf Unternehmensebene außer Kraft gesetzt werden können. Weitere Informationen finden Sie unter [Überschreiben von Abrechnungsraten auf Projektebene mit Abrechnungsraten auf Unternehmensebene](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: [!UICONTROL Standard]</p>
   <p>Oder</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf Unternehmen, wenn Sie kein Systemadministrator sind</p>
   <p>Zugriff auf Finanzdaten bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Feste Abrechnungsrate für eine bestimmte Stellenrolle überschreiben oder ändern

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Unternehmen]**.
1. Suchen Sie das Unternehmen, dem die Auftragsrolle zugewiesen ist.
1. Klicken Sie auf den Unternehmensnamen in der Liste.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Abrechnungsraten]**.
1. Klicken Sie auf **[!UICONTROL Abrechnungsrate hinzufügen] > [!UICONTROL Neue Abrechnungsrate]** oder wählen Sie eine vorhandene Rate aus, die bearbeitet werden soll.
1. Wählen Sie im Dialogfeld [!UICONTROL Neue Abrechnungsrate] eine [!UICONTROL **Auftragsrolle**] aus, um die Abrechnungsrate für festzulegen.

   Die [!UICONTROL **standardmäßige Abrechnungsrate**] zeigt die Systemebene der Auftragsrolle an.

   ![Dialogfeld &quot;Neue Abrechnungsrate&quot;](assets/date-effective-billing-rates-for-company.png)

1. Geben Sie im Feld [!DNL **Abrechnungsraten 1**] den Abrechnungskurs ein. Klicken Sie dann auf [!UICONTROL **Speichern**] , um die Abrechnungsrate einmal zu überschreiben.

   Oder

   Klicken Sie auf [!UICONTROL **Rate hinzufügen**] , um weitere Abrechnungsraten mit effektiven Datumswerten hinzuzufügen.

1. (Bedingt) Wenn Sie mehr als eine Abrechnungsrate hinzufügen, geben Sie die folgenden Informationen ein:

   * **[!UICONTROL Abrechnungsraten 1], 2 usw.**: Der Wert des Abrechnungskurses für den Zeitraum.
   * **[!UICONTROL Startdatum]**: Das Datum, an dem die Rate wirksam wird.
   * **[!UICONTROL Enddatum]**: Das Datum, an dem die Rate endet.

     Der Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum. Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie Abrechnungsrate 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird zum Abrechnungskurs 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

1. Klicken Sie auf [!UICONTROL **Speichern**].

   >[!NOTE]
   >
   >Die auf dem Projekt geänderten Job-Rollenraten wirken sich nur auf dieses Projekt aus. Die auf Unternehmensebene geänderten Tarife wirken sich auf alle Projekte aus. Weitere Informationen finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten für Auftragsrollen und die Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
