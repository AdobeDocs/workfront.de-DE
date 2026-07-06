---
title: Deaktivieren oder Reaktivieren von Benutzern
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront-Administratoren können Benutzende deaktivieren oder reaktivieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zHLRYheTPbZUMzGm93gmS4iL-tbYlV9x3a0rWJq1ozo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c091cec41c202b4684d243014bd0a8ef08a92836
workflow-type: tm+mt
source-wordcount: 1090
ht-degree: 6%

---

# Deaktivieren oder Reaktivieren einer Person {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="Deaktivieren einer Person"
>abstract="Durch das Deaktivieren von Benutzenden werden diese aus Workfront und Frame.io entfernt. Deaktivierte Benutzende können später wieder aktiviert werden."

<!--Audited 5/2025-->

Wenn ein(e) Benutzende(r) das Unternehmen verlässt, wird empfohlen, ihn/sie im System zu deaktivieren, um zu vermeiden, dass andere(r) Benutzende(r) verwirrt wird, wenn er/sie Aktualisierungen hinzufügt oder ihnen Arbeit zuweist. Wenn Sie einen Benutzer deaktivieren, sehen andere Benutzer seinen Namen nicht mehr, wenn sie nach Personen im System suchen.

Admins sehen inaktive Benutzende im Bereich „Setup“.

Sie können einen Benutzer jederzeit reaktivieren.

>[!IMPORTANT]
>
>* Es wird empfohlen, Benutzer zu deaktivieren, die die Organisation verlassen haben, anstatt sie zu löschen. Wenn ein(e) Benutzende(r) gelöscht wird, geht der gesamte Verlauf in Workfront verloren, der diesem/r Benutzenden zugeordnet ist. Dazu gehören ihre Arbeitszuweisungen, ihre Zuordnung zu Notizen, Stunden, Dokumenten und allen anderen Objekten, die sie einmal erstellt haben.
>
>* Wenn Sie einen Benutzer in Workfront deaktivieren, werden die Lizenzen des Benutzers sowohl für Workfront als auch für das digitale Proofing entfernt. Darüber hinaus kann dem Benutzer keine Arbeit mehr zugewiesen werden. Wenn eine Benutzerin bzw. ein Benutzer deaktiviert wird, steht die Workfront-Lizenz und Proofing-Lizenz dieser Person zur Verwendung durch eine andere Person zur Verfügung. Alle anderen Informationen im Profil des deaktivierten Benutzers bleiben unverändert.
>
>* Wenn Sie einen Benutzer in Workfront deaktivieren, wird er nicht aus dem Workfront-Produktprofil in Adobe Admin Console entfernt. Weitere Informationen finden Sie unter [Benutzer löschen](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).
>
>* Wenn sich ein(e) Benutzende(r) in einer oder mehreren Admin Console-Benutzergruppen befindet und das Produktprofil zu einer oder mehreren dieser Benutzergruppen hinzugefügt wurde, werden diese Benutzenden nicht tatsächlich aus dem Produkt entfernt, wenn Sie sie aus Workfront deaktivieren. Der/die Benutzende muss/müssen aus den Benutzergruppen in Admin Console entfernt werden.


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Bevor Sie einen Workfront-Administrator oder einen Standard- oder Plan-Lizenzbenutzer deaktivieren, müssen Sie dessen Objekte und Aktivitäten mit einem anderen Benutzer verknüpfen.

Weitere Informationen finden Sie unter [Informationen zum Deaktivieren von Workfront-Administratoren und Standard- oder Plan](#about-deactivating-workfront-administrators-and-plan-license-users)Lizenzbenutzern in diesem Artikel.

## Deaktivieren einer Person

Beachten Sie beim Deaktivieren von Benutzern Folgendes:

* Der/die Benutzende kann nicht auf das System zugreifen.
<!--
* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.
   -->
* Alle mit dem Benutzer verknüpften Daten werden beibehalten.
* Sie können die Lizenz eines deaktivierten Benutzers einem anderen Benutzer zuweisen.

So deaktivieren Sie einen Benutzer:

{{step-1-to-users}}

1. Wählen Sie einen Benutzer in der Benutzerliste aus.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol](assets/more-icon.png) und dann auf **Deaktivieren**.

1. Klicken Sie **Dialogfeld** Benutzer deaktivieren **auf**.

## Planen von Benutzern für die Deaktivierung

Als Manager sollten Sie Benutzer zur Deaktivierung markieren, bevor sie Ihr Unternehmen tatsächlich verlassen. Wenn Sie beispielsweise mit einem vertraglich gebundenen Benutzer arbeiten, der sich für eine begrenzte Zeit in Ihrem System befindet und dessen Kündigungsdatum bekannt ist. Sie können planen, dass sie an diesem Datum deaktiviert werden.

Workfront-Administratoren und Benutzende mit Planlizenzen können das Deaktivierungsdatum in ihrem Benutzerprofil sehen.

So planen Sie die Deaktivierung eines Benutzers:

{{step-1-to-users}}

1. Wählen Sie den Benutzer in der Benutzerliste aus.

   ODER

   (Optional) Wählen Sie mehrere Benutzer aus, um sie für die Massendeaktivierung zu planen.

1. Klicken Sie auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).
1. Klicken Sie im linken Bereich des Felds **Benutzer bearbeiten** auf **Ressourcenplanung**.
1. Klicken Sie **Deaktivierungsdatum festlegen**.

1. Wählen Sie das Datum für das **Deaktivierungsdatum** aus.

   >[!NOTE]
   >
   >* Das ausgewählte Datum entspricht der Zeitzone des Computers des Benutzers, der die Deaktivierung plant.

1. Klicken Sie auf **Speichern**.

Der Benutzer wird um 12:00 :00 am ausgewählten Datum deaktiviert. Wenn Sie mehrere Benutzer ausgewählt haben, die stapelweise deaktiviert werden sollen, werden alle ausgewählten Benutzer am ausgewählten Datum :00 12 Uhr morgens deaktiviert.

Es wird empfohlen, einen Bericht für Benutzer zu erstellen, für die Sie die Deaktivierung geplant haben, um über bevorstehende Deaktivierungen von Benutzern auf dem Laufenden zu bleiben. Es gibt keine Bestätigung, dass die Deaktivierung erfolgt ist, nachdem die Benutzer deaktiviert wurden.

## Benutzer reaktivieren

{{step-1-to-users}}

1. Wählen Sie einen Benutzer aus, klicken Sie auf das Symbol **Mehr** ![Mehr](assets/more-icon.png) und klicken Sie dann auf **Aktivieren**.

1. Wählen **Dialogfeld „Benutzer**&quot; im Dropdown-Menü eine neue **Zugriffsebene** und klicken Sie dann auf **Reaktivieren**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration.
-->

### Auswirkungen des Proofings bei der Reaktivierung eines Benutzers

Deaktivierte Benutzende verlieren ihre zugewiesene Standard-Proofing-Rolle und ihre Proofing-Lizenz (wenn Sie einen veralteten Workfront Premium-Plan verwenden). Wenn Sie den Benutzer erneut aktivieren möchten, müssen Sie:

* Weisen Sie die Lizenz neu zu (wenn Sie einen alten Workfront Premium-Plan verwenden). Weitere Informationen zu Workfront-Proofing-Plänen finden Sie unter [Zugriff auf die Proofing-Funktionalität in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Stellen Sie sicher, dass sie die richtige Korrekturabzugsrolle haben. Reaktivierte Korrekturabzugsbenutzende erhalten die Rolle, die als Standard-Korrekturabzugsrolle für neue Benutzende festgelegt ist. Weitere Informationen [&#x200B; Sie unter „Konfigurieren &#x200B;](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) Proofing-Standardrollen“.

## Informationen zur Deaktivierung von Workfront-Administratoren und Benutzern von Standard- oder Planlizenzen

Bevor Sie einen Workfront-Administrator oder eine Benutzerin bzw. einen Benutzer mit einer Planlizenz deaktivieren, müssen Sie nach Workfront-Objekten und -Aktivitäten suchen, an denen diese Person beteiligt ist, und sie dann ggf. einem anderen Workfront-Administrator oder einer Person mit einer Planlizenz zuordnen.

Diese Objekte und Aktivitäten können Folgendes umfassen:

* Dem Benutzer zugewiesene Aufgaben oder Probleme.
* Projekte, die dem Benutzer gehören.
* Berichte, die für die Ausführung mit den Zugriffsrechten des Benutzers eingerichtet wurden.
* Vorlagen, die dem Benutzer gehören.
* Projekte und Vorlagen, für die der Benutzer als Ressourcenmanager festgelegt wurde.
* Routingregeln für Anfrage-Warteschlangen Der Workfront-Administrator oder Plan-Lizenzbenutzer ist der standardmäßige Bearbeiter.
* Genehmigungsprozesse, die über eine Phase verfügen, in der der Benutzer eingeschlossen ist (insbesondere wenn er die einzige genehmigende Person auf der Phase war).
* Arbeitszeittabellen, in denen der Benutzer als genehmigende Person aufgeführt ist.
* Arbeitszeittabellen-Profile, in denen der Benutzer als genehmigende Person aufgeführt ist.
* Proofing von automatisierten Workflows, die den Benutzer enthalten.

## Auswirkung auf die Ressourcenplanung bei der Planung einer Benutzerdeaktivierung

Wenn Sie einen Benutzer für die Deaktivierung planen, werden diese im Ressourcenplaner nicht mehr als für die Budgetierung von Stunden verfügbar angezeigt. Wenn sie Teil der Ressourcenpools bleiben, werden sie im Ressourcenplaner angezeigt, ihre Verfügbarkeit wird jedoch auf null Stunden ab dem Datum ihrer geplanten Deaktivierung eingestellt.

Der Ressourcenplaner berücksichtigt alle Aufgabengebiete der Benutzer und die geplanten Abschlussdaten der Aufgaben und berechnet die Ressourcen entsprechend.

Weitere Informationen zum Ressourcenplaner finden Sie unter [Überblick über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

