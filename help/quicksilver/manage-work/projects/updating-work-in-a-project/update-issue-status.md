---
product-area: projects
navigation-topic: update-work-in-a-project
title: Status des Problems aktualisieren
description: Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem liegt und wie es weitergeht.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# Status des Problems aktualisieren

Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem liegt und wie es weitergeht.

## Zugriffsanforderungen

<!--drafted for P&P;

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
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Problemstatus

Im Folgenden finden Sie die Standardstatus für Probleme in Workfront:

* Neu
* In Arbeit
* Warten auf Feedback
* Zurückgestellt
* Lässt sich nicht lösen
* Neu geöffnet
* Geschlossen
* Gelöst

Ihr Adobe Workfront-Administrator kann benutzerdefinierte Status für Probleme in Ihrem Unternehmen hinzufügen. Sie können auch Status je nach Problemtyp verfügbar machen.

Weitere Informationen zu benutzerdefinierten Status und Problemtypen finden Sie in den folgenden Artikeln:

* [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Erstellen von Problemen](../../../manage-work/issues/manage-issues/create-issues.md)

Sie können den Problemstatus manuell aktualisieren oder Workfront automatisch aktualisieren lassen, wenn bestimmte Aktionen ausgeführt werden.

## Problemstatus manuell aktualisieren

Wenn Sie einen Problemstatus aktualisieren, können Sie auch eine Erklärung zum neuen Status hinzufügen und andere Probleminformationen wie das Commitdatum ändern.

1. Gehen Sie zu einem Problem, dem Sie zugewiesen sind und für das Sie den Status aktualisieren möchten.
1. Klicken Sie auf **Status** in der Kopfzeile des Problems ein und wählen Sie einen neuen Status aus.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Um einen visuellen Hinweis zum Abschluss von Problemen anzuzeigen, ziehen Sie die Blase unter **Prozent abgeschlossen** in der Kopfzeile des Problems.

   Oder

   Klicken Sie in die Blase in der Kopfzeile des Problems, um einen Prozentsatz einzugeben.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um weitere Informationen zur Aktualisierung bereitzustellen, und klicken Sie dann auf **Aktualisieren** oder, wenn das Problem einen Status hat, der mit &quot;Complete&quot;übereinstimmt, klicken Sie auf **Fertig:**

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, navigieren Sie zum **Updates** und klicken Sie auf **Neue Aktualisierung starten** und geben Sie Ihre Notiz ein.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie deren Namen in das **Benachrichtigen** ein, das angezeigt wird, wenn Sie einen Hinweis zur Aktualisierung eingeben. Weitere Informationen finden Sie unter [Tagging anderer Benutzer auf Updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Um die Bedingung des Problems zu aktualisieren, klicken Sie auf **Bedingung** und wählen Sie dann die Bedingung aus, die die aktuelle Bedingung des Problems am besten widerspiegelt. Wählen Sie aus den folgenden Optionen aus:

      * Keine Probleme
      * Kleinere Probleme
      * Größere Probleme
   * Um das Datum des Versands des Problems zu aktualisieren, erweitern Sie die **Datum der Übermittlung** und wählen Sie ein neues Datum aus.


## Status des Problems automatisch aktualisieren

Workfront aktualisiert den Status eines Problems automatisch in einen anderen Status, wenn die in der folgenden Tabelle aufgeführten Aktionen ausgeführt werden.

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
   <td>Aktualisierung des Prozentsatzes der Ausgabe auf 100 %</td> 
   <td>Neu oder in Bearbeitung</td> 
   <td>Geschlossen</td> 
  </tr> 
  <tr> 
   <td>Aktualisierung des Prozentsatzes für die Fertigstellung des Problems von 100 % auf eine niedrigere Zahl</td> 
   <td>Geschlossen </td> 
   <td>In Arbeit</td> 
  </tr> 
  <tr> 
   <td>Status eines auflösenden Objekts aktualisieren, das an das Problem angehängt ist</td> 
   <td>Verschiedene Status</td> 
   <td> <p>Verschiedene Status</p> <p>Informationen zum Auflösen von Objekten und deren Auswirkungen auf den Status von Problemen finden Sie im Artikel unter "Synchronisieren des Status des auflösbaren Objekts mit dem des auflösenden Objekts" <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche Problem starten , um die Bearbeitung eines Ihnen zugewiesenen Problems zu akzeptieren.</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Problem starten in den Einstellungen des Startseiten-Teams verknüpft ist. </p> <p>Informationen zum Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche "Start Issue"(Problem starten) finden Sie unter <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a></span><span>.</span> </p> <p>Tipp: Klicken <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Schaltfläche "Rückgängig"</span> Wenn Sie auf Problem starten klicken, wird der Status auf Neu zurückgesetzt. </p> </td> 
  </tr> 
 </tbody> 
</table>
