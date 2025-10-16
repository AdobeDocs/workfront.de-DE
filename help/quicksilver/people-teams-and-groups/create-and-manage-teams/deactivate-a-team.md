---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deaktivieren oder Löschen eines Teams
description: Sie können Teams, die Sie nicht mehr verwenden, deaktivieren, während Sie die zugehörigen historischen Daten beibehalten. Adobe Workfront-Administratoren können ein Team jederzeit über den Bereich Teams im Setup reaktivieren.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Deaktivieren oder Löschen eines Teams

Sie können Teams, die Sie nicht mehr verwenden, deaktivieren, während Sie die zugehörigen historischen Daten beibehalten. [!DNL Adobe Workfront] Administratoren können ein Team jederzeit im Bereich Teams im Setup erneut aktivieren. Wenn Sie ein Team deaktivieren, wird das Team nicht mehr in den folgenden Bereichen angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Felder mit automatischer Textvervollständigung in benutzerdefinierten Formularen</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Dialogfeld „Freigeben“ für Objekte</p> </li> 
     <li> <p>[!UICONTROL Benutzerprofil]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Dropdown-Menü für die Hauptauswahl im Bereich [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Assignments] mit automatischer Textvervollständigung</p> </li> 
     <li> <p>Dialogfeld [!UICONTROL Zu Kanban hinzufügen] in einem Projekt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Deaktivierte Teams werden bei der Suche nach einem Team nicht angezeigt, werden aber weiterhin im [!UICONTROL Home-Team] und „Andere Teams“ angezeigt, wenn der Benutzer dem Team vor der Deaktivierung zugewiesen wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Konfigurationen der Zugriffsebene</td>
   <td><p>Um ein Team zu deaktivieren, sind keine Konfigurationen erforderlich.</p>
   <p>Um ein Team zu löschen, müssen Sie Systemadministrator sein.</p></td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Team deaktivieren

Alle Arbeiten, die dem Team vor der Deaktivierung zugewiesen wurden, bleiben zugewiesen. Es wird empfohlen, Arbeit neu zuzuweisen, bevor Sie das Team deaktivieren.

>[!TIP]
>
>Sie können einen Bericht erstellen, um nach allen Aufgaben oder Problemen zu filtern, denen das deaktivierte Team noch zugewiesen ist.

Wenn Sie bei Verwendung von Anfrage-Warteschlangen ein Team deaktivieren, das in einer Routing-Regel als Standard-Team zugewiesen ist, bleibt das Team bestehen und Anfragen werden weiterhin an das deaktivierte Team weitergeleitet. Es wird empfohlen, Routing-Regeln mit aktiven Teams zu aktualisieren, bevor Sie das Team deaktivieren.

{{step1-to-team}}

1. Klicken Sie auf das **[!DNL Switch team]** und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![](assets/edit-team-settings.png)

1. Deaktivieren Sie **[!UICONTROL Kontrollkästchen „Ist]**&quot; in den Team-Einstellungen.
1. Klicken Sie **[!UICONTROL Änderungen speichern]**.

## Bekannte Einschränkungen bei der Deaktivierung eines Teams

Deaktivierte Teams werden in den folgenden Bereichen angezeigt:

* Das Feld „Besitzer“ in [!DNL Workfront Goals]. Dies erfordert eine zusätzliche Lizenz für [!DNL Adobe Workfront Goals]. Weitere Informationen finden Sie unter [Erste Schritte mit [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Team löschen

Nur ein Systemadministrator kann ein Team löschen. Wenn Sie Teameigentümer sind (aber kein Administrator) und versuchen, ein Team zu löschen, wird eine Fehlermeldung angezeigt.

Löschen eines Teams:

{{step1-to-team}}

1. Klicken Sie auf das **[!DNL Switch team]** und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Löschen]** aus.

   ![](assets/edit-team-settings.png)

1. Klicken Sie [!UICONTROL **der**] auf „Bestätigen“, um das Team dauerhaft zu löschen. Gelöschte Teams können nicht wiederhergestellt werden.
