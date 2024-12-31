---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Aufgabengebiete deaktivieren
description: Als  [!DNL Adobe Workfront]  oder Benutzer mit administrativem Zugriff auf Aufgabengebiete können Sie Aufgabengebiete deaktivieren, die in Ihrem System veraltet sind. Wenn Sie ein Aufgabengebiet deaktivieren, anstatt es zu löschen, können Sie alle historischen Informationen beibehalten, die mit ihm verknüpft sind.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 1%

---

# Aufgabengebiete deaktivieren

Als [!DNL Adobe Workfront] oder Benutzer mit administrativem Zugriff auf Aufgabengebiete können Sie Aufgabengebiete deaktivieren, die in Ihrem System veraltet sind. Wenn Sie ein Aufgabengebiet deaktivieren, anstatt es zu löschen, können Sie alle historischen Informationen beibehalten, die mit ihm verknüpft sind.

Sie können auch Aufgabengebiete reaktivieren, die zuvor deaktiviert wurden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: [!UICONTROL Standard]</p>
   <p>Oder</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf Aufgabengebiete</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Die Auswirkungen der Deaktivierung von Aufgabengebieten

Wenn Sie ein Aufgabengebiet deaktivieren, wird es nicht mehr in den folgenden Bereichen angezeigt:

* Das Feld [!UICONTROL Arbeitsaufträge] mit automatischer Textvervollständigung (für Aufgaben, Vorlagenaufgaben, Probleme, Genehmigungen und Routing-Regeln)
* Die [!UICONTROL Arbeitsaufträge] Felder in Listen und Berichten
* Benutzerprofile

  >[!NOTE]
  >
  >Wenn Sie einem Benutzer eine neue Rolle hinzufügen, wird ein deaktiviertes Aufgabengebiet nicht angezeigt. Er wird jedoch weiterhin in den Feldern [!UICONTROL Primäre Rolle] und [!UICONTROL Andere Rollen] angezeigt, wenn der/die Benutzende mit dem Aufgabengebiet verknüpft war, bevor es deaktiviert wurde.

* Das Dialogfeld [!UICONTROL Freigabe] für Objekte, einschließlich der Zuweisung von Layout-Vorlagen
* Felder mit automatischer Textvervollständigung in benutzerdefinierten Formularen
* Das Feld [!UICONTROL Pool-Mitglieder] in [!UICONTROL Ressourcenpools]
* Das Feld [!UICONTROL Aufgabengebiet] eines Bearbeitungsbildschirms [!UICONTROL Abrechnungssatz], wenn ein Benutzer Abrechnungssätze für Projekte überschreibt
* Das [!UICONTROL  „Zuweisung zu Kanban-Board hinzufügen] in einem Projekt
* Das [!UICONTROL Aufgabengebiet] eines Plans oder einer Initiative, wenn jemand die [!DNL Adobe Workfront Scenario Planner] verwendet.

  Die [!DNL Scenario Planner] ist nur in der neuen [!DNL Adobe Workfront] verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter [Die [!DNL Scenario Planner] Übersicht](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Deaktivierte Rollen werden immer in Filtern in Listen, Berichten und anderen Tools wie dem [!UICONTROL Workload Balancer) ].

## Überlegungen vor der Deaktivierung eines Aufgabengebiets

Es ist besser, veraltete Aufgabengebiete zu deaktivieren als zu löschen, damit Sie alle historischen Informationen zu Funktionen behalten können, die Sie in der Vergangenheit möglicherweise verwendet haben.

>[!NOTE]
>
>Jede Arbeit, die dem Aufgabengebiet vor der Deaktivierung zugewiesen wurde, bleibt zugewiesen.

Es wird empfohlen, Folgendes zu tun, bevor Sie ein nicht verwendetes Aufgabengebiet deaktivieren:

* Erstellen Sie Berichte für alle Objekte, die der Rolle zugewiesen sind, die Sie deaktivieren möchten, und weisen Sie sie einem aktiven Aufgabengebiet zu. Informationen zum Erstellen von Berichten finden Sie [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Sie können einen Bericht erstellen, um nach allen Aufgaben oder Problemen zu filtern, denen die deaktivierte Rolle zugewiesen ist. Verwenden Sie dann den Bericht, um ausstehende Aufgaben oder Probleme einer aktiven Rolle zuzuweisen.

* Erfassen Sie eine Bestandsaufnahme aller Genehmigungsprozesse, aktuellen Genehmigungspfade und Routingregeln oder anderer Objekte, die dem Aufgabengebiet zugewiesen sind, das Sie deaktivieren möchten, und weisen Sie sie einer aktiven Funktion zu.

  >[!TIP]
  >
  >Wenn Sie bei Verwendung von Anfrage-Warteschlangen ein Aufgabengebiet deaktivieren, das in einer Routing-Regel als standardmäßiger Beauftragter zugewiesen ist, bleibt die Rolle bestehen und Anfragen werden weiterhin an die deaktivierte Rolle weitergeleitet. Es wird empfohlen, Routing-Regeln mit aktiven Rollen zu aktualisieren, bevor Sie das Team deaktivieren.

  Informationen zum Erstellen von Genehmigungsprozessen und Routing-Regeln finden Sie in den folgenden Artikeln:

   * [Einen Genehmigungsprozess für Arbeitselemente erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Routingregeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Aufgabengebiet deaktivieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf &#x200B;**[!UICONTROL Aufgabengebiete].**
1. (Optional) Wählen Sie im Dropdown **[!UICONTROL Menü]** Filter **[!UICONTROL die Option „Aktiv]** aus, um nur aktive Aufgabengebiete anzuzeigen.
1. Klicken Sie auf den Namen des Aufgabengebiets, das Sie deaktivieren möchten.
1. Wählen Sie im Dropdown **[!UICONTROL Menü]** Ist aktiv“ die Option **[!UICONTROL Nein]** aus.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   Das Aufgabengebiet ist deaktiviert und kann nicht mehr der Arbeit zugewiesen und mit Layout-Vorlagen verknüpft werden usw. Informationen zu allen Verwendungen von Aufgabengebieten in [!DNL Workfront] finden Sie unter [Aufgabengebiet - Übersicht](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
