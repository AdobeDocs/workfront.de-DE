---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Anpassen von Standardausgabetypen
description: Sie können die Bezeichnungen für jeden Standardausgabetyp anpassen, um die in Ihrer Organisation verwendete Terminologie besser abzustimmen. Problemtypen sind nützlich zum Anpassen des Problemstatus und Erstellen von Anforderungswarteschlangen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Anpassen von Standardausgabetypen

Problemtypen sind unter folgenden Umständen nützlich:

* Beim Anpassen des Problemstatus, wie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Beim Erstellen einer Anforderungswarteschlange, wie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Sie können die Bezeichnungen für jeden Standardausgabetyp anpassen, um die in Ihrer Organisation verwendete Terminologie besser abzustimmen.

## Zugriffsanforderungen

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standardmäßige Problemtypen

Wenn Sie [!DNL Adobe Workfront] [!UICONTROL administrator] Zugriff haben, können Sie vier standardmäßige Problemtypen konfigurieren und umbenennen:

* **[!UICONTROL Fehlerbericht]** Wird verwendet, um gemeldete Fehler im System zu verfolgen.
* **[!UICONTROL Reihenfolge ändern]** Wird verwendet, um Probleme zu verfolgen, die aktualisiert oder überarbeitet werden müssen.
* **[!UICONTROL Problem]** Ein Objekt in [!DNL Workfront] das ungeplante Arbeit vermittelt, ein Problem auftritt oder etwas, das gelöst werden muss, um eine Aufgabe fortzusetzen.
* **[!UICONTROL Anfrage]** Ein Problem, das für eine Anforderungswarteschlange gilt, in der Benutzer Anforderungen in Workfront stellen.

![](assets/default-issue-types.png)

## Anpassen eines Ausgabetyps

Beachten Sie Folgendes zum Anpassen von Problemtypen:

* Sie können den Titel für einen Problemtyp ändern, dessen Funktion jedoch nicht geändert werden kann.
* Sie können keine zusätzlichen Ausgabetypen erstellen.
* Sie können die Filterwerte für den Namen eines Problems nicht ändern. Wenn Sie also einen Filter für einen Problembericht erstellen, spiegelt der Wert des Filters (Schlüssels) nicht den benutzerdefinierten Namen des Problemtyps wider.
* Jedem Problemtyp sind drei Standardstatus zugeordnet: [!UICONTROL Neu], [!UICONTROL In Bearbeitung]und [!UICONTROL Geschlossen]. Sie können diese Status nicht löschen oder aus einem Problemtyp entfernen, sie können aber umbenennen.
* Sie können die im Dropdownmenü angezeigten Optionen für jeden Ausgabetyp neu anordnen.

So passen Sie einen Problemtyp an:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Status]**.

1. Klicken Sie auf **[!UICONTROL Probleme]** Registerkarte.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über den anzupassenden Problemtyp und klicken Sie auf [!UICONTROL Bearbeiten] icon ![](assets/edit-icon.png) wird ganz rechts angezeigt, und geben Sie dann einen neuen Namen für den Problemtyp ein.

      ![](assets/customize-issue-type.png)

   * Klicken Sie auf [!UICONTROL Problemtyp] , um die zugehörigen Status aufzulisten, ziehen Sie dann die Handles, die angezeigt werden, wenn Sie den Mauszeiger darüber bewegen, und legen Sie sie in der Reihenfolge ab, in der sie im Problem Ihrer Benutzer angezeigt werden sollen **[!UICONTROL Status]** Dropdown-Menü.
