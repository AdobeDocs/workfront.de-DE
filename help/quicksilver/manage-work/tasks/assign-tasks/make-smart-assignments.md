---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Smart-Zuweisungen vornehmen
description: Sie können intelligente Zuweisungen verwenden, um zu ermitteln, wer die Arbeit am besten erledigen kann. Intelligente Zuweisungen sind Vorschläge für Benutzende, Rollen oder Teams, die Adobe Workfront Ihnen vorstellt, wenn Sie Ressourcen Arbeitselemente auf der Grundlage eines Algorithmus zuweisen, der die am besten geeignete Ressource für den Auftrag bestimmt. Informationen zu Smart-Zuweisungen finden Sie unter Smart-Zuweisungen - Übersicht .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Smart-Zuweisungen vornehmen

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die nur in der Produktionsumgebung für Kunden verfügbar sind, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> Diese Funktion wird für Kunden, die die Schnellversion mit Version 25.1 im Januar 2025 aktiviert haben, aus der Produktionsumgebung entfernt. Weitere Informationen zur Version 25.1 finden Sie unter [Übersicht über die Version im ersten Quartal 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

Sie können intelligente Zuweisungen verwenden, um zu ermitteln, wer die Arbeit am besten erledigen kann.

Intelligente Zuweisungen sind Vorschläge für Benutzende, Rollen oder Teams, die Adobe Workfront Ihnen beim Zuweisen von Arbeitselementen zu Ressourcen vorlegt. Workfront stützt seine Vorschläge auf einen Algorithmus, der die am besten geeignete Ressource für den Auftrag bestimmt.

<span class="preview">In Workfront gibt es zwei separate Algorithmen zur Berechnung von Smart Assignments, die für Aufgaben und Probleme unterschiedlich funktionieren.</span>

Weitere Informationen über die Kriterien zur Bestimmung von Smart-Zuweisungen finden Sie unter [Smart-Zuweisungen - Übersicht](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
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
   <td> <p>Contribute oder höhere Berechtigungen mit der Möglichkeit, Zuweisungen zu Aufgaben und Problemen vorzunehmen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Smart-Zuweisungen vornehmen

Smart-Zuweisungen sind an den meisten Stellen verfügbar, an denen Sie Zuweisungen in Workfront vornehmen können.

1. Wechseln Sie zu den folgenden Bereichen und klicken Sie auf das Feld **Arbeitsaufträge** oder **Diesen zuweisen zu**:

   * Aufgaben- oder Problemliste oder Bericht
   * Kopfzeile einer Aufgabe oder eines Problems
   * Das Bedienfeld „Aufgaben- oder Problemzusammenfassung“
   * <span class="preview">Eine neue Aufgabe</span> oder ein neues Problem, wenn Sie <span class="preview">eine neue Aufgabe</span> oder ein Problem zu einem Projekt hinzufügen
   * Eine Aufgabe oder ein Problem im Workload Balancer

1. Platzieren Sie den Cursor im Feld Arbeitsaufträge und warten Sie zwei Sekunden.

   Bei Problemen werden die Smart-Zuweisungen in den folgenden Abschnitten angezeigt:

   * **Benutzer und Teams**
   * **Aufgabengebiete**

   ![](assets/smart-assignments-issue-header.png)

   Für Aufgaben werden die Smart Assignments in den folgenden Abschnitten angezeigt, je nachdem, in welcher Phase der Algorithmusberechnung die Zuweisungen identifiziert wurden:

   * <span class="preview">**Vorgeschlagene Zuweisungen**: Zeigt Zuweisungen an, die in der ersten Phase des Smart Assignment-Algorithmus für Aufgaben identifiziert wurden.</span>
   * **Benutzer und Teams**, **Aufgabengebiete** oder <span class="preview">**Tarifkarten-Aufgabengebiete**</span>: Zuweisungen, die in der zweiten Phase der Algorithmusberechnung der Smart-Zuweisung für die Aufgabe identifiziert wurden.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Weitere Informationen finden Sie unter [Smart Assignments - Übersicht](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Wählen Sie die Ressource in der Liste Recommendations aus, indem Sie auf ihren Namen klicken.

1. (Optional) Klicken Sie auf **Mir zuweisen**, um das Arbeitselement sich selbst zuzuweisen.

   >[!TIP]
   >
   >Wenn keine Vorschläge vorliegen, wird die Vorschlagsliste nicht geöffnet.

1. (Optional) Wenn Sie keinen der empfohlenen Benutzer aus der Liste „Smart Assignments“ verwenden möchten, geben Sie den Namen der gewünschten Ressource ein und wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie **Enter**, um die Zuweisung vorzunehmen.

   Der ausgewählte Benutzer wird der Aufgabe oder dem Problem zugewiesen.
