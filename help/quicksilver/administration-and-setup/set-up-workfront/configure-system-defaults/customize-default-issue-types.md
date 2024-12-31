---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Standardanfragetypen anpassen
description: Sie können die Bezeichnungen für jeden standardmäßigen Problemtyp anpassen, sodass sie besser mit der in Ihrem Unternehmen verwendeten Terminologie übereinstimmen. Anfragetypen sind nützlich, um den Anfragestatus anzupassen und Anfragewarteschlangen zu erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Anpassen der standardmäßigen Anfragetypen

Anfragetypen sind unter folgenden Umständen nützlich:

* Beim Anpassen des Anfragestatus, wie in [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) beschrieben.
* Beim Erstellen einer Anfrage-Warteschlange, wie in [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) beschrieben.

Sie können die Bezeichnungen für jeden standardmäßigen Problemtyp anpassen, sodass sie besser mit der in Ihrem Unternehmen verwendeten Terminologie übereinstimmen.

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

## Standardmäßige Problemtypen

Wenn Sie [!DNL Adobe Workfront] [!UICONTROL Admin]-Zugriff haben, gibt es vier standardmäßige Problemtypen, die Sie konfigurieren und umbenennen können:

* **[!UICONTROL Fehlerbericht]** Wird verwendet, um gemeldete Fehler im System zu verfolgen.
* **[!UICONTROL Änderungsanforderung]** Dient zum Nachverfolgen von Problemen, die aktualisiert oder überarbeitet werden müssen.
* **[!UICONTROL Problem]** Ein Objekt in [!DNL Workfront], das ungeplante Arbeiten, ein auftretendes Problem oder etwas kommuniziert, das gelöst werden muss, um eine Aufgabe fortzusetzen.
* **[!UICONTROL Anfrage]** Ein Problemtyp, der für eine Anfrage-Warteschlange gilt, in der Benutzer Anfragen in Workfront stellen.

![](assets/default-issue-types.png)

## Anfragetyp anpassen

Beachten Sie Folgendes zum Anpassen von Problemtypen:

* Sie können die Beschriftung für einen Anfragetyp ändern, aber nicht seine Funktion.
* Zusätzliche Anfragetypen können nicht erstellt werden.
* Die Filterwerte für den Namen eines Problemtyps können nicht geändert werden. Wenn Sie also einen Filter für einen Problembericht erstellen, spiegelt der Wert des Filters (Schlüssels) nicht den benutzerdefinierten Namen des Problemtyps wider.
* Jedem Anfragetyp sind drei Standardstatus zugeordnet: [!UICONTROL Neu], [!UICONTROL In Bearbeitung] und [!UICONTROL Geschlossen]. Sie können diese Status nicht löschen oder aus einem Problemtyp entfernen, aber Sie können sie umbenennen.
* Sie können die Optionen, die im Dropdown-Menü angezeigt werden, für jeden Problemtyp neu anordnen.

So passen Sie einen Problemtyp an:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Status]**.

1. Klicken Sie auf die **[!UICONTROL Probleme]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über den Anfragetyp, den Sie anpassen möchten, klicken Sie auf das [!UICONTROL Bearbeiten]-Symbol ganz rechts ![](assets/edit-icon.png) und geben Sie dann einen neuen Namen für den Anfragetyp ein.

     ![](assets/customize-issue-type.png)

   * Klicken Sie auf einen [!UICONTROL Anfragetyp], um die zugehörigen Status aufzulisten. Ziehen Sie dann die Handles, die angezeigt werden, wenn Sie den Mauszeiger über sie bewegen, und legen Sie sie in der Reihenfolge ab, in der sie im Dropdown-Menü **[!UICONTROL Status]** der Benutzenden angezeigt werden sollen.
