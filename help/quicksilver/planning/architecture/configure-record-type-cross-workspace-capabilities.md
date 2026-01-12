---
title: Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen
description: Sie können in Adobe Workfront Planning festlegen, dass ein Datensatztyp entweder einem anderen Arbeitsbereich hinzugefügt oder über einen anderen Arbeitsbereich verbunden werden kann.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 895fcc9e8bfc6ef21e82ae6dab4c370b0e267cad
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 1%

---


<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->

# Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen

<!--this article is linked to the UI in the Advanced settings/ Cross-workspace settings tab - do not delete or change the URL-->

{{planning-important-intro}}

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

In Adobe Workfront Planning können Sie Datensatztypen so konfigurieren, dass sie in mehreren Arbeitsbereichen funktionieren.

Sie können einen Datensatztyp als einen der folgenden Typen festlegen:

* <span class="preview">**Ein globaler Datensatztyp**: Benutzer können globale Datensatztypen zu anderen Arbeitsbereichen hinzufügen, die sie verwalten können.</span>
* **Ein verbindbarer Datensatztyp**: Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

Sie müssen zunächst die arbeitsbereichsübergreifenden Funktionen eines Datensatztyps definieren, bevor Workspace-Manager ihn entweder zu anderen Arbeitsbereichen hinzufügen oder von anderen Arbeitsbereichen aus verbinden können.

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
<p>So konfigurieren Sie verbindbare Datensatztypen: </p>
<ul> 
<li><p>Jedes Workfront-Paket und jedes Planungspaket</p></li>
ODER
<li>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>

<div class="preview">
<p>So konfigurieren Sie globale Datensatztypen:</p>

<ul> 
<li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
ODER
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p>

</div> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Workflow Prime or Ultimate package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> -->

<div class="preview">

## Konfigurieren globaler Datensatztypen

<!--this is a UI term; don't change the title of this section-->

Als Workspace-Manager können Sie einen Datensatztyp als globalen Datensatztyp konfigurieren. Ein globaler Datensatztyp kann anderen Arbeitsbereichen hinzugefügt werden.

Ein Workspace-Manager kann einem von ihm verwalteten Workspace einen globalen Datensatztyp hinzufügen. Die ursprünglichen Felder des Datensatztyps werden auch dem sekundären Arbeitsbereich hinzugefügt.

Benutzer können Datensätze zu einem globalen Datensatztyp aus jedem Arbeitsbereich hinzufügen, in dem sie über die Berechtigung Beitragen verfügen und in dem der globale Datensatztyp hinzugefügt wird, einschließlich des ursprünglichen Arbeitsbereichs. Sie können Datensätze aus Arbeitsbereichen anzeigen, für die sie nur über Anzeigeberechtigungen verfügen.

Weitere Informationen finden Sie unter [Übersicht über Workspace-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

So konfigurieren Sie einen Datensatztyp als global:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie als „global“ konfigurieren möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp . <!--add new screen shot without Share for now-->

     ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps.
1. Klicken Sie **Bearbeiten** oder **Einstellungen**.

   >[!TIP]
   >
   >Wenn ein Datensatztyp zu einem anderen Arbeitsbereich hinzugefügt wird, wird er in diesem Arbeitsbereich als globaler Datensatztyp angezeigt. In diesem Fall sind die Optionen Bearbeiten und Einstellungen abgeblendet.

1. (Bedingt) Wenn Sie **Bearbeiten** im Feld **Datensatztyp bearbeiten** auf die Registerkarte **Workspace-Einstellungen** geklickt haben

   Wenn Sie auf **Einstellungen** geklickt haben, klicken Sie alternativ auf den **Arbeitsbereichsübergreifende Einstellungen** im linken Bedienfeld.
1. Aktivieren Sie die **Zulassen, dass dieser Datensatztyp anderen Arbeitsbereichen hinzugefügt**).

   ![Bearbeiten des Datensatztyps Arbeitsbereichsübergreifende Einstellungen mit aktivierter Option „Zu anderen Arbeitsbereichen hinzufügen“](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >Nachdem Sie einen globalen Datensatztyp zu einem anderen Arbeitsbereich hinzugefügt haben, kann diese Einstellung nicht mehr deaktiviert werden.

1. Fügen Sie im Feld **Auswählen, wer diesen Datensatztyp zu von ihm verwalteten Arbeitsbereichen hinzufügen kann** Entitäten hinzu, denen Sie erlauben möchten, diesen Datensatztyp zu von ihnen verwalteten Arbeitsbereichen hinzuzufügen.

   Ihr Name wird dem Feld automatisch hinzugefügt.

   Sie können einzelne Benutzer, Gruppen, Teams, Aufgabengebiete oder Unternehmen hinzufügen, deren Benutzer diesen Datensatztyp den von ihnen verwalteten Arbeitsbereichen hinzufügen dürfen.

   Sie können dieses Feld bearbeiten, nachdem Sie den Datensatztyp gespeichert haben.

1. (Optional) Entfernen Sie Ihren Namen aus dem Feld **Auswählen, wer diesen Datensatztyp zu den von ihm verwalteten Arbeitsbereichen hinzufügen kann**.

   >[!TIP]
   >
   >Sie müssen mindestens eine Entität (Benutzer, Team, Gruppe, Rolle oder Unternehmen) festlegen, um diese Einstellung aktivieren zu können.

1. (Bedingt) Klicken Sie **** Feld **Datensatztyp bearbeiten** auf „Speichern“ oder klicken Sie links neben **Einstellungen** in der Seitenkopfzeile auf den Rückwärtspfeil, um Ihre Änderungen zu speichern.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt von den von Ihnen angegebenen Personen zu einem anderen Arbeitsbereich hinzugefügt werden.

   >[!NOTE]
   >
   >Sie können das Erscheinungsbild und die Einstellungen des Datensatztyps sowie seine ursprünglichen Felder nur über den ursprünglichen Arbeitsbereich bearbeiten.

   * Die Karte „Datensatztyp“ zeigt das Symbol **globaler Datensatztyp** ![Symbol für globalen Datensatztyp](assets/global-icon.png) an, um anzugeben, dass der Datensatztyp für das Hinzufügen zu anderen Arbeitsbereichen verfügbar ist.
   * Zur Tabellenansicht des Datensatztyps und **Details seiner Datensätze wird ein systemgeneriertes Workspace-Feld vom Typ** hinzugefügt.

     Das Feld Workspace zeigt den Arbeitsbereich an, aus dem jeder Datensatz erstellt wird.

     Dieses Feld ist schreibgeschützt und kann nicht gelöscht werden.
1. (Optional) Wechseln Sie zu einem anderen Arbeitsbereich und erstellen Sie einen Datensatztyp mithilfe eines vorhandenen Datensatztyps. Wählen Sie den Datensatztyp aus, den Sie in den obigen Schritten aktiviert haben.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Der Datensatztyp, der über einen globalen Datensatztyp im sekundären Arbeitsbereich hinzugefügt wurde, zeigt auch das Symbol **globaler Datensatztyp** (Symbol ![ globalen Datensatztyp](assets/global-icon.png) an.
1. (Optional) Wechseln Sie zurück zum ursprünglichen Arbeitsbereich, in dem Sie den globalen Datensatztyp erstellt haben, und bearbeiten Sie den Datensatztyp, indem Sie die Schritte 1 bis 4 oben <!--ensure this stays accurate-->
1. (Optional) Überprüfen Sie die Liste der Arbeitsbereiche, denen der globale Datensatz hinzugefügt wurde, im Abschnitt **Arbeitsbereiche, in denen dieser Datensatztyp verwendet wird** . Der Workspace-Inhaber wird auch neben dem Workspace-Namen aufgeführt.

   ![Arbeitsbereiche, in denen dieser Datensatztyp verwendet wird](assets/workspaces-where-this-record-type-is-used.png)
1. (Optional) Klicken Sie auf den Namen eines der Arbeitsbereiche, die im Abschnitt **Arbeitsbereiche, in denen dieser Datensatztyp verwendet wird** aufgeführt sind, um diesen Arbeitsbereich zu öffnen.

</div>

## Konfigurieren verbindbarer Datensatztypen

<!--this is a UI term; don't change the title of this section-->

Sie können einen Datensatztyp konfigurieren, mit dem über andere Arbeitsbereiche eine Verbindung hergestellt werden soll, wenn Sie den Datensatztyp erstellen oder bearbeiten.

Die Konfiguration eines Datensatztyps, der verbindbar sein soll, hängt von der Umgebung ab, die Sie für Ihre Konfiguration auswählen.

### Konfigurieren von verbindbaren Datensatztypen in der Produktionsumgebung

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie als verbindbar konfigurieren möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp .

     ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)

   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen. Klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten**.

1. Klicken Sie auf die **Erweiterte Einstellungen**.

1. Aktivieren Sie die Einstellung **Verbindung zu diesem Datensatztyp von anderen Arbeitsbereichen aus zulassen**.

   ![Registerkarte „Erweiterte Einstellungen bearbeiten“ mit aktivierter Option „Von anderen Arbeitsbereichen verbinden“](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   Wenn diese Option aktiviert ist, kann über andere Arbeitsbereiche mit dem Datensatztyp verbunden werden, auf den zugegriffen werden kann.

1. Wählen Sie aus, aus welchen Arbeitsbereichen auf den Datensatztyp zugegriffen werden kann. Wählen Sie aus den folgenden Optionen:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **Systemweit**: Benutzer können von allen Arbeitsbereichen, für die sie über Verwaltungsberechtigungen verfügen, aus eine Verbindung zu diesem Datensatztyp herstellen.
   * **Spezifische Arbeitsbereiche**: Fügen Sie aus dem Dropdown-Menü die Namen der Arbeitsbereiche hinzu, über die sich Workspace-Manager mit diesem Datensatztyp verbinden können.
1. (Bedingt) Klicken Sie im Feld **Datensatztyp bearbeiten** auf **Speichern**, um Ihre Änderungen zu speichern.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt über die von Ihnen angegebenen Arbeitsbereiche mit verbunden werden.
   * Auf der Karte „Datensatztyp“ wird das Symbol „Verbindbarer Datensatztyp“ ![Symbol „Verbindbarer Datensatztyp„) angezeigt](assets/connect-from-other-workspaces-icon.png) um anzugeben, dass der Datensatztyp über jeden Arbeitsbereich, den Sie in Ihrer Konfiguration festgelegt haben, für die Verbindung verfügbar ist.

1. (Optional) Wechseln Sie zu einem anderen Arbeitsbereich und fügen Sie eine Verbindung zu dem Datensatztyp hinzu, den Sie in den obigen Schritten für eine Workspace-übergreifende Verbindbarkeit aktiviert haben.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

<div class="preview">

### Konfigurieren von verbindbaren Datensatztypen in der Vorschau-Umgebung

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie als verbindbar konfigurieren möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp .

     ![Weitere Menüoptionen auf der Karte „Datensatztyp“ mit Einstellungen](assets/more-menu-options-from-record-type-card-with-settings-link.png)

   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps.
1. Klicken Sie **Bearbeiten** oder **Einstellungen**.

1. (Bedingt) Wenn Sie **Bearbeiten** im Feld **Datensatztyp bearbeiten** auf die Registerkarte **Workspace-Einstellungen** geklickt haben

   Wenn Sie auf **Einstellungen** geklickt haben, klicken Sie alternativ auf den **Arbeitsbereichsübergreifende Einstellungen** im linken Bedienfeld.

1. Aktivieren Sie die **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** Einstellung. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![Registerkarte „Datensatztyp bearbeiten“ Arbeitsbereichsübergreifende Einstellungen mit aktivierter Option „Aus anderen Arbeitsbereichen verbinden“](assets/edit-record-type-box-cross-workspace-settings-connectable-record-type-enabled.png)

   Wenn diese Option aktiviert ist, ist der Datensatztyp verfügbar und kann von anderen Arbeitsbereichen aus mit verbunden werden.

1. Wählen Sie aus, aus welchen Arbeitsbereichen auf den Datensatztyp zugegriffen werden kann. Wählen Sie aus den folgenden Optionen:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **Alle Arbeitsbereiche**: Benutzer können von allen Arbeitsbereichen, für die sie über Verwaltungsberechtigungen verfügen, aus eine Verbindung zu diesem Datensatztyp herstellen.
   * **Spezifische Arbeitsbereiche**: Fügen Sie aus dem Dropdown-Menü die Namen der Arbeitsbereiche hinzu, über die sich Workspace-Manager mit diesem Datensatztyp verbinden können.
1. (Bedingt) Klicken Sie **** Feld **Datensatztyp bearbeiten** auf „Speichern“ oder klicken Sie links neben **Einstellungen** in der Seitenkopfzeile auf den Rückwärtspfeil, um Ihre Änderungen zu speichern.

   Folgendes geschieht:

   * Der Datensatztyp und seine Felder können jetzt über die von Ihnen angegebenen Arbeitsbereiche mit verbunden werden.
   * Auf der Karte „Datensatztyp“ wird das Symbol „Verbindbarer Datensatztyp“ ![Symbol „Verbindbarer Datensatztyp„) angezeigt](assets/connect-from-other-workspaces-icon.png) um anzugeben, dass der Datensatztyp über jeden Arbeitsbereich, den Sie in Ihrer Konfiguration festgelegt haben, für die Verbindung verfügbar ist.

1. (Optional) Wechseln Sie zu einem anderen Arbeitsbereich und fügen Sie eine Verbindung zu dem Datensatztyp hinzu, den Sie in den obigen Schritten für eine Workspace-übergreifende Verbindbarkeit aktiviert haben.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

</div>









