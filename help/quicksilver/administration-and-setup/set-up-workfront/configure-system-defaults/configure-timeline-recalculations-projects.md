---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Konfigurieren der Zeitleisten-Neuberechnungen für Projekte
description: Durch die Neuberechnung der Zeitleisten können Manager sehen, wie sich Kräfte außerhalb des Projekts auf die Zeitleiste des Projekts auswirken. Der Zeitplan eines Projekts bezieht sich auf die geplanten und geplanten Termine für das Projekt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Konfigurieren der Zeitleisten-Neuberechnungen für Projekte

Durch die Neuberechnung der Zeitleisten können Manager sehen, wie sich Kräfte außerhalb des Projekts auf die Zeitleiste des Projekts auswirken. Der Zeitplan eines Projekts bezieht sich auf die geplanten und geplanten Termine für das Projekt.

Als [!DNL Adobe Workfront] können Sie die Timelines für alle Projekte im System manuell neu berechnen. Projektbesitzer können Timelines für einzelne Projekte auch manuell neu berechnen. Weitere Informationen finden Sie unter [Projektzeitleisten neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

In diesem Artikel wird beschrieben, wie Sie als [!DNL Workfront] feststellen können, wie und wann [!DNL Workfront] Projektzeitleisten automatisch berechnet, indem Sie die Projektvoreinstellungen im Bereich [!UICONTROL Setup] konfigurieren.

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
       <p>[!UICONTROL-Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Automatische Neuberechnungen konfigurieren

Als [!DNL Adobe Workfront] können Sie konfigurieren, wenn [!DNL Workfront] Projektzeitleisten automatisch neu berechnet. [!DNL Workfront] können Projektzeitleisten entweder jede Nacht oder bei einer Änderung des Projektumfangs oder beides neu berechnen.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Projekte].**

1. Aktivieren **[!UICONTROL im Abschnitt]** Timelines“ eine oder beide der folgenden Einstellungen. Standardmäßig sind beide Einstellungen aktiviert.

   * **Jede Nacht:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] berechnet Timelines einmal alle 24 Stunden, nachts, nur für Projekte mit dem Status [!UICONTROL aktuell], die in den letzten drei Monaten aktualisiert wurden. Je nach Systemlast und anderen Faktoren kann sich die Neuberechnungszeit um mehr als 24 Stunden verzögern.

     In diesem Fall berechnet [!DNL Workfront] die Zeitleiste für alle Projekte neu, die einen [!UICONTROL Aktualisierungstyp] von [!UICONTROL Automatisch] oder [!UICONTROL Automatisch und Bei Änderung].

   * **Wenn sich der Projektumfang ändert**: Informationen dazu, was eine Änderung des Projektumfangs ausmacht, finden Sie unter [Neuberechnen von Projektzeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     In diesem Fall berechnet [!DNL Workfront] die Zeitleiste für alle Projekte neu, die den Aktualisierungstyp &quot;[!UICONTROL &quot; und „Bei Änderung] oder „Nur [!UICONTROL &quot; ].
Informationen zu Projektaktualisierungstypen finden Sie unter [Übersicht über Projektaktualisierungstypen](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die Zeitleiste aller Projekte im System wird automatisch auf der Grundlage des Aktualisierungstyps jedes Projekts neu berechnet.

>[!IMPORTANT]
>
>Für die Sandbox-Umgebungen „Vorschau“ und „Benutzerdefinierte Aktualisierung“ ist die nächtliche Neuberechnung deaktiviert und die Projektzeitleisten werden nicht automatisch neu berechnet. Sie müssen die Zeitleiste des Projekts für die Sandbox-Umgebungen „Vorschau“ und „Benutzerdefinierte Aktualisierung“ manuell neu berechnen. Weitere Informationen finden Sie unter [Neuberechnen von Projektzeitleisten](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Berechnen Sie die Timelines für die gesamte [!DNL Workfront] neu

Sie können die Diagnose [!UICONTROL Timeline neu berechnen] ausführen, um alle Timelines im [!DNL Workfront] manuell neu zu berechnen. Auf diese Weise können alle Projektmanager den Einfluss externer Änderungen sowohl bei geplanten als auch bei geplanten Terminen sofort sehen. Weitere Informationen finden Sie unter [Verwenden von Diagnoseprogrammen zum Trigger automatisierter Prozesse](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
