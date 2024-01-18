---
product-area: projects
navigation-topic: update-work-in-a-project
title: Status des Problems aktualisieren
description: Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem liegt und wie es weitergeht.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 2%

---

# Status des Problems aktualisieren

<!--Audited: 01/2024-->

Sie können den Status eines Problems aktualisieren, um andere darüber zu informieren, wo das Problem liegt und wie es weitergeht.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Mitarbeiter oder höher</p>
   Oder
   <p>Aktuelle Lizenz: Anfrage oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Sie können den Problemstatus in den folgenden Bereichen von Workfront aktualisieren:

* Die Ausgabe-Kopfzeile auf der Aufgabenseite.
* Das Feld Problem bearbeiten , wenn ein Problem bearbeitet wird.
* den Abschnitt Details auf der Problemseite.
* Wenn in einer Problemliste oder einem Bericht das Feld Status in der Ansicht sichtbar ist.
* Im Bereich Zusammenfassung des Problems.

So aktualisieren Sie den Problemstatus in der Kopfzeile des Problems manuell:

1. Gehen Sie zu einem Problem, bei dem Sie den Status aktualisieren möchten.
1. Klicken Sie auf **Status** in der Kopfzeile des Problems ein und wählen Sie einen neuen Status aus.
1. Um einen visuellen Hinweis zum Abschluss von Problemen anzuzeigen, ziehen Sie die Blase unter **Prozent abgeschlossen** im Header des Problems

   Oder

   Klicken Sie in die Blase in der Kopfzeile des Problems, um einen Prozentsatz einzugeben.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um zusätzliche Informationen über die Aktualisierung bereitzustellen:

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, navigieren Sie zum **Updates** und klicken Sie auf **Neuer Kommentar**, und geben Sie eine Notiz ein.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie deren Namen in das **Personen oder Teams taggen** -Feld, das angezeigt wird, wenn Sie einen Kommentar eingeben. Weitere Informationen finden Sie unter [Tagging anderer Benutzer auf Updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Um das Datum des Versands des Problems zu aktualisieren, klicken Sie auf **Problemdetails**, bearbeiten Sie dann die **Datum der Übermittlung** -Feld. Weitere Informationen finden Sie unter [Probleme bearbeiten](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Nur Problemverantwortliche können das Veröffentlichungsdatum aktualisieren.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

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
   <td><b>Aktion</b></td> 
   <td><b>Originalstatus</b></td> 
   <td><b>Neuer Status</b></td> 
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
   <td> <p>Verschiedene Status</p> <p>Informationen zum Auflösen von Objekten und deren Auswirkungen auf den Status von Problemen finden Sie im Artikel unter "Synchronisieren des Status des auflösbaren Objekts mit dem des auflösenden Objekts". <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche Problem starten , um die Bearbeitung eines Ihnen zugewiesenen Problems zu akzeptieren.</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Problem starten in den Einstellungen des Startseiten-Teams verknüpft ist. </p> <p>Informationen zum Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche "Start Issue"(Problem starten) finden Sie unter <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a></span><span>.</span> </p> <p>Tipp: Klicken <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Schaltfläche "Rückgängig"</span> Wenn Sie auf Problem starten klicken, wird der Status auf Neu zurückgesetzt. </p> </td> 
  </tr> 
 </tbody> 
</table>
