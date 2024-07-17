---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Konfigurieren von Timeline-Neuberechnungen für Projekte
description: Durch die Neuberechnung der Zeitpläne können Manager sehen, wie Kräfte außerhalb des Projekts die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf die geplanten und geplanten Daten für das Projekt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Konfigurieren von Timeline-Neuberechnungen für Projekte

Durch die Neuberechnung der Zeitpläne können Manager sehen, wie Kräfte außerhalb des Projekts die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf die geplanten und geplanten Daten für das Projekt.

Als [!DNL Adobe Workfront] -Administrator können Sie Zeitpläne für alle Projekte im System manuell neu berechnen. Projekteigentümer können Zeitpläne für einzelne Projekte auch manuell neu berechnen. Weitere Informationen finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

In diesem Artikel wird beschrieben, wie Sie als [!DNL Workfront] -Administrator feststellen können, wie und wann [!DNL Workfront] Projektzeitpläne automatisch berechnet, indem Sie die Projekteinstellungen im Bereich [!UICONTROL Einrichtung] konfigurieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriffsstufe des Systemadministrators</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Automatische Neuberechnungen konfigurieren

Als [!DNL Adobe Workfront] -Administrator können Sie konfigurieren, wann [!DNL Workfront] die Projektzeitpläne automatisch neu berechnet. [!DNL Workfront] kann die Projektzeitpläne entweder jede Nacht neu berechnen, wenn sich der Projektumfang ändert oder beides.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts oder, falls verfügbar, auf das Symbol [!UICONTROL **Hauptmenü**] ![](assets/lines-main-menu.png) in der oberen linken Ecke von [!DNL Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Projekte].**

1. Aktivieren oder deaktivieren Sie im Abschnitt **[!UICONTROL Zeitleisten]** eine oder beide der unten stehenden Einstellungen. Standardmäßig sind beide Einstellungen aktiviert.

   * **Jede Nacht:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] berechnet die Zeitpläne einmal alle 24 Stunden nachts neu, nur für Projekte mit dem Status [!UICONTROL Aktuell] und die in den letzten drei Monaten aktualisiert wurden. Abhängig von der Systemlast und anderen Faktoren kann die Neuberechnungszeit um mehr als 24 Stunden verzögert sein.

     In diesem Fall berechnet [!DNL Workfront] die Timeline für alle Projekte neu, deren [!UICONTROL Aktualisierungstyp] den Wert [!UICONTROL Automatisch] oder [!UICONTROL Automatisch und Bei Änderung] aufweist.

   * **Wenn sich der Umfang eines Projekts ändert**: Informationen dazu, was eine Änderung des Projektumfangs darstellt, finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In diesem Fall berechnet [!DNL Workfront] die Timeline für alle Projekte mit dem Aktualisierungstyp [!UICONTROL Automatisch und Bei Änderung] oder [!UICONTROL Nur bei Änderung] neu.
Informationen zu den Aktualisierungstypen für Projekte finden Sie unter [Übersicht über den Aktualisierungstyp für Projekte](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die Timeline aller Projekte im System wird automatisch basierend auf dem Aktualisierungstyp jedes Projekts neu berechnet.

## Neuberechnen von Zeitleisten für die gesamte [!DNL Workfront]-Instanz

Sie können die Diagnose [!UICONTROL Timeline neu berechnen] ausführen, um alle Timelines im System [!DNL Workfront] manuell neu zu berechnen. Dadurch können alle Projektmanager den Einfluss externer Änderungen sofort an geplanten und geplanten Terminen erkennen. Weitere Informationen finden Sie unter [Verwenden der Diagnose für den Trigger automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
