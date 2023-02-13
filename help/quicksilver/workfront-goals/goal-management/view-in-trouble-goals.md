---
product-previous: workfront-goals
navigation-topic: goal-management
title: Überprüfen von Problemzielen in Adobe Workfront-Zielen
description: Diejenigen Ziele, bei denen der Fortschritt in Schwierigkeiten zu verzeichnen ist, laufen Gefahr, nicht erreicht zu werden, und werden durch eine rote Fortschrittsleiste in den Adobe Workfront-Zielen repräsentiert. Sie sollten Ihre Ziele oft überprüfen und verstehen, warum der Fortschritt hinkt.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Überprüfen von Problemzielen in Adobe Workfront-Zielen

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Ziele mit Fortschritten bei Problembehebung laufen Gefahr, nicht erreicht zu werden, und werden durch eine rote Fortschrittsleiste bei den Adobe Workfront-Zielen repräsentiert. Sie sollten Ihre Ziele oft überprüfen und verstehen, warum der Fortschritt hinkt. Informationen zum Zielfortschritt finden Sie unter [Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Zugriffsanforderungen

<!--drafted for P&P release: replace the existing requirements with this:

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die Adobe Workfront Goals erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele oder höher bearbeiten</p> <p><b>NOTIZ</b><p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Berechtigungen für das Ziel verwalten</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Recommendations verhindert, dass Ziele in Schwierigkeiten Fortschritte erzielen

Bevor Ziele einen Fortschritt von In Trouble erreichen, können Sie sie oft beobachten und ihren Fortschritt anpassen, wenn sie einen Fortschritt von &quot;Risiko&quot; erreichen. Ziele, die gefährdet sind, laufen Gefahr, in Schwierigkeiten zu geraten. Weitere Informationen zum Zielfortschritt finden Sie unter [Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/calculate-goal-progress.md)

Bevor Ihre Ziele den Fortschritt von In Trouble erreichen, empfehlen wir Folgendes:

* Überprüfen Sie Ziele, die häufig mit einem Risiko verbunden sind, das Ihnen zugewiesen ist, sowie Organisationsziele, die Ihren Teams, Gruppen oder Ihrer Organisation zugewiesen sind, die vom Fortschritt Ihrer Ziele beeinflusst werden können. Risikoziele laufen Gefahr, in Schwierigkeiten zu geraten. Die gefährdeten Ziele sind durch einen gelben Fortschrittsbalken gekennzeichnet. Verwenden Sie die Zielliste, um Ziele anzuzeigen, die zu Ihnen, Ihren Teams, Gruppen oder Ihrer Organisation gehören.


## Überprüfen von Problemzielen in der Zielliste

Sie können Ziele in jedem Abschnitt der Workfront-Ziele überprüfen. Weitere Informationen zu den Workfront-Zielen finden Sie unter [Überblick über die Adobe Workfront-Ziele - Abschnitte](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

In diesem Artikel wird beschrieben, wie Sie Ziele in der Zielliste überprüfen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Workfront-Zielbereich geöffnet und der Abschnitt &quot;Zielliste&quot;wird standardmäßig angezeigt.

1. (Empfohlen) Passen Sie die folgenden Filter für den Bereich &quot;Zielliste&quot;an, um Risikoziele zu überprüfen:

   * Klicken **Firma**, dann **Meine Teams**, dann **Meine Gruppen**, dann **Persönlich** Ziele in dieser Reihenfolge anzeigen, um Ziele anzuzeigen, die zu Ihrer Organisation, Ihren Teams, Gruppen und dann Ihren eigenen Zielen gehören.

      >[!TIP]
      >
      >Unter Adobe Workfront-Ziele zeigt der Filter Unternehmen die Ziele an, für die Ihr Unternehmen als Inhaber ausgewählt wurde.
      >
      >
      >Sie können nicht nach Unternehmen suchen, die dieses Feld verwenden. Standardmäßig wird nur Ihr Unternehmen ausgewählt, das Eigentümer Ihrer Workfront-Instanz ist.

   * Klicken Sie für jede der oben ausgewählten Organisationseinheiten auf **Neuer Filter** > **Fortschritt** > **In Schwierigkeiten** >**Anwenden.**
   * (Optional) Wählen Sie den Zeitraum aus, für den Sie Ziele anzeigen möchten.

      Die Fortschrittsleistenanzeige wird für jedes Ziel in der Zielliste rot angezeigt.

      Weitere Informationen zum Filtern von Zielen mithilfe aller anderen Kriterien im rechten Bereich finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Bewegen Sie den Mauszeiger über den Fortschrittsleistenindikator, um zu sehen, was der tatsächliche Fortschrittsprozentsatz ist und welcher erwartete Wert für den aktuellen Tag ist.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Optional) Verwenden Sie die Filter, um Ziele zu finden, die zu einem bestimmten Eigentümer gehören.

   In Schwierigkeiten befindliche Ziele für die ausgewählten Benutzer werden in der Zielliste angezeigt.

1. Klicken Sie auf einen Zielnamen, um die Zielseite zu öffnen, und klicken Sie dann auf **Fortschrittsanzeigen** im linken Bereich. Zeigen Sie an, welcher Fortschrittsindikator dafür sorgt, dass das Ziel im Rückstand ist, und aktualisieren Sie den Fortschritt des Indikators inline im **Tatsächlicher Fortschritt** in der Liste der Fortschrittsindikatoren.

   Informationen zur Aktualisierung von Ergebnissen und Aktivitäten finden Sie unter [Aktualisieren des Zielfortschritts in Adobe Workfront-Zielen](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >Sie können nur die Ergebnisse und Aktivitäten in der Liste der Fortschrittsindikatoren aktualisieren. Sie müssen die Fortschrittsindikatoren der Kinderziele aktualisieren, indem Sie auf die Ziele zugreifen, und die Aufgaben der verbundenen Projekte aktualisieren, um den Fortschritt der Projekte zu aktualisieren.


