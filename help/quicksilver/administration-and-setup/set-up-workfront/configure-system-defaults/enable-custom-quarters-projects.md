---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Benutzerdefinierte Quartal für Projekte aktivieren
description: Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die nicht mit Kalenderdaten identisch sind (z. B. Geschäftstage oder Einkaufstage).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Benutzerdefinierte Quartale für Projekte aktivieren

<!--Audited: 11/2024-->

Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die nicht mit Kalenderdaten identisch sind (z. B. Geschäftstage oder Einkaufstage).

Sie können bis zu acht benutzerdefinierte Quartale für Ihr [!DNL Adobe Workfront]-System konfigurieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Quartale für Ihr [!DNL Workfront] -System einrichten

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Projekte].**

1. Wählen Sie im Abschnitt **[!UICONTROL Zeitleisten]** die Option **[!UICONTROL Benutzerdefinierte Quartal aktivieren]**.

1. Geben Sie einen Namen für das benutzerdefinierte Quartal ein, z. B. &quot;Fiscal Q1 2021&quot;.
1. Wählen Sie das Start- und Enddatum für das benutzerdefinierte Quartal aus.

   ![](assets/custom-quarters-nwe.png)

1. (Optional) Klicken Sie auf **[!UICONTROL Benutzerdefiniertes Quartal hinzufügen]** , um dem System weitere benutzerdefinierte Quartale hinzuzufügen.
1. (Optional) Erstellen Sie ein Berichterstellungselement, das auf die Geschäftsquartale verweist.

   **Beispiel:** Erstellen Sie einen Filter für eine Liste mit dem Namen [!UICONTROL Projekt] und fügen Sie das geplante Abschlussdatum eines Projekts ein, das auf die benutzerdefinierten Quartale verweist.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Die Verweise auf &quot;Dieses Quartal&quot;, &quot;Nächstes Quartal&quot;und &quot;Letztes Quartal&quot;werden durch neue Verweise auf die benutzerdefinierten Quartale ersetzt.

   Informationen zu Berichterstellungselementen finden Sie unter [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Informationen zum Erstellen von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
