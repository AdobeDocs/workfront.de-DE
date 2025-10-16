---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Benutzerdefinierte Quartale aktivieren
description: Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---

# Benutzerdefinierte Quartale aktivieren

<!--Audited: 11/2024-->

Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).

Je nachdem, welche Produkte Ihr Unternehmen gekauft hat, können Sie die folgende Anzahl von Quartalen in Ihrem Workfront-Setup-Bereich konfigurieren:

* Kunden, die nur [!DNL Workfront] erworben haben, können bis zu acht benutzerdefinierte Quartale für ihr [!DNL Adobe Workfront] konfigurieren.
* Kunden, die [!DNL Workfront] und [!DNL Workfront Planning] erworben haben, können bis zu 100 Quartale für ihr [!DNL Workfront] konfigurieren, die auch in [!DNL Planning] verfügbar sind.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL -Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Quartale für Ihr [!DNL Workfront] einrichten

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte].**

1. Wählen **[!UICONTROL Abschnitt &quot;]**&quot; die Option **[!UICONTROL Benutzerdefinierte Quartale aktivieren]**.

1. Geben Sie einen Namen für das benutzerdefinierte Quartal ein, z. B. „Geschäftsjahr 1 2021“.
1. Wählen Sie das Start- und Enddatum für das benutzerdefinierte Quartal aus.

   ![Benutzerdefinierte Quartale](assets/custom-quarters-nwe.png)

1. (Optional) Klicken Sie **[!UICONTROL Benutzerdefiniertes Quartal hinzufügen]**, um dem System zusätzliche benutzerdefinierte Quartale hinzuzufügen.

   >[!IMPORTANT]
   >
   > Wenn Ihr Unternehmen [!DNL Workfront Planning] gekauft hat, können Sie Ihre benutzerdefinierten Quartale nicht speichern, wenn es Lücken oder Überschneidungen zwischen den Quartalen gibt.
   >![Benutzerdefinierte Quartale mit Überschneidungswarnung](assets/custom-quarters-with-overlap-warning.png)
   >Lücken und Überschneidungen zwischen den Quartalen sind nur für [!DNL Workfront] Kunden zulässig.

1. (Optional und bedingt) Wenn Ihr Unternehmen nur [!DNL Workfront] gekauft hat, erstellen Sie [!DNL Workfront Planning] ein Berichtselement, das sich auf das Geschäftsquartal bezieht.


   **Beispiel** Erstellen Sie einen Filter für eine [!UICONTROL Projekt]Liste und geben Sie das geplante Abschlussdatum eines Projekts an, das auf die benutzerdefinierten Quartale verweist.

   ![Projektfilter mit benutzerdefinierten Quartalen](assets/example-of-project-filter-with-custom-quarters.png)

   Die Verweise auf „Dieses Quartal“, „Nächstes Quartal“ und „Letztes Quartal“ werden durch neue Verweise auf die benutzerdefinierten Quartale ersetzt.

   Informationen zu Berichtselementen finden Sie unter [Berichtselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Informationen zum Erstellen von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional und bedingt) Wenn Sie Zugriff auf [!DNL Workfront Planning] haben, navigieren Sie zu einer Seite für den Datensatztyp und öffnen Sie eine Zeitleisten -Ansicht. Die Ansicht zeigt die neuen benutzerdefinierten Quartale an.
Weitere Informationen finden Sie unter [Verwalten der Zeitleisten-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).
