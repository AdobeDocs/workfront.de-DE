---
title: Datensatztypen erstellen
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# Datensatztypen erstellen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die arbeitsbezogenen Elemente veranschaulichen, die im Lebenszyklus Ihres Unternehmens benötigt werden.

Weitere Informationen zu Datensatztypen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
<p>Beliebiges Workfront- und Planungspaket</p>
<p>Beliebiges Workflow- und Planungspaket</p>
<p><b>NOTIZ</b></p>
<p>So konfigurieren Sie verbindbare Datensatztypen: </p>
<ul> 
<li><p>Jedes Workfront-Paket und jedes Planungspaket</p></li>
<p>Oder</p>
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>

<div class="preview">
<p>So konfigurieren Sie globale Datensatztypen:</p>

<ul> 
<li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
<p>Oder</p>
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p>

</div>
   </td> </tr>
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
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> -->

## Überlegungen zum Erstellen von Datensatztypen

* Datensatztypen können auf folgende Weise in einem Arbeitsbereich erstellt werden:

   * Automatisch:
      * Wenn Sie einen Arbeitsbereich mithilfe einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Wenn Sie sie mithilfe einer CSV- oder Excel-Datei importieren.

        Weitere Informationen finden Sie unter [Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

     >[!TIP]
     >
     >Wenn Sie einen Datensatztyp aus einer CSV- oder Excel-Datei importieren, können Sie auch Datensätze und Felder importieren.

   * Manuell:

      * Von Grund auf.

        In diesem Artikel wird beschrieben, wie Sie Datensatztypen von Grund auf neu erstellen.

     <!--
        * <span class="preview">By adding them from another workspace</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


* Sie können Datensatztypen innerhalb eines Abschnitts und von einem Abschnitt eines Arbeitsbereichs in einen anderen verschieben. Datensatztypen können nicht von einem Workspace in einen anderen Workspace verschoben werden.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Datensatztypen können automatisch erstellt werden, wenn Sie einen Arbeitsbereich mithilfe einer Workfront Planning-Vorlage erstellen. Jede Vorlage enthält Beispiel-Datensatztypen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Informationen darüber, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Arbeitsbereichsvorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, werden die Datensatztypen in den folgenden Abschnitten gruppiert:

* Operative Datensatztypen
* Taxonomien

Sie können Datensatztypen manuell sowohl in den Abschnitten Operative Datensatztypen als auch in den Abschnitten Taxonomien hinzufügen. Weitere Informationen finden Sie im Abschnitt [Neuerstellen eines Datensatzes](#create-a-record-type-from-scratch) in diesem Artikel.

## Neuerstellen eines Datensatztyps

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie einen Datensatztyp erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Abschnitt hinzufügen**, um einen neuen Abschnitt zum Arbeitsbereich hinzuzufügen.
1. Klicken Sie **Datensatztyp hinzufügen** und dann **Manuell hinzufügen**.

   Das Feld Datensatztyp hinzufügen wird geöffnet. <!--update screen shot for preview-->

   ![Feld für Datensatztyp mit Darstellungsoptionen hinzufügen](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen auf der Registerkarte **Erscheinungsbild**:

   * Ersetzen Sie „Unbenannter Datensatztyp“ durch den Namen Ihres zukünftigen Datensatztyps. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschreibung**: Fügen Sie weitere Informationen über den Datensatztyp hinzu.
   * Wählen Sie eine Farbe und eine Form für das Symbol aus, das mit dem Datensatztyp verknüpft ist. Gehen Sie folgendermaßen vor:
      * Farbe zur Identifizierung des neuen Datensatztyps auswählen. Dies ist die Farbe des Symbols für den Datensatztyp. Grau ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. (Optional und bedingt) Wenn Sie Systemadministrator sind, klicken Sie auf die Registerkarte **Erweiterte Einstellungen** <span class="preview">oder **Arbeitsbereichsübergreifende Einstellungen**</span> und aktualisieren Sie die Informationen zu den arbeitsbereichsübergreifenden Funktionen des Datensatztyps.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production - Jan 2026-->

   ![Feld „Datensatztyp bearbeiten“ mit der Registerkarte „Erweiterte Einstellungen“](assets/edit-record-type-box-advanced-settings-tab.png)

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Klicken Sie auf **Speichern**.

   Die Karte Datensatztyp wird dem ausgewählten Abschnitt und Arbeitsbereich hinzugefügt.
Die Beschreibung des Datensatztyps wird auf der Karte angezeigt.

   ![Karte vom Typ „Datensatz“ mit Beschreibung](assets/record-type-card-with-description.png)

   Wenn Sie ausgewählt haben, diesen Datensatz von anderen Arbeitsbereichen zu verbinden, wird das Symbol **Verbindbarer Datensatz** (Symbol ![&#x200B; Verbindung von anderen &#x200B;](assets/connect-from-other-workspaces-icon.png)) auf der Datensatzkarte angezeigt.

   <span class="preview">Wenn Sie ausgewählt haben, dass dieser Datensatz anderen Arbeitsbereichen hinzugefügt werden kann, wird das Symbol **Globaler** Globaler![Datensatz](assets/global-icon.png) auf der Datensatzkarte angezeigt. </span>

1. (Optional) Zeigen Sie mit der Maus auf die Karte für den Datensatztyp und klicken Sie oben rechts auf **Mehr**-Symbol ![Mehr](assets/more-menu.png) und dann auf **Bearbeiten** oder <span class="preview">**Einstellungen**</span>, um Informationen zum Datensatztyp zu ändern.

   Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Klicken Sie auf die Karte „Datensatztyp“, um die Seite „Datensatztyp“ zu öffnen.

   ![Operativer Datensatztyp leer](assets/operational-record-type-blank.png)

   Die Seite „Datensatztyp“ wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operativen Datensatztyps angezeigt:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf das **Mehr**-Symbol ![Mehr &#x200B;](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten**, um ihn umzubenennen oder die zugehörigen Informationen zu ändern. Weitere Informationen finden Sie unter [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Klicken Sie auf **+ Neuer**, um Datensätze des ausgewählten Datensatztyps hinzuzufügen. Weitere Informationen finden Sie unter [Einträge erstellen](/help/quicksilver/planning/records/create-records.md).
1. (Optional) Klicken Sie auf das Symbol **+** in der oberen rechten Ecke der Tabelle, um dem Datensatztyp weitere Felder hinzuzufügen.

   Weitere Informationen zum Erstellen von Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

1. (Optional) Klicken Sie auf den nach links zeigenden Pfeil links neben dem Namen des Datensatztyps in der Kopfzeile, um zum ausgewählten Arbeitsbereich zurückzukehren.

1. (Optional) Klicken Sie im Arbeitsbereich auf eine Karte für den Datensatztyp und halten Sie diese gedrückt, um den Datensatztyp per Drag-and-Drop an die gewünschte Stelle zu ziehen oder in einen anderen Abschnitt zu verschieben.

   Die Änderungen werden automatisch gespeichert.

   Weitere Informationen zum Hinzufügen von Datensätzen, Löschen oder Bearbeiten von Datensatztypen oder Aktualisieren der Ansicht auf der Seite „Datensatztyp“ finden Sie in den folgenden Artikeln:

   * [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md)
   * [Datensatztypen löschen](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Datensatzansichten verwalten](/help/quicksilver/planning/views/manage-record-views.md)

## Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei

Beim Importieren von Informationen aus einer CSV- oder Excel-Datei können Sie Folgendes importieren:

* Eintragstypen
* Einträge
* Datensatzfelder

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

<!--

<div class="preview">

## Create record types by adding existing ones from another workspace 

You can add record types to a workspace by adding existing ones from another workspace. You can only add record types that have been configured as global record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->