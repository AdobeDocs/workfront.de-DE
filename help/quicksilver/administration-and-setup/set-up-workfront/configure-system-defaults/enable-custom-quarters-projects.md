---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Benutzerdefinierte Quartale für Projekte aktivieren
description: Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Benutzerdefinierte Quartale für Projekte aktivieren

<!--Audited: 11/2024-->

Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).

Sie können bis zu acht benutzerdefinierte Quartale für Ihr [!DNL Adobe Workfront] konfigurieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Quartale für Ihr [!DNL Workfront] einrichten

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte].**

1. Wählen **[!UICONTROL Abschnitt &quot;]**&quot; die Option **[!UICONTROL Benutzerdefinierte Quartale aktivieren]**.

1. Geben Sie einen Namen für das benutzerdefinierte Quartal ein, z. B. „Geschäftsjahr 1 2021“.
1. Wählen Sie das Start- und Enddatum für das benutzerdefinierte Quartal aus.

   ![Benutzerdefinierte Quartale](assets/custom-quarters-nwe.png)

1. (Optional) Klicken Sie **[!UICONTROL Benutzerdefiniertes Quartal hinzufügen]**, um dem System zusätzliche benutzerdefinierte Quartale hinzuzufügen.
1. (Optional) Erstellen Sie ein Berichterstellungselement, das sich auf das Geschäftsquartal bezieht.

   **Beispiel** Erstellen Sie einen Filter für eine [!UICONTROL Projekt]Liste und geben Sie das geplante Abschlussdatum eines Projekts an, das auf die benutzerdefinierten Quartale verweist.

   ![Projektfilter mit benutzerdefinierten Quartalen](assets/example-of-project-filter-with-custom-quarters.png)

   Die Verweise auf „Dieses Quartal“, „Nächstes Quartal“ und „Letztes Quartal“ werden durch neue Verweise auf die benutzerdefinierten Quartale ersetzt.

   Informationen zu Berichtselementen finden Sie unter [Berichtselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Informationen zum Erstellen von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
