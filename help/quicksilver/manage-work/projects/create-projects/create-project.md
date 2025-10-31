---
product-area: projects
navigation-topic: create-projects
title: Erstellen eines Projekts
description: Ein Projekt ist eine große Arbeitseinheit in Adobe Workfront. Sie können Projekte von Grund auf neu erstellen, eine Vorlage verwenden oder Probleme oder Aufgaben in Projekte konvertieren.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 1%

---

# Erstellen eines Projekts

<!--remove Preview and Production references-->

<!-- Audited: 110/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Projekte stellen einen großen Arbeitsaufwand dar, der in Adobe Workfront erledigt werden muss.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->


## Möglichkeiten zum Erstellen von Projekten

Sie können ein Projekt in Workfront mit einer der folgenden Methoden erstellen:

* Erstellen Sie ein Projekt von Grund auf ohne Verwendung einer Vorlage. In diesem Artikel wird beschrieben, wie Sie ein Projekt von Grund auf neu erstellen.

* Kopieren eines vorhandenen Projekts.\
  Weitere Informationen zum Kopieren eines Projekts finden Sie unter [Kopieren eines Projekts](../../../manage-work/projects/manage-projects/copy-project.md).

* Verwenden Sie eine Vorlage.\
  Weitere Informationen zur Verwendung einer Vorlage zum Erstellen eines neuen Projekts finden Sie unter [Erstellen eines Projekts mithilfe einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importieren Sie ein Projekt aus Microsoft Project.\
  Weitere Informationen zum Importieren eines Projekts aus MS Project finden Sie [Projekt aus Microsoft Project importieren](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importieren Sie ein Projekt mithilfe von Kickstarts.

  Als Workfront-Administrator können Sie Projekte über einen Kickstart importieren.

  Informationen zum Importieren von Daten mithilfe von Kickstarts in Workfront finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Informationen zum Importieren von Projekten mithilfe von Kickstarts finden Sie unter [Kickstartszenario: Einfache Vorbereitung für den Projekt- und Aufgabenimport](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Veröffentlichen Sie eine Initiative aus einem Szenario im Adobe Workfront-Szenarioplaner.

  Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

  Informationen zum Erstellen von Projekten aus Veröffentlichungsinitiativen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

* Fügen Sie Projekte hinzu, während Sie sie über einen Datensatztyp in Workfront Planning verbinden.

  Informationen zum Zugriff auf Workfront Planning finden Sie unter [Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

  Informationen zum Erstellen von Projekten durch Hinzufügen zu Datensätzen finden Sie im Abschnitt „Erstellen von Projekten, wenn diese mit Datensätzen aus Workfront Planning verbunden werden“ im Artikel [Erstellen von Workfront-Objekten aus Workfront Planning, während Sie sie mit Datensätzen verbinden](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes sicherstellen:

* Ihr System- oder Gruppenadministrator hat die Einstellung „Benutzern erlauben, Projekte ohne Vorlage zu erstellen“ im Bereich „Setup“ aktiviert.

  Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Standardeinstellungen für neue Projekte

Wenn Sie ein Projekt erstellen, wendet Workfront eine Reihe von Standardeinstellungen darauf an. Beispielsweise sind der Status, die Gruppe und der Zeitplanmodus beim Erstellen eines Projekts vordefiniert.

Beachten Sie Folgendes:

* Als Workfront-Administrator oder Gruppenadministrator können Sie die Standardeinstellungen für ein neues Projekt konfigurieren, wenn Sie die Projekteinstellungen für Ihre gesamte Workfront-Instanz oder für eine Gruppe konfigurieren.
* Workfront wendet ggf. die Einstellungen der Gruppe an, bevor die vom Workfront-Administrator festgelegten Einstellungen angewendet werden.
* Der Standardstatus eines neuen Projekts entspricht dem Status, den Ihr Workfront-Administrator im Hauptbereich Projektvoreinstellungen oder ein Gruppenadministrator (oder Workfront-Administrator) im Bereich Projektvoreinstellungen für eine Gruppe definiert hat.

  >[!NOTE]
  >
  >Es wird empfohlen, dass der Standardstatus für ein neues Projekt „Planung“ lautet. Wenn Sie Änderungen am neuen Projekt vornehmen, wird dadurch sichergestellt, dass Benachrichtigungen nicht an die dem Projekt zugewiesenen Benutzer gesendet werden.
  >
  >Weitere Informationen zum Einrichten des Standardstatus und anderer Standardeinstellungen für ein neues Projekt finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) oder [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Die folgenden Szenarien zeigen, wie Workfront die Gruppe und den Status eines neuen Projekts definiert:

   * Wenn Sie ein Projekt von Grund auf neu erstellen, ist die Gruppe des Projekts Ihre Hauptgruppe.

     Der Status des Projekts ist der Standardstatus in den Projektvoreinstellungen Ihrer Hauptgruppe (sofern vorhanden) oder Ihrer Workfront-Instanz. Sie können den Standardstatus beim Erstellen des Projekts in einen beliebigen Status ändern, der für die Gruppe des Projekts verfügbar ist.

   * Wenn Sie ein Projekt mithilfe einer Vorlage erstellen, haben die Einstellungen aus der Vorlage Vorrang vor den vom Workfront- oder Gruppenadministrator festgelegten Einstellungen.

     Die Gruppe des neuen Projekts ist die Gruppe der Vorlage. Wenn die Vorlage keiner Gruppe zugeordnet ist, ist die Gruppe des Projekts die Hauptgruppe des Benutzers, der das Projekt erstellt.

     Der Standardstatus eines neuen Projekts, das über eine Vorlage erstellt wurde, entspricht dem Status, den Ihr Workfront-Administrator im Hauptbereich Projektvoreinstellungen oder ein Gruppenadministrator (oder Workfront-Administrator) im Bereich Projektvoreinstellungen für die Gruppe definiert hat. Sie können den Standardstatus beim Erstellen eines Projekts über eine Vorlage in einen der Status der Gruppe des Projekts ändern, die entweder die Gruppe der Vorlage oder die Hauptgruppe des Benutzers ist, der das Projekt erstellt.

   * Wenn Sie ein Projekt durch Konvertieren eines Problems erstellen, ist die Gruppe eines neuen Projekts die Gruppe des vorhandenen Projekts des Problems. Wenn der/die Benutzende, der/die das Problem konvertiert, keinen Zugriff auf das Problemprojekt hat oder wenn das Problemprojekt keine Gruppe hat, ist die Gruppe des neuen Projekts die Hauptgruppe des/r Benutzenden, der/die das Problem konvertiert.

     Die Status des neuen Projekts stimmen mit den Gruppenstatus der mit dem Projekt verknüpften Gruppe überein, bei der es sich entweder um die Gruppe des ursprünglichen Projekts oder die Hauptgruppe der Person handelt, die das Problem konvertiert.

     Wenn Sie beim Erstellen des Projekts eine Vorlage verwenden, indem Sie das Problem konvertieren, sehen Sie im zweiten obigen Szenario nach, welche Gruppe und welcher Status Workfront für das neue Projekt gilt.

## Ein Projekt von Grund auf neu erstellen

>[!NOTE]
>
>Wenn Sie ein Projekt mithilfe einer Vorlage erstellen, empfehlen wir, auch den Artikel [Erstellen eines Projekts mithilfe einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) anzuzeigen.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke oder auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront, falls verfügbar, klicken Sie dann auf **Projekte** und erweitern Sie **Neues Projekt**.
   * Gehen Sie zu einem Portfolio und erweitern Sie dann **Neues Projekt**.
   * Wechseln Sie zu einem Programm und erweitern Sie dann **Neues Projekt**.
   * Wenn Sie Gruppenadministrator sind, können Sie im Abschnitt Projekte einer Gruppe, die Sie verwalten, auch ein Projekt erstellen. Weitere Informationen finden Sie unter [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menü „Neues Projekt“](assets/new-project-dropdown-nwe-350x358.png)

1. Klicken Sie **Menü** Neues Projekt“, um ein Projekt von Grund auf neu zu erstellen.
1. Geben Sie einen Namen für Ihr Projekt ein. Drücken Sie die Eingabetaste, um den Namen zu speichern.

   ![Geben Sie einen Namen für das Projekt ein](assets/rename-untitled-project.png)

   In der Kopfzeile der Projektseite erhalten Sie einen schnellen Überblick über den aktuellen Status und den Fortschritt eines Projekts. Die Informationen im Projekt-Header ändern sich, wenn die Projektinformationen aktualisiert werden.

1. Klicken Sie **Aufgaben hinzufügen**.

   Oder

   Klicken Sie auf **Neue Aufgabe**, um dem Projekt Aufgaben hinzuzufügen und ihnen Ressourcen zuzuweisen.

   Weitere Informationen zum Hinzufügen von Aufgaben zu einem Projekt finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Bearbeiten Sie die Projektdetails, indem Sie auf das Menü **Mehr** rechts neben dem Projektnamen in der Kopfzeile und dann auf **Bearbeiten** ![Bearbeiten](assets/qs-edit-icon.png) neben dem Projektnamen klicken.

   Das **Projekt bearbeiten** wird geöffnet.

1. Fügen Sie Informationen über das Projekt hinzu.

   Weitere Informationen zum Bearbeiten eines Projekts finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >Der Status des Projekts sollte „Planung“ oder ein anderer Status sein, der nicht „Aktuell“ ist. Auf diese Weise können Sie Änderungen am Projekt vornehmen, ohne Benachrichtigungen an die Projektteilnehmer zu generieren.

1. Klicken Sie **Speichern**, um Ihre Änderungen zu speichern.

1. (Optional) Nachdem Sie die Projekteinstellungen konfiguriert und die Aufgaben hinzugefügt haben, können Sie den Status des Projekts in der Projekt **Kopfzeile** Aktuell“ ändern.

   Dies bedeutet, dass das Projekt nun startbereit ist und Benutzende, die den Aufgaben zugewiesen sind, nun mit der Arbeit daran beginnen können.

   Weitere Informationen zum Projektstatus finden Sie unter [Zugriff auf die Liste der Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
