---
title: Benutzer deaktivieren oder reaktivieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Workfront-Administrator können Sie einen Benutzer deaktivieren oder reaktivieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Benutzer deaktivieren oder reaktivieren

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Deaktivieren eines Benutzers in der Adobe Admin Console finden Sie im Artikel unter &quot;Benutzer entfernen&quot; [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oder wenden Sie sich an Ihren Adobe Admin Console-Administrator.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Möglicherweise verlassen Ihre Benutzer die Organisation und Sie müssen sie möglicherweise aus Adobe Workfront entfernen. Sie sollten nicht im System aktiv bleiben, da dies für andere Benutzer Verwirrung stiften würde, wenn sie zu Aktualisierungen hinzugefügt oder sie zugewiesen werden. Wenn Sie einen Benutzer deaktivieren, sehen andere Benutzer seinen Namen nicht mehr, wenn sie nach Personen im System suchen.

Administratoren können inaktive Benutzer im Bereich Einrichtung anzeigen.

Sie können einen Benutzer jederzeit reaktivieren.

>[!IMPORTANT]
>
>Es wird empfohlen, Benutzer, die die Organisation verlassen haben, zu deaktivieren, anstatt sie zu löschen. Wenn ein Benutzer gelöscht wird, geht der gesamte mit diesem Benutzer verknüpfte Verlauf in Workfront verloren. Dazu gehören ihre Arbeitsaufgaben, ihre Verknüpfung mit Notizen, Stunden, Dokumenten und allen anderen Objekten, die sie einmal erstellt haben.
>
>Durch das Deaktivieren eines Benutzers in Workfront werden die Anwenderlizenzen für Workfront und Digital Testing entfernt. Darüber hinaus kann dem Benutzer keine Arbeit mehr zugewiesen werden. Wenn ein Benutzer deaktiviert wird, werden die Workfront-Lizenz und die Testlizenz dieses Benutzers für die Verwendung durch einen anderen Benutzer verfügbar. Alle anderen Informationen im Profil des deaktivierten Benutzers bleiben unverändert.
>
>Weitere Informationen zu den Auswirkungen des Löschens und der Deaktivierung von Benutzern finden Sie unter [Benutzer löschen](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzer-Admin</b> Optionen aktiviert unter <b>Einstellungen anpassen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Deaktivieren eines Benutzers

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol Mehr . ![](assets/more-icon.png)Klicken Sie auf **Deaktivieren**.

1. Klicken **Deaktivieren** in das Feld, das angezeigt wird.

## Planen von Benutzern für die Deaktivierung

Als Manager möchten Sie möglicherweise Benutzer zur Deaktivierung markieren, bevor sie Ihr Unternehmen tatsächlich verlassen. Wenn Sie z. B. mit einem Benutzer arbeiten, der vertraglich gebunden ist, befinden sich diese für einen begrenzten Zeitraum in Ihrem System und Sie kennen ihr Kündigungsdatum. Sie können die Deaktivierung an diesem Datum planen.

Workfront-Administratoren und Benutzer der Lizenzplanung können das Deaktivierungsdatum in ihrem Benutzerprofil sehen.

So planen Sie die Deaktivierung eines Benutzers:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Wählen Sie den Namen des Benutzers aus.

   Oder

   (Optional) Wählen Sie mehrere Benutzer aus, um sie für die Deaktivierung in großen Mengen zu planen.

1. Klicken Sie auf das Symbol Bearbeiten . ![](assets/edit-icon.png).
1. Klicken Sie im angezeigten Feld &quot;Benutzer bearbeiten&quot;auf **Ressourcenplanung** um in diese Gegend zu gehen.
1. Aktivieren Sie die **Deaktivierung planen** -Option.

1. Geben Sie im Kalender, der angezeigt wird, das Datum und die Uhrzeit für die **Geplantes Deaktivierungsdatum**.

   >[!NOTE]
   >
   >* Im Zeitfeld können Sie nur Zeitabstände (Ganzstundenabstände, keine Minuten) auswählen.
   >* Wenn Sie eine Uhrzeit für den aktuellen Tag auswählen, der vergangen ist, plant Workfront die Deaktivierung für den folgenden Tag um 12:00 Uhr. Die ausgewählte Zeit stimmt mit der Zeitzone des Computers überein, in dem der Benutzer die Deaktivierung plant.


1. Klicken **Änderungen speichern**.

   Der Benutzer wird am ausgewählten Tag manchmal nach der ausgewählten Zeit deaktiviert. Wenn Sie mehrere Benutzer ausgewählt haben, die stapelweise deaktiviert werden sollen, werden alle ausgewählten Benutzer am ausgewählten Tag deaktiviert, manchmal nach der ausgewählten Zeit.

Es wird empfohlen, einen Bericht für Benutzer zu erstellen, die für die Deaktivierung eingeplant sind, um Sie über die zukünftigen Deaktivierungen der Benutzer auf dem Laufenden zu halten. Es gibt keine Bestätigung, dass die Deaktivierung erfolgte, nachdem die Benutzer deaktiviert wurden.

## Benutzer erneut aktivieren

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol Mehr . ![](assets/more-icon.png)Klicken Sie auf **Aktivieren**.

1. Neu zuweisen **Zugriffsstufe** im Dropdown-Menü.

### Auswirkungen der Prüfung beim erneuten Aktivieren eines Benutzers

Deaktivierte Benutzer verlieren ihre zugewiesene standardmäßige Testing-Rolle und ihre Testversandlizenz (wenn Sie einen Workfront Premium Legacy Plan verwenden). Wenn Sie den Benutzer reaktivieren möchten, müssen Sie:

* Weisen Sie die Lizenz erneut zu (wenn Sie einen Workfront Premium Legacy Plan nutzen). Weitere Informationen zu Workfront-Testplänen finden Sie unter [Zugriff auf die Testversandfunktion in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Überprüfen Sie, ob sie die richtige Rolle für den Testversand haben. Benutzern mit aktiviertem Testversand werden die Standardeinstellungen zugewiesen, die für neue Benutzer als Testversand-Rolle festgelegt wurden. Siehe [Konfigurieren von standardmäßigen Testrollen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) für weitere Informationen.

## Informationen zum Deaktivieren von Workfront-Administratoren und zum Planen von Lizenzanwendern

Bevor Sie einen Workfront-Administrator oder einen Benutzer mit einer Planungslizenz deaktivieren, müssen Sie nach Workfront-Objekten und -Aktivitäten, an denen diese Person beteiligt ist, suchen und sie dann bei Bedarf einem anderen Workfront-Administrator oder Planen-Lizenzanwender zuordnen.

Diese Objekte und Aktivitäten können Folgendes umfassen:

* Dem Benutzer zugewiesene Aufgaben oder Probleme
* Projekte, die dem Benutzer gehören
* Berichte, die für die Ausführung mit den Zugriffsrechten des Benutzers eingerichtet sind
* Vorlagen, die dem Benutzer gehören
* Projekte und Vorlagen, für die der Benutzer als Ressourcen-Manager festgelegt wurde
* Routing-Regeln für Warteschlangen anfordern, für die der Workfront-Administrator oder Planlizenzbenutzer der Standardverantwortliche ist
* Genehmigungsprozesse mit einer Phase einschließlich des Benutzers (insbesondere wenn sie der einzige Genehmiger auf der Bühne waren)
* Timesheets, die den Benutzer als Genehmiger auflisten
* Datenblatt-Profile, die den Benutzer als Genehmiger auflisten
* Testen automatisierter Workflows mit dem Benutzer

## Auswirkungen der Ressourcenplanung bei der Planung der Deaktivierung eines Benutzers

Wenn Sie die Deaktivierung eines Benutzers planen, erscheinen diese nicht mehr im Ressourcen-Planer als für die Budgetplanung verfügbar. Wenn sie weiterhin Teil der Ressourcen-Pools sind, werden sie im Ressourcen-Planer angezeigt, ihre Verfügbarkeit wird jedoch auf null Stunden festgelegt, beginnend mit dem Datum der geplanten Deaktivierung.

Der Ressourcen-Planer berücksichtigt alle Aufgabenrollen der Benutzer und geplante Abschlussdaten der Aufgaben und berechnet die Ressourcen entsprechend.

Weitere Informationen zum Ressourcen-Planer finden Sie unter [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
