---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Verwalten von Meldungen und Problemen auf der Scrum-Pinnwand
description: Sie können eine Meldung oder ein Problem aus dem Scrum-Board in eine andere Iteration oder in den Rückstand verschieben oder aus dem Scrum-Board löschen. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Meldungen und Probleme auf der [!UICONTROL Scrum]-Pinnwand verwalten

Sie können eine Meldung oder ein Problem von der [!UICONTROL Scrum]-Pinnwand in eine andere Iteration oder in den Rückstand verschieben oder aus der [!UICONTROL Scrum]-Pinnwand löschen. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf die Aufgabe oder das Problem verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Geschichte oder Problem aus der [!UICONTROL Scrum]-Pinnwand verschieben

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)
1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein Scrum-Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf das Symbol **[!UICONTROL Mehr]** für die Meldung oder das Problem und wählen Sie **[!UICONTROL Verschieben nach]** aus.

   ![Löschen oder Verschieben einer Geschichte von der Trommelplatine](assets/scrum-delete-move-story.png)

1. Wählen Sie in der Bestätigungsnachricht eine der folgenden Optionen:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Weitere Iteration]</strong></td>
        <td>Wählen Sie aus, um das Element in eine andere Iteration zu verschieben, und wählen Sie dann aus, zu welcher Iteration die Geschichte oder das Problem verschoben werden soll. Wenn keine zukünftigen Iterationen definiert sind, können Sie das Element nicht verschieben.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Wählen Sie diese Option aus, um die Meldung oder das Problem in den Rückstand des Teams zu verschieben.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Das Arbeitselement [!UICONTROL Vorgesehenes Startdatum] und [!UICONTROL Vorgesehenes Abschlussdatum] sind von einer Einstellung auf der Seite [!UICONTROL Team bearbeiten] betroffen. Weitere Informationen finden Sie im Abschnitt [[!UICONTROL Konfigurieren], wie Daten angewendet werden, wenn Arbeitselemente zu einer Iteration hinzugefügt werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicken Sie auf **[!UICONTROL Verschieben]**.

## Meldung oder Problem aus der [!UICONTROL Scrum]-Pinnwand löschen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)
1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein Scrum-Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf das Symbol **[!UICONTROL Mehr]** für die Meldung oder das Problem und wählen Sie **[!UICONTROL Meldung löschen]** oder **[!UICONTROL Problem löschen]** aus.

   ![Löschen oder Verschieben einer Geschichte von der Trommelplatine](assets/scrum-delete-move-story.png)

1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Ja, löschen Sie sie]**.
