---
title: Deaktivieren oder Reaktivieren von Benutzern
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Workfront-Administrator können Sie Benutzende deaktivieren oder reaktivieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: bb6697241701160f878dc3fde2c7dd4d57ec097e
workflow-type: tm+mt
source-wordcount: '1105'
ht-degree: 0%

---

# Benutzer deaktivieren oder reaktivieren

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/de/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Wenn ein(e) Benutzende(r) das Unternehmen verlässt, müssen Sie ihn/sie möglicherweise aus Adobe Workfront entfernen. Sie sollten im System nicht aktiv bleiben, da dies für andere Benutzende Verwirrung stiften würde, wenn sie Aktualisierungen hinzufügen oder ihnen Arbeit zuweisen. Wenn Sie einen Benutzer deaktivieren, sehen andere Benutzer seinen Namen nicht mehr, wenn sie nach Personen im System suchen.

Admins sehen inaktive Benutzende im Bereich „Setup“.

Sie können einen Benutzer jederzeit reaktivieren.

>[!IMPORTANT]
>
>* Es wird empfohlen, Benutzer zu deaktivieren, die die Organisation verlassen haben, anstatt sie zu löschen. Wenn ein(e) Benutzende(r) gelöscht wird, geht der gesamte Verlauf in Workfront verloren, der diesem/r Benutzenden zugeordnet ist. Dazu gehören ihre Arbeitszuweisungen, ihre Zuordnung zu Notizen, Stunden, Dokumenten und allen anderen Objekten, die sie einmal erstellt haben.
>
>   Wenn Sie einen Benutzer in Workfront deaktivieren, werden die Lizenzen des Benutzers sowohl für Workfront als auch für das digitale Proofing entfernt. Darüber hinaus kann dem Benutzer keine Arbeit mehr zugewiesen werden. Wenn eine Benutzerin bzw. ein Benutzer deaktiviert wird, steht die Workfront-Lizenz und Proofing-Lizenz dieser Person zur Verwendung durch eine andere Person zur Verfügung. Alle anderen Informationen im Profil des deaktivierten Benutzers bleiben unverändert.
>
>   Weitere Informationen über die Auswirkungen des Löschens und der Deaktivierung von Benutzern finden Sie unter [Benutzer löschen](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).
>
>* Wenn Sie einen Benutzer in Workfront deaktivieren, wird er nicht aus dem Workfront-Produktprofil in Adobe Admin Console entfernt.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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

## Voraussetzungen

Bevor Sie einen Workfront-Administrator oder einen Standard- oder Plan-Lizenzbenutzer deaktivieren, müssen Sie dessen Objekte und Aktivitäten mit einem anderen Benutzer verknüpfen.

Weitere Informationen finden Sie unter [Informationen zum Deaktivieren von Workfront-Administratoren und Plan](#about-deactivating-workfront-administrators-and-plan-license-users)Lizenzanwendern in diesem Artikel.

## Deaktivieren von Benutzern

Beachten Sie beim Deaktivieren von Benutzern Folgendes:

* Der/die Benutzende kann nicht auf das System zugreifen.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Alle mit dem Benutzer verknüpften Daten werden beibehalten.
* Sie können die Lizenz eines deaktivierten Benutzers einem anderen Benutzer zuweisen.

So deaktivieren Sie einen Benutzer:

{{step-1-to-users}}

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol **Mehr** ![Mehr](assets/more-icon.png) und klicken Sie dann auf **Deaktivieren**.

1. Klicken **in** angezeigten Feld auf „Deaktivieren“.

## Planen von Benutzern für die Deaktivierung

Als Manager sollten Sie Benutzer zur Deaktivierung markieren, bevor sie Ihr Unternehmen tatsächlich verlassen. Wenn Sie beispielsweise mit einem vertraglich gebundenen Nutzer arbeiten, der sich für eine begrenzte Zeit in Ihrem System befindet und dessen Kündigungsdatum bekannt ist. Sie können planen, dass sie an diesem Datum deaktiviert werden.

Workfront-Administratoren und Benutzende mit Planlizenzen können das Deaktivierungsdatum in ihrem Benutzerprofil sehen.

So planen Sie die Deaktivierung eines Benutzers:

{{step-1-to-users}}

1. Wählen Sie den Namen des Benutzers aus.

   Oder

   (Optional) Wählen Sie mehrere Benutzer aus, um sie für die Massendeaktivierung zu planen.

1. Klicken Sie auf das Symbol Bearbeiten ![Symbol Bearbeiten](assets/edit-icon.png).
1. Klicken Sie im angezeigten Feld „Benutzer bearbeiten“ auf **Ressourcenplanung**, um zu diesem Bereich zu wechseln.
1. Aktivieren Sie die **Deaktivierung planen**.

1. Geben Sie in dem angezeigten Kalender das Datum und die Uhrzeit für das Datum **Geplantes Deaktivierungsdatum“**.

   >[!NOTE]
   >
   >* Im Zeitfeld können Sie nur Ganzstundenschritte und nicht Minuten auswählen.
   >* Wenn Sie eine Uhrzeit für den aktuellen Tag auswählen, der vergangen ist, plant Workfront die Deaktivierung für den folgenden Tag um 00:00 Uhr. Die ausgewählte Zeit entspricht der Zeitzone des Computers des Benutzers, der die Deaktivierung plant.

1. Klicken Sie auf **Änderungen speichern**.

   Der Benutzer wird am ausgewählten Tag irgendwann nach der ausgewählten Zeit deaktiviert. Wenn Sie mehrere Benutzer ausgewählt haben, die stapelweise deaktiviert werden sollen, werden alle ausgewählten Benutzer am ausgewählten Tag irgendwann nach der ausgewählten Zeit deaktiviert.

Es wird empfohlen, einen Bericht für Benutzer zu erstellen, für die Sie die Deaktivierung geplant haben, um über bevorstehende Deaktivierungen von Benutzern auf dem Laufenden zu bleiben. Es gibt keine Bestätigung, dass die Deaktivierung stattgefunden hat, nachdem die Benutzer deaktiviert wurden.

## Benutzer reaktivieren

{{step-1-to-users}}

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol Mehr ![Mehr](assets/more-icon.png) und dann auf **Aktivieren**.

1. Weisen Sie **Dropdown-Menü eine neue Zugriffsebene** und klicken Sie dann auf **Reaktivieren**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Auswirkungen des Proofings bei der Reaktivierung eines Benutzers

Deaktivierte Benutzende verlieren ihre zugewiesene Standard-Proofing-Rolle und ihre Proofing-Lizenz (wenn Sie einen veralteten Workfront Premium-Plan verwenden). Wenn Sie den Benutzer erneut aktivieren möchten, müssen Sie:

* Weisen Sie die Lizenz neu zu (wenn Sie einen alten Workfront Premium-Plan verwenden). Weitere Informationen zu Workfront-Proofing-Plänen finden Sie unter [Zugriff auf die Proofing-Funktionalität in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Stellen Sie sicher, dass sie die richtige Korrekturabzugsrolle haben. Reaktivierte Korrekturabzugsbenutzende erhalten die Rolle, die als Standard-Korrekturabzugsrolle für neue Benutzende festgelegt ist. Weitere Informationen [ Sie unter „Konfigurieren ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) Proofing-Standardrollen“.

## Informationen zur Deaktivierung von Workfront-Administratoren und Benutzern von Standard- oder Planlizenzen

Bevor Sie einen Workfront-Administrator oder eine Benutzerin bzw. einen Benutzer mit einer Planlizenz deaktivieren, müssen Sie nach Workfront-Objekten und -Aktivitäten suchen, an denen diese Person beteiligt ist, und sie dann ggf. einem anderen Workfront-Administrator oder einer Person mit einer Planlizenz zuordnen.

Diese Objekte und Aktivitäten können Folgendes umfassen:

* Dem Benutzer zugewiesene Aufgaben oder Probleme
* Projekte im Besitz des Benutzers
* Für die Ausführung mit den Zugriffsrechten des Benutzers eingerichtete Berichte
* Vorlagen, die dem Benutzer gehören
* Projekte und Vorlagen, für die der Benutzer als Ressourcenmanager festgelegt wurde
* Routingregeln für Anforderungswarteschlangen, für die der Workfront-Administrator oder Plan-Lizenzbenutzer der standardmäßige Bearbeiter ist
* Genehmigungsprozesse, die über eine Phase verfügen, in der der Benutzer eingeschlossen ist (insbesondere wenn er die einzige genehmigende Person auf der Phase war)
* Arbeitszeittabellen, in denen der Benutzer als genehmigende Person aufgeführt ist
* Arbeitszeittabellen-Profile, in denen der Benutzer als genehmigende Person aufgeführt ist
* Proofing automatisierter Workflows, die den Benutzer enthalten

## Auswirkung auf die Ressourcenplanung bei der Planung einer Benutzerdeaktivierung

Wenn Sie einen Benutzer für die Deaktivierung planen, werden diese im Ressourcenplaner nicht mehr als für die Budgetierung von Stunden verfügbar angezeigt. Wenn sie Teil der Ressourcenpools bleiben, werden sie im Ressourcenplaner angezeigt, ihre Verfügbarkeit wird jedoch auf null Stunden ab dem Datum ihrer geplanten Deaktivierung eingestellt.

Der Ressourcenplaner berücksichtigt alle Aufgabengebiete der Benutzer und die geplanten Abschlussdaten der Aufgaben und berechnet die Ressourcen entsprechend.

Weitere Informationen zum Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
