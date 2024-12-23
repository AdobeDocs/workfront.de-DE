---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deaktivieren oder Löschen eines Teams
description: Sie können nicht mehr verwendete Teams deaktivieren und dabei die zugehörigen historischen Daten beibehalten. Adobe Workfront-Administratoren können ein Team jederzeit über den Bereich Teams in der Einrichtung reaktivieren.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Deaktivieren oder Löschen eines Teams

Sie können nicht mehr verwendete Teams deaktivieren und dabei die zugehörigen historischen Daten beibehalten. [!DNL Adobe Workfront] -Administratoren können ein Team jederzeit über den Bereich Teams in der Einrichtung reaktivieren. Wenn Sie ein Team deaktivieren, wird das Team nicht mehr in den folgenden Bereichen angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Felder mit Schreibvorgängen in benutzerdefinierten Formularen</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Dialogfeld "Freigeben"für Objekte</p> </li> 
     <li> <p>[!UICONTROL Benutzerprofil]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Dropdown-Menü Hauptauswahl im Bereich [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Zuweisung] typeahead</p> </li> 
     <li> <p>[!UICONTROL Zum Kanban-Board-Dialog in einem Projekt hinzufügen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Deaktivierte Teams werden nicht angezeigt, wenn Sie nach einem Team suchen. Sie werden jedoch weiterhin im [!UICONTROL Startseiten-Team] und in anderen Teams angezeigt, wenn der Benutzer dem Team vor der Deaktivierung zugewiesen wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr>
  <tr>
   <td>Konfigurationen auf Zugriffsebene</td>
   <td><p>Zum Deaktivieren eines Teams sind keine Konfigurationen erforderlich.</p>
   <p>Um ein Team zu löschen, müssen Sie Systemadministrator sein.</p></td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deaktivieren eines Teams

Alle dem Team vor der Deaktivierung zugewiesenen Aufgaben bleiben zugewiesen. Es wird empfohlen, die Arbeit erneut zu unterschreiben, bevor Sie das Team deaktivieren.

>[!TIP]
>
>Sie können einen Bericht erstellen, um nach Aufgaben oder Problemen zu filtern, denen das deaktivierte Team weiterhin zugewiesen ist.

Wenn Sie Anforderungswarteschlangen verwenden und ein in einer Routing-Regel als Standardteam zugewiesenes Team deaktivieren, bleibt das Team erhalten und die Anforderungen werden weiterhin an das deaktivierte Team weitergeleitet. Es wird empfohlen, Routing-Regeln mit aktiven Teams zu aktualisieren, bevor Sie das Team deaktivieren.

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!DNL Switch team]** und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![](assets/edit-team-settings.png)

1. Deaktivieren Sie in den Teameinstellungen das Kontrollkästchen **[!UICONTROL Ist aktiv]** .
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Bekannte Einschränkungen beim Deaktivieren eines Teams

Deaktivierte Teams werden in den folgenden Bereichen angezeigt:

* Das Feld Inhaber in [!DNL Workfront Goals]. Dies erfordert eine zusätzliche Lizenz für [!DNL Adobe Workfront Goals]. Weitere Informationen finden Sie unter [Erste Schritte mit  [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Team löschen

Nur ein Systemadministrator kann ein Team löschen. Wenn Sie ein Team-Eigentümer (aber kein Administrator) sind und versuchen, ein Team zu löschen, wird eine Fehlermeldung angezeigt.

Löschen eines Teams:

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!DNL Switch team]** und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Löschen]** aus.

   ![](assets/edit-team-settings.png)

1. Klicken Sie in der Bestätigungsmeldung auf [!UICONTROL **Bestätigen**] , um das Team dauerhaft zu löschen. Gelöschte Teams können nicht wiederhergestellt werden.
