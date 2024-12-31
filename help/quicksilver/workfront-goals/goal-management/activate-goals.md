---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktivieren von Zielen in Adobe Workfront Goals
description: Wenn Sie ein Ziel erstellen, wird es von Adobe Workfront Goals mit dem Status Entwurf gespeichert. Entworfene Ziele sind nicht Teil des Zielmanagements.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---

# Aktivieren von Zielen in Adobe Workfront Goals

Wenn Sie ein Ziel erstellen, wird es von Adobe Workfront Goals mit dem Status Entwurf gespeichert. Entworfene Ziele sind nicht Teil des Zielmanagements.

Um zu verfolgen, wie nahe Sie einem Ziel sind, indem Sie dessen Fortschritt aktualisieren, müssen Sie es aktivieren. Dadurch wird der Status in „Aktiv“ geändert.

Informationen zum Erstellen eines Ziels finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Sie müssen ein Ziel aktivieren, bevor Sie den Fortschritt seiner Ergebnisse und Aktivitäten aktualisieren können.


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für die neue Plan- und Lizenzstruktur:
  <ul><li>Ein Ultimate-Plan </li></ul>
   </p>
<p>Für die aktuelle Plan- und Lizenzstruktur: 
<ul><li> Ein Profi oder höher </li>
  <li>Eine Adobe Workfront-Ziellizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitwirkende oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderung, eine der folgenden: </p>
<ul>
<li>Einen ausgewählten oder Prime Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderung: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Voraussetzungen

Um ein Ziel zu aktivieren, muss das Ziel mit einer Fortschrittsanzeige wie einer Aktivität, einem Ergebnis oder einem Projekt verknüpft oder mit einem anderen aktiven Ziel ausgerichtet sein.

Führen Sie mindestens einen der folgenden Schritte aus, um ein Ziel aktivieren zu können:

* Ergebnis zum Ziel hinzufügen

  Weitere Informationen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Hinzufügen einer Aktivität zum Ziel

  Weitere Informationen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Verbinden eines Projekts mit dem Ziel

  Weitere Informationen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).

* Ein weiteres Ziel an dem Ziel ausrichten, das Sie aktivieren möchten

  Weitere Informationen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Aktivieren von Zielen

Sie können Ziele aktivieren, die Sie erstellt haben, oder ein Ziel, für das Sie über Verwaltungsberechtigungen verfügen.

1. Navigieren Sie zu einem Ziel, das Sie aktivieren möchten. Die Zielseite wird geöffnet.

1. Klicken Sie auf **Mehr**-![](../goal-management/assets/more-icon.png) rechts neben dem Zielnamen und dann auf **Aktivieren**.

   ![](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   Der Zielstatus ändert sich in Aktiv. Sie können jetzt den Fortschritt beim Ziel verfolgen. Das Ziel wird im Abschnitt Einchecken angezeigt und wird in den Diagrammabschnitten der Workfront-Ziele berücksichtigt
