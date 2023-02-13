---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierung des Aufgabenstatus
description: Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe befindet (und wie das Gesamtprojekt) und wie sie vorankommt.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Aktualisierung des Aufgabenstatus

Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe befindet (und wie das Gesamtprojekt) und wie sie vorankommt.

Die Standardstatus sind &quot;Neu&quot;, &quot;In Bearbeitung&quot;und &quot;Abgeschlossen&quot;. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Status für Ihre Organisation hinzufügen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Sie können den Aufgabenstatus manuell aktualisieren oder Workfront automatisch aktualisieren lassen, wenn bestimmte Aktionen ausgeführt werden.

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um Aufgaben manuell aktualisieren zu können:

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aufgabenstatus manuell aktualisieren

Wenn Sie einen Aufgabenstatus aktualisieren, können Sie auch eine Erläuterung zum neuen Status eingeben und andere Aufgabeninformationen wie das Fälligkeitsdatum ändern.

1. Gehen Sie zu einer Aufgabe, der Sie zugewiesen sind und für die Sie den Status aktualisieren möchten.
1. Klicken Sie auf **Status** in der Aufgabenüberschrift ein und wählen Sie einen neuen Status aus.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um weitere Informationen zur Aktualisierung bereitzustellen, und klicken Sie dann auf **Aktualisieren** oder wenn die Aufgabe die **Fertig** status, click **Fertig:**

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, navigieren Sie zum **Updates** Bereich und Klicken **Neue Aktualisierung starten** und geben Sie Ihre Notiz ein.

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie deren Namen in das **Benachrichtigen** ein, das angezeigt wird, wenn Sie einen Hinweis zur Aktualisierung eingeben. Weitere Informationen finden Sie unter [Tagging anderer Benutzer auf Updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Um die Bedingung der Aufgabe zu aktualisieren, klicken Sie auf **Bedingung auswählen** rechts von der **Benachrichtigen** (diese werden angezeigt, wenn Sie einen Hinweis zur Aktualisierung eingeben), wählen Sie dann die Bedingung aus, die die aktuelle Bedingung der Aufgabe am besten widerspiegelt.

   * Um das Übermittlungsdatum der Aufgabe zu aktualisieren, erweitern Sie die **Datum der Übermittlung** und wählen Sie einen neuen Termin für die Veröffentlichung aus.
   * Um einen visuellen Hinweis zum Abschluss von Aufgaben bereitzustellen, ziehen Sie die Blase unter &quot;Percent Complete&quot;oder doppelklicken Sie darauf, um einen Prozentwert einzugeben.\
      ![](assets/drag-the-progress-bar-350x155.png)

## Automatisches Aktualisieren des Aufgabenstatus

Workfront aktualisiert den Status einer Aufgabe automatisch in einen anderen Status, wenn die in der folgenden Tabelle aufgelisteten Aktionen ausgeführt werden.

>[!NOTE]
>
>Die Status in der folgenden Tabelle sind standardmäßige Systemstatus. Ihr Workfront-Administrator oder ein Gruppenadministrator kann die Status in Ihrer Workfront-Instanz umbenennen. Informationen zum Erstellen und Verwalten von Status in Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Aktion</td> 
   <td>Originalstatus</td> 
   <td>Neuer Status</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Prozentsatz der abgeschlossenen Aufgaben auf 100 %</td> 
   <td>Neu oder in Bearbeitung</td> 
   <td>Abgeschlossen</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Prozentsatz der abgeschlossenen Aufgaben von 100 % auf eine niedrigere Zahl.</td> 
   <td>Abgeschlossen</td> 
   <td>In Arbeit</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche Aufgabe starten , um die Arbeit an einer Aufgabe zu akzeptieren, die Ihnen zugewiesen ist.</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Aufgabe starten in den Einstellungen des Startseiten-Teams verknüpft ist.</p> <p>Weitere Informationen zum Ersetzen der Schaltfläche "Work On It"durch eine Schaltfläche "Start Task", finden Sie unter <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a></span>.</p> <p>Tipp: <span>Klicken</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Schaltfläche "Rückgängig"</span>Wenn Sie auf Aufgabe starten klicken, wird der Status auf Neu zurückgesetzt. </p> </td> 
  </tr> 
 </tbody> 
</table>
