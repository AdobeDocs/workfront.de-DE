---
product-area: projects
navigation-topic: create-projects
title: Projekt erstellen
description: '(HINWEIS: Diese wird über die Benutzeroberfläche im Abschnitt "Globale Projekte"in Classic über die globale Navigationsleiste verknüpft. Nicht ändern/entfernen)'
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Projekt erstellen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

Die Projekte stellen einen großen Teil der Arbeit dar, die in Adobe Workfront geleistet werden muss.

## Zugriffsanforderungen

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Projekte finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Projektzugriff gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt </p> <p> Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Möglichkeiten zum Erstellen von Projekten

Sie können ein Projekt in Workfront mit einer der folgenden Methoden erstellen:

* Erstellen Sie ein Projekt von Grund auf neu, ohne eine Vorlage zu verwenden. In diesem Artikel wird beschrieben, wie Sie ein Projekt von Grund auf neu erstellen.

* Kopieren Sie ein vorhandenes Projekt.\
   Weitere Informationen zum Kopieren von Projekten finden Sie unter [Projekt kopieren](../../../manage-work/projects/manage-projects/copy-project.md).

* Verwenden Sie eine Vorlage.\
   Weitere Informationen zur Verwendung einer Vorlage zum Erstellen eines neuen Projekts finden Sie unter [Erstellen eines Projekts mit einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importieren Sie ein Projekt aus Microsoft Project.\
   Weitere Informationen zum Importieren eines Projekts aus einem MS-Projekt finden Sie unter [Importieren eines Projekts aus einem Microsoft-Projekt](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importieren Sie ein Projekt mit Kick-Start.

   Als Workfront-Administrator können Sie Projekte mit einem Schnellstart importieren.

   Informationen zum Importieren von Daten mit Kick-Start in Workfront finden Sie unter [Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

   Informationen zum Importieren von Projekten mit Kick-Start finden Sie unter [Kick-Starts-Szenario: einfache Vorbereitung des Projekt- und Aufgabenimports](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* Veröffentlichen Sie eine Initiative aus einem Szenario im Adobe Workfront-Szenario-Planer. Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md). Informationen zum Erstellen von Projekten aus Veröffentlichungsinitiativen finden Sie unter  [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sicherstellen, dass

* Ihr System- oder Gruppenadministrator hat im Bereich &quot;Einrichtung&quot;die Voreinstellung &quot;Benutzer können Projekte ohne Verwendung einer Vorlage erstellen dürfen&quot;aktiviert.

   Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Neue Standardeinstellungen für Projekte

Wenn Sie ein Projekt erstellen, wendet Workfront eine Reihe von Standardeinstellungen an. Beispielsweise sind der Status-, Gruppen- oder Planungsmodus beim Erstellen eines Projekts voreingestellt.

Beachten Sie Folgendes:

* Als Workfront-Administrator oder Gruppenadministrator können Sie bei der Konfiguration von Projekteinstellungen die Standardeinstellungen für ein neues Projekt konfigurieren.
* Workfront wendet gegebenenfalls die Gruppeneinstellungen an, bevor die vom Workfront-Administrator festgelegten angewendet werden.
* Wenn Sie ein Projekt mit einer Vorlage erstellen, haben die Einstellungen aus der Vorlage Vorrang vor den Einstellungen, die vom Workfront- oder Gruppenadministrator festgelegt wurden.

>[!NOTE]
>
>Es wird empfohlen, den Standardstatus für ein neues Projekt &quot;Planung&quot;festzulegen. Wenn Sie Änderungen am neuen Projekt vornehmen, wird sichergestellt, dass keine Benachrichtigungen an die dem Projekt zugewiesenen Benutzer Trigger werden.

Weitere Informationen zum Einrichten des Standardstatus und anderer Standardeinstellungen für ein neues Projekt finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).



## Neues Projekt erstellen

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png)klicken **Projekte**, dann erweitern **Neues Projekt**.
   * Wechseln Sie zu einem Portfolio und erweitern Sie **Neues Projekt**.

      >[!TIP]
      >
      >Wenn Sie ein Projekt mit einer Vorlage aus einem Portfolio erstellen, wird das Projektfeld des neuen Portfolios aktualisiert, um das Portfolio anzuzeigen, aus dem Sie das Projekt erstellen möchten. Dadurch wird das Feld Portfolio in der Vorlage überschrieben, sofern angegeben.

   * Navigieren Sie zu einem Programm und erweitern Sie **Neues Projekt**.

      >[!TIP]
      >
      >Wenn Sie ein Projekt mithilfe einer Vorlage aus einem Programm erstellen, wird das Programmfeld der neuen Projekte aktualisiert, um das Programm anzuzeigen, aus dem Sie das Projekt erstellen möchten. Das Feld Portfolio der Vorlage wird aktualisiert und zeigt das Portfolio des Programms an, aus dem Sie das Projekt erstellen möchten. Dadurch werden die Portfolio- und Programmfelder in der Vorlage überschrieben, sofern sie angegeben wurden.

   * Als Gruppenadministrator können Sie auch ein Projekt im Abschnitt &quot;Projekte&quot;einer von Ihnen verwalteten Gruppe erstellen. Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >Wenn Sie ein Projekt mit einer Vorlage aus einer Gruppe erstellen, wird die Gruppe, aus der Sie das Projekt erstellen, nur dann im Feld Gruppe des neuen Projekts angezeigt, wenn das Feld Gruppe der Vorlage nicht angegeben ist. Wenn das Vorlagengruppenfeld angegeben ist, ist das Gruppenfeld des neuen Projekts das des Vorlagenfelds.
   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Klicken **Neues Projekt** , wenn Sie ein Projekt von Grund auf neu erstellen möchten.
1. Geben Sie einen Namen für Ihr Projekt ein. Drücken Sie die Eingabetaste , um den Namen zu speichern.

   ![](assets/untitled-project-rename-new-project-nwe-350x127.png)

   In der Kopfzeile der Projektseite wird ein kurzer Überblick über den aktuellen Zustand und Fortschritt eines Projekts angezeigt. Die Informationen in der Projektheader ändern sich mit der Aktualisierung der Projektinformationen.

1. Klicken **Hinzufügen beginnen** **Aufgaben**.

   Oder

   Klicken **Neue Aufgabe** , um dem Projekt Aufgaben hinzuzufügen und ihnen Ressourcen zuzuweisen.\
   Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Bearbeiten Sie die Projektdetails, indem Sie auf die **Mehr Menü** und dann **Bearbeiten** ![](assets/qs-edit-icon.png) neben dem Namen des Projekts.

   Die **Projekt bearbeiten** wird geöffnet.

   Weitere Informationen zum Bearbeiten eines Projekts finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Optional) Nachdem Sie die Projekteinstellungen konfiguriert und die Aufgaben hinzugefügt haben, können Sie den Status des Projekts in **Aktuell**.

   Dies weist darauf hin, dass das Projekt jetzt startbereit ist und die den Aufgaben zugewiesenen Benutzer jetzt mit der Bearbeitung beginnen können.

   Weitere Informationen zum Projektstatus finden Sie unter [Zugriff auf die Liste der Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
