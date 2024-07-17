---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Kalenderberichte freigeben
description: Sie können einen Kalender für andere Benutzer freigeben und ihn öffentlich zugänglich machen, sodass auch Benutzer ohne  [!DNL Adobe Workfront] Lizenz ihn anzeigen können.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Kalenderberichte freigeben

Sie können einen Kalender für andere Benutzer freigeben und ihn öffentlich zugänglich machen, sodass auch Benutzer ohne [!DNL Adobe Workfront] -Lizenz ihn anzeigen können.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höher Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für den Kalenderbericht mit Zugriff auf die Freigabe</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Kalender für [!DNL Workfront] Benutzer freigeben {#share-a-calendar-with-workfront-users}

Das Freigeben eines Kalenders ähnelt dem Freigeben anderer Objekte. Weitere Informationen zum Freigeben von Objekten in [!DNL Adobe Workfront] finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Für Sie freigegebene Kalender werden mit einem Sternchen (&#42;) neben dem Kalendernamen angezeigt.

So geben Sie einen Kalender innerhalb von [!DNL Workfront] frei:

1. Gehen Sie zum Kalender, den Sie freigeben möchten.
1. Klicken Sie auf **[!UICONTROL Kalenderaktionen]** und dann auf **[!UICONTROL Freigabe]**.

1. Geben Sie im Feld **[!UICONTROL Kalenderzugriff auf]** geben Sie den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/die Sie den Kalender freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.\
   Weitere Informationen zum Festlegen von Berechtigungen finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Wiederholen Sie Schritt 3 für jeden Benutzer, jedes Team, jede Rolle oder jede Gruppe, dem/der Sie Zugriff auf den Kalender gewähren möchten.
1. Geben Sie die Berechtigungen für jeden Benutzer, jedes Team, jede Rolle, jede Gruppe oder jedes Unternehmen an, die Sie in Schritt 3 hinzugefügt haben, indem Sie auf das Dropdown-Menü klicken und dann die Berechtigungsebene auswählen, die Sie gewähren möchten:

   * **[!UICONTROL Ansicht]:** Benutzer können den Kalender überprüfen und freigeben.

     ![Kalenderfreigabe mit Ansichtszugriff](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL Verwalten]:** Benutzer haben vollen Zugriff auf den Kalender abzüglich der Administratorrechte, die auf Zugriffsebene gewährt werden, sowie aller Anzeigeberechtigungen.

     ![Kalenderfreigabe mit Zugriff verwalten](assets/calendar-share-manage-permissions-350x241.png)

     >[!NOTE]
     >
     >Der Administrator [!DNL Workfront] und der Ersteller des Kalenders haben die Möglichkeit, Berechtigungen aus diesen Entitäten zu entfernen.

1. (Optional) Abhängig von der Rolle eines Benutzers können Sie möglicherweise auf **[!UICONTROL Erweiterte Optionen]** klicken und dann auf **[!UICONTROL Freigabe]** &#x200B;, damit der Benutzer den Kalender für andere Benutzer freigeben kann.

   Weitere Informationen zu den Berechtigungsstufen finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Optional) Um den Kalender für alle [!DNL Workfront] -Benutzer verfügbar zu machen, klicken Sie auf das Zahnradsymbol und dann im Dropdown-Menü auf **[!UICONTROL Dieses Objekt systemweit anzeigen]** , um es allen [!DNL Workfront] -Benutzern zur Verfügung zu stellen.\
   Alle Benutzer können das Objekt anhand der von Ihnen festgelegten Berechtigungen anzeigen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Einen Kalender mit einem öffentlichen Link teilen

Sie können einen Kalender veröffentlichen und einen Link für Personen freigeben, die keine [!DNL Workfront] -Lizenz haben.

1. Gehen Sie zum Kalender, den Sie freigeben möchten.
1. Klicken Sie auf **[!UICONTROL Kalenderaktionen]** und dann auf **[!UICONTROL Freigabe]**.

1. Klicken Sie auf das Zahnradsymbol und klicken Sie dann auf **[!UICONTROL Diese für externe Benutzer veröffentlichen]**.
1. Klicken Sie auf **[!UICONTROL Link kopieren]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Kalender mit einem privaten Link freigeben

Sie können einen privaten Kalender-Link für [!DNL Workfront] Benutzer freigeben. Benutzer müssen sich anmelden, um den Kalender anzuzeigen, wenn sie den Link verwenden.

1. Gehen Sie zum Kalender, den Sie freigeben möchten.
1. Klicken Sie auf **[!UICONTROL Kalenderaktionen]** und dann auf **[!UICONTROL Freigabe-Link abrufen]**.

1. Klicken Sie auf **[!UICONTROL Link kopieren]**.

   >[!NOTE]
   >
   >[!DNL Workfront] -Benutzer müssen Zugriff auf den Kalender haben, um über den Link darauf zugreifen zu können. Informationen zum Gewähren des Zugriffs finden Sie unter [Freigeben eines Kalenders für  [!DNL Workfront] Benutzer](#share-a-calendar-with-workfront-users).\
   >Wenn Benutzer keinen Zugriff haben, können sie ihn anfordern, nachdem sie den Link in ihren Browser eingefügt haben.
