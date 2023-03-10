---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagging anderer Benutzer auf Updates
description: Wenn Sie Aktualisierungskommentare für ein Adobe Workfront-Objekt bereitstellen, können alle Benutzer des Projekts die übermittelten Informationen sehen. Es kann jedoch vorkommen, dass Benutzer, die nicht am Projekt teilnehmen, von der Anzeige dieser Informationen profitieren. Anstatt diese Benutzer in das Projekt aufzunehmen, können Sie sie in der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Tagging-Benutzer erhalten eine Ereignisbenachrichtigung.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 1eba586f4d3ce6db667839b0620dfeb65f6e28be
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Tagging anderer Benutzer auf Updates

Wenn Sie Aktualisierungskommentare für ein Adobe Workfront-Objekt bereitstellen, können alle Benutzer des Projekts die übermittelten Informationen sehen. Es kann jedoch vorkommen, dass Benutzer, die nicht am Projekt teilnehmen, von der Anzeige dieser Informationen profitieren. Anstatt diese Benutzer in das Projekt aufzunehmen, können Sie sie in der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Tagging-Benutzer erhalten eine Ereignisbenachrichtigung.

>[!NOTE]
>
>Eine Ereignisbenachrichtigung muss aktiviert sein, damit ein Benutzer sie empfangen kann. Administratoren können Benachrichtigungen für das gesamte System oder für eine Gruppe der obersten Ebene aktivieren. Ein Benutzer kann auch individuelle Ereignisbenachrichtigungen in seinem eigenen Benutzerprofil aktivieren und deaktivieren. Weitere Informationen finden Sie unter folgenden Themen:
>
>* [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


>[!NOTE]
>
>Wenn ein Problem in ein Projekt oder eine Aufgabe konvertiert wird, werden die Aktualisierungen in das neue Projekt oder die neue Aufgabe kopiert, die getaggten Benutzer jedoch nicht. Um das Gespräch fortzusetzen, müssen Sie die Teilnehmer erneut taggen.

Informationen zum Hinzufügen von Aktualisierungen zu Workfront-Objekten finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anfrage oder höher für Probleme und Dokumente; Überprüfen oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Anforderer oder höher für Probleme und Dokumente; Für alle anderen Objekte validieren oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Tagging anderer Benutzer auf Updates

1. Aktualisieren Sie ein Arbeitselement, wie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Im **Benachrichtigen** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie einbeziehen möchten, und auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   Oder

   Geben Sie das @-Symbol in die **Neue Aktualisierung starten** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie in die Aktualisierung aufnehmen möchten, und dann auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Um den richtigen Benutzer zu identifizieren, wenn es Benutzer mit ähnlichen oder identischen Namen gibt, beachten Sie den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Taggen in einer Aktualisierung angezeigt werden können.

   ![](assets/tag-users-in-update.png)

1. (Optional) Um die Aktualisierung privat zu machen, aktivieren Sie **Privatperson in meinem Unternehmen** in der rechten unteren Ecke des Aktualisierungsfelds. Dadurch wird die Aktualisierung nur für Benutzer in Ihrem Unternehmen sichtbar.

   >[!NOTE]
   >
   >Mit Tags versehene Benutzer außerhalb des Unternehmens können weiterhin eine In-App-Benachrichtigung oder E-Mail erhalten, auch wenn sie die privaten Kommentare nicht auf der Registerkarte Updates sehen. Es wird empfohlen, externe Benutzer bei einer Aktualisierung nicht mit Tags zu versehen, wenn Sie die Informationen nicht für sie freigeben möchten.

1. (Optional) Wiederholen Sie Schritt 2, um mehrere Benutzer und Teams hinzuzufügen.

   >[!NOTE]
   >
   >Alle im Feld Benachrichtigung aufgeführten Benutzer und Teammitglieder erhalten eine In-App-Benachrichtigung zu der Aktualisierung und erhalten je nach Konfiguration ihrer E-Mail-Benachrichtigungseinstellungen eine E-Mail. Benutzer, die sich in einem Kommentar oder einer Antwort mit Tags versehen, erhalten eine Benachrichtigung zu diesem Kommentar oder dieser Antwort und können ihren Namen für den Rest des Threads im Feld Benachrichtigen anzeigen. Sie erhalten jedoch keine weitere Benachrichtigung, es sei denn, sie taggen sich selbst. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) und [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicken **Aktualisieren**.\
   Benutzer, die in der Aktualisierung enthalten sind, erhalten automatisch die Berechtigung zum Anzeigen des Objekts und können Aktualisierungen anzeigen und auf diese reagieren.

   Oben im Aktualisierungs-Thread können Sie sehen, wer in jeder Antwort getaggt wurde. Diese Benutzer erhalten zusammen mit allen Benutzern, die das Objekt abonniert haben, eine Benachrichtigung, sobald ein Objekt aktualisiert oder beantwortet wird.

   ![](assets/tagging-transparency-350x192.png)

   Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
