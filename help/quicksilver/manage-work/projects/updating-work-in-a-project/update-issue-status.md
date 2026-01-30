---
product-area: projects
navigation-topic: update-work-in-a-project
title: Problemstatus aktualisieren
description: Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem ist und wie es fortschreitet.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 6%

---

# Problemstatus aktualisieren

<!--Audited: 01/2024-->

Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem ist und wie es fortschreitet.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Status ausgeben

Im Folgenden finden Sie die Standardstatus für Probleme in Workfront:

* Neu
* In Arbeit
* Warten auf Feedback
* Zurückgestellt
* Lässt sich nicht lösen
* Neu geöffnet
* Geschlossen
* Gelöst

Ihr Adobe Workfront-Administrator kann benutzerdefinierte Status für Probleme für Ihr Unternehmen hinzufügen. Je nach Problemtyp können sie auch Status verfügbar machen.

Weitere Informationen zu benutzerdefinierten Status und Problemtypen finden Sie in den folgenden Artikeln:

* [Status erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Probleme erstellen](../../../manage-work/issues/manage-issues/create-issues.md)

Sie können den Anfragestatus manuell aktualisieren. Alternativ können Sie festlegen, dass Workfront ihn automatisch aktualisiert, wenn bestimmte Aktionen ausgeführt werden.

## Problemstatus manuell aktualisieren

Sie können den Problemstatus in den folgenden Bereichen von Workfront aktualisieren:

* Die Problem-Kopfzeile auf der Aufgabenseite.
* Im Feld „Problem bearbeiten“ beim Bearbeiten eines Problems.
* Der Abschnitt „Details“ auf der Problemseite.
* Wenn in einer Problemliste oder einem Bericht das Feld Status in der Ansicht sichtbar ist.
* Im Bedienfeld Zusammenfassung des Problems.

So aktualisieren Sie den Anfragestatus in der Anfragekopfzeile manuell:

1. Navigieren Sie zu einer Anfrage, für die Sie den Status aktualisieren möchten.
1. Klicken Sie auf **Status** in der Anfragekopfzeile und wählen Sie einen neuen Status aus.
1. Um einen visuellen Hinweis zum Abschluss des Problems zu geben, ziehen oder doppelklicken Sie auf die Blase unter **Prozent abgeschlossen** in der Kopfzeile des Problems

   ODER

   Klicken Sie in die Blase in der Kopfzeile des Problems, um einen Prozentsatz einzugeben.

   ![Update der Aufgabe in Prozent abgeschlossen in der Kopfzeile](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um zusätzliche Informationen zur Aktualisierung bereitzustellen:

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, gehen Sie zum Abschnitt **Aktualisierungen** und klicken Sie auf **Neuer Kommentar** und geben Sie dann einen Hinweis ein.

     ![Meldungsfeld „Anfrage-Aktualisierungsverlauf“](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie ihre Namen in das Feld **Personen oder Teams taggen** ein, das angezeigt wird, wenn Sie einen Kommentar eingeben. Weitere Informationen finden Sie unter [Andere bei Updates taggen](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Um das Commit-Datum des Problems zu aktualisieren, klicken Sie auf **Problemdetails** und bearbeiten Sie dann das Feld **Commit-Datum**. Weitere Informationen finden Sie unter [Probleme bearbeiten](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Nur Problembevollmächtigte können das Commit-Datum aktualisieren.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![Issue status expanded in header](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![Update task percent in header](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Problemstatus automatisch aktualisieren

Workfront aktualisiert automatisch den vorhandenen Status eines Problems in einen anderen Status, wenn die in der folgenden Tabelle aufgeführten Aktionen auftreten.

>[!NOTE]
>
>Die in der folgenden Tabelle aufgeführten Statuswerte sind standardmäßige Systemstatus. Ihr Workfront-Administrator oder ein Gruppenadministrator kann die Status in Ihrer Workfront-Instanz umbenennen. Informationen zum Erstellen und Verwalten von Status in Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Aktion</b></td> 
   <td><b>Originalzustand</b></td> 
   <td><b>Neuer Status</b></td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Problemprozentsatz auf 100 %.</td> 
   <td>Neu oder in Bearbeitung</td> 
   <td>Geschlossen</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Problemprozentsatz abgeschlossen von 100 % auf eine niedrigere Zahl.</td> 
   <td>Geschlossen </td> 
   <td>In Arbeit</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren des Status eines Lösungsobjekts, das mit der Anfrage verbunden ist</td> 
   <td>Verschiedene Status</td> 
   <td> <p>Verschiedene Status</p> <p>Informationen zu Lösungsobjekten und deren Auswirkungen auf den Status von Problemen finden Sie im Abschnitt „Synchronisieren des Status des lösbaren Objekts mit dem des Lösungsobjekts“ im Artikel <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über lösbare und lösbare Objekte </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche „Problem starten“, um die Bearbeitung eines Ihnen zugewiesenen Problems zuzulassen</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Problem starten in den Einstellungen Ihres Home-Teams verknüpft ist. </p> <p>Informationen zum Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Problem starten“ finden Sie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten</a></span><span>.</span> </p> <p>Tipp: Wenn Sie nach <span data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Klicken auf die Schaltfläche „Rückgängig</span> klicken, wird der Status des Problems auf „Neu“ zurückgesetzt. </p> </td> 
  </tr> 
 </tbody> 
</table>
