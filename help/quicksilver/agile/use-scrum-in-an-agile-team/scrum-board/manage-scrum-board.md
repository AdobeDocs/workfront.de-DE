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
source-wordcount: '490'
ht-degree: 0%

---

# Verwalten Sie Meldungen und Probleme in [!UICONTROL Scrum] Pinnwand

Sie können eine Geschichte oder ein Problem aus dem [!UICONTROL Scrum] -Pinnwand in eine andere Iteration oder in das -Rückstadium platziert oder aus dem [!UICONTROL Scrum] Pinnwand. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.

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
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf die Aufgabe oder das Problem verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Verschieben Sie die Geschichte oder das Problem über [!UICONTROL Scrum] Pinnwand

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.
1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein Scrum-Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich die Option **[!UICONTROL Iterationen]** , um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf **[!UICONTROL Mehr]** auf dem Artikel oder Problem angezeigt werden, und wählen Sie **[!UICONTROL Verschieben nach]**.

   ![Löschen oder verschieben Sie eine Geschichte aus der Scrum-Pinnwand](assets/scrum-delete-move-story.png)

1. Wählen Sie in der Bestätigungsnachricht eine der folgenden Optionen aus:

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
   >Das Arbeitselement [!UICONTROL Geplantes Startdatum] und [!UICONTROL Geplantes Abschlussdatum] sind von einer Einstellung in der [!UICONTROL Team bearbeiten] Seite. Weitere Informationen finden Sie im Abschnitt . [[!UICONTROL Konfigurieren] wie Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration angewendet werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicken **[!UICONTROL Verschieben]**.

## Löschen Sie die Geschichte oder das Problem aus dem [!UICONTROL Scrum] Pinnwand

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.
1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein Scrum-Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich die Option **[!UICONTROL Iterationen]** , um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf **[!UICONTROL Mehr]** auf dem Artikel oder Problem angezeigt werden, und wählen Sie **[!UICONTROL Meldung löschen]** oder **[!UICONTROL Problem löschen]**.

   ![Löschen oder verschieben Sie eine Geschichte aus der Scrum-Pinnwand](assets/scrum-delete-move-story.png)

1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Ja, löschen]**.
