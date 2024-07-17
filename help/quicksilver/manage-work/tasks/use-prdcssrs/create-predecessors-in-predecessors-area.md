---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen einer Vorgängerbeziehung im Bereich "Vorgänger"
description: Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängen, zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei (abhängige Aufgabe) hosten, bevor Sie die Einladungen versenden (vorherige Aufgabe).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Erstellen einer Vorgängerbeziehung im Bereich &quot;Vorgänger&quot;

Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängen, zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei (abhängige Aufgabe) hosten, bevor Sie die Einladungen versenden (vorherige Aufgabe).

Dieser Artikel zeigt, wie Sie in einer Aufgabe mithilfe der Registerkarte &quot;Vorgänger&quot;Vorgänger festlegen können.

Weitere Informationen zum Festlegen von Vorgängern in einer Liste von Aufgaben finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Sie können die Vorgänger von Aufgaben in den folgenden Bereichen von Adobe Workfront anzeigen:

* Im Abschnitt &quot;Vorgänger&quot;der abhängigen Aufgaben
* Im Gantt-Diagramm
* In der Aufgabenliste in der Spalte &quot;Vorgänger&quot;

Weitere Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenverfasser](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## Erstellen eines Vorgängers für eine Aufgabe

1. Wechseln Sie zu einer Aufgabe, die Sie als abhängige Aufgabe festlegen möchten, und klicken Sie dann im linken Bereich auf **Vorgänger** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Vorgänger** klicken.

1. Klicken Sie auf **+Vorgänger hinzufügen**.
1. (Optional) Um einen projektübergreifenden Vorgänger hinzuzufügen, ersetzen Sie den Namen des Projekts im Feld **Übergeordnetes Projekt** durch ein anderes Projekt und geben Sie dann den Namen der Aufgabe oder Aufgaben ein, die Sie als Vorgänger verwenden möchten.

   Weitere Informationen zum Hinzufügen projektübergreifender Vorgänger finden Sie unter [Erstellen projektübergreifender Vorgänger](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Geben Sie den Namen der Aufgabe bzw. der Aufgaben ein, die Sie als Vorgänger festlegen möchten.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Wählen Sie einen **Abhängigkeitstyp** aus.

   Weitere Informationen zu Aufgabenabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie einen **Lag** -Betrag in Tagen an.

   Informationen zu Lag-Typen finden Sie unter &#x200B; [Übersicht über Lag-Typen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Wählen Sie **Erzwungen** aus, wenn Sie die Vorgängerbeziehung zwischen den beiden Aufgaben erzwingen möchten.

   Weitere Informationen zum Durchsetzen von Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klicken Sie auf **Speichern**.
