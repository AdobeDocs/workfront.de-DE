---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben
description: Sie können in Adobe Workfront auf verschiedene Weise Vorgängerbeziehungen erstellen. Eine Methode besteht darin, Aufgaben zu verketten.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben

Sie können in Adobe Workfront auf verschiedene Weise Vorgängerbeziehungen erstellen. Eine Methode besteht darin, Aufgaben zu verketten.

Weitere Informationen zu Vorgängeraufgaben finden Sie unter [Übersicht über Aufgabenvorherigen](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Durch das Verketten von Aufgaben können Sie dem System erlauben, die Vorgängerbeziehungen automatisch für ausgewählte Aufgaben zu erstellen, anstatt manuell eine Beziehung für jede Aufgabe selbst zu erstellen. Zwischen Aufgaben können weiterhin verschiedene Vorgänger-Beziehungstypen verwendet werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgaben und das Projekt verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aufgaben verketten, um Vorgängerbeziehungen zu erstellen

1. Wechseln Sie zu dem Projekt, das die Aufgaben enthält, die Sie verketten möchten.
1. Klicken Sie im linken Bereich auf **Aufgaben** .
1. (Bedingt) Wählen Sie oben rechts in der Aufgabenliste die Option **Automatisches Speichern** aus und wählen Sie dann die Aufgaben aus, die Sie verketten möchten.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Das Verketten von Aufgaben in einer Aufgabenliste ist nicht möglich, wenn Sie Änderungen an Aufgaben manuell speichern oder den Timeline-Planungsmodus zum Speichern von Aufgaben verwenden.

1. Klicken Sie mit der rechten Maustaste auf die ausgewählten Aufgaben und klicken Sie dann auf **Kette**.
1. Wählen Sie aus den folgenden Abhängigkeitstypen aus:

   * **finish-start**
   * **Finish-Finish**
   * **Start-Start**
   * **Start-Finish**

   Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Optional) Klicken Sie auf **Unchain** , wenn einige der Aufgaben zuvor verkettet wurden.

   >[!CAUTION]
   >
   >Bei der Massenbearbeitung werden nur sequenzielle Vorgänger mit der Option &quot;Unchain&quot;entfernt.

   Ihre ausgewählten Aufgaben sind nun durch frühere Beziehungen verknüpft.
