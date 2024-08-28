---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Verwalten von Meldungen und Problemen auf der Trommelfläche
description: Sie können eine Meldung oder ein Problem aus dem Scrum-Board in eine andere Iteration oder in den Rückstand verschieben oder aus dem Scrum-Board löschen. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Meldungen und Probleme auf der [!UICONTROL Scrum]-Pinnwand verwalten

Sie können eine Meldung oder ein Problem von der [!UICONTROL Scrum]-Pinnwand in eine andere Iteration oder in den Rückstand verschieben oder aus der [!UICONTROL Scrum]-Pinnwand löschen. Wenn Sie einen Artikel oder ein Problem löschen, wird er 30 Tage lang in den Papierkorb verschoben und kann nur vom Systemadministrator abgerufen werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Zugriff auf die Aufgabe oder das Problem verwalten </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verschieben Sie eine Geschichte oder ein Problem aus der [!UICONTROL Scrum]-Pinnwand.

{{step1-to-team}}

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

## Löschen Sie eine Geschichte oder ein Problem aus der [!UICONTROL Scrum]-Pinnwand

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein Scrum-Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf das Symbol **[!UICONTROL Mehr]** für die Meldung oder das Problem und wählen Sie **[!UICONTROL Meldung löschen]** oder **[!UICONTROL Problem löschen]** aus.

   ![Löschen oder Verschieben einer Geschichte von der Trommelplatine](assets/scrum-delete-move-story.png)

1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Ja, löschen Sie sie]**.
