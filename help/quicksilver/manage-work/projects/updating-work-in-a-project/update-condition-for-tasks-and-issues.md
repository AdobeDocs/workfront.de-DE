---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für Aufgaben und Probleme
description: Die Bedingung einer Aufgabe oder eines Problems ist eine Kennzeichnung, die angibt, wie es sich entwickelt. Dies unterscheidet sich vom Status des Arbeitselements, der den aktuellen Entwicklungsstand des Elements angibt.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 2%

---

# Aktualisierungsbedingung für Aufgaben und Probleme

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Die Bedingung einer Aufgabe oder eines Problems ist eine Kennzeichnung, die angibt, wie es sich entwickelt. Dies unterscheidet sich vom Status des Arbeitselements, der den aktuellen Entwicklungsstand des Elements angibt.

Sie können die Bedingung einer Aufgabe oder eines Problems entweder automatisch oder manuell festlegen.

Die Bedingungswerte, auf die wir in diesem Artikel verweisen, sind standardmäßig in Workfront verfügbar. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.

## Zugriffsanforderungen {#access-requirements}

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <ul><li><p>Standard für Aufgaben</p></li>
   <li><p>Mitwirkender oder höher für Probleme</p></li></ul>
  <p>ODER</p>
   <ul><li><p>Arbeit oder höher für Aufgaben</p></li>
   <li><p>Anfrage oder höher für Probleme</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Zugriff auf Aufgaben und Probleme bearbeiten </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern der Berechtigungen für Aufgaben und Probleme zum Anzeigen ihrer Bedingung</p>
   <p>Mitwirken an Berechtigungen für Aufgaben und Probleme, um die Bedingung zu aktualisieren</p>
  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>
   Current:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Contribute permissions on tasks and issues to update the Condition</p>
  </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

Sie müssen einer Aufgabe oder einem Problem zugewiesen sein, um seine Bedingung manuell aktualisieren zu können.

## Suchen des Status von Aufgaben und Problemen

Bedingungen werden als Markierung für Aufgaben oder Probleme angezeigt. Sie können auch mit einer Zahl verknüpft werden, die in Berichten anstelle des Titels angezeigt werden kann. Weitere Informationen zum Verknüpfen von Bedingungen mit Zahlen finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Sie können den Zustand von Aufgaben und Problemen in den folgenden Bereichen von Workfront ermitteln:

* Die Detailseite, nachdem sie ein Workfront- oder Gruppen-Administrator Ihrer Layout-Vorlage hinzugefügt hat. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* Die Kopfzeile einer Aufgabe oder eines Problems, nachdem ein Workfront- oder Gruppenadministrator sie zu Ihrer Layout-Vorlage hinzugefügt hat. Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* Nachdem ein Workfront- oder Gruppen-Administrator bzw. eine Administratorin das Bedienfeld Zusammenfassung zu Ihrer Layout-Vorlage hinzugefügt hat, erfolgt das Hinzufügen. Weitere Informationen finden Sie [Anpassen des Bedienfelds Zusammenfassung mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Berichte und Listen, wenn das Bedingungsfeld in einer Ansicht oder Gruppierung angezeigt wird.

  >[!NOTE]
  >
  >Wenn im Feld Feldname eines Journaleintragsberichts das Wort „Bedingung“ angezeigt wird, bedeutet dies, dass die Bedingung eines Elements aktualisiert wurde. Wenn das Bedingungsfeld in den Journaleintragsberichten verfolgt wird, zeigen die neuen und alten Zahlenwerte die mit der Bedingung verknüpfte Zahl anstelle ihres Namens an. Wenn eine Bedingung ursprünglich für eine Aufgabe oder ein Problem nicht definiert wurde und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den alten Zahlenwert des Bedingungsfelds als -2.147.483.648 an.

## Bedingung durch Aktualisieren des Status automatisch aktualisieren

Wenn Ihnen eine Aufgabe oder ein Problem zugewiesen ist und Sie auf **Bearbeiten** , Aufgabe starten oder Problem starten oder ihren Status aktualisieren, ändert sich der Zustand der Aufgabe oder des Problems automatisch in die Standardbedingung für **reibungslosen Ablauf**.

Informationen zur Verwendung einer benutzerdefinierten Bedingung als Standardbedingung finden Sie in den Artikeln [Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) und [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Informationen zum Ändern des Aufgabenstatus finden Sie unter [Aufgabenstatus aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Informationen zum Ändern des Problemstatus finden Sie unter [Problemstatus aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Informationen dazu, wie Sie die Schaltfläche „Bearbeiten“ auf die Schaltfläche „Aufgabe starten“ oder „Problem starten“ setzen, finden Sie [Ersetzen Sie die Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Bedingung manuell aktualisieren

Sie müssen einer Aufgabe oder einem Problem zugewiesen sein oder über Verwaltungsberechtigungen dafür verfügen, um die Bedingung dafür festlegen zu können.

Sie können die Bedingung einer Aufgabe oder eines Problems in einem Aufgaben- oder Problembericht oder einer Liste manuell aktualisieren, wenn Sie das Feld „Bedingung“ in der Ansicht anzeigen.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld „Bedingung“ zu Ihrem Bedienfeld „Zusammenfassung“ oder zu den Kopfzeilen- oder Detailseiten für Aufgaben oder Probleme hinzuzufügen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Übersicht](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Passen Sie das Bedienfeld Zusammenfassung mithilfe einer Layout-Vorlage &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Sie können den Zustand von Aufgaben und Problemen in verschiedenen Bereichen von Workfront manuell aktualisieren. In den folgenden Abschnitten wird beschrieben, wie Sie den Zustand von Aufgaben und Problemen manuell aktualisieren können.

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems in der Aufgaben- oder Problem-Kopfzeile

1. (Bedingt) Wenn der Workfront- oder Gruppen-Administrator das Feld Bedingung zur Aufgaben- oder Problem-Kopfzeile der Layout-Vorlage hinzugefügt hat, klicken Sie auf das Feld **Bedingung** in der Kopfzeile und wählen Sie aus den folgenden Optionen aus:
   * Keine Probleme
   * Kleinere Probleme
   * Größere Probleme

   ![Bedingung in der Aufgabenkopfzeile](assets/condition-in-task-header-0925.png)

<!--1. Click Enter to save the Condition.-->

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems im Abschnitt mit den Aufgaben- oder Problemdetails

1. (Bedingt) Wenn der Workfront- oder Gruppen-Administrator das Feld Bedingung zum Abschnitt Details einer Aufgabe oder eines Problems in der Layout-Vorlage hinzugefügt hat, klicken Sie im linken Bereich auf **Details** und dann auf **Aufgabenbedingung** oder **Problembedingung** und wählen Sie aus den folgenden Optionen aus:
   * Keine Probleme
   * Kleinere Probleme
   * Größere Probleme
1. Klicken Sie **Änderungen speichern**. Die Bedingung der Aufgabe oder des Problems wird aktualisiert.

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems in einem Bericht oder einer Liste

1. Navigieren Sie zu einer Liste von Aufgaben oder Problemen, für die Sie über Verwaltungsberechtigungen verfügen. Stellen Sie sicher **dass** Feld „Bedingung“ in der Listenansicht sichtbar ist.

1. Aktualisieren Sie **Bedingung** des Problems oder der Aufgabe inline, indem Sie auf die vorhandene Bedingung doppelklicken und einen neuen Wert aus dem Dropdown-Menü auswählen.

   ![Bedingungswerte in der Aufgabenliste](assets/condition-values-in-task-list-0925.png)

   >[!NOTE]
   >
   >Die Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung möglicherweise mehr als drei Optionen für die Bedingung finden. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Drücken Sie **Eingabetaste** auf der Tastatur oder klicken Sie außerhalb des Felds Bedingung , um die neue Aufgabe oder Problembedingung zu speichern.

   >[!NOTE]
   >
   >In der Ansicht „Standardbedingung“ ist **Feld** Bedingung“ ein Feldtyp, der nicht inline bearbeitet werden kann. Wenn Sie das Feld **Bedingung** separat zu einer Ansicht hinzufügen, kann es bearbeitet werden. Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


