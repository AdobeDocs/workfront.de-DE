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
source-wordcount: '454'
ht-degree: 0%

---

# Konfigurieren von Timeline-Neuberechnungen für Projekte

Durch die Neuberechnung der Zeitpläne können Manager sehen, wie Kräfte außerhalb des Projekts die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf die geplanten und geplanten Daten für das Projekt.

Als [!DNL Adobe Workfront] -Administrator können Sie Zeitpläne für alle Projekte im System manuell neu berechnen. Projekteigentümer können Zeitpläne für einzelne Projekte auch manuell neu berechnen. Weitere Informationen finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

In diesem Artikel wird beschrieben, wie Sie [!DNL Workfront] -Administrator kann bestimmen, wie und wann [!DNL Workfront] berechnet automatisch die Projektzeitpläne, indem Sie die Projektvoreinstellungen im Abschnitt [!UICONTROL Einrichtung] Bereich.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriffsstufe des Systemadministrators</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Automatische Neuberechnungen konfigurieren

Als [!DNL Adobe Workfront] Administrator können Sie konfigurieren, wann [!DNL Workfront] berechnet automatisch die Projektzeitpläne neu. [!DNL Workfront] kann die Projektzeitpläne entweder jede Nacht neu berechnen, den Projektumfang ändern oder beides.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke oder [!UICONTROL **Hauptmenü**] icon ![](assets/lines-main-menu.png) in der linken oberen Ecke von [!DNL Workfront], falls verfügbar, klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicks **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte].**

1. Im **[!UICONTROL Zeitpläne]** -Abschnitt, aktivieren oder deaktivieren Sie eine oder beide der unten stehenden Einstellungen. Standardmäßig sind beide Einstellungen aktiviert.

   * **Jede Nacht:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] berechnet die Zeitpläne nur bei Projekten mit dem Status [!UICONTROL Aktuell] und die in den letzten drei Monaten aktualisiert wurden. Abhängig von der Systemlast und anderen Faktoren kann die Neuberechnungszeit um mehr als 24 Stunden verzögert sein.

     In diesem Fall [!DNL Workfront] berechnet die Zeitleiste für alle Projekte mit [!UICONTROL Aktualisierungstyp] von [!UICONTROL Automatisch] oder [!UICONTROL Automatisch und Bei Änderung].

   * **Wenn sich der Umfang eines Projekts ändert**: Weitere Informationen zu einer Änderung des Projektumfangs finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In diesem Fall [!DNL Workfront] berechnet die Timeline für alle Projekte mit dem Aktualisierungstyp neu [!UICONTROL Automatisch und Bei Änderung] oder [!UICONTROL Nur bei Änderung].
Weitere Informationen zu den Aktualisierungstypen für Projekte finden Sie unter [Übersicht über den Projektaktualisierungstyp](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die Timeline aller Projekte im System wird automatisch basierend auf dem Aktualisierungstyp jedes Projekts neu berechnet.

## Neuberechnung der Zeitpläne für das gesamte [!DNL Workfront] instance

Sie können die [!UICONTROL Timeline neu berechnen] Diagnose, um alle Zeitleisten im [!DNL Workfront] System. Dadurch können alle Projektmanager den Einfluss externer Änderungen sofort an geplanten und geplanten Terminen erkennen. Weitere Informationen finden Sie unter [Verwenden der Diagnose für den Trigger automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
