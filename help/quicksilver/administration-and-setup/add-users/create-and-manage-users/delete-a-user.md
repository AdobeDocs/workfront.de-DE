---
title: Benutzer löschen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Wenn ein(e) Benutzende(r) Ihre Organisation verlässt, kann er/sie diesen Benutzenden aus Workfront entfernen. Wir empfehlen jedoch, Benutzende zu deaktivieren, anstatt sie zu löschen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Benutzer löschen

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht auf der Adobe Business Platform integriert haben. Wenn Sie das Onboarding für die Adobe-Geschäftsplattform abgeschlossen haben, müssen Sie Benutzende in der Adobe Admin Console löschen.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen die Adobe-Geschäftsplattform eingeführt hat, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Wenn ein(e) Benutzende(r) Ihre Organisation verlässt, können Sie diesen/diese Benutzende aus Adobe Workfront entfernen.

>[!IMPORTANT]
>
>Beim Löschen eines Benutzers aus dem System werden auch mit dem Benutzer verknüpfte Informationen gelöscht, die Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
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

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen oder Deaktivieren von Benutzern

Wenn Sie einen Benutzer deaktivieren, passiert Folgendes:

* Entfernt die Benutzerlizenzen für Workfront und Workfront Proof, wenn die Workfront Proof-Komponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zu Workfront Proof finden Sie unter [Workfront Proof: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für Benutzende freigegeben werden.
* Ihre Zuordnung zu den folgenden Objekten bleibt intakt:

   * Aufgaben, Probleme, Projekte, Portfolios
   * Dashboards

     >[!NOTE]
     >
     >Wenn Sie einen Benutzer deaktivieren und die mit einem Benutzer verknüpften Berichte oder Dashboards nicht mehr anzeigen können, müssen Sie möglicherweise das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** aktualisieren.\
     >Weitere Informationen finden Sie unter [Warum kann ich nicht auf einen Bericht zugreifen, der einem deaktivierten Benutzer gehört?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) Abschnitt des Artikels [Häufig gestellte Fragen zu Berichten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) .

   * Dokumente
   * Updates
   * Stunden

* Wenn der Benutzer Dokumente ausgecheckt hat, bleiben die Dokumente ausgecheckt, sobald Sie sie deaktivieren. Nur ein Workfront-Administrator kann sie wieder einchecken. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

Beim Löschen eines Benutzers passiert Folgendes:

* Entfernt die Benutzerlizenzen für Workfront und Workfront Proof, wenn die Workfront Proof-Komponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zu Workfront Proof finden Sie unter [Workfront Proof: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für Benutzende freigegeben werden.
* Löscht die Verknüpfung dieses Benutzers mit den folgenden Objekten:

   * Aufgaben, Probleme, Projekte, Portfolio
   * Dashboards

     >[!NOTE]
     >
     >Sie verlieren auch den Zugriff auf benutzerdefinierte Abschnitte, die Dashboards enthalten, die mit dem gelöschten Benutzer verknüpft sind.\
     >Weitere Informationen finden Sie unter [Wie greife ich auf ein Dashboard zu, das einen Bericht eines gelöschten Benutzers enthält?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) Abschnitt des Artikels [Häufig gestellte Fragen zu Berichten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) .

   * Updates
   * Stunden

     >[!NOTE]
     >
     >Diese Objekte verbleiben in Workfront, aber der Eigentümer des Objekts ist jetzt leer.

* Wenn der Benutzer Dokumente unter dem Bereich Dokumente in der globalen Navigationsleiste hochgeladen hat, werden die Dokumente ebenfalls gelöscht.
* Wenn der/die Benutzende Dokumente ausgecheckt hat, deren Inhaber er/sie ist, und die Dokumente im Hauptdokumentenbereich hochgeladen wurden (der Zugriff erfolgt über das Hauptmenü), werden die Dokumente mit dem/der Benutzenden gelöscht. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

Weitere Informationen zum Deaktivieren von Benutzern finden Sie unter [Deaktivieren oder Reaktivieren von Benutzern](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Sie können Benutzer einzeln oder mehrere Benutzer gleichzeitig dauerhaft löschen. Wenn Sie einzelne Benutzer löschen, müssen Sie warten, bis der Löschvorgang abgeschlossen ist, bevor Sie zu anderen Aktivitäten in Workfront wechseln. Der Prozess des Löschens mehrerer Benutzer gleichzeitig wird als Hintergrundprozess ausgeführt, sodass Sie Workfront weiterhin verwenden können, während die Benutzer gelöscht werden.

## Löschen eines oder mehrerer Benutzer

{{step-1-to-users}}

1. Wählen Sie mindestens einen zu löschenden Benutzer aus, klicken Sie auf die ![](assets/more-icon.png) Mehr und anschließend auf **Löschen**.
1. Klicken Sie im angezeigten Feld auf **Löschen**, um den Löschvorgang zu bestätigen.

   Der Prozess zum Löschen von Benutzenden wird als Hintergrundprozess ausgeführt, sodass Sie Workfront weiter verwenden können, wenn die Benutzenden gelöscht werden.

   Je nach der Anzahl der Benutzer, die Sie löschen möchten, kann der Vorgang mehrere Minuten oder sogar einige Stunden dauern.

   Nachdem Sie in Workfront die Bestätigung erhalten haben, dass die Benutzer gelöscht wurden, werden sie möglicherweise weiterhin im System angezeigt, bis der Löschvorgang im Hintergrund abgeschlossen ist.

   Wenn Sie zu einem späteren Zeitpunkt feststellen, dass ein oder mehrere Benutzer nicht erfolgreich gelöscht wurden, versuchen Sie, sie einzeln zu löschen.
