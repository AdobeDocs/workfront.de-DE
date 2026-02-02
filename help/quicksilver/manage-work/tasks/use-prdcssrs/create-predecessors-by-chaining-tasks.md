---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben
description: Sie können Vorgängerbeziehungen in Adobe Workfront auf verschiedene Weise erstellen. Eine Methode besteht darin, Aufgaben zu verketten.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 6%

---

# Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben

Sie können Vorgängerbeziehungen in Adobe Workfront auf verschiedene Weise erstellen. Eine Methode besteht darin, Aufgaben zu verketten.

Informationen zu Vorgängeraufgaben finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Durch Verketten von Aufgaben können Sie dem System erlauben, die Vorgängerbeziehungen automatisch für ausgewählte Aufgaben zu erstellen, anstatt manuell eine Beziehung zu jeder Aufgabe selbst zu erstellen. Zwischen Aufgaben können weiterhin verschiedene Beziehungstypen für Vorgänger verwendet werden.

## Zugriffsanforderungen

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgaben und das Projekt</p></td> 
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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Verketten von Aufgaben zum Erstellen von Vorgängerbeziehungen

1. Wechseln Sie zu dem Projekt, das die Aufgaben enthält, die Sie verketten möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. (Bedingt) Wählen **oben rechts in** Aufgabenliste die Option „Automatisches Speichern“ und wählen Sie dann die Aufgaben aus, die Sie verketten möchten.

   ![Symbol für automatisches Speichern auf hervorgehoben](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Das Verketten von Aufgaben in einer Aufgabenliste ist nicht möglich, wenn Sie Änderungen an Aufgaben manuell speichern oder den Timeline-Planungsmodus zum Speichern von Aufgaben verwenden.

1. Klicken Sie mit der rechten Maustaste auf die ausgewählten Aufgaben und dann auf **Kette**.
1. Wählen Sie aus den folgenden Abhängigkeitstypen aus:

   * **Beenden-Start**
   * **Beenden-Beenden**
   * **start-start**
   * **Start-Ende**

   Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Optional) Klicken Sie auf **Verkettung aufheben**, wenn einige der Aufgaben zuvor verkettet wurden.

   >[!CAUTION]
   >
   >Nur sequenzielle Vorgänger werden entfernt, indem die Option Verkettung aufheben verwendet wird, wenn Aufgaben zur Massenbearbeitung ausgeführt werden.

   Ihre ausgewählten Aufgaben sind jetzt durch Vorgängerbeziehungen verknüpft.
