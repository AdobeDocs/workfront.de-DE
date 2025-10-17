---
product-area: setup
navigation-topic: notifications
keywords: ändern,E-Mail,Benachrichtigung,Einstellungen
title: Eigene E-Mail-Benachrichtigungen ändern
description: In diesem Artikel wird beschrieben, wie Sie Ihre E-Mail-Benachrichtigungen in Ihrem Benutzerprofil verwalten können.
author: Courtney, Becky
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Eigene E-Mail-Benachrichtigungen ändern

<!-- Audited: 1/2024 -->

Der Adobe-[!DNL Workfront] konfiguriert, welche E-Mail-Benachrichtigungen Benutzende erhalten, wenn Ereignisse in Workfront auftreten (wie unter [[!UICONTROL Konfigurieren von ] für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) beschrieben).

Ihr Gruppenadministrator kann auch konfigurieren, welche Benachrichtigungen für Sie und die Benutzer in Ihrer [!UICONTROL Hauptgruppe“ aktiviert ]. Wenn Ihre [!UICONTROL Hauptgruppe] eine Untergruppe ist, erhalten Sie die Benachrichtigungen, die für die Gruppe der obersten Ebene über Ihrer Gruppe aktiviert sind.

Sie können dies weiter anpassen, indem Sie konfigurieren, welche Benachrichtigungen Sie erhalten. Sie können auch auswählen, ob Sie Benachrichtigungen bei Ereignissen oder in einer täglichen Digest-E-Mail erhalten möchten.

Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Wenn Sie einen Benachrichtigungstyp aktivieren und dann feststellen, dass Sie keine Benachrichtigungen dieses Typs erhalten, kann dies daran liegen, dass dieser Typ nicht für Ihre Rolle gilt.
>* Der [!DNL Workfront] oder ein Gruppenadministrator kann keine Benachrichtigungen für [!DNL Workfront Goals] konfigurieren. Weitere Informationen dazu, welche Benachrichtigungen der [!DNL Workfront]-Administrator konfigurieren kann, finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Weitere Informationen zum Konfigurieren von individuellen Benachrichtigungen für [!DNL Workfront Goals] finden Sie in diesem Artikel.
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-Mail-Benachrichtigungseinstellungen anzeigen und ändern

{{step1-click-profile-pic}}

1. Klicken Sie auf das **[!UICONTROL Mehr]**-Symbol ![Mehr](assets/more-icon.png) neben Ihrem Namen und dann auf **[!UICONTROL Bearbeiten]**.

1. Gehen Sie im **[!UICONTROL Person bearbeiten]** angezeigten Feld zum Abschnitt **[!UICONTROL Benachrichtigungen]**.

1. Klicken Sie auf eine Kategorie, um die Benachrichtigungseinstellungen anzuzeigen, die sich auf diese Kategorie beziehen.

   ![Meine Profilbenachrichtigungen](assets/my-profile-notifications.png)

1. Aktivieren oder deaktivieren Sie die Kontrollkästchen auf der rechten Seite, um anzugeben, ob Sie Benachrichtigungen täglich, sofort oder beides erhalten möchten.

   Sie können auch die Kontrollkästchen für eine Kategorie verwenden, um alle Benachrichtigungen in dieser Kategorie zu aktivieren oder zu deaktivieren.

   >[!NOTE]
   >
   >Wenn Sie Teammitglied für ein Projekt sind, erhalten Sie weiterhin E-Mail-Benachrichtigungen dafür, bis Sie aus dem Team entfernt werden, auch wenn Sie keinen Zugriff mehr auf das Projekt haben. Anweisungen zum Entfernen von Benutzern aus einem Team finden Sie unter [Entfernen von Benutzern aus Projekten](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Für die Kategorie **[!UICONTROL Kommunikation]** können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Um Benachrichtigungen in einer täglichen Zusammenfassung bereitzustellen, müssen Sie alle auswählen.

   Wenn alle E-Mail-Benachrichtigungen für eine bestimmte Kategorie aktiviert sind, wird das Feld im Kategorientitel als ausgewählt angezeigt. Wenn alle E-Mail-Benachrichtigungen in einer bestimmten Kategorie deaktiviert sind, wird das Kontrollkästchen deaktiviert. Wenn einige Benachrichtigungen aktiviert und andere deaktiviert sind, wird das Kategorie-Kontrollkästchen als gerade Linie angezeigt.\
   Wenn Sie eine Benachrichtigungseinstellung ändern, wird für diese Benachrichtigungseinstellung **[!UICONTROL Titel &quot;]**&quot; angezeigt, um Sie darüber zu informieren, dass diese Benachrichtigungseinstellung geändert wurde.

1. Wenn Sie Benachrichtigungen als tägliche Zusammenfassung gesendet haben, wählen Sie die Tageszeit, zu der Sie Benachrichtigungen erhalten möchten, oben im Abschnitt **[!UICONTROL Benachrichtigungen]** im Menü **[!UICONTROL Tägliche Zusammenfassung senden nach]** aus.

   ![Daily Digest - Tageszeit auswählen](assets/digest-time-stamp-my-settings-350x78.png)

   Die tägliche Zusammenfassung enthält Ereignisse, die den Kriterien der Benachrichtigungen 24 Stunden vor der ausgewählten Zeit entsprechen. Sie erhalten für jeden Benachrichtigungstyp eine tägliche Auswahl-E-Mail.\
   Die tägliche Zusammenfassung kann nach der von Ihnen ausgewählten Zeit eintreffen, je nachdem, wie viele E-Mails im System für den Versand in die Warteschlange gestellt werden. Die aufgelistete Zeit ist die Ortszeit, die in Ihren Browser-Einstellungen angegeben ist.

1. (Bedingt und optional) Wenn Sie die E-Mail-Benachrichtigungseinstellungen in der Vorschau -Umgebung ändern, aktivieren Sie die Einstellung **[!UICONTROL E-Mails von dieser Testumgebung empfangen]**, um E-Mails zu empfangen. E-Mails werden nicht automatisch aus der Vorschau-Umgebung generiert.

   ![E-Mails von Sandbox empfangen](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
