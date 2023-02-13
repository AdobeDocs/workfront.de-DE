---
product-area: resource-management
navigation-topic: resource-scheduling
title: Mehrere Benutzerzuweisungen zu Aufgaben in den Planungsbereichen ändern
description: Ändern Sie die Zuweisung mehrerer Benutzer zu Aufgaben in den Planungsbereichen.
author: Alina
feature: Resource Management
exl-id: 545a5033-a09e-4019-a10e-c388cf977ae4
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# Mehrere Benutzerzuweisungen zu Aufgaben in den Planungsbereichen ändern


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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

This article refers to modifying user assignments for multiple tasks using the Scheduling area of Adobe Workfront. Also see the following articles for modifying assignments on multiple tasks in other areas:

* For information about modifying assignments on multiple tasks in a task list, see [Modify multiple user assignments in a task list](../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md). 
* For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
-->
Sie können Benutzer gleichzeitig mehreren Aufgaben zuweisen, wenn Sie den Ressourcen-Planer verwenden.

>[!NOTE]
>
>Dieser Artikel gilt nur bei der Planung von Ressourcen für mehrere Projekte (im Abschnitt Planung ) oder für ein einzelnes Projekt (im Abschnitt Planung ). Sie können Benutzerzuweisungen für mehrere Aufgaben nicht wie in diesem Abschnitt beschrieben verwalten, wenn Sie Ressourcen für ein Team planen (siehe Abschnitt Planung ).

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
   <td role="rowheader">Übersicht über Adobe Workfront-Lizenzen*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte, Aufgaben und Probleme</p> <p><b>NOTE</b> Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen, für die Sie Zuweisungen aktualisieren.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Ausführen mehrerer Zuweisungen in den Planungsbereichen

Sie können Benutzerzuweisungen für mehrere Aufgaben und Probleme in einem oder mehreren Projekten schnell verwalten (Änderungen werden dann in der Planung widergespiegelt).

Sie können einen Benutzer allen Aufgaben zuweisen, die derzeit einer Auftragsrolle zugewiesen sind, die Benutzerzuweisungen zwischen Benutzern austauschen oder die Zuweisung eines Benutzers zu allen Aufgaben aufheben.

Beispiel:

* Ein Ressourcen-Manager ist für die Zuweisung von Benutzern zu einem neuen Projekt verantwortlich. Das Projekt wurde ursprünglich als Vorlage erstellt und die verschiedenen Aufgaben im Projekt sind bereits mit den verschiedenen Aufgaben verbunden. Der Ressourcen-Manager möchte allen Aufgaben, die derzeit einer Auftragsrolle zugewiesen sind, einen bestimmten Benutzer zuweisen.
* Jackie Simms wird 45 Aufgaben aus 3 verschiedenen Projekten zugewiesen. Jackie verlässt die Organisation und jetzt muss der Ressourcen-Manager ihre Aufgaben einem anderen Benutzer neu zuweisen.

>[!NOTE]
>
>Beachten Sie beim Verwalten von Benutzerzuweisungen für mehrere Aufgaben die folgenden Einschränkungen:
>
>* Beim Planen von Ressourcen für mehrere Projekte müssen die von Ihnen verwalteten Projekte einen der folgenden Status aufweisen (oder einen Status, der mit einem dieser Status übereinstimmt): Planung, Aktuell oder Genehmigt. Weitere Informationen zum Projektstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Bei der Planung von Ressourcen für ein einzelnes Projekt hat der Projektstatus keine Auswirkungen auf die Verfügbarkeit dieser Funktion.
>* Sie können Ressourcenänderungen für Benutzer mit den folgenden Lizenzen vornehmen: Planen, Arbeiten und Überprüfen. Sie können keine Ressourcenänderungen für Benutzer mit einer Anforderungslizenz vornehmen.
>


## Benutzerzuweisungen für ein oder mehrere Projekte verwalten

1. Gehen Sie zur Zeitleiste für die Planung mehrerer Projekte oder einzelner Projekte:

   * **Für mehrere Projekte**:  Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen > Lastenausgleich**, wählen Sie **Planung** im Dropdown-Menü oben links.
   * **Für ein einzelnes Projekt**: Wechseln Sie zu einem Projekt, klicken Sie auf die **Lastenausgleich** im linken Bereich, und wählen Sie dann **Planung** aus dem Dropdown-Menü oben links.

1. Klicken **Aktionen**.\
   ![resource_scheduling.png](assets/resource-scheduling.png)

1. Im **Projekt auswählen** Gehen Sie je nachdem, ob Sie die Planung für mehrere Projekte (auf der Registerkarte Planung ) oder für ein einzelnes Projekt (auf der Registerkarte Strukturierung ) anzeigen, wie folgt vor:

   * **Für mehrere Projekte:** Beginnen Sie mit der Eingabe des Namens des Projekts, an dem Sie Zuweisungsänderungen vornehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird. Oder klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Projekten auszuwählen. Wiederholen Sie diesen Vorgang, um Zuweisungsänderungen über mehrere Projekte hinweg vorzunehmen.\
      Lassen Sie dieses Feld leer, um Zuweisungsänderungen an allen Projekten vorzunehmen, für die Sie der Ressourcen-Manager sind.

      >[!NOTE]
      >
      >Projekte können nur ausgewählt werden, wenn:
      >
      >   
      >   
      >   * Sie sind im Projekt als Ressourcen-Manager benannt.\
         >     Weitere Informationen finden Sie unter [Ressourcen-Manager für ein Projekt oder eine Vorlage bestimmen](../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md).
      >   
      >   * Das Projekt weist einen der folgenden Status auf (oder einen Status, der mit einem dieser Status übereinstimmt): Planung, aktuell oder genehmigt\
         >     Weitere Informationen zum Projektstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
      >   
      >   * Sie sind Benutzer mit einer Planungslizenz.


   * **Für ein einzelnes Projekt:** Die **Projekt auswählen** -Feld kann nicht geändert werden. Die **Projekt auswählen** -Feld enthält immer den Namen des Projekts, das Sie anzeigen.

1. (Optional) Klicken Sie auf **Aufgaben angeben** , um Zuweisungsänderungen für einzelne Aufgaben zu ändern. Wenn Sie einzelne Aufgaben angeben, werden alle Projekte ausgewählt, die Sie in der **Projekt auswählen** -Feld ignoriert werden.\
   Im **Aufgaben auswählen** eingeben, beginnen Sie mit der Eingabe des Namens der Aufgabe, an der Sie Zuweisungsänderungen vornehmen möchten. Wiederholen Sie diesen Schritt, um Zuweisungsänderungen an zusätzlichen Aufgaben vorzunehmen.\
   Wenn Sie dieses Feld leer lassen, sind alle Aufgaben innerhalb der in Schritt 3 ausgewählten Projekte betroffen.\
   Wenn Sie Zuweisungsänderungen an einzelnen Aufgaben vornehmen, werden Änderungen auf alle Unteraufgaben für die von Ihnen angegebenen Aufgaben angewendet. Änderungen werden auch auf alle Probleme angewendet, die mit den Aufgaben verbunden sind, wenn Probleme so konfiguriert sind, dass sie in der Planung angezeigt werden, wie beschrieben in [Sie können verschiedene Einstellungen konfigurieren, um anzupassen, wie und welche Informationen in der Planung angezeigt werden.](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md#configuring-issues-to-display-on-the-scheduling-timeline) in [Einstellungen in den Planungsbereichen konfigurieren](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md).

1. Fahren Sie mit einem der folgenden Abschnitte fort:

   * [Benutzer zuweisen](#assign-a-user)
   * [Benutzer austauschen](#swap-a-user)
   * [Zuweisung eines Benutzers aufheben](#unassign-a-user)

### Benutzer zuweisen {#assign-a-user}

Sie können einen Benutzer allen Aufgaben zuweisen, die derzeit innerhalb der ausgewählten Projekte einer bestimmten Rolle zugewiesen sind.

Wenn Sie einen Benutzer auf diese Weise zuweisen, wird der Benutzer nicht den folgenden Arten von Aufgaben zugewiesen:

* Zuweisungen zu Aufgaben, die bereits einem Benutzer zugewiesen sind
* Abgeschlossene Aufgaben

So weisen Sie einen Benutzer während der ausgewählten Projekte oder Aufgaben Aufgaben zu:

1. Auswählen **Benutzer zuweisen** im **Aktion auswählen** Abschnitt.\
   ![](assets/resource-scheduling-assign-350x678.png)

1. Im **Rolle auswählen** klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Rollen auszuwählen. Es werden nur Rollen angezeigt, die Aufgaben innerhalb der angegebenen Projekte zugewiesen sind.\
   Wenn Sie einen Benutzer zuweisen, ersetzt der Benutzer die Rollen, die Sie hier auswählen.

1. Im **Benutzer zum Zuweisen auswählen** klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen.\
   Wenn die Variable **Zuweisung auf Benutzer mit einer übereinstimmenden Rolle begrenzen** im Bereich Einstellungen aktiviert ist, können Benutzer nur auswählen, wenn ihnen die ausgewählte Rolle in ihren Benutzereinstellungen zugewiesen ist (entweder als Primäre Rolle oder als Sonstige Rolle). Wenn diese Option deaktiviert ist, können Sie mit der Eingabe des Namens eines anderen Benutzers beginnen, den Sie zuweisen möchten, auch wenn für diesen Benutzer im System keine entsprechende Rolle definiert ist. Die Option ist standardmäßig aktiviert.\
   Weitere Informationen zu dieser Option finden Sie unter [Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). Standardmäßig können Zuweisungen nur Benutzern vorgenommen werden, die eine Rolle in ihrem Benutzerprofil definiert haben, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die/das ihnen zugewiesen wird.

1. Klicken **Zuweisen**.\
   Sie können maximal 1.000 Zuweisungen in einer einzigen Aktion vornehmen. Wenn die von Ihnen vorgenommenen Auswahlen mehr als 1.000 Zuweisungsänderungen bewirken, müssen Sie Ihre Auswahl neu anpassen und es erneut versuchen.

### Benutzer austauschen {#swap-a-user}

Sie können die Aufgabenzuweisungen eines Benutzers durch Aufgabenzuweisungen eines anderen Benutzers in den ausgewählten Projekten oder für die ausgewählten Aufgaben ersetzen.

Wenn Sie die Aufgabenzuweisungen eines Benutzers wie in diesem Abschnitt beschrieben austauschen, werden bereits als &quot;Abgeschlossen&quot;gekennzeichnete Zuweisungen nicht vertauscht.

So tauschen Sie die Aufgabenzuweisungen eines Benutzers durch die Aufgabenzuweisungen eines anderen Benutzers aus:

1. Auswählen **Benutzer tauschen** im **Aktion auswählen** Abschnitt.\
   ![](assets/resource-scheduling-swap-350x674.png)

1. Im **Benutzer auswählen** klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen (oder beginnen Sie mit der Eingabe des Namens des Benutzers, den Sie austauschen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird).\
   Benutzer werden nur angezeigt, wenn sie innerhalb der angegebenen Projekte einer oder mehreren unvollständigen Aufgaben zugewiesen sind.

1. (Bedingt) Die Variable **Rolle auswählen** wird nur angezeigt, wenn der ausgewählte Benutzer mehreren Aufgaben mit unterschiedlichen Rollen zugewiesen ist. (Informationen zum Anzeigen der für die Aufgabe festgelegten Aufgabenrolle für einen Benutzer finden Sie in der **Rolle des Bevollmächtigten** im Dialogfeld &quot;Erweiterte Zuweisung&quot;für die Aufgabe, wie beschrieben in [Erweiterte Zuweisungen erstellen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)).\
   Im **Rolle auswählen** -Feld die Rolle auswählen, um die Art der Aufgaben zu bestimmen, die Sie austauschen möchten. Dem neuen Benutzer werden nur die Aufgaben zugewiesen, denen der Benutzer diese Rolle zugewiesen hat.\
   Hanna Marin wird beispielsweise fünf Aufgaben für das Projekt zugewiesen. Bei 2 der Aufgaben wird ihre berufliche Rolle als &quot;Ingenieur&quot;definiert. Bei den restlichen 3 ihrer Aufgaben wird ihre Rolle als &quot;Designer&quot;definiert. Wenn Sie Designer im Feld &quot;Rolle auswählen&quot;auswählen, möchten Sie die Zuweisung für alle 3 Aufgaben von Hanna ändern, für die ihre Rolle als &quot;Designer&quot;definiert ist. Die beiden Aufgaben, bei denen ihre berufliche Rolle als &quot;Ingenieur&quot;definiert ist, bleiben unverändert.\
   ![](assets/resource-scheduling-swap-role.png)

1. Im **Benutzer zum Zuweisen auswählen** klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen. Benutzer können nur dann zugewiesen werden, wenn ihre Rollen (wie in den Benutzereinstellungen definiert) mit den Rollen der Arbeit übereinstimmen, die dem zu ersetzenden Benutzer zugewiesen ist.\
   Wenn die Variable **Zuweisung auf Benutzer mit einer übereinstimmenden Rolle begrenzen** aktiviert ist, können Benutzer nur dann im Bereich Einstellungen zugewiesen werden, wenn ihre Rollen (wie in den Benutzereinstellungen definiert) mit den Rollen der zu ersetzenden Benutzer übereinstimmen. Wenn diese Option deaktiviert ist, können Sie mit der Eingabe des Namens eines anderen Benutzers beginnen, den Sie zuweisen möchten, auch wenn für diesen Benutzer im System keine entsprechende Rolle definiert ist. Die Option ist standardmäßig aktiviert.\
   Weitere Informationen zu dieser Option finden Sie unter [Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md). Standardmäßig können Zuweisungen nur Benutzern vorgenommen werden, die eine Rolle in ihrem Benutzerprofil definiert haben, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die/das ihnen zugewiesen wird.\
   Wenn der Benutzer, den Sie ersetzen, in mehreren Rollen für Aufgaben in den ausgewählten Projekten zugewiesen ist und Sie mehrere Rollen in der **Rolle auswählen** -Feld, die **Benutzer zum Zuweisen auswählen** zeigt nur Benutzer an, die alle angegebenen Rollen haben.

1. Klicken **Tauschen**.\
   Sie können maximal 1.000 Zuweisungen in einer einzigen Aktion vornehmen. Wenn die von Ihnen vorgenommenen Auswahlen mehr als 1.000 Zuweisungsänderungen bewirken, müssen Sie Ihre Auswahl neu anpassen und es erneut versuchen.

### Zuweisung eines Benutzers aufheben {#unassign-a-user}

Sie können die Zuweisung eines Benutzers zu allen Aufgaben, denen der Benutzer in den ausgewählten Projekten oder für die ausgewählten Aufgaben zugewiesen ist, aufheben. Wenn Sie die Zuweisung eines Benutzers aufheben, werden alle diesem Benutzer zugewiesenen Aufgaben wieder in den Zuweisungsstatus zurückgesetzt, bevor der Benutzer zugewiesen wurde.

Wenn für einen Benutzer eine primäre Rolle im System definiert ist und Sie die Zuweisung des Benutzers aufheben, wird die Aufgabe automatisch der primären Rolle des Benutzers zugewiesen, wenn Sie die Zuweisung des Benutzers aufheben. Oder sie wird der Rolle zugewiesen, der sie vor der Zuweisung des Benutzers zugewiesen wurde.

Wenn für einen Benutzer keine primäre Rolle im System definiert ist und Sie die Zuweisung des Benutzers aufheben, wird die Aufgabe beim Aufheben der Zuweisung des Benutzers in einen nicht zugewiesenen Status versetzt.

Aufgaben, die als &quot;Abgeschlossen&quot;markiert sind, können nicht zugewiesen werden.

So heben Sie die Zuweisung eines Benutzers zu Aufgaben im gesamten ausgewählten Projekt oder für die ausgewählten Aufgaben auf:

1. Auswählen **Benutzer aufheben** im **Aktion auswählen** Abschnitt.\
   ![](assets/resource-scheduling-unassign-350x618.png)

1. Im **Benutzer auswählen** klicken Sie auf den Dropdown-Pfeil, um aus einer Liste von Benutzern auszuwählen (oder beginnen Sie mit der Eingabe des Namens des Benutzers, dessen Zuweisung aufgehoben werden soll, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird). Sie können die Zuweisung von jeweils nur einem Benutzer aufheben.
1. (Bedingt) Die Variable **Rolle auswählen** wird nur angezeigt, wenn der ausgewählte Benutzer mehreren Aufgaben mit unterschiedlichen Rollen zugewiesen ist. (Informationen dazu, welche Stellenrolle für die Aufgabe eines Benutzers festgelegt ist, finden Sie in der **Rolle des Bevollmächtigten** im Dialogfeld &quot;Erweiterte Zuweisung&quot;für die Aufgabe, wie beschrieben in [Erweiterte Zuweisungen erstellen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)).\
   Im **Rolle auswählen** -Feld die Rolle auswählen, um die Art der Aufgaben zu bestimmen, deren Zuweisung Sie aufheben möchten. Die Zuweisung wird nur für die Aufgaben aufgehoben, denen der Benutzer diese Rolle zugewiesen hat.\
   Hanna Marin wird beispielsweise fünf Aufgaben in einem Projekt zugewiesen. Bei zwei Aufgaben ist ihre berufliche Rolle als Ingenieur definiert. Bei den restlichen 3 ihrer Aufgaben ist ihre Rolle als Designer definiert. Wenn Sie Designer im Feld &quot;Rolle auswählen&quot;auswählen, bedeutet dies, dass Sie die Zuweisung von Hanna zu allen drei Aufgaben aufheben möchten, für die ihre Rolle als Designer definiert ist. Die beiden Aufgaben, bei denen ihre berufliche Rolle als Ingenieur definiert ist, bleiben unverändert.\
   ![](assets/resource-scheduling-unassign-role.png)

1. Klicken **Zuweisung aufheben**.\
   Sie können maximal 1.000 Zuweisungen in einer einzigen Aktion vornehmen. Wenn die von Ihnen vorgenommenen Auswahlen mehr als 1.000 Zuweisungsänderungen bewirken, müssen Sie Ihre Auswahl neu anpassen und es erneut versuchen.
