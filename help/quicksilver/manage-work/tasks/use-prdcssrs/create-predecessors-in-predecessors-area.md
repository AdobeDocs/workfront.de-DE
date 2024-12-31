---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen einer Vorgängerbeziehung mithilfe des Bereichs „Vorgänger“
description: Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei hosten (abhängige Aufgabe), bevor Sie die Einladungen versenden (Vorgängeraufgabe).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Erstellen einer Vorgängerbeziehung mithilfe des Bereichs „Vorgänger“

Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei hosten (abhängige Aufgabe), bevor Sie die Einladungen versenden (Vorgängeraufgabe).

Dieser Artikel zeigt, wie Sie in einer Aufgabe mithilfe der Registerkarte Vorgänger Vorgänger Vorgänger festlegen können.

Informationen zum Festlegen von Vorgängern in einer Aufgabenliste finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Sie können die Vorgänger von Aufgaben in den folgenden Bereichen von Adobe Workfront anzeigen:

* Im Abschnitt Vorgänger der abhängigen Aufgaben
* Im Gantt-Diagramm
* In der Aufgabenliste in der Spalte Vorgänger

Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## Vorgänger für eine Aufgabe erstellen

1. Wechseln Sie zu einer Aufgabe, der Sie eine abhängige Aufgabe zuweisen möchten, und klicken Sie dann im linken Bereich **Vorgänger**.

   Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Vorgänger** klicken.

1. Klicken Sie auf **+ Vorgänger hinzufügen**.
1. (Optional) Um einen projektübergreifenden Vorgänger hinzuzufügen, ersetzen Sie den Namen des Projekts im Feld **Übergeordnetes Projekt** durch ein anderes Projekt und geben Sie dann den Namen der Aufgabe oder der Aufgaben ein, die Sie als Vorgänger hinzufügen möchten.

   Informationen zum Hinzufügen von projektübergreifenden Vorgängern finden Sie unter [Erstellen von projektübergreifenden Vorgängern](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Geben Sie den Namen der Aufgabe(n) ein, die Sie als Vorgänger festlegen möchten.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Wählen Sie einen **Abhängigkeitstyp** aus.

   Informationen zu Aufgabenabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie einen **Verzögerung**-Betrag in Tagen an.

   Weitere Informationen zu Verzögerungsarten finden Sie unter &#x200B; [Übersicht über Verzögerungsarten](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Wählen **Erzwungen** aus, wenn Sie die Vorgängerbeziehung zwischen den beiden Aufgaben erzwingen möchten.

   Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klicken Sie auf **Speichern**.
