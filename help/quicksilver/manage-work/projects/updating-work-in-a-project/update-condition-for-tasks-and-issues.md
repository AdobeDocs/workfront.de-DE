---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für Aufgaben und Probleme
description: Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 1%

---

# Aktualisierungsbedingung für Aufgaben und Probleme

{{highlighted-preview}}

Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.

Sie können die Bedingung einer Aufgabe oder eines Problems entweder automatisch oder manuell festlegen.

Die Bedingungswerte, auf die wir in diesem Artikel verweisen, sind standardmäßig in Workfront verfügbar. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Zugriffsanforderungen {#access-requirements}

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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

Für die neuen Lizenzen:
<ul><li><p>Standard für Aufgaben</p></li>
   <li><p>Beitragende oder höher für Probleme</p></li></ul>


Für aktuelle Lizenzen:
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
   <p>Verwalten von Berechtigungen für Aufgaben und Probleme zum Aktualisieren der Bedingung</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen einer Aufgabe oder einem Problem zugewiesen sein, damit Sie ihre Bedingung manuell aktualisieren können.

## Finden Sie die Bedingung der Aufgaben und Probleme

Bedingungen werden als Markierung angezeigt, die mit Aufgaben oder Problemen verknüpft ist. Sie können auch mit einer Zahl verknüpft werden, die in Berichten anstelle der Bezeichnung angezeigt werden kann. Weitere Informationen zum Verknüpfen von Bedingungen mit Zahlen finden Sie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Sie finden die Bedingungen für Aufgaben und Probleme in den folgenden Bereichen von Workfront:

* <span class="preview">Die Detailseite, nachdem sie von einem Workfront- oder Gruppenadministrator Ihrer Layoutvorlage hinzugefügt wurde. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md). </span>

* <span class="preview">Die Kopfzeile einer Aufgabe oder eines Problems, nachdem ein Workfront- oder Gruppenadministrator sie zu Ihrer Layoutvorlage hinzugefügt hat. Weitere Informationen finden Sie unter [Objektüberschriften mithilfe einer Layoutvorlage anpassen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). </span>

* Nachdem ein Workfront- oder Gruppenadministrator sie Ihrer Layoutvorlage hinzugefügt hat, wird sie im Bereich &quot;Zusammenfassung&quot;angezeigt. Weitere Informationen finden Sie unter [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

* Berichte und Listen, wenn Sie das Feld Bedingung in einer Ansicht oder Gruppierung anzeigen.

  >[!NOTE]
  >
  >Wenn das Wort &quot;Bedingung&quot;im Feld Feldname eines Journaleintragsberichts angezeigt wird, deutet dies darauf hin, dass die Bedingung eines Elements aktualisiert wurde. Wenn das Feld Bedingung in den Berichten Journaleinträge nachverfolgt wird, zeigen die Werte Neue und Alte Zahl anstelle des Namens die mit der Bedingung verknüpfte Zahl an. Wenn eine Bedingung ursprünglich nicht für eine Aufgabe oder ein Problem definiert wurde und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den Wert der alten Nummer des Felds Bedingung als -2.147.483.648 an.

## Automatische Aktualisierung der Bedingung durch Aktualisierung des Status

Wenn Sie eine Aufgabe oder ein Problem zugewiesen haben und auf **Arbeiten daran** , Aufgabe starten oder Problem starten oder den Status aktualisieren, ändert sich die Bedingung der Aufgabe oder des Problems automatisch in die Standardbedingung, die mit **Gehe sanft**.

Informationen zur Verwendung einer benutzerdefinierten Bedingung als Standardbedingung finden Sie in den Artikeln  [Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) und [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Informationen zum Ändern des Aufgabenstatus finden Sie unter [Aktualisierung des Aufgabenstatus](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Informationen zum Ändern des Problemstatus finden Sie unter [Status des Problems aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Informationen zum Festlegen der Schaltfläche &quot;Work On It&quot;auf eine Schaltfläche &quot;Start Task&quot;oder &quot;Start Issue&quot;finden Sie unter [Ersetzen der Schaltfläche &quot;Work On It&quot;durch die Schaltfläche Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Manuelles Aktualisieren der Bedingung

Sie müssen einer Aufgabe oder dem Problem zugewiesen sein oder über die Berechtigung &quot;Verwalten&quot;verfügen, damit Sie die Bedingung darauf festlegen können.

Wenn Sie das Feld Bedingung in der Ansicht anzeigen, können Sie die Bedingung einer Aufgabe oder eines Problems in einem Aufgaben- oder Problembericht oder einer Liste manuell aktualisieren.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld Bedingung zu Ihrem Zusammenfassungsbereich hinzuzufügen, um die Aktualisierung in verschiedenen Bereichen von Workfront zu vereinfachen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Zusammenfassungsübersicht](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

Führen Sie einen der folgenden Schritte aus, um die Bedingung einer Aufgabe oder eines Problems manuell zu aktualisieren:

<div class="preview">

1. So aktualisieren Sie die Bedingung einer Aufgabe oder eines Problems in der Aufgaben- oder Problemkopfzeile:

   1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator das Feld Bedingung zur Aufgaben- oder Problemüberschrift Ihrer Layoutvorlage hinzugefügt hat, klicken Sie auf das **Bedingung** in der Kopfzeile ein und wählen Sie aus den folgenden Optionen aus:
      * Keine Probleme
      * Kleinere Probleme
      * Größere Probleme

      ![](assets/condition-in-task-header.png)
   1. Klicken Sie auf Eingabetaste , um die Bedingung zu speichern.

1. So aktualisieren Sie die Bedingung einer Aufgabe oder eines Problems im Abschnitt &quot;Aufgaben- oder Problemdetails&quot;:

   1. (Bedingt) Wenn Ihr Workfront- oder Gruppenadministrator das Feld Bedingung zum Bereich Details einer Aufgabe oder eines Problems in Ihrer Layoutvorlage hinzugefügt hat, klicken Sie auf **Details** Klicken Sie im linken Bereich auf das **Bedingung** und wählen Sie aus den folgenden Optionen aus:
      * Keine Probleme
      * Kleinere Probleme
      * Größere Probleme
1. Klicks **Änderungen speichern**. Die Bedingung der Aufgabe oder des Problems wird aktualisiert.

</div>

So aktualisieren Sie die Bedingung einer Aufgabe oder eines Problems in einem Bericht oder einer Liste:

1. Rufen Sie eine Liste der Aufgaben oder Probleme auf, für die Sie über Verwaltungsberechtigungen verfügen. Stellen Sie die **Bedingung** -Feld in der Listenansicht angezeigt.

1. Aktualisieren Sie die **Bedingung** durch Doppelklicken auf die vorhandene Bedingung und Auswahl eines neuen Werts aus dem Dropdown-Menü.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Presse **Eingabe** auf der Tastatur klicken oder außerhalb des Bedingungsfelds klicken, um die neue Aufgabe oder Problembedingung zu speichern.

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


