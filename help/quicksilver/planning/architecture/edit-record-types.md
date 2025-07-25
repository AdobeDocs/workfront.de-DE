---
title: Datensatztypen bearbeiten
description: Datensatztypen können nach ihrem Speichern bearbeitet werden. Datensatztypen sind die Objekttypen von Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 2%

---


# Datensatztypen bearbeiten

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. Sie können das Erscheinungsbild von Datensatztypen bearbeiten, die Sie oder eine andere Person erstellt haben. Informationen zum Erstellen von Workfront Planning-Datensatztypen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

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
   <td><p> Standard </p>
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
   <td>   <p>Verwalten der Berechtigungen für einen Arbeitsbereich und Datensatztyp </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Nur Systemadministratoren können Datensatztypen für die Verbindung von anderen Arbeitsbereichen aktivieren</p> </td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Datensatztypen bearbeiten

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp und klicken Sie dann auf **Bearbeiten**
oder
   * <span class="preview">Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie dann auf **Bearbeiten**. </span>

   <span class="preview">![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card.png)</span>

1. Im Feld **Datensatztyp bearbeiten** wird standardmäßig die Registerkarte **Erscheinungsbild** geöffnet.

   ![Registerkarte „Erscheinungsbild des Felds „Datensatztyp bearbeiten“ ](assets/edit-record-type-box-appearance-tab.png)

   Aktualisieren Sie die folgenden Informationen auf der Registerkarte **Erscheinungsbild**:

   * Bearbeiten Sie bei Bedarf den Namen des Datensatztyps. <!--did they add a field label for this?-->
   * **Beschreibung**: Bearbeiten oder fügen Sie eine Beschreibung für den Datensatztyp mit weiteren Informationen hinzu.
   * Bearbeiten Sie die Farbe und Form des Symbols, das mit dem Datensatztyp verknüpft ist. Gehen Sie folgendermaßen vor:
      * Farbe zur Identifizierung des Datensatztyps auswählen. Dies ist die Farbe des Symbols für den Datensatztyp.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

   <!--old info: 
   1. (Conditional) If you are a system administrator, click the **Advanced settings** tab in the **Edit record type** box. 
      ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
   1. (Conditional) Update the following information in the **Advanced settings** tab: 
      * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
      * Choose from which workspaces the record type can be accessed. Choose from the following options:
         * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
         * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.-->


1. (Optional und bedingt) Wenn Sie Systemadministrator sind, klicken Sie auf **Erweiterte Einstellungen** und aktualisieren Sie die folgenden Informationen im Abschnitt **Arbeitsbereichsübergreifende**): <!--the info here is duplicated in the Create record types article-->
   * Aktivieren Sie die **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** Einstellung: Damit können Workspace-Manager von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.\
     Sie können festlegen, aus welchen Arbeitsbereichen dieser Datensatztyp verbunden werden kann. Sie können sie für alle Arbeitsbereiche verfügbar machen oder bestimmte Arbeitsbereiche festlegen, in die Sie sie importieren können.
Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Registerkarte „Erweiterte Einstellungen“ im Feld „Datensatztyp bearbeiten“](assets/edit-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types:
      1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
         * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
               You can designate specific users who can add this record type to other workspaces. 
         * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
               You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
         For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  
         ******** replace screen shot below **********
         ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
      -->

1. Klicken Sie auf **Speichern**.

   Auf der Karte „Datensatztyp“ im Arbeitsbereich wird oben rechts das Symbol „Verbindung ![ anderen Arbeitsbereichen herstellen](assets/connect-from-other-workspaces-icon.png) angezeigt, um anzugeben, dass der Datensatz jetzt von anderen Arbeitsbereichen aus zugänglich ist.

1. (Optional) Klicken Sie im Arbeitsbereich auf die Karte Datensatztyp , um die Seite des Datensatztyps zu öffnen, und benennen Sie dann den Datensatztyp in der Kopfzeile um.

1. (Optional) Zum Bearbeiten eines anderen Datensatztyps erweitern Sie auf der Seite „Datensatztyp“ den nach unten zeigenden Pfeil rechts neben dem Namen eines Datensatztyps, suchen Sie nach einem Datensatztyp und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   ![Dropdown-Liste „Datensatztyp“ auf der Seite „Datensatztyp“ mit Suchfeld](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
