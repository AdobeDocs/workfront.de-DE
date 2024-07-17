---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Anfragetypen konfigurieren
description: Bei der Arbeit an einem Projekt können Sie feststellen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine bestimmte Aufgabe protokollieren. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anforderungswarteschlange bezeichnet wird. Probleme und Anforderungen werden in Adobe Workfront als austauschbar betrachtet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Anfragetypen konfigurieren

Bei der Arbeit an einem Projekt können Sie feststellen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine bestimmte Aufgabe protokollieren. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anforderungswarteschlange bezeichnet wird. Probleme und Anforderungen werden in Adobe Workfront als austauschbar betrachtet.

Informationen zum Erstellen von Problemen in [!DNL Workfront] finden Sie unter [Erstellen von Problemen](../../../manage-work/issues/manage-issues/create-issues.md). Informationen zum Erstellen von Anforderungen in [!DNL Workfront] finden Sie unter [Erstellen und Senden [!DNL Adobe Workfront] von Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md). Informationen zum Verknüpfen von Anfragetypen mit Projekten finden Sie unter [Definieren von Anfragetypen für ein Projekt](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Zugriffsanforderungen

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

Als [!DNL Workfront] -Administrator können Sie die Namen der Anfragetypen in Ihrem System konfigurieren. Die neuen Namen sind in jedem Bereich von [!DNL Workfront] sichtbar, in dem die Felder **[!UICONTROL Ausgabetyp]** oder **[!UICONTROL Anforderungstyp]** angezeigt werden:

* Im Bereich **[!UICONTROL Queue Details]** eines Projekts, das die Probleme oder Anforderungen erhält.
* Wenn für eine Anforderungswarteschlange mehr als ein Anfragetyp ausgewählt ist, wird im Feld **[!UICONTROL Neues Problem] Formular** im Feld **[!UICONTROL Ausgabetyp]** beim Erstellen eines neuen Problems oder Senden einer neuen Anforderung Folgendes angezeigt:

  Weitere Informationen zum Erstellen von Problemen in [!DNL Workfront] finden Sie unter [Probleme erstellen](../../../manage-work/issues/manage-issues/create-issues.md)

  Weitere Informationen zum Erstellen von Anforderungen in [!DNL Workfront] finden Sie unter [Erstellen und Senden [!DNL Adobe Workfront] von Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Wenn Sie im Formular **[!UICONTROL Detail des Warteschlangenthemas]** das Thema &quot;Warteschlange&quot;konfigurieren,\
   Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Themen für Warteschlangen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

So passen Sie die Namen der Anfragetypen an:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Status]**.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Probleme]**.
1. Bewegen Sie oben auf der Registerkarte **[!UICONTROL Probleme]** den Mauszeiger über den Namen eines Anfragetyps und klicken Sie dann auf das daraufhin angezeigte Symbol **[!UICONTROL Bearbeiten]** .

   ![](assets/edit-request-type-name-nwe.png)

1. Geben Sie in das angezeigte Feld einen neuen Namen ein und drücken Sie dann die Eingabetaste ]**.**[!UICONTROL 

## Konfigurieren des Problemstatus in verschiedenen Anfragetypen

Sie können jeden Anfragetyp mit verschiedenen Problemstatus verknüpfen. Sie können auch die Reihenfolge ändern, in der die Status zu einem Problem angezeigt werden, je nach Art des Problems.

Weitere Informationen zum Ändern der Standardreihenfolge der Problemstatus und zum Konfigurieren des Problemstatus finden Sie im Abschnitt [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) in [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
