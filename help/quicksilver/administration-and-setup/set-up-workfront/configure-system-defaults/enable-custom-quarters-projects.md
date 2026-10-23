---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Benutzerdefinierte Quartale und Wochen aktivieren
description: Zu Berichtszwecken können Sie benutzerdefinierte Quartale konfigurieren, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage). Wenn Ihr Unternehmen Workfront Planning-Pakete kauft, können Sie auch benutzerdefinierte Wochen konfigurieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: c7c74fdba29c4c6d28d12447459c5903a34c7856
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%
---
# Benutzerdefinierte Quartale und Wochen aktivieren

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Zu Berichtszwecken können Sie benutzerdefinierte Quartale erstellen, wenn die Quartale Ihres Unternehmens auf bestimmten Kriterien basieren, die keine Kalenderdaten sind (z. B. Geschäftstage oder Einkaufstage).

Je nachdem, welche Produkte Ihr Unternehmen gekauft hat, können Sie die folgende Anzahl von Quartalen in Ihrem Workfront-Setup-Bereich konfigurieren:

* Kunden, die nur [!DNL Workfront] erworben haben, können bis zu acht benutzerdefinierte Quartale für ihr [!DNL Adobe Workfront] konfigurieren.
* Kunden, die [!DNL Workfront] und [!DNL Workfront Planning] erworben haben, können bis zu 100 Quartale für ihr [!DNL Workfront] konfigurieren, die auch in [!DNL Planning] verfügbar sind.

* Kunden, die [!DNL Workfront] und [!DNL Workfront Planning] erworben haben, können benutzerdefinierte Wochen für jedes benutzerdefinierte Quartal konfigurieren. Die benutzerdefinierten Wochen sind in den [!DNL Planning] Zeitleisten-Ansichten sichtbar.

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
   <td><p>[!UICONTROL Workflow Standard] oder [!UICONTROL Workfront Plan] Lizenz</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## Benutzerdefinierte Quartale für Ihr [!DNL Workfront] einrichten

<!--
Setting up custom quarters differs depending on which environment you use. 

### Set up custom quarters for your [!DNL Workfront] system in the Production environment

{{step-1-to-setup}}

1. Click **[!UICONTROL Custom Quarters]**.

1. Select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter, such as "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

   ![Custom quarters](assets/custom-quarters-nwe.png)

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) If your company purchased only [!DNL Workfront], without [!DNL Workfront Planning], create a reporting element that refers to the fiscal quarters.

   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) If your company purchased Workfront Planning and you have access to [!DNL Workfront Planning], go to a record type page and open a timeline view. The view displays the new custom quarters. 
For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

<div class="preview">

### Set up custom quarters for your [!DNL Workfront] system in the Preview environment

-->

>[!NOTE]
>
>Wenn Ihr Unternehmen ein Planungspaket zusätzlich zu einem Workflow-Paket erworben hat oder wenn es Workfront Planning als eigenständiges Paket erworben hat, können Sie zusätzlich zu benutzerdefinierten Quartalen benutzerdefinierte Wochen konfigurieren.
> 
>Benutzerdefinierte Wochen sind für Workfront-Berichte und -Listen nicht verfügbar.

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Quartale]**.

1. Wählen Sie **[!UICONTROL Benutzerdefinierte Quartale aktivieren]** aus.

1. Geben Sie einen Namen für das benutzerdefinierte Quartal ein. Beispiel: „Geschäftsjahr 1 2021“.
1. Wählen Sie das Start- und Enddatum für das benutzerdefinierte Quartal aus.

1. (Optional) Wählen Sie die Option **Startet eine neue benutzerdefinierte**.

   Wenn diese Option ausgewählt ist, wird der Beginn des benutzerdefinierten Quartals als der Beginn der ersten benutzerdefinierten Woche des Quartals in der Ansicht „Planning-Zeitleiste“ festgelegt.
1. (Optional) Wählen Sie im Bereich **Benutzerdefiniertes Wochen** Label-Format **Format** für die benutzerdefinierten Wochen-Labels aus. Wählen Sie aus den folgenden Optionen:

   * **W1, W2, W3 …** . Dies ist das Standardformat.
   * **FW1, FW2, FW3 …**
   * **Woche1, Woche 2, Woche 3, …**
   * **Benutzerspezifisch**

1. (Bedingt) Wenn Sie **Benutzerdefiniert** für das Feld **Format** ausgewählt haben, geben Sie einen **benutzerdefinierten Titel** ein, um die benutzerdefinierten Wochen anzugeben.

   Benutzerdefinierte Wochen werden in Zeitleisten-Ansichten für die Planung angezeigt.

   >[!TIP]
   >
   >Beim Hinzufügen einer benutzerdefinierten Beschriftung können Sie bis zu 100 Zeichen eingeben.
   >
   >Sie können den Namen der ersten Woche angeben, und in den folgenden Wochen wird dieselbe Bezeichnung gefolgt von einer fortlaufenden Nummer verwendet.
   >
   >Beispiel: Bei einer **benutzerdefinierten Beschriftung** „Geschäftswoche“ werden die Beschriftungen „Geschäftswoche 1, Geschäftswoche 2, Geschäftswoche 3 …“ hinzugefügt für den Rest der Wochen in der Sequenz.

1. (Optional) Klicken Sie **[!UICONTROL Benutzerdefiniertes Quartal hinzufügen]**, um dem System zusätzliche benutzerdefinierte Quartale hinzuzufügen.

   >[!IMPORTANT]
   >
   > Wenn Ihr Unternehmen [!DNL Workfront Planning] gekauft hat, können Sie Ihre benutzerdefinierten Quartale nicht speichern, wenn es Lücken oder Überschneidungen zwischen den Quartalen gibt.
   >![Benutzerdefinierte Quartale mit Überschneidungswarnung](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >Lücken und Überschneidungen zwischen den Quartalen sind nur für [!DNL Workfront] Kunden zulässig.

1. (Optional und bedingt) Um die benutzerdefinierten Quartale in Workfront anzuzeigen, erstellen Sie ein Berichterstellungselement, das auf die benutzerdefinierten Quartale verweist.

   **Beispiel** Erstellen Sie einen Filter für eine [!UICONTROL Projekt]Liste und geben Sie das geplante Abschlussdatum eines Projekts an, das auf die benutzerdefinierten Quartale verweist.

   ![Projektfilter mit benutzerdefinierten Quartalen](assets/example-of-project-filter-with-custom-quarters.png)

   Die Verweise auf „Dieses Quartal“, „Nächstes Quartal“ und „Letztes Quartal“ werden durch neue Verweise auf die benutzerdefinierten Quartale ersetzt.

   Informationen zu Berichtselementen finden Sie unter [Berichtselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Informationen zum Erstellen von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional und bedingt) Um benutzerdefinierte Quartale und Wochen in Workfront Planning anzuzeigen, gehen Sie zu einer Datensatztypseite und öffnen Sie eine Zeitleisten -Ansicht. Die Ansicht zeigt die neuen benutzerdefinierten Quartale und Wochen an.

   Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).


