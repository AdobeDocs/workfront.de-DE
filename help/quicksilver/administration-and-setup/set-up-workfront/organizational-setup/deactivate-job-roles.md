---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deaktivieren von Vorgangsrollen
description: Als [!DNL Adobe Workfront] Administrator oder Benutzer mit administrativem Zugriff auf "Vorgangsrollen"können Sie Aufgabenrollen deaktivieren, die in Ihrem System veraltet sind. Wenn Sie eine Auftragsrolle deaktivieren, anstatt sie zu löschen, können Sie alle zugehörigen historischen Informationen beibehalten.
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

Als [!DNL Adobe Workfront] -Administrator oder Benutzer mit administrativem Zugriff auf &quot;Vorgangsrollen&quot;können Sie Stellenrollen deaktivieren, die in Ihrem System veraltet sind. Wenn Sie eine Auftragsrolle deaktivieren, anstatt sie zu löschen, können Sie alle zugehörigen historischen Informationen beibehalten.

Sie können auch zuvor deaktivierte Vorgangsrollen reaktivieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Lizenz*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf die Rollen "Aufträge"</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Auswirkungen der Deaktivierung von Vorgangsrollen

Wenn Sie eine Auftragsrolle deaktivieren, wird sie nicht mehr in den folgenden Bereichen angezeigt:

* Das typeahead-Feld [!UICONTROL Zuweisungen] (für Aufgaben, Vorlagenaufgaben, Probleme, Genehmigungen und Routing-Regeln)
* Die Felder [!UICONTROL Zuweisungen] in Listen und Berichten
* Benutzerprofile

  >[!NOTE]
  >
  >Wenn Sie einem Benutzer eine neue Rolle hinzufügen, wird keine deaktivierte Auftragsrolle angezeigt. Sie wird jedoch weiterhin in den Feldern [!UICONTROL Primäre Rolle] und [!UICONTROL Andere Rollen] angezeigt, wenn der Benutzer mit der Auftragsrolle verknüpft war, bevor sie deaktiviert wurde.

* Das Dialogfeld [!UICONTROL Freigabe] für Objekte, einschließlich der Zuweisung von Layoutvorlagen
* Felder mit Schreibvorgängen in benutzerdefinierten Formularen
* Das Feld [!UICONTROL Poolmitglieder] in [!UICONTROL Ressourcenpools]
* Das Feld [!UICONTROL Auftragsrolle] auf einem Bearbeitungsbildschirm für die [!UICONTROL Abrechnungsrate] , wenn ein Benutzer die Abrechnungsraten für Projekte außer Kraft setzt
* Dialogfeld [!UICONTROL Zuweisung zur Kanban-Pinnwand hinzufügen] in einem Projekt
* Das Feld [!UICONTROL Auftragsrolle] eines Plans oder einer Initiative, wenn jemand die [!DNL Adobe Workfront Scenario Planner] verwendet.

  Die [!DNL Scenario Planner] ist nur im neuen [!DNL Adobe Workfront] -Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter [Überblick [!DNL Scenario Planner] 3}.](../../../scenario-planner/scenario-planner-overview.md)

>[!TIP]
>
>Deaktivierte Rollen werden immer in Filtern in Listen, Berichten und anderen Werkzeugen wie dem [!UICONTROL Arbeitslast-Ausgleich] angezeigt.

## Überlegungen zum Deaktivieren einer Stellenrolle

Es ist besser, veraltete Vorgangsrollen zu deaktivieren, anstatt sie zu löschen, damit Sie alle historischen Informationen beibehalten können, die mit Rollen verknüpft sind, die Sie in der Vergangenheit verwendet haben.

>[!NOTE]
>
>Alle Arbeiten, die der Auftragsrolle vor der Deaktivierung zugewiesen wurden, bleiben zugewiesen.

Es wird empfohlen, folgende Schritte durchzuführen, bevor Sie eine nicht verwendete Vorgangsrolle deaktivieren:

* Erstellen Sie Berichte für alle Objekte, die der Rolle zugewiesen sind, die Sie deaktivieren möchten, und weisen Sie sie einer aktiven Auftragsrolle zu. Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

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

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf &#x200B; **[!UICONTROL Vorgangsrollen].**
1. (Optional) Wählen Sie im Dropdown-Menü **[!UICONTROL Filter]** die Option **[!UICONTROL Aktiv]** aus, um nur aktive Auftragsrollen anzuzeigen.
1. Klicken Sie auf den Namen der Auftragsrolle, die Sie deaktivieren möchten.
1. Wählen Sie im Dropdownmenü **[!UICONTROL Ist aktiv]** die Option **[!UICONTROL Nein]** aus.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   Die Auftragsrolle ist deaktiviert und kann nicht mehr der Arbeit zugewiesen werden, mit Layoutvorlagen verknüpft sind usw. Weitere Informationen zu allen Verwendungen von Auftragsrollen in [!DNL Workfront] finden Sie unter [Übersicht über Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
