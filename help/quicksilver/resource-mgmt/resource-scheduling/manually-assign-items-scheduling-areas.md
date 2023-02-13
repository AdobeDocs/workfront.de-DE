---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen
description: Über die Planung können Sie Benutzerzuweisungen verwalten und festlegen, wie viel Zeit jedem Benutzer für ein Arbeitselement zugewiesen wird.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen

>[!IMPORTANT]
>  
><span class="preview">Die in diesem Artikel beschriebene Planungsfunktion wird seit der Version 23.1 im Januar 2023 nicht mehr unterstützt und aus Adobe Workfront entfernt.   </span>
>  
> <span class="preview"> Dieser Artikel wird auch kurz nach der Version 23.1 (Anfang 2023) entfernt. Zu diesem Zeitpunkt empfehlen wir, alle Lesezeichen entsprechend zu aktualisieren. </span>
> 
><span class="preview"> Sie können jetzt den Lastenausgleich verwenden, um die Arbeit für Ihre Ressourcen zu planen. </span>
>  
> <span class="preview">Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie im Abschnitt [Der Lastenausgleich](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Über die Planung können Sie Benutzerzuweisungen verwalten und festlegen, wie viel Zeit jedem Benutzer für ein Arbeitselement zugewiesen wird.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

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
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte, Aufgaben und Probleme</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen von Berechtigungen zu Projekten, Aufgaben und Problemen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen vor dem Zuweisen von Aufgaben und Problemen in der Zeitleiste &quot;Planung&quot;

Bevor Sie mit der Verwaltung von Benutzerzuweisungen wie in diesem Abschnitt beschrieben beginnen, sollten Sie sich mit der Funktionsweise der Ressourcenplanung in Workfront vertraut machen, wie hier beschrieben: [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Um Benutzerzuweisungen erfolgreich zu verwalten, wie in diesem Abschnitt beschrieben, müssen Sie zunächst sicherstellen, dass Sie, Ihre Projekte sowie Ihre Aufgaben und Probleme die Voraussetzungen erfüllen, die in der [Voraussetzungen für die Verwendung der Planungswerkzeuge in Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) im Artikel [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

In den folgenden Abschnitten wird beschrieben, wie Sie Benutzerzuweisungen manuell, automatisch oder durch Austausch von Zuweisungen nach Benutzer oder Rolle ändern.

## Nicht zugewiesene Aufgaben oder Probleme Benutzern manuell zuweisen

Die Planung bietet die erforderliche Sichtbarkeit, damit Benutzer die Aufgabe oder das Problem abschließen können.\
Weitere Informationen zur Planung finden Sie unter [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Sie können den Benutzern in der Planung einzelne Aufgaben und Probleme aus den folgenden Bereichen von Workfront zuweisen:

* Der Abschnitt Planung unter Ressourcen (bei der Planung von Ressourcen für mehrere Projekte).
* Der Abschnitt Planung unter einem Projekt (beim Planen von Ressourcen für ein einzelnes Projekt).
* Der Abschnitt Planung unter einem Team (beim Planen von Ressourcen für ein Team).

Die im Bereich Nicht zugewiesen am oberen Rand der Planungszeitleiste angezeigten Informationen unterscheiden sich je nach Bereich von Workfront, in dem Sie die Ressourcenplanung verwenden (entweder im Bereich Planung (bei der Planung von Ressourcen für mehrere Projekte), im Bereich Planung (bei der Planung von Ressourcen für ein einzelnes Projekt) oder im Bereich Planung (bei der Planung von Ressourcen für ein Team). Weitere Informationen finden Sie im Abschnitt . [Im Bereich Planung verfügbare Funktionen](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) im Artikel [Übersicht über die Planungsbereiche](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Abhängig vom Bereich von Workfront, in dem Sie die Planung anzeigen, sind möglicherweise nur einige Benutzer berechtigt, Arbeitsaufgaben zugewiesen zu bekommen. Weitere Informationen finden Sie unter [Übersicht über die Planungsbereiche](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

So weisen Sie Benutzern nicht zugewiesene Aufgaben oder Probleme in der Planung zu:

1. Gehen Sie zur Zeitleiste für die Planung mehrerer Projekte, eines einzelnen Projekts oder eines Teams:

   * **Für mehrere Projekte**:  Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen > Lastenausgleich**, wählen Sie **Planung** im Dropdown-Menü oben links.
   * **Für ein einzelnes Projekt**: Wechseln Sie zu einem Projekt, klicken Sie auf die **Lastenausgleich** im linken Bereich, und wählen Sie dann **Planung** aus dem Dropdown-Menü oben links.
   * **Für ein Team**: Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Teams**, wählen Sie ein Team aus, klicken Sie auf **Lastenausgleich** Wählen Sie im linken Bereich die Option **Planung** aus dem Dropdown-Menü oben links.

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. (Optional) Erstellen Sie einen Filter, um anzupassen, welcher Inhalt auf der Zeitleistensegment der Planung angezeigt wird, wie unter [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Damit beispielsweise Probleme in der Planung angezeigt werden, müssen Sie einen Filter erstellen.

1. (Optional) Ändern Sie den Datumsbereich, der auf der Zeitleistensegment der Planung angezeigt wird, wie unter [Datumsbereich der Planungsbereiche anpassen](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Gehen Sie wie folgt vor, um eine nicht zugewiesene Aufgabe oder ein Problem zuzuweisen:

   * Ziehen Sie die Aufgabe oder das Problem in die Zeile des Benutzers, den Sie zuweisen möchten.\
      Für einen bestimmten Benutzer werden maximal 10 Aufgaben pro Tag angezeigt. Sie können die Liste erweitern, um alle Aufgaben anzuzeigen, die diesem Benutzer derzeit zugewiesen sind. (Nach Durchführung von Zuweisungen in der Planung werden möglicherweise vorübergehend mehr als 10 Aufgaben angezeigt.)\
      Beim Ziehen eines Elements werden die folgenden Informationen angezeigt, bevor die Aufgabe oder das Problem freigegeben und die Zuweisung abgeschlossen wird:

   * Wenn die Benutzerzuordnung in der Zeitleiste der Planung aktiviert ist, werden die roten Überzuordnungsanzeiger angezeigt, wenn das Abschließen der Zuweisung dazu führt, dass der Benutzer übergeordnet wird.\
      Weitere Informationen zu Überverteilungsindikatoren finden Sie im Abschnitt . [Zuordnungsindikatoren](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) im Artikel [Verwalten von Benutzerzuweisungen in den Planungsbereichen](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Wenn die Variable **Zuweisung auf Benutzer mit einer übereinstimmenden Rolle begrenzen** im Bereich Einstellungen aktiviert ist, werden Benutzer, die nicht für die Zuweisung berechtigt sind, abgeblendet angezeigt. Wenn diese Option deaktiviert ist, stehen alle Benutzer für den Empfang der Zuweisung zur Verfügung. Die Option ist standardmäßig aktiviert.\
      Weitere Informationen zu dieser Option finden Sie unter [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      In der Zeile des Benutzers wird ein Dropindikator angezeigt. Auf diese Weise können Sie sehen, wo ein Element vor der Zuweisung zugewiesen wird.

      Erweitern Sie die Aufgabe oder das Problem, die/das Sie zuweisen möchten, und klicken Sie auf den Dropdown-Pfeil im **Zuweisungen** eingeben, den Namen des Benutzers eingeben, den Sie zuweisen möchten, und dann in der Dropdown-Liste auf den Namen des Benutzers klicken.\
      ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)

1. (Bedingt) Nachdem Sie einem Benutzer eine nicht zugewiesene Aufgabe oder ein Problem zugewiesen haben, möchten Sie möglicherweise die vorhandenen Zuweisungen für Aufgaben und Probleme unter den Benutzern in der Zeitleiste der Planung anpassen. Beim Planen von Ressourcen für Projekte (entweder auf der Registerkarte Planung oder auf der Registerkarte Zuordnung ) können nur Benutzer mit derselben Auftragsrolle die Zuweisung erhalten.\
   Um eine Aufgabe oder ein Problem einem anderen Benutzer erneut zuzuweisen, ziehen Sie die Aufgabe aus der Zeile eines Benutzers in die Zeile eines anderen Benutzers.
1. (Optional) Konfigurieren Sie die Anzahl der Stunden, die jeder zugewiesene Benutzer der Aufgabe oder dem Problem zugewiesen ist, wie in [Verwalten von Benutzerzuweisungen in den Planungsbereichen](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
