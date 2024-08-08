---
title: Deaktivieren oder Reaktivieren eines Benutzers
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Workfront-Administrator können Sie einen Benutzer deaktivieren oder reaktivieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 0%

---

# Benutzer deaktivieren oder reaktivieren

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Wenn ein Benutzer die Organisation verlässt, müssen Sie ihn möglicherweise aus Adobe Workfront entfernen. Sie sollten nicht im System aktiv bleiben, da dies für andere Benutzer Verwirrung stiften würde, wenn sie zu Aktualisierungen hinzugefügt oder sie zugewiesen werden. Wenn Sie einen Benutzer deaktivieren, sehen andere Benutzer seinen Namen nicht mehr, wenn sie nach Personen im System suchen.

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td>  <p>Neu: Standard </p> <p>Oder </p><p>Aktuell: Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs eines Benutzers</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsebene, die für den Zugriff auf <b>Bearbeiten</b> konfiguriert ist, wobei <b>Erstellen</b> und mindestens eine der beiden Optionen <b>Benutzeradministrator</b> unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png"> aktiviert sind. </p> <p>Wenn von diesen beiden Optionen Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zur Einstellung <b>Benutzer</b> in einer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Voraussetzungen

Bevor Sie einen Workfront-Administrator oder einen Standard- oder Planen-Lizenzbenutzer deaktivieren, müssen Sie dessen Objekte und Aktivitäten mit einem anderen Benutzer verknüpfen.

Weitere Informationen finden Sie unter [Über das Deaktivieren von Workfront-Administratoren und das Planen von Lizenzanwendern](#about-deactivating-workfront-administrators-and-plan-license-users) in diesem Artikel.

## Deaktivieren eines Benutzers

Beachten Sie beim Deaktivieren eines Benutzers Folgendes:

* Der Benutzer kann nicht auf das System zugreifen.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Alle mit dem Benutzer verknüpften Daten werden beibehalten.
* Sie können die Lizenz eines deaktivierten Benutzers einem anderen Benutzer zuweisen.

So deaktivieren Sie einen Benutzer:

{{step-1-to-users}}

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol **Mehr** ![](assets/more-icon.png) und dann auf **Deaktivieren**.

1. Klicken Sie in dem angezeigten Feld auf **Deaktivieren** .

## Planen von Benutzern für die Deaktivierung

Als Manager können Sie Benutzer zur Deaktivierung markieren, bevor sie Ihr Unternehmen verlassen. Wenn Sie z. B. mit einem Benutzer arbeiten, der vertraglich gebunden ist, befinden sich diese für einen begrenzten Zeitraum in Ihrem System und Sie kennen ihr Kündigungsdatum. Sie können die Deaktivierung an diesem Datum planen.

Workfront-Administratoren und Benutzer der Lizenzplanung können das Deaktivierungsdatum in ihrem Benutzerprofil sehen.

So planen Sie die Deaktivierung eines Benutzers:

{{step-1-to-users}}

1. Wählen Sie den Namen des Benutzers aus.

   Oder

   (Optional) Wählen Sie mehrere Benutzer aus, um sie für die Deaktivierung in großen Mengen zu planen.

1. Klicken Sie auf das Bearbeitungssymbol ![](assets/edit-icon.png).
1. Klicken Sie im angezeigten Feld &quot;Benutzer bearbeiten&quot;auf **Ressourcenplanung** , um zu diesem Bereich zu wechseln.
1. Aktivieren Sie die Option **Deaktivierung planen** .

1. Geben Sie im Kalender, der angezeigt wird, das Datum und die Uhrzeit für das **Geplante Deaktivierungsdatum** an.

   >[!NOTE]
   >
   >* Im Zeitfeld können Sie nur Zeitabstände (Ganzstundenabstände, keine Minuten) auswählen.
   >* Wenn Sie eine Uhrzeit für den aktuellen Tag auswählen, der vergangen ist, plant Workfront die Deaktivierung für den folgenden Tag um 12:00 Uhr. Die ausgewählte Zeit stimmt mit der Zeitzone des Computers überein, in dem der Benutzer die Deaktivierung plant.

1. Klicken Sie auf **Änderungen speichern**.

   Der Benutzer wird am ausgewählten Tag nach der ausgewählten Zeit deaktiviert. Wenn Sie mehrere Benutzer ausgewählt haben, die stapelweise deaktiviert werden sollen, werden alle ausgewählten Benutzer am ausgewählten Tag nach der ausgewählten Zeit deaktiviert.

Es wird empfohlen, einen Bericht für Benutzer zu erstellen, die für die Deaktivierung eingeplant sind, um Sie über die zukünftigen Deaktivierungen der Benutzer auf dem Laufenden zu halten. Es gibt keine Bestätigung, dass die Deaktivierung erfolgte, nachdem die Benutzer deaktiviert wurden.

## Benutzer erneut aktivieren

{{step-1-to-users}}

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol &quot;Mehr&quot;![](assets/more-icon.png) und dann auf **Aktivieren**.

1. Weisen Sie im Dropdown-Menü eine neue **Zugriffsebene** zu und klicken Sie dann auf **Reactivate** .
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Auswirkungen der Prüfung bei der Reaktivierung eines Benutzers

Deaktivierte Benutzer verlieren ihre zugewiesene standardmäßige Testing-Rolle und ihre Testversandlizenz (wenn Sie einen Workfront Premium Legacy Plan verwenden). Wenn Sie den Benutzer reaktivieren möchten, müssen Sie:

* Weisen Sie die Lizenz erneut zu (wenn Sie einen Workfront Premium Legacy Plan nutzen). Weitere Informationen zu Workfront-Testplänen finden Sie unter [Zugriff auf die Testfunktion in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Überprüfen Sie, ob sie die richtige Rolle für den Testversand haben. Benutzern mit aktiviertem Testversand werden die Standardeinstellungen zugewiesen, die für neue Benutzer als Testversand-Rolle festgelegt wurden. Weitere Informationen finden Sie unter [Konfigurieren von standardmäßigen Testing-Rollen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) .

## Über das Deaktivieren von Workfront-Administratoren und Standard- oder Planen von Lizenzbenutzern

Bevor Sie einen Workfront-Administrator oder einen Benutzer mit einer Planungslizenz deaktivieren, müssen Sie nach Workfront-Objekten und -Aktivitäten, an denen diese Person beteiligt ist, suchen und sie dann bei Bedarf einem anderen Workfront-Administrator oder Planen-Lizenzanwender zuordnen.

Diese Objekte und Aktivitäten können Folgendes umfassen:

* Dem Benutzer zugewiesene Aufgaben oder Probleme
* Projekte, die dem Benutzer gehören
* Berichte, die mit den Zugriffsrechten des Benutzers ausgeführt werden
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

Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
