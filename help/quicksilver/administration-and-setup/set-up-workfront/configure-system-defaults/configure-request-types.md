---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Konfigurieren von Anfragetypen
description: Bei der Arbeit an einem Projekt kann es vorkommen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine bestimmte Aufgabe protokollieren. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anfrage-Warteschlange festgelegt ist. Probleme und Anfragen werden in Adobe Workfront als austauschbar betrachtet.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 3%

---

# Konfigurieren von Anfragetypen

Bei der Arbeit an einem Projekt kann es vorkommen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine bestimmte Aufgabe protokollieren. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anfrage-Warteschlange festgelegt ist. Probleme und Anfragen werden in Adobe Workfront als austauschbar betrachtet.

Informationen zum Erstellen von Problemen in [!DNL Workfront] finden Sie unter [Erstellen von Problemen](../../../manage-work/issues/manage-issues/create-issues.md). Informationen zum Erstellen von Anfragen in [!DNL Workfront] finden Sie unter [Erstellen und Senden [!DNL Adobe Workfront] Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md). Informationen zum Verknüpfen von Anfragetypen mit Projekten finden Sie [Definieren von Anfragetypen für ein Projekt](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

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

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Anpassen der Namen der Anfragetypen

Als [!DNL Workfront] können Sie die Namen der Anfragetypen in Ihrem System konfigurieren. Die neuen Namen sind in allen Bereichen von [!DNL Workfront] sichtbar, in denen die Felder **[!UICONTROL Anfragetyp]** oder **[!UICONTROL Anfragetyp]** angezeigt werden:

* Im Bereich **[!UICONTROL Warteschlangendetails]** eines Projekts, das die Probleme oder Anfragen erhält.
* Wenn für eine Anfrage-Warteschlange mehr als ein Anfragetyp ausgewählt ist, im Formular **[!UICONTROL Neues Problem]** im Feld **[!UICONTROL Anfragetyp]**, wenn Sie ein neues Problem erstellen oder eine neue Anfrage senden.

  Weitere Informationen zum Erstellen von Problemen in [!DNL Workfront] finden Sie unter [Erstellen von Problemen](../../../manage-work/issues/manage-issues/create-issues.md)

  Weitere Informationen zum Erstellen von Anfragen in [!DNL Workfront] finden Sie unter [Erstellen und Senden [!DNL Adobe Workfront] Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Im Formular **[!UICONTROL Warteschlangenthema-Detail]** beim Konfigurieren des Warteschlangenthemas.\
   Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

So passen Sie die Namen der Anfragetypen an:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Status]**.

1. Klicken Sie auf die **[!UICONTROL Probleme]**.
1. Klicken Sie oben auf der Registerkarte **[!UICONTROL Probleme]** auf das Dropdown-Menü, wählen Sie einen Anfragetyp aus und klicken Sie dann auf das **[!UICONTROL Bearbeiten]**-Symbol.

   ![Name des Anforderungstyps bearbeiten](assets/edit-request-type-name-nwe.png)

1. Geben Sie im angezeigten Feld einen neuen Namen ein und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

## Problemstatus in verschiedenen Anfragetypen konfigurieren

Sie können jeden Anfragetyp mit verschiedenen Problemstatus verknüpfen. Sie können auch die Reihenfolge ändern, in der die Status eines Problems angezeigt werden, je nachdem, um welche Art von Problem es sich handelt.

Weitere Informationen zum Ändern der Standardreihenfolge von Problemstatus und zum Konfigurieren des Problemstatus finden Sie im Abschnitt [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) in [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
