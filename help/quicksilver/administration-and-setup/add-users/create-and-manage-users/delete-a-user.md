---
title: Benutzer löschen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Wenn ein Benutzer Ihre Organisation verlässt, kann ihn aus Workfront entfernen. Wir empfehlen jedoch, Benutzer zu deaktivieren, anstatt sie zu löschen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: b3717fc89e45983b80471fdd629c79b82086c6ff
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Benutzer löschen

Wenn ein Benutzer Ihre Organisation verlässt, können Sie ihn aus Adobe Workfront entfernen.

>[!IMPORTANT]
>
>Durch das Löschen eines Benutzers aus dem System werden auch Informationen gelöscht, die mit dem Benutzer verknüpft sind, den Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter [Benutzer deaktivieren oder reaktivieren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzeradministrator</b> Optionen aktiviert unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Löschen oder Deaktivieren eines Benutzers

Das Deaktivieren eines Benutzers bewirkt Folgendes:

* Entfernt die Lizenzen des Benutzers für Workfront- und Workfront-Testsendungen, wenn die Workfront-Testkomponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zum Workfront-Testversand finden Sie unter [Workfront-Testversand: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für den Benutzer freigegeben werden.
* Ihre Verknüpfung mit den folgenden Objekten bleibt intakt:

   * Aufgaben, Probleme, Projekte, Portfolios
   * Dashboards

     >[!NOTE]
     >
     >Wenn Sie einen Benutzer deaktivieren und die mit einem Benutzer verknüpften Berichte oder Dashboards nicht mehr anzeigen können, müssen Sie möglicherweise die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld.\
     >Weitere Informationen finden Sie unter [Warum kann ich nicht auf einen Bericht zugreifen, der einem deaktivierten Benutzer gehört?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) Abschnitt [Häufig gestellte Fragen zu Berichten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) Artikel.

   * Dokumente
   * Updates
   * Stunden

* Wenn der Benutzer ausgecheckte Dokumente hat, bleiben die Dokumente bei der Deaktivierung ausgecheckt. Nur ein Workfront-Administrator kann sie wieder einchecken. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Dokumente auschecken](../../../documents/managing-documents/check-out-documents.md).

Das Löschen eines Benutzers bewirkt Folgendes:

* Entfernt die Lizenzen des Benutzers für Workfront und Workfront Testversand, wenn die Workfront-Testkomponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zum Workfront-Testversand finden Sie unter [Workfront-Testversand: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für den Benutzer freigegeben werden.
* Löscht die Zuordnung dieses Benutzers zu den folgenden Objekten:

   * Aufgaben, Probleme, Projekte, Portfolio
   * Dashboards

     >[!NOTE]
     >
     >Außerdem verlieren Sie den Zugriff auf benutzerdefinierte Abschnitte, die Dashboards enthielten, die dem gelöschten Benutzer zugeordnet waren.\
     >Weitere Informationen finden Sie unter [Wie greife ich auf ein Dashboard zu, das einen Bericht eines gelöschten Benutzers enthält?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) Abschnitt [Häufig gestellte Fragen zu Berichten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) Artikel.

   * Updates
   * Stunden

     >[!NOTE]
     >
     >Diese Objekte verbleiben in Workfront, aber der Eigentümer des Objekts ist jetzt leer.

* Wenn der Benutzer Dokumente im Bereich &quot;Dokumente&quot;in der Leiste &quot;Globale Navigation&quot;hochgeladen hat, werden die Dokumente ebenfalls gelöscht.
* Wenn der Benutzer Dokumente ausgecheckt hat, deren Inhaber er ist, und die Dokumente in den Hauptbereich &quot;Dokumente&quot;hochgeladen werden (Zugriff erfolgt über das Hauptmenü), werden die Dokumente mit dem Benutzer gelöscht. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Dokumente auschecken](../../../documents/managing-documents/check-out-documents.md).

Weitere Informationen zum Deaktivieren von Benutzern finden Sie unter [Benutzer deaktivieren oder reaktivieren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Sie können Benutzer einzeln löschen oder mehrere Benutzer gleichzeitig dauerhaft löschen. Wenn Sie einzelne Benutzer löschen, müssen Sie warten, bis der Löschvorgang abgeschlossen ist, bevor Sie zu anderen Aktivitäten in Workfront wechseln. Das Löschen mehrerer Benutzer gleichzeitig wird als Hintergrundprozess ausgeführt, sodass Sie Workfront weiterhin verwenden können, wenn die Benutzer gelöscht werden.

## Löschen eines oder mehrerer Benutzer

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicks **Benutzer**.
1. Wählen Sie mindestens einen Benutzer aus, den Sie löschen möchten, und klicken Sie auf das Menü Mehr . ![](assets/more-icon.png)Klicken Sie auf **Löschen**.
1. Klicken Sie im angezeigten Feld auf **Löschen** , um den Löschvorgang zu bestätigen.

   Der Prozess zum Löschen von Benutzern wird als Hintergrundprozess ausgeführt, sodass Sie Workfront weiterhin verwenden können, wenn Benutzer gelöscht werden.

   Je nach der Anzahl der Benutzer, die Sie löschen, kann der Prozess mehrere Minuten oder sogar einige Stunden dauern.

   Nachdem Sie in Workfront bestätigt haben, dass die Benutzer gelöscht wurden, werden sie möglicherweise weiterhin im System angezeigt, bis der Löschvorgang im Hintergrund abgeschlossen ist.

   Wenn Sie zu einem späteren Zeitpunkt feststellen, dass ein oder mehrere Benutzer nicht erfolgreich gelöscht wurden, versuchen Sie, sie einzeln zu löschen.
