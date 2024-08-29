---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für Aufgaben und Probleme
description: Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# Aktualisierungsbedingung für Aufgaben und Probleme

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.

Sie können die Bedingung einer Aufgabe oder eines Problems entweder automatisch oder manuell festlegen.

Die Bedingungswerte, auf die wir in diesem Artikel verweisen, sind standardmäßig in Workfront verfügbar. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie in [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.

## Zugriffsanforderungen {#access-requirements}

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   Neu:
   <ul><li><p>Standard für Aufgaben</p></li>
   <li><p>Beitragende oder höher für Probleme</p></li></ul>
   Aktuell:
   <ul><li><p>Arbeit oder höher für Aufgaben</p></li>
   <li><p>Anfrage oder höher für Probleme</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Anzeigen oder Verbessern des Zugriffs auf Projekte</p> <p>Zugriff auf Aufgaben und Probleme bearbeiten </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für Aufgaben und Probleme zur Anzeige ihrer Bedingung</p>
   <p>Contribute-Berechtigungen für Aufgaben und Probleme beim Aktualisieren der Bedingung</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einer Aufgabe oder einem Problem zugewiesen sein, damit Sie ihre Bedingung manuell aktualisieren können.

## Finden Sie die Bedingung der Aufgaben und Probleme

Bedingungen werden als Markierung angezeigt, die mit Aufgaben oder Problemen verknüpft ist. Sie können auch mit einer Zahl verknüpft werden, die in Berichten anstelle der Bezeichnung angezeigt werden kann. Weitere Informationen zum Zuordnen von Bedingungen zu Zahlen finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Sie finden die Bedingungen für Aufgaben und Probleme in den folgenden Bereichen von Workfront:

* Die Detailseite, nachdem sie von einem Workfront- oder Gruppenadministrator Ihrer Layoutvorlage hinzugefügt wurde. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

* Die Kopfzeile einer Aufgabe oder eines Problems, nachdem ein Workfront- oder Gruppenadministrator sie zu Ihrer Layoutvorlage hinzugefügt hat. Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

* Nachdem ein Workfront- oder Gruppenadministrator sie Ihrer Layoutvorlage hinzugefügt hat, wird sie im Bereich &quot;Zusammenfassung&quot;angezeigt. Weitere Informationen finden Sie unter [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Berichte und Listen, wenn Sie das Feld Bedingung in einer Ansicht oder Gruppierung anzeigen.

  >[!NOTE]
  >
  >Wenn das Wort &quot;Bedingung&quot;im Feld Feldname eines Journaleintragsberichts angezeigt wird, deutet dies darauf hin, dass die Bedingung eines Elements aktualisiert wurde. Wenn das Feld Bedingung in den Berichten Journaleinträge nachverfolgt wird, zeigen die Werte Neue und Alte Zahl anstelle des Namens die mit der Bedingung verknüpfte Zahl an. Wenn eine Bedingung ursprünglich nicht für eine Aufgabe oder ein Problem definiert wurde und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den Wert der alten Nummer des Felds Bedingung als -2.147.483.648 an.

## Automatische Aktualisierung der Bedingung durch Aktualisierung des Status

Wenn Sie eine Aufgabe oder ein Problem zugewiesen haben und auf &quot;**Bearbeiten**&quot;, &quot;Aufgabe starten&quot;oder &quot;Problem starten&quot;klicken oder den Status aktualisieren, ändert sich die Bedingung der Aufgabe oder des Problems automatisch in die Standardbedingung, die mit &quot;**Gehe reibungslos&quot;** verknüpft ist.

Informationen zur Verwendung einer benutzerdefinierten Bedingung als Standardbedingung finden Sie in den Artikeln [Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) und [Benutzerdefinierte Bedingung als Standard für Projekte festlegen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) .

Informationen zum Ändern des Aufgabenstatus finden Sie unter [Status der Aufgabe aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Informationen zum Ändern des Problemstatus finden Sie unter [Update des Problemstatus](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Informationen zum Festlegen der Schaltfläche &quot;Work On It&quot;auf die Schaltfläche &quot;Start Task&quot;oder &quot;Start Issue&quot;finden Sie unter [Ersetzen der Schaltfläche Work On It durch eine Schaltfläche Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Manuelles Aktualisieren der Bedingung

Sie müssen einer Aufgabe oder dem Problem zugewiesen sein oder über die Berechtigung &quot;Verwalten&quot;verfügen, damit Sie die Bedingung darauf festlegen können.

Wenn Sie das Feld Bedingung in der Ansicht anzeigen, können Sie die Bedingung einer Aufgabe oder eines Problems in einem Aufgaben- oder Problembericht oder einer Liste manuell aktualisieren.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld Bedingung zu Ihrem Zusammenfassungsbereich hinzuzufügen oder die Aufgaben- oder Problemüberschrift oder Detailseiten hinzuzufügen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Überblick über die Zusammenfassung](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Passen Sie die Startseite und die Zusammenfassung mit einer Layoutvorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Sie können die Bedingungen für Aufgaben und Probleme in verschiedenen Bereichen von Workfront manuell aktualisieren. In den folgenden Abschnitten wird beschrieben, wie Sie die Bedingung von Aufgaben und Problemen manuell aktualisieren können.

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems in der Aufgaben- oder Problemkopfzeile

1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator das Feld Bedingung zur Aufgaben- oder Problemüberschrift Ihrer Layoutvorlage hinzugefügt hat, klicken Sie in der Kopfzeile auf das Feld **Bedingung** und wählen Sie aus den folgenden Optionen aus:
   * Keine Probleme
   * Kleinere Probleme
   * Größere Probleme

   ![](assets/condition-in-task-header.png)
1. Klicken Sie auf Eingabetaste , um die Bedingung zu speichern.

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems im Abschnitt mit den Aufgaben- oder Problemdetails

1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator das Feld Bedingung zum Bereich Details einer Aufgabe oder eines Problems in Ihrer Layoutvorlage hinzugefügt hat, klicken Sie im linken Bereich auf **Details** , klicken Sie dann auf **Aufgabenbedingung** oder **Problembedingung** und wählen Sie eine der folgenden Optionen aus:
   * Keine Probleme
   * Kleinere Probleme
   * Größere Probleme
1. Klicken Sie auf **Änderungen speichern**. Die Bedingung der Aufgabe oder des Problems wird aktualisiert.

### Aktualisieren der Bedingung einer Aufgabe oder eines Problems in einem Bericht oder einer Liste

1. Rufen Sie eine Liste der Aufgaben oder Probleme auf, für die Sie über Verwaltungsberechtigungen verfügen. Stellen Sie sicher, dass das Feld **Bedingung** in der Listenansicht sichtbar ist.

1. Aktualisieren Sie die **Bedingung** des Problems oder der Aufgabe inline, indem Sie auf die vorhandene Bedingung doppelklicken und einen neuen Wert aus dem Dropdown-Menü auswählen.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Drücken Sie auf der Tastatur die **Eingabetaste** oder klicken Sie außerhalb des Felds Bedingung auf , um die neue Aufgabe oder Problembedingung zu speichern.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


