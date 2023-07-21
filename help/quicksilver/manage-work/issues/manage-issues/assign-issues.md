---
product-area: projects
navigation-topic: manage-issues
title: Zuweisen von Problemen
description: Sie können Benutzern, Rollen und Teams Probleme zuweisen, um anzugeben, wer für das Abschließen der Probleme verantwortlich ist. Allgemeine Informationen zum Zuweisen von Problemen finden Sie unter Problemzuweisungen ändern - Übersicht.
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: c7eb3266081a601d0aeaec1a2bd21272d05d1bc6
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 0%

---

# Zuweisen von Problemen

Sie können Benutzern, Rollen und Teams Probleme zuweisen, um anzugeben, wer für das Abschließen der Probleme verantwortlich ist. Allgemeine Informationen zum Zuweisen von Problemen finden Sie unter [Übersicht über Problemzuweisungen ändern](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
>
>Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
>
>* Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
>* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.

Zusätzlich zu diesem Artikel empfehlen wir, die folgenden Artikel zu lesen, um weitere Informationen zur Problemzuweisung zu erhalten:

* [Übersicht über Problemzuweisungen ändern](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Smart-Zuweisungen vornehmen](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Sie können ein Problem einer oder mehreren Ressourcen auf der Ebene einzelner Probleme zuweisen oder mehrere Ressourcen gleichzeitig mehreren Problemen zuweisen.

Das Zuweisen von Problemen und Aufgaben ist in Adobe Workfront ähnlich. Allgemeine Informationen zum Zuweisen von Aufgaben finden Sie unter [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> <p>Tragen Sie Berechtigungen zu dem Element bei, in das Sie das Problem kopieren und Probleme hinzufügen können.</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Benutzern Zugriff gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zur Mehrfachzuweisung von Stellenrollen, Teams und Benutzern

Beachten Sie beim Zuweisen mehrerer Ressourcen zu einem Arbeitselement Folgendes:

* Benutzern kann mehr als eine Auftragsrolle mit ihrem Profil zugeordnet sein. Informationen zum Zuordnen von Benutzern zu Aufgabenrollen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Aufgaben oder Probleme werden normalerweise zuerst einer oder mehreren Auftrags- oder Teams zugewiesen. Wenn Projekte startbereit sind, müssen sie möglicherweise auch Benutzern zugewiesen werden.

  Wenn eine Aufgabe oder ein Problem einer oder mehreren Rollen zugewiesen ist und Sie dann auch einen Benutzer zuweisen, bestimmt Adobe Workfront gemäß den folgenden Regeln, welche Vorgangsrolle dem zusätzlichen Benutzer zugeordnet werden soll (falls vorhanden):

   * Wenn nur eine Auftragsrolle zugewiesen ist und sie mit der Primären Rolle des Benutzers übereinstimmt, wird die Aufgabe bzw. das Problem nur dem Benutzer zugewiesen, der seine Primäre Rolle erfüllt.
   * Wenn mehrere Rollen zugewiesen sind und mindestens eine der Rollen mit den sekundären Rollen des Benutzers übereinstimmt, wird die Aufgabe bzw. das Problem dem Benutzer zugewiesen, der eine seiner &quot;Sonstige Rollen&quot;(die Workfront zufällig auswählt, wenn mehrere Übereinstimmungen vorliegen) erfüllt, sowie allen weiteren zugewiesenen Rollen.
   * Wenn eine oder mehrere Aufgabenrollen zugewiesen sind und die Benutzerrollen nicht übereinstimmen, wird die Aufgabe bzw. das Problem sowohl den Rollen oder Rollen als auch dem Benutzer zugewiesen.

* Wenn eine Aufgabe oder ein Problem einem Team zugewiesen ist und Sie auch einen Benutzer zuweisen, bleibt die Aufgabe bzw. das Problem sowohl dem Team als auch dem Benutzer zugewiesen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Zuweisen eines einzelnen Problems

1. Gehen Sie zu einem Problem, das Sie zuweisen möchten.
1. Klicken **Zuweisen zu** in der oberen rechten Ecke der Kopfzeile des Problems in der **Zuweisungen** area

   Oder

   Klicken Sie auf den Namen der aktuellen Zuweisungen, falls das Problem bereits zugewiesen wurde.

   ![](assets/nwe-assign-to-button-in-header-350x77.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie zuweisen möchten, und klicken Sie dann auf den Namen, wenn er/sie in der Liste angezeigt wird.

     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

   * (Bedingt) Klicken Sie auf einen der Namen im **Vorgeschlagene Zuweisungen** Liste
   * Klicken **Zuweisen** , um es sich selbst zuzuweisen
   * Klicken **Erweitert**

     Das Erstellen erweiterter Zuweisungen ähnelt dem Erstellen von Aufgaben und Problemen. Informationen zum Ausführen erweiterter Zuweisungen finden Sie unter [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
     >
     >Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
     >
     >Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)


1. Klicken **Speichern** , um die Zuweisung des Problems abzuschließen.
1. (Optional) Klicken Sie auf die **X-Symbol** neben dem Namen der Zuweisungen im Bereich Zuweisungen in der Kopfzeile des Problems, um eine Zuweisung zu entfernen.

## Zuweisen eines Problems in einer Liste

Sie können Probleme in einer Liste oder einem Bericht zuweisen, wenn eines der Zuweisungsfelder in der Listenansicht sichtbar ist. Auf diese Weise können Probleme schneller zugewiesen werden.

Je nachdem, welches Feld in der Ansicht sichtbar ist, können Sie dem Problem die folgenden Entitäten zuweisen:

| Option | Zugewiesene Entitäten |
|---|---|
| **Zuweisen zu** | Benutzer zuweisen |
| **Zugewiesen** | Benutzer zuweisen |
| **Arbeitsaufträge** | Weisen Sie Benutzer, Auftragsrollen oder Teams zu. |

So weisen Sie Probleme in einer Liste zu:

1. Rufen Sie eine Liste der Probleme auf, für die in der Ansicht die Felder &quot;Zugeordnet&quot;, &quot;Zugeordnet&quot;oder &quot;Zuweisungen&quot;vorhanden sind.
1. Führen Sie einen der folgenden Schritte aus, um Probleme zuzuweisen:

   * Klicken Sie in die **Zugeordnet zu** oder **Zugeordnet** und beginnen Sie mit der Eingabe des Namens eines aktiven Benutzers, den Sie dem Problem zuweisen möchten, und klicken Sie dann auf ihn, wenn er in der Liste angezeigt wird.

     ![](assets/assigned-to-field-task-list-nwe.png)

   * Klicken Sie in die **Zuweisungen** eingeben und den Namen eines aktiven Benutzers, einer Rolle oder eines aktiven Teams eingeben, das Sie dem Problem zuweisen möchten, und klicken Sie dann darauf, wenn es in der Liste angezeigt wird.

     ![](assets/assignments-field-task-list-nwe.png)

   >[!TIP]
   >
   >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden.
   >
   >Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
   >
   Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. (Bedingt) Wenn im Feld Zuweisungen sichtbar, klicken Sie auf die Schaltfläche **Personensymbol** ![](assets/teams.png) in der rechten oberen Ecke des Zuweisungsfelds, um das Feld Erweiterte Zuweisungen zu öffnen und erweiterte Zuweisungen zu erstellen. Weitere Informationen finden Sie unter [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Sie können keine erweiterten Zuweisungen aus den Feldern Zugeordnet oder Zugeordnet vornehmen.

1. Nachdem Sie Ihre Bevollmächtigten zum Problem hinzugefügt haben, drücken Sie die Eingabetaste oder klicken Sie auf eine beliebige Stelle auf der Seite, um Ihre Änderungen zu speichern.

## Zuweisen von Problemen in großen Mengen

1. Gehen Sie zu einer Liste der Probleme, die Sie stapelweise zuweisen möchten.
1. Wählen Sie mehrere Probleme in der Liste aus.
1. Klicken Sie auf **Symbol Bearbeiten** ![](assets/qs-edit-icon.png).

   Die **Probleme bearbeiten** wird geöffnet.

1. Im **Zuweisungen** Bereich, wählen Sie die **Bevollmächtigter** und geben Sie dann den Namen eines Benutzers, einer Rolle oder eines Teams ein, die bzw. das Sie allen Problemen zuweisen möchten.

   >[!IMPORTANT]
   >
   >Wenn eines der Probleme bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Problemen hinzugefügt, anstatt die vorhandenen Ressourcen zu den Problemen zu ersetzen.

1. (Optional) Wählen Sie das Optionsfeld im **Eigentümer des Problems** gibt an, welche Ressource der primäre Verantwortliche oder Eigentümer des Problems ist, wenn Sie dem Problem mehrere Ressourcen zuweisen. Dies ist nicht für Teams verfügbar.
1. (Optional) Wählen Sie eine Rolle aus, die der Benutzer für das Problem im **Rolle auswählen** Dropdown-Menü im **Rolle des Bevollmächtigten** angezeigt, wenn Sie Benutzern Probleme zuweisen. Wenn Sie keine Rolle auswählen, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. (Optional) Wenn Sie vorhandene Bevollmächtigte aus allen Problemen entfernen möchten, führen Sie einen der folgenden Schritte aus:

   1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie aus dem Problem entfernen möchten, wählen Sie ihn aus, wenn er/sie in der Liste angezeigt wird, und klicken Sie auf **Zuweisung entfernen** , um weitere zu entfernende Bevollmächtigte hinzuzufügen.
   1. Klicken **Alle vorhandenen Zuweisung entfernen** um alle Bevollmächtigten aus allen ausgewählten Problemen zu entfernen.

1. Klicken **Änderungen speichern**.
1. (Optional und bedingt) Wenn die Felder Zugeordnet oder Zuweisungen in Ihrer Liste der Probleme angezeigt werden, klicken Sie für ein Problem in eine dieser Spalten und klicken Sie dann auf die Schaltfläche **X-Symbol** neben dem Namen eines Bevollmächtigten, um ihn aus dem Problem zu entfernen.
