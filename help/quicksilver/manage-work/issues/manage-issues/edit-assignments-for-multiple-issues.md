---
product-area: projects
navigation-topic: manage-issues
title: Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste
description: Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7aa420946115fc612ad1d9e310583e5453ae0678
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 2%

---

# Ändern von Benutzerzuweisungen für mehrere Probleme in einer Liste

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Sie können gleichzeitig Benutzerzuweisungen für mehrere Probleme ändern. Informationen zum Bearbeiten oder Zuweisen von Problemen einzeln finden Sie in den folgenden Artikeln:

* [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Probleme zuweisen](../../../manage-work/issues/manage-issues/assign-issues.md)

Allgemeine Informationen zum Zuweisen von Problemen finden Sie unter [Übersicht über das Ändern von Problemzuweisungen](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Sie müssen mindestens über die Berechtigung Beitragen für ein Problem verfügen, um Zuweisungen an das Problem vornehmen zu können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Zugriff auf Projekte und Aufgaben anzeigen oder höher, um ein Problem zuzuweisen</p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> <p>Tragen Sie Berechtigungen oder mehr zu dem Projekt oder der Aufgabe bei, in dem/der sich das Problem befindet, wenn Sie mehrere Probleme zuweisen.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Zuweisung für mehrere Anfragen ändern

1. Navigieren Sie zur Anfrageliste mit den Anfragen, deren Zuweisungen Sie ändern möchten.
1. (Optional) Erstellen Sie einen Filter, um nur Probleme anzuzeigen, die dem Verantwortlichen zugewiesen wurden, den Sie ändern möchten.

   Sie können beispielsweise einen Filter erstellen, um nur Probleme mit einer bestimmten Rolle als Verantwortlicher anzuzeigen. Anschließend können Sie die Rolle durch einen bestimmten Benutzer ersetzen. Gehen Sie folgendermaßen vor:

   1. Klicken Sie auf **Dropdown** Liste Filter und dann auf **Neuer Filter**.

      Das Dialogfeld Neuer Filter wird angezeigt.

   1. Klicken Sie **Filterregel hinzufügen.**
   1. Um nach einer bestimmten Rolle zu filtern, erweitern Sie **Arbeitsauftrag - Rollen** klicken Sie dann auf **ID.**

      Oder

      Um nach einem bestimmten Benutzer zu filtern, erweitern Sie **Arbeitsauftrag - Benutzer** und klicken Sie dann auf **ID.**

      >[!TIP]
      >
      >Verwenden Sie nicht **Zugewiesen an** da sich dieses Feld nur auf den Problembesitzer und nicht auf alle Zugewiesenen bezieht.

   1. Wählen Sie in der Dropdown-Liste **Gleich** als Filterqualifizierer aus.
   1. Geben Sie den Namen des Benutzers oder der Rolle ein, nach dem bzw. der gefiltert werden soll, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
   1. Klicken Sie auf **Filter speichern.**

1. Wählen Sie die Probleme aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png).

   Die **Probleme bearbeiten** wird angezeigt. Die bearbeiteten Elemente werden in der oberen linken Ecke der Seite angezeigt.

1. Gehen Sie zum Abschnitt **Arbeitsaufträge** und wählen Sie dann **Verantwortlicher** aus.

   ![Bereich „Zuweisungen](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Führen Sie einen der folgenden Schritte aus:

   1. So fügen Sie einen neuen Bevollmächtigten hinzu:

      1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, einer Rolle oder eines Teams und wählen Sie ihn aus, wenn er/sie in der Liste angezeigt wird. Die Zuweisung wird hinzugefügt und ersetzt nicht die aktuellen Zuweisungen in den ausgewählten Problemen.

         >[!TIP]
         >
         >Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
         >
         >Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
         >
         >* Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
         >* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.

         Es werden Informationen angezeigt, die für alle ausgewählten Probleme gelten. Wenn beispielsweise allen Problemen derselbe Benutzer zugewiesen ist, wird dieser Benutzer in der Spalte &quot;**&quot;**. Wenn die Informationen zu den ausgewählten Problemen nicht gleich sind, werden keine Informationen angezeigt.

   1. So entfernen Sie einzelne Zugewiesene:

      1. Klicken Sie auf das **X**-Symbol neben dem Namen des Verantwortlichen, den Sie entfernen möchten, wenn der Verantwortliche in der Zuweisungsliste angezeigt wird.

         Oder

         (Bedingt) Wenn der Verantwortliche, den Sie entfernen möchten, nicht im Abschnitt Zuweisungen angezeigt wird, da der Verantwortliche nur einigen der von Ihnen ausgewählten Probleme zugewiesen ist, klicken Sie auf **Verantwortlichen entfernen** und geben Sie den Namen des Verantwortlichen ein, den Sie entfernen möchten. Klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

      1. Klicken Sie **erneut auf &quot;** entfernen“, um einen weiteren zu entfernenden Bevollmächtigten hinzuzufügen.

   1. So entfernen Sie alle vorhandenen Zugewiesenen:

      1. Klicken Sie **Alle vorhandenen Bevollmächtigten entfernen** und klicken Sie dann auf **Ja, Alle Bevollmächtigten löschen**.

         Dadurch werden nicht nur die allgemeinen Bevollmächtigten (Bevollmächtigte, die im Dialogfeld „Bearbeiten“ angezeigt werden) entfernt, sondern auch alle Bevollmächtigten für alle ausgewählten Probleme.

1. (Optional) Ändern Sie eine der folgenden Optionen für die Bevollmächtigten, die Sie für die Probleme ausgewählt haben:

   * **Anfragebesitzer:** Wählen Sie das Optionsfeld aus, um anzugeben, welcher Bevollmächtigte als Anfragebesitzer bestimmt wird. Wenn diese Option deaktiviert ist, bestimmt Adobe Workfront den ersten Bearbeiter als Anfragebesitzer. Dies ist nicht für Team-Arbeitsaufträge verfügbar.
   * **Rolle des Verantwortlichen**: Wählen Sie eine Rolle aus der Dropdown-Liste aus. Wenn die Option deaktiviert bleibt, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. Klicken Sie auf **Änderungen speichern**.
