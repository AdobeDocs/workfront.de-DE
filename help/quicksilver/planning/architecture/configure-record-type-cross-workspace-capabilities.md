---
title: Konfigurieren von arbeitsbereichsübergreifenden Funktionen für den Datensatztyp
description: Sie können festlegen, dass ein Datensatztyp entweder einem anderen Arbeitsbereich hinzugefügt oder über einen anderen Arbeitsbereich verbunden werden kann.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Sie können Datensatztypen so konfigurieren, dass sie in mehreren Arbeitsbereichen funktionieren.

Im Folgenden finden Sie arbeitsbereichsübergreifende Funktionen von Datensatztypen:

* Sie können einen Datensatztyp als zentralisiert festlegen. Benutzer können zentralisierte Datensatztypen zu anderen Arbeitsbereichen hinzufügen, die sie verwalten können.
* Sie können einen Datensatztyp als verbindbaren Datensatz festlegen. Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

Sie müssen zunächst die arbeitsbereichsübergreifenden Funktionen eines Datensatztyps definieren, bevor Workspace-Manager ihn entweder aus verbinden oder zu anderen Arbeitsbereichen hinzufügen können.

Sie definieren die arbeitsbereichsübergreifenden Funktionen eines Datensatztyps, wenn Sie einen Datensatztyp erstellen oder bearbeiten.

Weitere Informationen finden Sie in einem der folgenden Artikel:

* [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md)
* [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul><li><p>Beliebiges Workfront-Paket</p></li>
<p>Und</p>
<li><p>Beliebiges Planungspaket zum Erstellen verbindbarer Datensatztypen</p></li>
<li><p>Planning Plus-Paket zum Erstellen zentralisierter Datensatztypen</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Konfigurieren von zentralisierten Datensatztypen

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

Als Workspace-Manager können Sie einen Datensatztyp als zentralisierten Datensatztyp konfigurieren. Ein zentralisierter Datensatztyp kann anderen Arbeitsbereichen hinzugefügt werden.

Ein Workspace-Manager kann einem von ihm verwalteten Workspace einen zentralen Datensatztyp hinzufügen. Die ursprünglichen Felder des Datensatztyps werden ebenfalls hinzugefügt.

Benutzer können Datensätze zu einem zentralisierten Datensatztyp aus jedem Arbeitsbereich hinzufügen, für den sie über Beitragsberechtigungen verfügen, und wo der zentralisierte Datensatztyp hinzugefügt wird, einschließlich des ursprünglichen Arbeitsbereichs. Sie können Datensätze aus dem Arbeitsbereich anzeigen, für den sie nur über die Berechtigung Anzeigen verfügen.

Weitere Informationen finden Sie unter [Übersicht über Workspace-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

So konfigurieren Sie einen Datensatztyp als zentralisiert:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie als zentralisiert konfigurieren möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp .
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps.
1. Klicken Sie auf **Bearbeiten**.

   ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >Wenn ein Datensatztyp bereits als zentralisierter Datensatztyp festgelegt wurde und zu anderen Arbeitsbereichen hinzugefügt wurde, ist die Option Bearbeiten abgeblendet.

1. Klicken Sie im Feld **Datensatztyp bearbeiten** auf die Registerkarte **Erweiterte Einstellungen**.
1. Aktivieren Sie die **Zulassen, dass dieser Datensatztyp anderen Arbeitsbereichen hinzugefügt**).

   ![Datensatztyp bearbeiten Erweiterte Einstellungen mit Aktivieren von Zu anderen Arbeitsbereichen hinzufügen](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Nachdem Sie einen zentralisierten Datensatztyp zu einem anderen Arbeitsbereich hinzugefügt haben, kann diese Einstellung nicht mehr deaktiviert werden.

1. Fügen Sie im Feld **Auswählen, wer diesen Datensatztyp zu von ihm verwalteten Arbeitsbereichen hinzufügen kann** Entitäten hinzu, denen Sie erlauben möchten, diesen Datensatztyp zu von ihnen verwalteten Arbeitsbereichen hinzuzufügen.

   Ihr Name wird dem Feld automatisch hinzugefügt.

   Sie können einzelne Benutzer oder Gruppen, Teams, Aufgabengebiete oder Unternehmen hinzufügen, deren Benutzer diesen Datensatztyp den von ihnen verwalteten Arbeitsbereichen hinzufügen dürfen.

   Sie müssen mindestens eine Entität (Benutzer, Team, Gruppe, Rolle oder Unternehmen) festlegen, um diese Einstellung aktivieren zu können.

   Sie können dieses Feld bearbeiten, nachdem Sie den Datensatztyp gespeichert haben.

1. (Optional) Entfernen Sie Ihren Namen aus dem Feld **Auswählen, wer diesen Datensatztyp zu den von ihm verwalteten Arbeitsbereichen hinzufügen kann**.

1. Klicken Sie auf **Speichern**.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt von den von Ihnen angegebenen Personen zu einem anderen Arbeitsbereich hinzugefügt werden.

   >[!NOTE]
   >
   >Sie können das Erscheinungsbild und die Einstellungen des Datensatztyps sowie seine ursprünglichen Felder nur über den ursprünglichen Arbeitsbereich bearbeiten.

   * Auf der Karte „Datensatztyp“ wird das Symbol &quot;![ Datensatztyp“ angezeigt](assets/global-icon.png) um anzugeben, dass der Datensatztyp für das Hinzufügen zu anderen Arbeitsbereichen verfügbar ist.
   * Zur Tabellenansicht des Datensatztyps und **Details seiner Datensätze wird ein systemgeneriertes Workspace-Feld vom Typ** hinzugefügt.

     Das Feld Workspace zeigt den Arbeitsbereich an, aus dem jeder Datensatz erstellt wird.

     Dieses Feld ist schreibgeschützt und kann nicht gelöscht werden.
1. (Optional) Wechseln Sie zu einem anderen Arbeitsbereich und erstellen Sie einen Datensatztyp mithilfe eines vorhandenen Datensatztyps. Wählen Sie den Datensatztyp aus, den Sie in den obigen Schritten aktiviert haben.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Konfigurieren verbindbarer Datensatztypen

<!--this is a UI term; don't change the title of this section-->

Sie können einen Datensatztyp konfigurieren, mit dem über andere Arbeitsbereiche eine Verbindung hergestellt werden soll, wenn Sie den Datensatztyp erstellen oder bearbeiten.

So konfigurieren Sie einen Datensatztyp für die Verbindung von anderen Arbeitsbereichen aus, wenn Sie den Datensatztyp bearbeiten:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp und klicken Sie dann auf **Bearbeiten**
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie dann auf **Bearbeiten**.

   ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

1. Klicken Sie im Feld **Datensatztyp bearbeiten** auf die Registerkarte **Erweiterte Einstellungen**.
1. Aktivieren Sie die **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** Einstellung. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Registerkarte „Datensatztyp bearbeiten - Erweiterte Einstellungen“ mit aktivierter Option „Von anderen Arbeitsbereichen verbinden“](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Wenn diese Option aktiviert ist, ist der Datensatztyp verfügbar und kann von anderen Arbeitsbereichen aus mit verbunden werden.

1. Wählen Sie aus, aus welchen Arbeitsbereichen auf den Datensatztyp zugegriffen werden kann. Wählen Sie aus den folgenden Optionen:

   * **Systemweit**: Benutzer können von allen Arbeitsbereichen, für die sie über Verwaltungsberechtigungen verfügen, aus eine Verbindung zu diesem Datensatztyp herstellen.
   * **Spezifische Arbeitsbereiche**: Fügen Sie die Namen der Arbeitsbereiche hinzu, über die sich Workspace-Manager mit diesem Datensatztyp verbinden können.
1. Klicken Sie auf **Speichern**.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt über die von Ihnen angegebenen Arbeitsbereiche mit verbunden werden.
   * Auf der Karte „Datensatztyp“ wird das Symbol für eine arbeitsbereichsübergreifende Verbindung ![Symbol für eine arbeitsbereichsübergreifende Verbindung](assets/connect-from-other-workspaces-icon.png) angezeigt, um anzugeben, dass der Datensatztyp für die Verbindung über jeden Arbeitsbereich verfügbar ist, den Sie in Ihrer Konfiguration festgelegt haben.

   Der Datensatztyp wird in den vorgesehenen Arbeitsbereichen verfügbar, mit dem eine Verbindung hergestellt werden kann.
1. (Optional) Wechseln Sie zu einem anderen Arbeitsbereich und fügen Sie eine Verbindung zu dem Datensatztyp hinzu, den Sie in den obigen Schritten für eine Workspace-übergreifende Verbindbarkeit aktiviert haben.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).









