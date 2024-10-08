---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Anpassen von Standardausgabetypen
description: Sie können die Bezeichnungen für jeden Standardausgabetyp anpassen, um die in Ihrer Organisation verwendete Terminologie besser abzustimmen. Problemtypen sind nützlich zum Anpassen des Problemstatus und Erstellen von Anforderungswarteschlangen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Anpassen von Standardausgabetypen

Problemtypen sind unter folgenden Umständen nützlich:

* Beim Anpassen des Problemstatus, wie in [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) beschrieben.
* Beim Erstellen einer Anforderungswarteschlange, wie in [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) beschrieben.

Sie können die Bezeichnungen für jeden Standardausgabetyp anpassen, um die in Ihrer Organisation verwendete Terminologie besser abzustimmen.

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

## Standardmäßige Problemtypen

Wenn Sie Zugriff auf [!DNL Adobe Workfront] [!UICONTROL administrator] haben, gibt es vier Standardfehlertypen, die Sie konfigurieren und umbenennen können:

* **[!UICONTROL Fehlerbericht]** Wird verwendet, um gemeldete Fehler im System zu verfolgen.
* **[!UICONTROL Reihenfolge ändern]** Wird verwendet, um Probleme zu verfolgen, die aktualisiert oder überarbeitet werden müssen.
* **[!UICONTROL Problem]** Ein Objekt in [!DNL Workfront], das ungeplante Arbeit, ein auftretendes Problem oder etwas kommuniziert, das gelöst werden muss, um eine Aufgabe fortzusetzen.
* **[!UICONTROL Anfrage]** Ein Problem, das für eine Anforderungswarteschlange gilt, in der Benutzer Anforderungen in Workfront stellen.

![](assets/default-issue-types.png)

## Anpassen eines Ausgabetyps

Beachten Sie Folgendes zum Anpassen von Problemtypen:

* Sie können den Titel für einen Problemtyp ändern, dessen Funktion jedoch nicht geändert werden kann.
* Sie können keine zusätzlichen Ausgabetypen erstellen.
* Sie können die Filterwerte für den Namen eines Problems nicht ändern. Wenn Sie also einen Filter für einen Problembericht erstellen, spiegelt der Wert des Filters (Schlüssels) nicht den benutzerdefinierten Namen des Problemtyps wider.
* Jedem Ausgabetyp sind drei Standardstatus zugeordnet: [!UICONTROL Neu], [!UICONTROL In Bearbeitung] und [!UICONTROL Geschlossen]. Sie können diese Status nicht löschen oder aus einem Problemtyp entfernen, sie können aber umbenennen.
* Sie können die im Dropdownmenü angezeigten Optionen für jeden Ausgabetyp neu anordnen.

So passen Sie einen Problemtyp an:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Status]**.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Probleme]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über den anzupassenden Problemtyp, klicken Sie auf das Symbol [!UICONTROL Bearbeiten] ![](assets/edit-icon.png), das ganz rechts angezeigt wird, und geben Sie dann einen neuen Namen für den Problemtyp ein.

     ![](assets/customize-issue-type.png)

   * Klicken Sie auf einen [!UICONTROL Problemtyp] , um die zugehörigen Status aufzulisten. Ziehen Sie dann die Handles, die angezeigt werden, wenn Sie den Mauszeiger über sie bewegen, und legen Sie sie in der Reihenfolge ab, in der sie im Dropdownmenü für Benutzerprobleme angezeigt werden sollen **[!UICONTROL Status]**.
