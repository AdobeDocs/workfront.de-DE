---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Kalenderbericht freigeben
description: Sie können einen Kalender für andere Benutzer freigeben und ihn öffentlich zugänglich machen, sodass jemand ohne  [!DNL Adobe Workfront] Lizenz ihn anzeigen kann.
author: Courtney
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 8%

---

# Freigeben eines Kalenderberichts


Sie können einen Kalender für andere Benutzer freigeben und ihn öffentlich zugänglich machen, sodass jemand ohne [!DNL Adobe Workfront]-Lizenz ihn anzeigen kann.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Leicht</p>
       <p>Überprüfung</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p> Anzeigen oder erweitern des Zugriffs auf Berichte, Dashboards und Kalender</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Berechtigungen für den Kalenderbericht anzeigen oder höher mit Zugriff auf die Freigabe</td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Kalender für [!DNL Workfront] Benutzer freigeben {#share-a-calendar-with-workfront-users}

Die Freigabe eines Kalenders ähnelt der Freigabe anderer Objekte. Weitere Informationen zum Freigeben von Objekten in [!DNL Adobe Workfront] finden Sie unter [Übersicht über die Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Kalender, die für Sie freigegeben wurden, werden mit einem Sternchen (&#42;) neben dem Kalendernamen angezeigt.

So geben Sie einen Kalender in [!DNL Workfront] frei:

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie auf das Menü **Mehr** neben dem Kalendernamen, und klicken Sie dann auf **Freigabe**.
   ![Kalender mehr Menü](assets/more-menu-calendar.png)
1. Beginnen Sie im Feld **[!UICONTROL Kalender Zugriff auf]** gewähren mit der Eingabe des Namens des Benutzers, des Teams, der Rolle, der Gruppe oder des Unternehmens, für den bzw. das Sie den Kalender freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.\
   Weitere Informationen zum Festlegen von Berechtigungen finden Sie unter [Übersicht über die Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Wiederholen Sie Schritt 3 für alle Benutzer, Teams, Rollen oder Gruppen, denen Sie Zugriff auf den Kalender gewähren möchten.
1. Geben Sie die Berechtigungen für jeden Benutzer, jedes Team, jede Rolle, jede Gruppe oder jedes Unternehmen an, die Sie in Schritt 3 hinzugefügt haben, indem Sie auf das Dropdown-Menü klicken, und wählen Sie dann die Berechtigungsebene aus, die Sie erteilen möchten:

   * **[!UICONTROL Anzeigen]:** Benutzer können den Kalender überprüfen und freigeben.

     ![Kalender mit Anzeigezugriff freigeben](assets/view-calendar.png)

   * **[!UICONTROL Verwalten]:** Benutzer haben vollständigen Zugriff auf den Kalender, abzüglich der Administratorrechte, die auf der Zugriffsebene gewährt werden, sowie aller Anzeigeberechtigungen.

     ![Kalender freigeben mit Zugriff verwalten](assets/manage-calendar.png)

     >[!NOTE]
     >
     >Der [!DNL Workfront]-Administrator und der Ersteller des Kalenders können Berechtigungen für diese Entitäten entfernen.

1. (Optional) Abhängig von der Rolle eines Benutzers können Sie auf **[!UICONTROL Erweiterte Optionen]** klicken und dann auf **[!UICONTROL Freigeben]** &#x200B; klicken, damit der Benutzer den Kalender für andere Benutzer freigeben kann.

   Weitere Informationen zu den Berechtigungsebenen finden Sie unter [Übersicht über die Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Um den Kalender allen [!DNL Workfront] Benutzern zur Verfügung zu stellen, klicken Sie auf das Zahnradsymbol und dann im Dropdown-Menü auf **[!UICONTROL Dieses Objekt systemweit sichtbar machen]**, um das Objekt allen [!DNL Workfront] Benutzern zur Verfügung zu stellen.\
   Alle Benutzer können das Objekt basierend auf den von Ihnen festgelegten Berechtigungen sehen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Freigeben eines Kalenders mit einem öffentlichen Link

Sie können einen Kalender veröffentlichen und einen Link für Personen freigeben, die keine [!DNL Workfront]-Lizenz haben.

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie auf **[!UICONTROL Kalenderaktionen]**, und klicken Sie dann auf **[!UICONTROL Freigeben]**.
1. Klicken Sie auf das Menü **Mehr** neben dem Kalendernamen.
   ![Kalender mehr Menü](assets/more-menu-calendar.png)
Klicken Sie auf **Öffentlichen Link kopieren**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Freigeben eines Kalenders mit einem privaten Link

Sie können einen privaten Kalenderlink für [!DNL Workfront] Benutzer freigeben. Benutzer müssen sich anmelden, um den Kalender anzuzeigen, wenn sie den Link verwenden.

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie auf das Menü **Mehr** neben dem Kalendernamen, und klicken Sie dann auf **[!UICONTROL Freigabe-Link abrufen]**.
   ![Kalender mehr Menü](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >[!DNL Workfront] Benutzer müssen Zugriff auf den Kalender haben, um mit dem Link darauf zuzugreifen. Informationen zum Gewähren des Zugriffs finden Sie unter [Freigeben eines Kalenders für  [!DNL Workfront] Benutzer](#share-a-calendar-with-workfront-users).\
   >Wenn Benutzer keinen Zugriff haben, können sie ihn anfordern, nachdem sie den Link in ihren Browser eingefügt haben.
