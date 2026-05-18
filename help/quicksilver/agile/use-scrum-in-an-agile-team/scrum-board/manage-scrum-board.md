---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Storys und Probleme auf dem Scrum-Board verwalten
description: Sie können eine Story oder ein Problem vom Scrum-Board in eine andere Iteration oder in den Rückstand verschieben oder aus dem Scrum-Board löschen. Wenn Sie eine Story oder ein Problem löschen, wird diese für 30 Tage in den Papierkorb verschoben und kann nur vom Systemadministrator wiederhergestellt werden.
author: Courtney
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ad56d95f676a2c499ca21fc480cb7de0773f29d4
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 8%

---

# Verwalten von Storys und Problemen auf dem [!UICONTROL Scrum]-Board

Sie können eine Story oder ein Problem von der [!UICONTROL Scrum]-Pinnwand in eine andere Iteration oder in den Rückstand verschieben oder aus der [!UICONTROL Scrum]-Pinnwand löschen. Wenn Sie eine Story oder ein Problem löschen, wird diese für 30 Tage in den Papierkorb verschoben und kann nur vom Systemadministrator wiederhergestellt werden.

Um eine Aufgabe oder ein Problem aus der Iteration zu entfernen, ohne sie zu löschen oder an den Rückstand zu senden, gehen Sie zum Projekt und entfernen Sie das Agile-Team aus der Arbeitsauftragsspalte. Dadurch wird die Aufgabe oder das Problem aus dem Scrum-Board entfernt, es verbleibt jedoch im Projekt.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Manage] Zugriff auf die Aufgabe oder das Problem </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Story oder Problem vom Scrum[!UICONTROL Board &#x200B;]

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]**, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Symbol in der Story oder im Problem und wählen Sie **[!UICONTROL Verschieben nach]**.

   ![Story vom Scrum-Board löschen oder verschieben](assets/scrum-delete-move-story.png)

1. Wählen Sie in der Bestätigungsnachricht eine der folgenden Optionen aus:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Weitere Iteration]</strong></td>
        <td>Wählen Sie diese Option aus, um das Element in eine andere Iteration zu verschieben, und wählen Sie dann aus, in welche Iteration die Story oder das Problem verschoben werden soll. Wenn keine zukünftigen Iterationen definiert sind, können Sie das Element nicht verschieben.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Rückstand]</strong></td>
        <td>Wählen Sie aus, ob die Story oder das Problem in den Rückstand des Teams verschoben werden soll.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Die Einstellungen [!UICONTROL &#x200B; Arbeitselement &#x200B;]Geplantes Startdatum) und [!UICONTROL Geplantes Abschlussdatum] werden von einer Einstellung auf der Seite [!UICONTROL Team bearbeiten] beeinflusst. Weitere Informationen finden Sie im Abschnitt [[!UICONTROL Konfigurieren], wie Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration angewendet werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicken Sie **[!UICONTROL Verschieben]**.

## Löschen einer Story oder eines Problems vom [!UICONTROL Scrum]-Board

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]**, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Symbol in der Story oder dem Problem und wählen Sie **[!UICONTROL Story löschen]** oder **[!UICONTROL Problem löschen]**.

   ![Story vom Scrum-Board löschen oder verschieben](assets/scrum-delete-move-story.png)

1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Ja, löschen]**.
