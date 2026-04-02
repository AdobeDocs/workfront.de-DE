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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 8%

---

# Aktivieren von benutzerdefinierten Quartalen

<!--Audited: 03/2026-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).

Je nachdem, welche Produkte Ihr Unternehmen gekauft hat, können Sie die folgende Anzahl von Quartalen in Ihrem Workfront-Setup-Bereich konfigurieren:

* Kunden, die nur [!DNL Workfront] erworben haben, können bis zu acht benutzerdefinierte Quartale für ihr [!DNL Adobe Workfront] konfigurieren.
* Kunden, die [!DNL Workfront] und [!DNL Workfront Planning] erworben haben, können bis zu 100 Quartale für ihr [!DNL Workfront] konfigurieren, die auch in [!DNL Planning] verfügbar sind.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Benutzerdefinierte Quartale für Ihr [!DNL Workfront] einrichten

{{step-1-to-setup}}

1. (Bedingt) Führen Sie je nachdem, über welche Umgebung Sie auf „Benutzerdefinierte Quartale“ zugreifen, einen der folgenden Schritte aus:

   * Klicken Sie in der Produktionsumgebung auf **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte].**
   * <span class="preview">Klicken Sie in der Vorschau-Umgebung auf **[!UICONTROL Benutzerdefinierte Quartale]**.</span>

1. Wählen Sie **[!UICONTROL Benutzerdefinierte Quartale aktivieren]** aus.

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
1. (Optional und bedingt) Wenn Ihr Unternehmen Workfront Planning erworben hat und Sie Zugriff auf [!DNL Workfront Planning] haben, navigieren Sie zu einer Seite für den Datensatztyp und öffnen Sie eine Zeitleisten -Ansicht. Die Ansicht zeigt die neuen benutzerdefinierten Quartale an.
Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).
