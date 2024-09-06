---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zuweisen von Massenarbeit mithilfe des Lastenausgleichs
description: Sie können mithilfe des Adobe Workfront Workload Balancer Ressourcen mehreren Aufgaben und Problemen in großen Mengen zuweisen.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 1%

---

# Stapelweises Zuweisen von Arbeiten mithilfe des Lastenausgleichs

<!--Audited: 07/2024-->

Sie können mithilfe des Adobe Workfront Workload Balancer Ressourcen mehreren Aufgaben und Problemen in großen Mengen zuweisen.

Allgemeine Informationen zum Zuweisen von Arbeit zu Benutzern mithilfe des Workload-Balancers finden Sie unter [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie bei Verwendung des Workload-Balancers im Ressourcenbereich;</br>
       Arbeiten bei Verwendung des Workload Balancers für ein Team oder Projekt</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Contribute-Berechtigungen oder höher für die Projekte, Aufgaben und Probleme, die Zuweisungen beinhalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Durchführen von Massenzuweisungen im Arbeitslastausgleich

* Sie können Benutzerzuweisungen schnell für mehrere Aufgaben und Probleme in einem oder mehreren Projekten verwalten. Änderungen bei Zuweisungen sind sofort im Arbeitslastausgleich sichtbar.
* Sie können keine Ressourcen für abgeschlossene Arbeitselemente oder für Elemente zuweisen, die sich in einem abgeschlossenen Projekt befinden.
* Sie können Folgendes tun, wenn Sie Benutzer stapelweise zuweisen:

   * Weisen Sie einen Benutzer allen Arbeitselementen zu, die derzeit einer Auftragsrolle zugewiesen sind.
   * Ersetzen Sie Benutzerzuweisungen zwischen Benutzern.
   * Heben Sie die Zuweisung eines Benutzers zu allen Arbeitselementen auf.

**BEISPIELE**

* Sie sind für die Benutzerzuweisung an mehreren neuen Projekten verantwortlich. Die Projekte wurden ursprünglich aus Vorlagen erstellt und die verschiedenen Aufgaben innerhalb der Projekte sind bereits mit den verschiedenen Aufgaben verbunden. Sie möchten allen Aufgaben, die derzeit einer Job-Rolle zugewiesen sind, einen bestimmten Benutzer, Jackie Simms, zuweisen. Sie können die Funktion Zuweisen verwenden, um diese Aufgaben Jackie Simms zuzuweisen.
* Jackie Simms wird 45 Aufgaben aus 3 verschiedenen Projekten zugewiesen. Jackie verlässt die Organisation und jetzt müssen Sie ihre Aufgaben einem anderen Benutzer neu zuweisen. Sie können die Funktion &quot;Ersetzen&quot;verwenden, um diese Aufgaben der neuen Person zuzuweisen.
* 10 Aufgaben aus 2 verschiedenen Projekten werden einem anderen Benutzer, Rick Kuvec, zugewiesen. Sie erkennen, dass Rick diesen Aufgaben irrtümlich zugewiesen wurde, aber Sie sind sich nicht sicher, wem sie zu diesem Zeitpunkt zugewiesen werden müssen. Sie müssen die Zuweisung von Rick zu allen Aufgaben gleichzeitig aufheben. Mit der Funktion &quot;Zuweisung aufheben&quot;können Sie Rick aus diesen Aufgaben entfernen.

## Stapelweises Zuweisen von Arbeiten im Arbeitslastausgleich

1. Wechseln Sie zum Arbeitslast-Balancer, dem Sie Arbeit zuweisen möchten.

   Sie können Benutzern mithilfe des Lastenausgleichs im Bereich &quot;Ressourcen&quot;, auf Projekt- oder Teamebene Arbeit zuweisen. Weitere Informationen darüber, wo sich der Arbeitslast-Balancer in Workfront befindet, finden Sie unter [Suchen des Arbeitslast-Balancers](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Klicken Sie oben im Arbeitslastausgleich auf **Massenzuweisungen** ![](assets/bulk-assignments-wb.png) .

   Das Bedienfeld &quot;Massenzuweisungen&quot;wird rechts neben dem Arbeitslastausgleich geöffnet.

1. (Bedingt) Wenn Sie über den Bereich &quot;Ressourcen&quot;oder für ein Team auf den Arbeitslastausgleich zugreifen, erweitern Sie das Dropdown-Menü **Projekt: Name** und wählen Sie mit den Filtermodifikatoren das Projekt oder die Projekte aus, für die Sie Zuweisungen vornehmen möchten. Sie können Projekte nach Name (dies ist die Standardoption) oder nach Status auswählen.

   Weitere Informationen zu Workfront-Filtermodifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Der Projektname wird standardmäßig ausgewählt, wenn Sie auf den Lastenausgleich für ein Projekt zugreifen.

   ![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Optional) Klicken Sie auf **Projektaufgaben auswählen** , um die Aufgaben auszuwählen, für die Sie Zuweisungen vornehmen möchten. Wählen Sie dann im Dropdown-Menü **Aufgabe: Name** Aufgaben nach Name (dies ist die Standardoption) oder Status aus und verwenden Sie die Filter-Modifikatoren, um nach bestimmten Aufgaben zu suchen.

   Weitere Informationen zu Workfront-Filtermodifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Sie können keine Aufgaben im Status Abgeschlossen auswählen.

   ![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >Lassen Sie diese Auswahl leer, wenn Sie Massenzuweisungen für Probleme sowie Aufgaben vornehmen möchten.

1. (Optional) Klicken Sie neben einem der ausgewählten Kriterien auf das Symbol **Löschen** ![](assets/delete.png)

   Oder

   Klicken Sie oben rechts im Bedienfeld &quot;Massenzuweisungen&quot;auf **Alle löschen** , um alle Auswahlen zu entfernen.

1. Wählen Sie eine der folgenden Optionen aus und fahren Sie mit den unten beschriebenen Schritten fort:

   * [Benutzer zuweisen](#assign-user)
   * [Benutzer ersetzen](#replace-user)
   * [Zuweisung des Benutzers aufheben](#unassign-user)

   >[!TIP]
   >
   >Wenn keine Elemente mit den ausgewählten Filtern übereinstimmen, werden diese Optionen abgeblendet angezeigt.

### Benutzer zuweisen {#assign-user}

Wenn Sie einen Benutzer mit der Funktion &quot;Massenzuweisungen&quot;im Arbeitslastausgleich zuweisen, treten die folgenden Dinge auf:

* Ein Benutzer wird allen Arbeitselementen zugewiesen, die derzeit innerhalb der ausgewählten Projekte einer bestimmten Rolle zugewiesen sind.
* Der Benutzer wird den folgenden Arten von Arbeitselementen nicht zugewiesen:

   * Elemente, die bereits einem Benutzer zugewiesen sind.
   * Abgeschlossene Elemente.

* Wenn der ausgewählte Benutzer nicht mit der angegebenen Rolle verknüpft ist, wird die Rolle durch den Benutzer in der Primären Rolle des Benutzers ersetzt.

So weisen Sie einen Benutzer Arbeitselementen zu, die zuvor Auftragsrollen zugewiesen wurden:

1. Beginnen Sie mit der Zuweisung von Arbeitselementen mithilfe von Massenzuweisungen im Arbeitslade-Balancer wie oben beschrieben und wählen Sie **Zuweisen** aus.

1. Klicken Sie im Feld **Rollenzuweisung** auf den Dropdown-Pfeil, um aus einer Liste von Rollen auszuwählen. Es werden nur Rollen angezeigt, die derzeit innerhalb der angegebenen Projekte zugewiesen sind. Dies ist ein Pflichtfeld.

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. Klicken Sie im Feld **Benutzer, der zugewiesen werden soll** auf den Dropdown-Pfeil, um aus einer Liste der vorgeschlagenen Benutzer auszuwählen oder den Namen eines anderen Benutzers einzugeben.

   Wählen Sie Benutzer aus den folgenden Bereichen aus:

   * **Vorgeschlagene Zuweisungen**: Benutzer, die die ausgewählte Rolle erfüllen und die Kriterien für Smart-Zuweisungen erfüllen. Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Sonstige Zuweisungen**: Alle Benutzer im System, die die ausgewählte Rolle erfüllen können.

     >[!TIP]
     >
     >Nur die ersten 50 Benutzer werden im Bereich &quot;Andere Zuweisungen&quot;aufgelistet.


   Nachdem Sie einen Benutzer ausgewählt haben, zeigt Workfront einen Hinweis zur Anzahl der Elemente an, denen der von Ihnen festgelegte Benutzer zugewiesen wird, und zu der Rolle, die er ersetzen wird.

   >[!TIP]
   >
   >Alle Rollen des Benutzers werden in der Liste unter dem Namen des Benutzers angezeigt.


1. Klicken Sie auf **Zuweisen**.

   Die angegebenen Rollen werden durch die von Ihnen ausgewählten Benutzer ersetzt.

   Sie erhalten eine Bestätigung darüber, wie viele Arbeitselemente mit der ausgewählten Rolle durch den ausgewählten Benutzer ersetzt wurden.

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Benutzer ersetzen {#replace-user}

Sie können einen Benutzer, der bereits Arbeitselementen zugewiesen ist, in den ausgewählten Projekten durch einen anderen Benutzer ersetzen.

Wenn Sie einen Benutzer durch einen anderen Benutzer ersetzen, der Massenzuweisungen im Arbeitslastausgleich verwendet, treten die folgenden Dinge auf:

* Der Ersatzbenutzer wird allen Arbeitselementen zugewiesen, die derzeit einem ursprünglichen Benutzer innerhalb der ausgewählten Projekte zugewiesen sind.

* Der neue Benutzer wird keinen Arbeitselementen zugewiesen, die bereits als Fertig gestellt markiert sind.
* Wenn die dem ersten Benutzer zugeordnete Rolle keiner der Rollen des zweiten Benutzers entspricht, wird der zweite Benutzer in seiner Primären Rolle zugewiesen.

So ersetzen Sie einen Benutzer durch einen anderen:

1. Beginnen Sie mit dem Zuweisen von Arbeitselementen im Arbeitslastausgleich wie oben beschrieben und wählen Sie **Ersetzen** aus.
1. Klicken Sie im Feld **Aktuell zugewiesener Benutzer** auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen. Es werden nur Benutzer angezeigt, die innerhalb der angegebenen Projekte unvollständigen Arbeitselementen zugewiesen sind. Dies ist ein Pflichtfeld.

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. Klicken Sie im Feld **Benutzer, der zugewiesen werden soll** auf den Dropdown-Pfeil, um aus einer Liste der vorgeschlagenen Benutzer auszuwählen oder einen anderen Benutzernamen einzugeben. Die in der Liste aufgeführten Benutzer entsprechen standardmäßig den Kriterien für Smart-Zuweisungen. Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront zeigt einen Hinweis zur Anzahl der Elemente an, bei denen der aktuell zugewiesene Benutzer den zweiten Benutzer ersetzt und welche Rollen ersetzt werden.

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Klicken Sie auf **Replace**.

   Der erste ausgewählte Benutzer wird in allen Arbeitselementen des ausgewählten Projekts durch den zweiten Benutzer ersetzt.

   Sie erhalten eine Bestätigung darüber, wie viele Arbeitselemente die ursprüngliche Benutzerzuweisung durch den ausgewählten zweiten Benutzer ersetzt haben.

### Zuweisung des Benutzers aufheben {#unassign-user}

Sie können die Zuweisung eines Benutzers zu allen Arbeitselementen aufheben, denen der Benutzer in den ausgewählten Projekten zugewiesen ist.

Wenn Sie die Zuweisung eines Benutzers zu all seinen Zuweisungen mithilfe von Massenzuweisungen im Arbeitslastausgleich aufheben, treten die folgenden Dinge auf:

* Der angegebene Benutzer wird aus allen Arbeitselementen entfernt, denen er zugewiesen ist.
* Wenn der nicht zugewiesene Benutzer mit Auftragsrollen verknüpft ist, bleiben die Aufgabenrollen den Arbeitselementen zugewiesen, wenn der Benutzer entfernt wird.

* Wenn der angegebene Benutzer Arbeitselementen zugewiesen ist, die abgeschlossen sind, bleibt der Benutzer diesen Arbeitselementen zugewiesen.

Weitere Informationen zu Benutzer- und Aufgabenrollenzuweisungen finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

So heben Sie die Zuweisung eines Benutzers zu Arbeitselementen in den ausgewählten Projekten oder für die ausgewählten Aufgaben oder Probleme auf, denen er zugewiesen ist:

1. Beginnen Sie mit dem Zuweisen von Arbeitselementen im Arbeitslastausgleich wie oben beschrieben und wählen Sie **Zuweisung aufheben** aus.

1. Klicken Sie im Feld **Benutzer, dessen Zuweisung aufgehoben werden soll** auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen. Es werden nur Benutzer angezeigt, die derzeit unvollständigen Arbeitselementen innerhalb der angegebenen Projekte zugewiesen sind. Dies ist ein Pflichtfeld.

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront zeigt einen Hinweis zur Anzahl der Elemente an, für die die Zuweisung des aktuell zugewiesenen Benutzers aufgehoben wird.

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Klicken Sie auf **Zuweisung aufheben**.\
   Sie erhalten eine Bestätigung über die Anzahl der Arbeitselemente, in denen der angegebene Benutzer entfernt wurde.


