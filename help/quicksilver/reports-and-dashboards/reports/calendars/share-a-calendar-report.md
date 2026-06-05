---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Kalenderbericht freigeben
description: Sie können einen Kalender für andere Benutzer freigeben und öffentlich verfügbar machen, sodass ihn  [!DNL Adobe Workfront]  ohne Lizenz anzeigen können.
author: Courtney
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/stg5BuJJo-hPWoXl3E7QnO2RW2h7rwQ4Pptw5H2MGq4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 593
ht-degree: 8%

---

# Freigeben eines Kalenderberichts

Sie können einen Kalender für andere Benutzer freigeben und öffentlich verfügbar machen, sodass ihn jemand ohne [!DNL Adobe Workfront] Lizenz anzeigen kann.

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
   <td> <p> Anzeigen oder Erweitern des Zugriffs auf Berichte, Dashboards und Kalender</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen von oder höheren Berechtigungen für den Kalenderbericht mit Zugriff auf die Freigabe</td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Kalender für [!DNL Workfront] Benutzer freigeben {#share-a-calendar-with-workfront-users}

Die Freigabe eines Kalenders ähnelt der Freigabe anderer Objekte. Weitere Informationen zum Freigeben von Objekten in [!DNL Adobe Workfront] finden Sie unter [Übersicht über Berechtigungen zum Freigeben von Objekten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Kalender, die für Sie freigegeben wurden, werden mit einem Sternchen (&#42;) neben dem Kalendernamen angezeigt.

So geben Sie einen Kalender in [!DNL Workfront] frei:

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie auf das **Mehr**-Menü neben dem Kalendernamen und dann auf **Freigabe**.
   ![Menü „Kalender Mehr“](assets/more-menu-calendar.png)
1. Beginnen Sie im Feld **[!UICONTROL Kalenderzugriff erteilen an]** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe, des Unternehmens oder des Geschäftsprofils, den/die Sie für den Kalender freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
   Weitere Informationen zum Festlegen von Berechtigungen finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Wiederholen Sie Schritt 3 für jeden Benutzer, jedes Team, jede Rolle oder jede Gruppe, dem bzw. der Sie Zugriff auf den Kalender gewähren möchten.
1. Geben Sie die Berechtigungen für jeden Benutzer, jedes Team, jede Rolle, jede Gruppe oder jedes Unternehmen an, die bzw. das Sie in Schritt 3 hinzugefügt haben, indem Sie auf das Dropdown-Menü klicken, und wählen Sie dann die Berechtigungsstufe aus, die Sie gewähren möchten:

   * **[!UICONTROL Anzeigen]:** Benutzer können den Kalender überprüfen und freigeben.

     ![Kalender mit Ansichtszugriff freigeben](assets/view-calendar.png)

   * **[!UICONTROL Verwalten]:** Benutzer haben vollen Zugriff auf den Kalender abzüglich Administratorrechten, die auf Zugriffsebene gewährt werden, sowie alle Anzeigeberechtigungen.

     ![Kalender mit „Zugriff verwalten“ freigeben](assets/manage-calendar.png)

     >[!NOTE]
     >
     >Der [!DNL Workfront] und der Ersteller des Kalenders können Berechtigungen aus diesen Entitäten entfernen.

1. (Optional) Abhängig von der Rolle eines Benutzers können Sie möglicherweise auf **[!UICONTROL Erweiterte Optionen]** und dann auf **[!UICONTROL Freigeben]** klicken&#x200B;, damit der Benutzer den Kalender für andere Benutzer freigeben kann.

   Weitere Informationen zu den Berechtigungsebenen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Um den Kalender für alle [!DNL Workfront] Benutzer verfügbar zu machen, klicken Sie auf das Zahnradsymbol und dann im Dropdown-Menü auf **[!UICONTROL Systemweit sichtbar machen]** um das Objekt für alle [!DNL Workfront] Benutzer verfügbar zu machen.\
   Alle Benutzer können das -Objekt basierend auf den von Ihnen festgelegten Berechtigungen sehen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Kalender über einen öffentlichen Link freigeben

Sie können einen Kalender öffentlich machen und einen Link für Personen freigeben, die keine [!DNL Workfront] haben.

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie **[!UICONTROL Kalenderaktionen]** und dann auf **[!UICONTROL Freigabe]**.
1. Klicken Sie auf das **Mehr**-Menü neben dem Kalendernamen.
   ![Menü „Mehr Kalender“](assets/more-menu-calendar.png)
Klicken Sie **Öffentlichen Link kopieren**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Kalender über einen privaten Link freigeben

Sie können einen Link für einen privaten Kalender für [!DNL Workfront] Benutzer freigeben. Benutzer müssen sich anmelden, um den Kalender anzuzeigen, wenn sie den Link verwenden.

1. Wechseln Sie zu dem Kalender, den Sie freigeben möchten.
1. Klicken Sie auf das **Mehr**-Menü neben dem Kalendernamen und dann auf **[!UICONTROL Freigebbaren Link abrufen]**.
   ![Menü „Kalender Mehr“](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >[!DNL Workfront] Benutzer müssen Zugriff auf den Kalender haben, damit sie mit dem Link darauf zugreifen können. Informationen zum Gewähren des Zugriffs finden Sie unter [Freigeben eines Kalenders für  [!DNL Workfront] Benutzer](#share-a-calendar-with-workfront-users).\
   >Wenn Benutzende keinen Zugriff haben, können sie ihn anfordern, nachdem sie den Link in ihren Browser eingefügt haben.
