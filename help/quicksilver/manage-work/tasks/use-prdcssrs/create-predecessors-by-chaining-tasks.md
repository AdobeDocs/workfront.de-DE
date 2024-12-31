---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben
description: Sie können Vorgängerbeziehungen in Adobe Workfront auf verschiedene Weise erstellen. Eine Methode besteht darin, Aufgaben zu verketten.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben

Sie können Vorgängerbeziehungen in Adobe Workfront auf verschiedene Weise erstellen. Eine Methode besteht darin, Aufgaben zu verketten.

Informationen zu Vorgängeraufgaben finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Durch Verketten von Aufgaben können Sie dem System erlauben, die Vorgängerbeziehungen automatisch für ausgewählte Aufgaben zu erstellen, anstatt manuell eine Beziehung zu jeder Aufgabe selbst zu erstellen. Zwischen Aufgaben können weiterhin verschiedene Beziehungstypen für Vorgänger verwendet werden.

## Zugriffsanforderungen

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgaben und das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Verketten von Aufgaben zum Erstellen von Vorgängerbeziehungen

1. Wechseln Sie zu dem Projekt, das die Aufgaben enthält, die Sie verketten möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. (Bedingt) Wählen **oben rechts in** Aufgabenliste die Option „Automatisches Speichern“ und wählen Sie dann die Aufgaben aus, die Sie verketten möchten.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

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
