---
title: Konfigurieren von arbeitsbereichsübergreifenden Funktionen für den Datensatztyp
description: Sie können festlegen, dass ein Datensatztyp entweder einem anderen Arbeitsbereich hinzugefügt oder über einen anderen Arbeitsbereich verbunden werden kann.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '1030'
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
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this imported record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Im Folgenden finden Sie arbeitsbereichsübergreifende Funktionen von Datensatztypen:

* Sie können einen Datensatztyp als zentralisiert festlegen. Benutzer können zentralisierte Datensatztypen zu anderen Arbeitsbereichen hinzufügen, die sie verwalten können.
* Sie können einen Datensatztyp als verbindbaren Datensatz festlegen. Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

Sie müssen zunächst die arbeitsbereichsübergreifenden Funktionen eines Datensatztyps definieren, bevor Workspace-Manager ihn entweder aus verbinden oder in andere Arbeitsbereiche importieren können.

Sie definieren die arbeitsbereichsübergreifenden Funktionen eines Datensatztyps, wenn Sie einen Datensatztyp erstellen oder bearbeiten.

Weitere Informationen finden Sie in einem der folgenden Artikel:

* [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md)
* [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Konfigurieren des Hinzufügens eines Datensatztyps zu anderen Arbeitsbereichen

Als Workspace-Manager können Sie einen Datensatztyp konfigurieren, der anderen Arbeitsbereichen hinzugefügt wird, wenn Sie einen Datensatztyp erstellen oder bearbeiten.

Wenn Sie das Hinzufügen eines Datensatztyps zu anderen Arbeitsbereichen konfigurieren, kann ein Workspace-Manager den Datensatztyp und alle zugehörigen Informationen in einen der von ihm verwalteten Arbeitsbereiche importieren.

So konfigurieren Sie das Hinzufügen eines Datensatztyps zu einem anderen Arbeitsbereich, wenn Sie den Datensatztyp bearbeiten:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp .
oder
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps.
1. Klicken Sie **Bearbeiten**.

   ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

1. Wählen Sie im Feld **Datensatztyp bearbeiten** die Registerkarte **Erweiterte Einstellungen** aus.
1. Aktivieren Sie die **Zulassen, dass dieser Datensatztyp anderen Arbeitsbereichen hinzugefügt**).

   ![Datensatztyp bearbeiten Erweiterte Einstellungen mit Aktivieren von Zu anderen Arbeitsbereichen hinzufügen](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. Fügen Sie im Feld **Auswählen, wer diesen Datensatztyp zu von ihm verwalteten Arbeitsbereichen hinzufügen kann** Benutzer hinzu, denen Sie erlauben möchten, diesen Datensatztyp zu von ihnen verwalteten Arbeitsbereichen hinzuzufügen.

   Ihr Name wird dem Feld automatisch hinzugefügt.

   Sie können einzelne Benutzer oder Gruppen, Teams, Aufgabengebiete oder Unternehmen hinzufügen, deren Benutzer diesen Datensatztyp den von ihnen verwalteten Arbeitsbereichen hinzufügen dürfen.

   Sie können dieses Feld bearbeiten, nachdem Sie den Datensatztyp gespeichert haben.
1. (Optional) Entfernen Sie Ihren Namen aus dem Feld **Auswählen, wer diesen Datensatztyp zu den von ihm verwalteten Arbeitsbereichen hinzufügen kann**.

1. Klicken Sie auf **Speichern**.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt von den von Ihnen angegebenen Personen zu einem anderen Arbeitsbereich hinzugefügt werden.

   >[!NOTE]
   >
   >Sie können den Datensatztyp und dessen Felder nur über den ursprünglichen Arbeitsbereich bearbeiten.

   * Die Karte „Datensatztyp“ zeigt das Symbol „Globaler ![&quot; an](assets/global-icon.png) um anzugeben, dass der Datensatztyp jedem Arbeitsbereich hinzugefügt werden kann, dessen Manager Sie in Ihrer Konfiguration angegeben haben.
   * Dem Datensatztyp wird ein vom System generiertes **** Workspace-Feld hinzugefügt.

     Das Feld Workspace zeigt den Arbeitsbereich an, aus dem jeder Datensatz erstellt wurde.

     Dieses Feld ist schreibgeschützt und kann nicht gelöscht werden.

## Konfigurieren der Verbindung zu einem Datensatztyp aus anderen Arbeitsbereichen

Sie können einen Datensatztyp konfigurieren, mit dem über andere Arbeitsbereiche eine Verbindung hergestellt werden soll, wenn Sie den Datensatztyp erstellen oder bearbeiten.

So konfigurieren Sie einen Datensatztyp für die Verbindung von anderen Arbeitsbereichen aus, wenn Sie den Datensatztyp bearbeiten:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp und klicken Sie dann auf **Bearbeiten**
oder
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie dann auf **Bearbeiten**.

   ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

1. Wählen Sie im Feld **Datensatztyp bearbeiten** die Registerkarte **Erweiterte Einstellungen** aus.
1. Aktivieren Sie die **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** Einstellung. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Registerkarte „Datensatztyp bearbeiten - Erweiterte Einstellungen“ mit aktivierter Option „Von anderen Arbeitsbereichen verbinden“](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Wenn diese Option aktiviert ist, ist der Datensatztyp verfügbar und kann von anderen Arbeitsbereichen aus verbunden werden.

1. Wählen Sie aus, aus welchen Arbeitsbereichen auf den Datensatztyp zugegriffen werden kann. Wählen Sie aus den folgenden Optionen:

   * **Systemweit**: Benutzer können von allen Arbeitsbereichen, in denen sie Berechtigungen verwalten, aus eine Verbindung zu diesem Datensatztyp herstellen.
   * **Spezifische Arbeitsbereiche**: Fügen Sie die Namen der Arbeitsbereiche hinzu, über die sich Workspace-Manager mit diesem Datensatztyp verbinden können.
1. Klicken Sie **Bearbeiten**.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt über die von Ihnen angegebenen Arbeitsbereiche verbunden werden.
   * Auf der Karte „Datensatztyp“ wird das Symbol für eine arbeitsbereichsübergreifende Verbindung ![Symbol für eine arbeitsbereichsübergreifende Verbindung](assets/connect-from-other-workspaces-icon.png) angezeigt, um anzugeben, dass der Datensatztyp über jeden Arbeitsbereich, den Sie in Ihrer Konfiguration angegeben haben, verbunden werden kann.

   Der Datensatztyp steht nun für die Verbindung über die vorgesehenen Arbeitsbereiche zur Verfügung.









