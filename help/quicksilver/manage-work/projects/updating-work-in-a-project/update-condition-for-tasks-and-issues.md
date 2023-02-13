---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für Aufgaben und Probleme
description: Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Aktualisierungsbedingung für Aufgaben und Probleme

Die Bedingung einer Aufgabe oder eines Problems ist eine Markierung, die darauf platziert wird, um anzugeben, wie es funktioniert. Dies unterscheidet sich vom Status des Arbeitselements, der die aktuelle Phase der Entwicklung des Elements angibt.

Sie können die Bedingung einer Aufgabe oder eines Problems entweder automatisch oder manuell festlegen.

Der Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Zugriffsanforderungen {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher für Aufgaben</p>
   <p>Anfrage oder höher für Probleme</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder Verbessern des Zugriffs auf Projekte</p> <p>Zugriff auf Aufgaben und Probleme bearbeiten </p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für Aufgaben und Probleme zur Anzeige ihrer Bedingung</p>
   <p>Verwalten von Berechtigungen für Aufgaben und Probleme zum Aktualisieren der Bedingung</p>
    <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Finden Sie die Bedingung der Aufgaben und Probleme

Bedingungen werden als Markierung angezeigt, die mit Aufgaben oder Problemen verknüpft ist. Sie können auch mit einer Zahl verknüpft werden, die in Berichten anstelle der Bezeichnung angezeigt werden kann. Weitere Informationen zum Verknüpfen von Bedingungen mit Zahlen finden Sie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Sie können die Bedingungen für Aufgaben und Probleme in den folgenden Bereichen ermitteln:

* Aufgaben- und Problemaktualisierungsbereich innerhalb eines Updates, wenn Sie der Aufgabe oder dem Problem zugewiesen sind.
* Berichte und Listen, wenn Sie das Feld Bedingung in einer Ansicht oder Gruppierung anzeigen.

>[!NOTE]
>
>Wenn das Wort &quot;Bedingung&quot;im Feld Feldname eines Journaleintragsberichts angezeigt wird, deutet dies darauf hin, dass die Bedingung eines Elements aktualisiert wurde. Wenn das Feld Bedingung in den Berichten Journaleinträge nachverfolgt wird, zeigen die Werte Neue und Alte Zahl anstelle des Namens die mit der Bedingung verknüpfte Zahl an. Wenn eine Bedingung ursprünglich nicht für eine Aufgabe oder ein Problem definiert wurde und Sie sie später aktualisieren, zeigt der Journaleintrag, der die Aktualisierung erfasst, den Wert der alten Nummer des Felds Bedingung als -2.147.483.648 an.

## Automatische Aktualisierung der Bedingung durch Aktualisierung des Status

Wenn Sie eine Aufgabe oder ein Problem zugewiesen haben, klicken Sie auf **Arbeiten daran** , Aufgabe starten oder Problem starten oder den Status aktualisieren, ändert sich die Bedingung der Aufgabe oder des Problems automatisch in die Standardbedingung für **Gehe sanft**.

Informationen zur Verwendung einer benutzerdefinierten Bedingung als Standardbedingung finden Sie in den Artikeln  [Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) und [Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Informationen zum Ändern des Aufgabenstatus finden Sie unter [Aktualisierung des Aufgabenstatus](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Informationen zum Ändern des Problemstatus finden Sie unter [Status des Problems aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Informationen zum Festlegen der Schaltfläche &quot;Work On It&quot;auf eine Schaltfläche &quot;Start Task&quot;oder &quot;Start Issue&quot;finden Sie unter [Ersetzen der Schaltfläche &quot;Work On It&quot;durch die Schaltfläche Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## Manuelles Aktualisieren der Bedingung

Sie müssen einer Aufgabe oder dem Problem zugewiesen sein oder über die Berechtigung &quot;Verwalten&quot;verfügen, damit Sie die Bedingung darauf festlegen können.

Die Aktualisierung der Bedingung einer Aufgabe oder eines Problems hängt davon ab, ob Sie ihr zugewiesen sind oder nicht:

* Sie können die Bedingung auf der Registerkarte Aktualisierungen oder in einer Liste von Aufgaben oder Problemen aktualisieren, wenn Sie ihnen zugewiesen sind.
* Sie können die Bedingung nur in einer Liste von Aufgaben oder Problemen aktualisieren, wenn Sie ihnen nicht zugewiesen sind, aber über Verwaltungsberechtigungen verfügen. In diesem Fall können Sie die Bedingung nicht auf der Registerkarte Aktualisieren der Aufgabe oder des Problems aktualisieren.

So legen Sie die Bedingung einer Aufgabe oder eines Problems manuell fest:

1. Gehen Sie zu einer Aufgabe oder einem Problem, die Ihnen zugewiesen ist und für die Sie die Bedingung festlegen möchten.

   Oder

   Rufen Sie eine Liste der Aufgaben oder Probleme auf, für die Sie zwar über die Berechtigung &quot;Verwalten&quot;verfügen, die Ihnen jedoch nicht zugewiesen sind.

1. Ändern Sie die Bedingung des Problems oder der Aufgabe wie folgt:

   * Wenn Sie der Aufgabe oder dem Problem zugewiesen sind und über Verwaltungsberechtigungen verfügen, finden Sie im **Updates** Registerkarte, klicken Sie auf **Neue Aktualisierung starten**, wählen Sie die **Bedingung** Geben Sie den Grund für die Änderung der Bedingung in die **Neue Aktualisierung starten** Bereich (optional) und klicken Sie dann auf **Aktualisieren**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
