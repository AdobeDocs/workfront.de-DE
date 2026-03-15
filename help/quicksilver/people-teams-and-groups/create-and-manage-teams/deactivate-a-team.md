---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Team deaktivieren oder löschen
description: Sie können Teams deaktivieren, die Sie nicht mehr verwenden, und gleichzeitig die zugehörigen Verlaufsdaten beibehalten. Adobe Workfront-Administratoren können ein Team jederzeit über den Bereich "Teams" im Fenster "Einrichtung" wieder aktivieren.
author: Courtney
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 10%

---

# Deaktivieren oder Löschen eines Teams

Sie können Teams deaktivieren, die Sie nicht mehr verwenden, und gleichzeitig die zugehörigen Verlaufsdaten beibehalten. [!DNL Adobe Workfront] Administratoren können ein Team jederzeit über den Bereich &quot;Teams&quot; im Setup erneut aktivieren. Wenn Sie ein Team deaktivieren, wird das Team nicht mehr in den folgenden Bereichen angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Vorauseilende Felder in benutzerdefinierten Formularen</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Dialogfeld "Freigeben" für Objekte</p> </li> 
     <li> <p>[!UICONTROL-Benutzerprofil]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Hauptauswahldropdownmenü im Bereich [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Assignments] typeahead</p> </li> 
     <li> <p>[!UICONTROL Zu Kanban hinzufügen] Board-Dialog in einem Projekt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Deaktivierte Teams werden nicht angezeigt, wenn Sie nach einem Team suchen, werden aber dennoch in [!UICONTROL Home Team] und anderen Teams angezeigt, wenn der Benutzer dem Team vor der Deaktivierung zugewiesen wurde.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Abo</p></td>
  </tr> 
  <tr>
   <td>Konfigurationen der Zugriffsebene</td>
   <td><p>Zum Deaktivieren eines Teams sind keine Konfigurationen erforderlich.</p>
   <p>Um ein Team zu löschen, müssen Sie ein Systemadministrator sein.</p></td>
  </tr>
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Team deaktivieren

Alle Arbeiten, die dem Team vor der Deaktivierung zugewiesen wurden, bleiben zugewiesen. Es wird empfohlen, die Arbeit neu zuzuweisen, bevor Sie das Team deaktivieren.

>[!TIP]
>
>Sie können einen Bericht erstellen, um alle Aufgaben oder Probleme zu filtern, denen das deaktivierte Team noch zugewiesen ist.

Wenn Sie bei der Verwendung von Anfragewarteschlangen ein Team deaktivieren, das als Standardteam in einer Routingregel zugewiesen ist, bleibt das Team erhalten und Anfragen werden weiterhin an das deaktivierte Team weitergeleitet. Es wird empfohlen, Routingregeln mit aktiven Teams zu aktualisieren, bevor Sie das Team deaktivieren.

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!DNL Switch team]** und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![](assets/edit-team-settings.png)

1. Deaktivieren Sie das Kontrollkästchen **[!UICONTROL Ist aktiv]** in den Teameinstellungen.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Bekannte Einschränkungen bei der Deaktivierung eines Teams

Deaktivierte Teams werden in den folgenden Bereichen angezeigt:

* Das Feld Eigentümer in [!DNL Workfront Goals]. Hierfür ist eine zusätzliche Lizenz für [!DNL Adobe Workfront Goals] erforderlich. Weitere Informationen finden Sie unter [Erste Schritte mit  [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Team löschen

Nur ein Systemadministrator kann ein Team löschen. Wenn Sie Teambesitzer (aber kein Administrator) sind und versuchen, ein Team zu löschen, wird eine Fehlermeldung angezeigt.

Löschen eines Teams:

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!DNL Switch team]** und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Löschen]** aus.

   ![](assets/edit-team-settings.png)

1. Klicken Sie in der Bestätigungsmeldung auf [!UICONTROL **Bestätigen**], um das Team endgültig zu löschen. Gelöschte Teams können nicht wiederhergestellt werden.
