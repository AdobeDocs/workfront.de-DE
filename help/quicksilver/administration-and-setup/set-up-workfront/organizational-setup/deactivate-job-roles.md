---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deaktivieren von Vorgangsrollen
description: Als [!DNL Adobe Workfront] -Administrator oder Benutzer mit Administratorzugriff auf "Auftragsrollen"können Sie die in Ihrem System veralteten Vorgangsrollen deaktivieren. Wenn Sie eine Auftragsrolle deaktivieren, anstatt sie zu löschen, können Sie alle zugehörigen historischen Informationen beibehalten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Deaktivieren von Vorgangsrollen

Als [!DNL Adobe Workfront] -Administrator oder Benutzer mit Administratorzugriff auf &quot;Auftragsrollen&quot;können Sie die in Ihrem System veralteten Vorgangsrollen deaktivieren. Wenn Sie eine Auftragsrolle deaktivieren, anstatt sie zu löschen, können Sie alle zugehörigen historischen Informationen beibehalten.

Sie können auch zuvor deaktivierte Vorgangsrollen reaktivieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Lizenz*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf die Rollen "Aufträge"</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Auswirkungen der Deaktivierung von Vorgangsrollen

Wenn Sie eine Auftragsrolle deaktivieren, wird sie nicht mehr in den folgenden Bereichen angezeigt:

* Die [!UICONTROL Zuweisungen] typeahead-Feld (für Aufgaben, Vorlagenaufgaben, Probleme, Genehmigungen und Routing-Regeln)
* Die [!UICONTROL Zuweisungen] Felder in Listen und Berichten
* Benutzerprofile

   >[!NOTE]
   >
   >Wenn Sie einem Benutzer eine neue Rolle hinzufügen, wird keine deaktivierte Auftragsrolle angezeigt. Sie wird jedoch weiterhin im [!UICONTROL Primäre Rolle] und [!UICONTROL Sonstige Rollen] -Felder, wenn der Benutzer mit der Auftragsrolle verknüpft war, bevor sie deaktiviert wurde.

* Die [!UICONTROL Freigabe] Dialogfeld für Objekte, einschließlich der Zuweisung von Layoutvorlagen
* Felder mit Schreibvorgängen in benutzerdefinierten Formularen
* Die [!UICONTROL Poolmitglieder] -Feld in [!UICONTROL Ressourcen-Pools]
* Die [!UICONTROL Auftragsrolle] Feld eines [!UICONTROL Abrechnungsrate] Bearbeitungsbildschirm, wenn ein Benutzer die Abrechnungsraten für Projekte außer Kraft setzt
* Die [!UICONTROL Hinzufügen einer Zuweisung zum Kanban-Board] Dialogfeld in einem Projekt
* Die [!UICONTROL Auftragsrolle] Feld eines Plans oder einer Initiative, wenn jemand die [!DNL Adobe Workfront Scenario Planner].

   Die [!DNL Scenario Planner] ist nur in der neuen [!DNL Adobe Workfront] Erfahrung und erfordert eine zusätzliche Lizenz. Informationen zum [!DNL Workfront Scenario Planner], siehe [Die [!DNL Scenario Planner] Übersicht](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Deaktivierte Rollen werden immer in Filtern in Listen, Berichten und anderen Tools wie dem [!UICONTROL Lastenausgleich].

## Überlegungen zum Deaktivieren einer Stellenrolle

Es ist besser, veraltete Vorgangsrollen zu deaktivieren, anstatt sie zu löschen, damit Sie alle historischen Informationen beibehalten können, die mit Rollen verknüpft sind, die Sie in der Vergangenheit verwendet haben.

>[!NOTE]
>
>Alle Arbeiten, die der Auftragsrolle vor der Deaktivierung zugewiesen wurden, bleiben zugewiesen.

Es wird empfohlen, folgende Schritte durchzuführen, bevor Sie eine nicht verwendete Vorgangsrolle deaktivieren:

* Erstellen Sie Berichte für alle Objekte, die der Rolle zugewiesen sind, die Sie deaktivieren möchten, und weisen Sie sie einer aktiven Auftragsrolle zu. Informationen zum Erstellen von Berichten finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >Sie können einen Bericht erstellen, um nach Aufgaben oder Problemen zu filtern, denen die deaktivierte Rolle zugewiesen ist. Verwenden Sie dann den Bericht, um ausstehende Aufgaben oder Probleme einer aktiven Rolle zuzuweisen.

* Nehmen Sie eine Bestandsaufnahme aller Genehmigungsprozesse, aktuellen Genehmigungspfade, Routing-Regeln oder anderer Objekte vor, die der Stellenrolle zugewiesen sind, die Sie deaktivieren möchten, und weisen Sie sie einer aktiven Rolle zu.

   >[!TIP]
   >
   >Wenn Sie bei Verwendung von Anforderungswarteschlangen eine Auftragsrolle deaktivieren, die in einer Routing-Regel als Standardverantwortlicher zugewiesen ist, bleibt die Rolle erhalten und die Anforderungen werden weiterhin an die deaktivierte Rolle weitergeleitet. Es wird empfohlen, Routing-Regeln mit aktiven Rollen zu aktualisieren, bevor Sie das Team deaktivieren.

   Informationen zum Erstellen von Genehmigungsprozessen und Routing-Regeln finden Sie in den folgenden Artikeln:

   * [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Erstellen von Routing-Regeln](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Deaktivieren einer Stellenrolle

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf &#x200B; **[!UICONTROL Vorgangsrollen].**
1. (Optional) Im **[!UICONTROL Filter]** Dropdown-Menü auswählen **[!UICONTROL Aktiv]** , um nur aktive Vorgangsrollen anzuzeigen.
1. Klicken Sie auf den Namen der Auftragsrolle, die Sie deaktivieren möchten.
1. Im **[!UICONTROL Ist aktiv]** Dropdown-Menü auswählen **[!UICONTROL Nein]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klicken **[!UICONTROL Änderungen speichern]**.

   Die Auftragsrolle ist deaktiviert und kann nicht mehr der Arbeit zugewiesen werden, mit Layoutvorlagen verknüpft sind usw. Weitere Informationen zu allen Verwendungen von Vorgangsrollen finden Sie unter [!DNL Workfront], siehe [Übersicht über die Auftragsrolle](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
