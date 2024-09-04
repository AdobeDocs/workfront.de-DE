---
title: Dateitypen bearbeiten
description: Sie können Datensatztypen nach dem Speichern bearbeiten. Datensatztypen sind die Objekttypen der Adobe Workfront-Planung.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 2%

---


# Datensatztypen bearbeiten

{{planning-important-intro}}

Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. Sie können das Erscheinungsbild von Datensatztypen bearbeiten, die Sie oder andere Benutzer erstellt haben. Informationen zum Erstellen von Workfront-Planungs-Datensatztypen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

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
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
   <p>Nur Systemadministratoren können Datensatztypen von anderen Arbeitsbereichen aus verbinden.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## Datensatztypen bearbeiten

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke der Datensatztypkarte und klicken Sie dann auf **Bearbeiten**
Oder
   * Klicken Sie auf eine Karte vom Typ Datensatz, um die Seite vom Typ Datensatz zu öffnen, klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie dann auf **Bearbeiten**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. Im Feld **Datensatz-Typ bearbeiten** wird standardmäßig die Registerkarte **Erscheinungsbild** geöffnet.

   ![](assets/edit-record-type-box-appearance-tab.png)

   Aktualisieren Sie die folgenden Informationen auf der Registerkarte **Erscheinungsbild** :

   * Bearbeiten Sie bei Bedarf den Namen des Datensatztyps. <!--did they add a field label for this?-->
   * **Beschreibung**: Bearbeiten oder fügen Sie eine Beschreibung für den Datensatztyp mit weiteren Informationen hinzu.
   * Bearbeiten Sie die Farbe und Form des Symbols, das dem Datensatztyp zugeordnet ist. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um den Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. (Bedingt) Wenn Sie Systemadministrator sind, klicken Sie im Feld **Datensatz-Typ bearbeiten** auf die Registerkarte **Erweiterte Einstellungen** .

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. (Bedingt) Aktualisieren Sie als Systemadministrator die folgenden Informationen auf der Registerkarte **Erweiterte Einstellungen**:

   * **Von anderen Arbeitsbereichen verbinden**: Wählen Sie diesen Umschalter aus, um Benutzern zu ermöglichen, von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herzustellen. Diese Option ist standardmäßig deaktiviert.
   * **Systemweit**: Wählen Sie diese Option, damit Benutzer von allen Arbeitsbereichen im System aus eine Verbindung zu diesem Datensatz herstellen können.
   * **Spezifische Arbeitsbereiche**: Wählen Sie diese Option, um die Arbeitsbereiche zu beschränken, von denen Benutzer eine Verbindung zu diesem Datensatztyp herstellen können. Erweitern Sie dann das Dropdown-Menü und wählen Sie die Arbeitsbereiche aus, aus denen Benutzer eine Verbindung zu diesem Datensatztyp herstellen sollen. Sie können mit der Eingabe des Namens eines Arbeitsbereichs beginnen und diesen auswählen, wenn er in der Liste angezeigt wird.

1. Klicken Sie auf **Speichern**.

   Auf der Datensatztyp-Karte im Arbeitsbereich wird oben rechts ein Verbindungssymbol ![](assets/connect-from-other-workspaces-icon.png) angezeigt, das angibt, dass der Datensatz jetzt über andere Arbeitsbereiche zugänglich ist.

1. (Optional) Klicken Sie im Arbeitsbereich auf die Karte vom Typ Datensatz , um die Seite des Datensatztyps zu öffnen, und benennen Sie dann den Datensatztyp in der Kopfzeile um.

1. (Optional) Um einen anderen Datensatztyp zu bearbeiten, erweitern Sie auf der Seite mit dem Datensatztyp den nach unten zeigenden Pfeil rechts neben dem Namen eines Datensatztyps, suchen Sie nach einem Datensatztyp und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)