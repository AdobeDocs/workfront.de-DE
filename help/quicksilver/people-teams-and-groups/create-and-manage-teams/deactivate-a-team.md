---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deaktivieren eines Teams
description: Sie können nicht mehr verwendete Teams deaktivieren und dabei die zugehörigen historischen Daten beibehalten. Adobe Workfront-Administratoren können ein Team jederzeit über den Bereich Teams in der Einrichtung reaktivieren.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Deaktivieren eines Teams

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

Deaktivierte Teams werden nicht angezeigt, wenn Sie nach einem Team suchen, werden jedoch weiterhin in [!UICONTROL Startseite] und Weitere Teams , wenn der Benutzer vor der Deaktivierung dem Team zugewiesen wurde.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Deaktivieren eines Teams

Alle dem Team vor der Deaktivierung zugewiesenen Aufgaben bleiben zugewiesen. Es wird empfohlen, die Arbeit erneut zu unterschreiben, bevor Sie das Team deaktivieren.

>[!TIP]
>
>Sie können einen Bericht erstellen, um nach Aufgaben oder Problemen zu filtern, denen das deaktivierte Team weiterhin zugewiesen ist.

Wenn Sie Anforderungswarteschlangen verwenden und ein in einer Routing-Regel als Standardteam zugewiesenes Team deaktivieren, bleibt das Team erhalten und die Anforderungen werden weiterhin an das deaktivierte Team weitergeleitet. Es wird empfohlen, Routing-Regeln mit aktiven Teams zu aktualisieren, bevor Sie das Team deaktivieren.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Teams]**.
1. Klicken Sie auf **[!DNL Switch team]** und wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   ![](assets/edit-team-settings-350x205.png)

1. Löschen Sie die **[!UICONTROL Ist aktiv]** aktivieren.
1. Klicken **[!UICONTROL Änderungen speichern]**.

## Bekannte Einschränkungen

Deaktivierte Teams werden in den folgenden Bereichen angezeigt:

* Das Feld Inhaber in [!DNL Workfront Goals]. Dies erfordert eine zusätzliche Lizenz für [!DNL Adobe Workfront Goals]. Weitere Informationen finden Sie unter [Erste Schritte mit [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
