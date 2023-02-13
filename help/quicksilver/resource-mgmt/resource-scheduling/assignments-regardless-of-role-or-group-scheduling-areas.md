---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen
description: Bei der Ressourcenplanung können Zuweisungen nur an Benutzer vorgenommen werden, deren Benutzerprofil eine Rolle definiert hat, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die bzw. das ihnen zugewiesen wird.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen

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
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

Standardmäßig können Zuweisungen nur Benutzern vorgenommen werden, die eine Rolle in ihrem Benutzerprofil definiert haben, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die bzw. das ihnen bei Verwendung der Tools für die Ressourcenplanung zugewiesen wird.

Sie können Adobe Workfront so konfigurieren, dass Aufgaben und Probleme jedem Benutzer zugewiesen werden können, unabhängig davon, ob für diesen Benutzer in seinem Benutzerprofil eine Rolle definiert ist, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die ihm zugewiesen wird. Wenn Sie einen Benutzer einer Aufgabe oder einem Problem zuweisen und dieser Benutzer keine Rolle besitzt, die mit der Rollenzuweisung für die Aufgabe oder das Problem übereinstimmt, wird die ursprüngliche Rollenzuweisung entfernt und die Rollenzuweisung an die Rolle des Benutzers geändert, den Sie zuweisen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte, Aufgaben und Probleme</p> <p><strong>NOTIZ</strong>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Projekten, Aufgaben und Problemen, für die Sie Zuweisungen aktualisieren.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zulassen von Zuweisungen für Benutzer unabhängig von der Rolle

1. Gehen Sie zur Zeitleiste für die Planung mehrerer Projekte, eines einzelnen Projekts oder eines Teams:

   * **Für mehrere Projekte**:  Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen > Lastenausgleich**, wählen Sie **Planung** im Dropdown-Menü oben links.
   * **Für ein einzelnes Projekt**: Wechseln Sie zu einem Projekt, klicken Sie auf die **Lastenausgleich** im linken Bereich, und wählen Sie dann **Planung** aus dem Dropdown-Menü oben links.
   * **Für ein Team**: Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Teams**, wählen Sie ein Team aus, klicken Sie auf **Lastenausgleich** Wählen Sie im linken Bereich die Option **Planung** aus dem Dropdown-Menü oben links.

1. Klicken Sie auf **Einstellungen** auf der Zeitleiste der Planung.
1. Option deaktivieren **Zuweisung auf Benutzer mit übereinstimmender Rolle begrenzen**.
1. Klicken **Zurück zur Planung**.

## Zulassen von Zuweisungen für Benutzer unabhängig von der Gruppenmitgliedschaft

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

Standardmäßig können Zuweisungen nur an Benutzer vorgenommen werden, die Mitglieder der Gruppe sind, die mit dem Projekt verknüpft ist (dies ist die Gruppe, die beim Bearbeiten des Projekts definiert wird).

>[!IMPORTANT]
>
>Diese Einstellung berücksichtigt nur die Mitglieder der Gruppe, die mit dem Projekt verknüpft ist, und keine Mitglieder der Untergruppen dieser Gruppe.

Sie können Workfront so konfigurieren, dass Aufgaben und Probleme jedem Benutzer zugewiesen werden können, unabhängig davon, ob dieser Benutzer Mitglied der Gruppe ist, die mit dem Projekt verknüpft ist, in dem sich die Aufgabe oder das Problem befindet.

1. Gehen Sie zur Zeitleiste für die Planung mehrerer Projekte, eines einzelnen Projekts oder eines Teams:

   * **Für mehrere Projekte**:  Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Ressourcen > Lastenausgleich**, wählen Sie **Planung** im Dropdown-Menü oben links.
   * **Für ein einzelnes Projekt**: Wechseln Sie zu einem Projekt, klicken Sie auf die **Lastenausgleich** im linken Bereich, und wählen Sie dann **Planung** aus dem Dropdown-Menü oben links.
   * **Für ein Team**: Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Teams**, wählen Sie ein Team aus, klicken Sie auf **Lastenausgleich** Wählen Sie im linken Bereich die Option **Planung** aus dem Dropdown-Menü oben links.

1. Klicken Sie auf **Einstellungen** auf der Zeitleiste der Planung.
1. Option deaktivieren **Zuweisung auf die mit dem Projekt verknüpfte Gruppe beschränken**.
1. Klicken **Zurück zur Planung**.

 
