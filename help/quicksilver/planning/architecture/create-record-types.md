---
title: Datensatztypen erstellen
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 459e3883101b644a91d5e2a32288cf5b02a02bd9
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# Datensatztypen erstellen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die arbeitsbezogenen Elemente veranschaulichen, die im Lebenszyklus Ihres Unternehmens benötigt werden.

Weitere Informationen zu Datensatztypen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>In der Produktionsumgebung müssen alle Benutzer, einschließlich der Systemadministratoren, einer Layoutvorlage zugewiesen werden, die Planning enthält.</p>
<p><span class="preview">In der Vorschau-Umgebung ist für Standardbenutzer und Systemadministratoren „Planung“ standardmäßig aktiviert.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
        * <span class="preview">By importing then from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add cross-workspace record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md). </span>-->


* Sie können Datensatztypen innerhalb eines Abschnitts und von einem Abschnitt eines Arbeitsbereichs in einen anderen verschieben. Datensatztypen können nicht von einem Workspace in einen anderen Workspace verschoben werden.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Datensatztypen können automatisch erstellt werden, wenn Sie einen Arbeitsbereich mithilfe einer Workfront Planning-Vorlage erstellen. Jede Vorlage enthält Beispiel-Datensatztypen.

Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, werden die Datensatztypen in den folgenden Abschnitten gruppiert:

* Operative Datensatztypen
* Taxonomien

Sie können Datensatztypen manuell sowohl in den Abschnitten Operative Datensatztypen als auch in den Abschnitten Taxonomien hinzufügen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Informationen darüber, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Arbeitsbereichsvorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

## Neuerstellen eines Datensatztyps

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie einen Datensatztyp erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Abschnitt hinzufügen**, um einen neuen Abschnitt zum Arbeitsbereich hinzuzufügen.
1. Klicken Sie **Datensatztyp hinzufügen** und dann **Manuell hinzufügen**.

   Das Feld Datensatztyp hinzufügen wird geöffnet.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![Feld für Datensatztyp mit Darstellungsoptionen hinzufügen](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen auf der Registerkarte **Erscheinungsbild**:

   * Ersetzen Sie „Unbenannter Datensatztyp“ durch den Namen Ihres zukünftigen Datensatztyps. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschreibung**: Fügen Sie weitere Informationen über den Datensatztyp hinzu.
   * Wählen Sie eine Farbe und eine Form für das Symbol aus, das mit dem Datensatztyp verknüpft ist. Gehen Sie folgendermaßen vor:
      * Farbe zur Identifizierung des neuen Datensatztyps auswählen. Dies ist die Farbe des Symbols für den Datensatztyp. Grau ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. (Optional und bedingt) Wenn Sie Systemadministrator sind, klicken Sie auf **Erweiterte Einstellungen** und aktualisieren Sie die folgenden Informationen im Abschnitt **Konnektivitätsbereich**: <!--the info here is duplicated in the Edit record types article-->

   * Aktivieren Sie die Einstellung **Verbindung von anderem Arbeitsbereich herstellen**. Wenn diese Option aktiviert ist, ist der Datensatztyp verfügbar und kann von anderen Arbeitsbereichen aus verbunden werden.
   * Wählen Sie aus, aus welchen Arbeitsbereichen auf den Datensatztyp zugegriffen werden kann. Wählen Sie aus den folgenden Optionen:

      * **Systemweit**: Benutzer können von allen Arbeitsbereichen, in denen sie Berechtigungen verwalten, aus eine Verbindung zu diesem Datensatztyp herstellen.
      * **Spezifische Arbeitsbereiche**: Fügen Sie die Namen der Arbeitsbereiche hinzu, über die sich Workspace-Manager mit diesem Datensatztyp verbinden können.

   ![Feld „Datensatztyp erstellen“ auf der Registerkarte „Erweiterte Einstellungen“](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
    <div class="preview">
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
        * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
            You can designate specific users who can add this record type to other workspaces. 
        * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
            You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
        For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
        ******** replace screen shot below **********
        ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
    -->

1. Klicken Sie auf **Erstellen**.

   Die Karte Datensatztyp wird dem ausgewählten Abschnitt und Arbeitsbereich hinzugefügt.
Die Beschreibung des Datensatztyps wird auf der Karte angezeigt.

   ![Karte vom Typ „Datensatz“ mit Beschreibung](assets/record-type-card-with-description.png)

1. (Optional) Zeigen Sie mit der Maus auf die Karte für den Datensatztyp und klicken Sie oben rechts auf **Mehr**-Symbol ![Mehr](assets/more-menu.png) und dann auf **Bearbeiten**, um Informationen zum Datensatztyp zu ändern.
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

   Klicken Sie auf das **Mehr**-Symbol ![Mehr ](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten**, um ihn umzubenennen oder die zugehörigen Informationen zu ändern. Weitere Informationen finden Sie unter [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

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

* Datensatztypen
* Einträge
* Datensatzfelder

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

<!--

<div class="preview">

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as cross-workspace record types. 

For information, see [Add cross-workspace record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

</div>

-->