---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Smart-Zuweisungen vornehmen
description: Sie können intelligente Zuweisungen verwenden, um zu ermitteln, wer die Arbeit am besten erledigen kann. Intelligente Zuweisungen sind Vorschläge für Benutzende, Rollen oder Teams, die Adobe Workfront Ihnen vorstellt, wenn Sie Ressourcen Arbeitselemente auf der Grundlage eines Algorithmus zuweisen, der die am besten geeignete Ressource für den Auftrag bestimmt. Informationen zu Smart-Zuweisungen finden Sie unter Smart-Zuweisungen - Übersicht .
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Smart-Zuweisungen vornehmen

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in der Vorschau-Umgebung verfügbar sind.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

Sie können intelligente Zuweisungen verwenden, um zu ermitteln, wer die Arbeit am besten erledigen kann.

Intelligente Zuweisungen sind Vorschläge für Benutzende, Rollen oder Teams, die Adobe Workfront Ihnen beim Zuweisen von Arbeitselementen zu Ressourcen vorlegt. Workfront stützt seine Vorschläge auf einen Algorithmus, der die am besten geeignete Ressource für den Auftrag bestimmt.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

Weitere Informationen über die Kriterien zur Bestimmung von Smart-Zuweisungen finden Sie unter [Smart-Zuweisungen - Übersicht](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p>
      Oder
      <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> <p>Zugriff auf Projekte anzeigen oder höher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Mitwirken an oder höhere Berechtigungen mit der Möglichkeit, Zuweisungen zu Aufgaben und Problemen vorzunehmen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Smart-Zuweisungen vornehmen

Smart-Zuweisungen sind an den meisten Stellen verfügbar, an denen Sie Zuweisungen in Workfront vornehmen können.

1. Wechseln Sie zu den folgenden Bereichen und klicken Sie auf das Feld **Arbeitsaufträge** oder **Diesen zuweisen zu**:

   * Aufgaben- oder Problemliste oder Bericht
   * Kopfzeile einer Aufgabe oder eines Problems
   * Das Bedienfeld „Aufgaben- oder Problemzusammenfassung“
   * Eine Aufgabe oder ein Problem im Workload Balancer
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. Platzieren Sie den Cursor im Feld Arbeitsaufträge und warten Sie zwei Sekunden.

   <!--For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![](assets/smart-assignments-issue-header.png)-->

   Smart-Zuweisungen werden in den folgenden Abschnitten angezeigt<!--, depending on which phase of the algorithm's calculation identified the assignments-->:

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **Benutzer und Teams**, **Aufgabengebiete** oder <span class="preview">**Tarifkarten-Aufgabengebiete**</span>: <!--Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![Beispiel für Smart Assignments in Aufgabenliste](assets/smart-assignments-task-list.png)

   Weitere Informationen finden Sie unter [Smart Assignments - Übersicht](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Wählen Sie die Ressource in der Liste Recommendations aus, indem Sie auf ihren Namen klicken.

1. (Optional) Klicken Sie auf **Mir zuweisen**, um das Arbeitselement sich selbst zuzuweisen.

   >[!TIP]
   >
   >Wenn keine Vorschläge vorliegen, wird die Vorschlagsliste nicht geöffnet.

1. (Optional) Wenn Sie keinen der empfohlenen Benutzer aus der Liste „Smart Assignments“ verwenden möchten, geben Sie den Namen der gewünschten Ressource ein und wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie **Enter**, um die Zuweisung vorzunehmen.

   Der ausgewählte Benutzer wird der Aufgabe oder dem Problem zugewiesen.
