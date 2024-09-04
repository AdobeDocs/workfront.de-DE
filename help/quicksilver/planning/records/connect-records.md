---
title: Datensätze verbinden
description: Nachdem Sie Verbindungen zwischen Datensatztypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden.
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '2713'
ht-degree: 1%

---


# Datensätze verbinden

{{planning-important-intro}}

Sie können Adobe Workfront Planning-Datensätze miteinander oder mit Objekten aus anderen Anwendungen verbinden.

In diesem Artikel wird beschrieben, wie Sie Datensätze verbinden können. Allgemeine Informationen zum Verbinden von Datensätzen finden Sie unter [Übersicht über verbundene Datensätze](/help/quicksilver/planning/records/connected-records-overview.md).

Zuerst müssen Sie zwei Datensatztypen miteinander verbinden oder einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden. Dadurch werden verknüpfte Datensatzfelder erstellt. Mithilfe der verknüpften Datensatzfelder können Sie dann Datensätze miteinander oder Datensätze mit anderen Objekten aus anderen Anwendungen verbinden.

Das Verbinden von Datensätzen ähnelt dem Verbinden von Datensätzen mit Objekten aus einer anderen Anwendung.

Informationen zum Verbinden von Datensatztypen untereinander oder mit Objektarten aus anderen Anwendungen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

Ein Beispiel für das Verbinden von Datensatztypen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

Sie können Folgendes verbinden:

* Adobe Workfront-Planungsaufzeichnungen
* Adobe Workfront-Planung von Datensätzen mit Objekten aus anderen Anwendungen.

  In den folgenden Anwendungen können Sie Datensätze mit Objekten der unten aufgeführten Typen verbinden:

   * Adobe Workfront

      * Projekte
      * Portfolios
      * Programme
      * Firma
      * Gruppe

   * Adobe Experience Manager Assets

      * Bilddateien
      * Ordner

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td> Standard
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
   <td>   <p>Berechtigungen für einen Arbeitsbereich zum Verbinden von Datensätzen verwalten </p>  
   <p>Zeigen Sie die Berechtigungen für einen Arbeitsbereich oder höher an, um alle Verbindungen zu Objekten und Feldern aus anderen Anwendungen anzuzeigen, unabhängig von Ihrem Zugriff in der anderen Anwendung. </p>
   <p>Zeigen Sie die Berechtigungen für die Objekte an, die Sie über Workfront oder Experience Manager Assets verknüpfen möchten. </p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>To connect Adobe Workfront Planning records with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace to connect records </p>  
   <p>View or higher permissions to a workspace to view all connections to objects and fields from other applications, regardless of your access in the other application. </p>
   <p>View or higher permissions to the objects you want to link from Workfront or Experience Manager Assets. </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++

## Voraussetzungen für das Verbinden von Datensätzen

Um Datensätze mit anderen Datensätzen oder Objekten zu verbinden, müssen Sie über Folgendes verfügen:

* Mindestens ein Arbeitsbereich, ein Datensatztyp und ein Datensatz.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md)
   * [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md)

* Verbindungen zwischen Datensatztypen oder zwischen Datensatztypen und Objekten aus anderen Anwendungen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Datensätze aus der Workfront-Planung verbinden

In den folgenden Bereichen eines Planungsdatensatzes können Sie Datensätze aus der Workfront-Planung verbinden:

* Die verbundenen Datensatzfelder in der Tabellenansicht.
* Vorschau oder Seite des Datensatzes in den verbundenen Datensatzfeldern auf der Registerkarte Details .
* Vorschau oder Seite des Datensatzes auf der Registerkarte Verbindungen .

### Verbinden von Adobe Workfront-Planungsdatensätzen über die Tabellenansicht oder die Registerkarte Details der Datensatzseite

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie verbinden möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Klicken Sie auf den Namen einer Tabellenansicht, um sie zu öffnen.
1. (Optional) Fügen Sie dem ausgewählten Datensatztyp durch Hinzufügen einer neuen Zeile zur Tabelle Datensätze hinzu. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit einem anderen Datensatztyp verbunden haben, wechseln Sie zur verknüpften Datensatzspalte und doppelklicken Sie auf die Zelle, die dem Datensatz entspricht, den Sie mit anderen Datensätzen verknüpfen möchten.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines verbundenen Datensatzes, um ihn zum ausgewählten Datensatz hinzuzufügen. Der Datensatz wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Datensatzes ein und klicken Sie darauf, wenn er in der Liste angezeigt wird. Der Datensatz wird automatisch hinzugefügt.

1. (Optional) Wenn Sie einen Datensatz oder ein Objekt zum Verbinden nicht finden und ihn hinzufügen möchten, klicken Sie auf **+ Hinzufügen** , um einen neuen Datensatz hinzuzufügen. Weitere Informationen finden Sie unter &quot;Erstellen von Datensätzen beim Verbinden&quot;im Artikel [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

   >[!TIP]
   >
   >    Sie können die Seite eines Datensatzes öffnen und andere Datensätze verknüpfen, indem Sie in der Tabellenansicht Folgendes tun:
   >1. Klicken Sie in der Ansicht auf den Namen des Datensatzes.
   >1. Suchen Sie das verknüpfte Datensatzfeld und doppelklicken Sie auf das Feld (falls bereits Datensätze verbunden sind).
   >Oder
   >Klicken Sie auf **Datensätze verbinden** (wenn das Feld leer ist), um Datensätze aus dem verbundenen Datensatz oder Objekttyp hinzuzufügen.
   >
   >![](assets/connect-records-from-record-page-field.png)

1. (Optional) Klicken Sie auf **Alle anzeigen** , um alle Datensätze anzuzeigen.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf &quot;**See all**&quot;geklickt haben, wird das Feld **Objekte verbinden** angezeigt.

   ![](assets/connected-objects-table-for-records.png)

1. Geben Sie den Namen eines Datensatzes in das Suchfeld ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Datensätze im Feld aus und klicken Sie dann auf **Objekte verbinden**.

   Folgendes wird hinzugefügt:

   * Die verknüpften Datensätze werden im verknüpften Datensatzfeld des Datensatzes angezeigt, den Sie in einem vorherigen Schritt ausgewählt haben.
   * Die verknüpften Felder werden mit den Informationen aus den verknüpften Datensätzen ausgefüllt, wenn Sie verknüpfte Suchfelder hinzugefügt haben, als Sie die Datensatztypen verbunden haben.

   Durch die Aktualisierung der verknüpften Datensätze werden die verknüpften Felder für die Datensätze aktualisiert, von denen Sie automatisch eine Verknüpfung herstellen. Verknüpfte Felder können nicht manuell bearbeitet werden.

   >[!TIP]
   >
   >* &quot;Verknüpfte Felder&quot;und &quot;Suchfelder&quot;werden synonym verwendet.
   >
   >* Wenn Sie mehrere Datensätze verbinden möchten, während Sie die Datensatztypen verbunden haben, werden die Feldwerte aus den verschiedenen Objekten entweder durch Kommas getrennt oder gemäß dem Aggregator, den Sie beim Verbinden der Datensatztypen ausgewählt haben, aggregiert.

1. (Optional) Schließen Sie die Seite mit dem Datensatztyp und wechseln Sie zum ausgewählten Arbeitsbereich.
1. Klicken Sie auf die Karte des Datensatztyps, mit dem Sie verknüpft sind.

   Wenn Sie beispielsweise den Datensatz **Kampagne** mit dem Produktdatensatz verbunden haben, klicken Sie auf die Karte **Produkt** .

   Die Karte vom Typ Datensatz sollte in der Tabellenansicht geöffnet werden. Wenn nicht, wählen Sie eine Tabellenansicht aus.

   Beachten Sie, dass im Feld **Kampagne** verknüpfter Datensatz die Namen der Kampagnen angezeigt werden, die Sie mit Produkten auf der Seite Produktdatensatz-Typ verknüpft haben. Durch die Aktualisierung der Campaign-Informationen wird das Campaign-verknüpfte Datensatzfeld für den Produktdatensatz-Typ automatisch aktualisiert.

### Verbinden von Adobe Workfront-Planungsdatensätzen mit Workfront-Objekten über die Tabellenansicht oder die Registerkarte &quot;Details&quot;der Datensatzseite

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

Nachdem Sie eine Verbindung zwischen einem Datensatztyp und einem Workfront-Objekttyp hergestellt haben, können Sie einzelne Datensätze mit Objekten in Workfront verbinden. Die Workfront-Felder, mit denen Sie eine Verbindung herstellen, werden automatisch in die Datensätze eingefügt, aus denen die Objekte verknüpft werden.

>[!NOTE]
>
>Sie können Workfront-Objekttypen nicht über Workfront mit Datensatztypen der Workfront-Planung verbinden.


{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie verbinden möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine **Tabellenansicht** aus dem Dropdownmenü **Ansicht** aus.

1. Klicken Sie auf **Neuer Datensatz** , um einzelne Datensätze zum ausgewählten Datensatztyp hinzuzufügen. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit einem Workfront-Objekttyp verbunden haben, wechseln Sie zur verknüpften Objektspalte und doppelklicken Sie auf die Zelle, die dem Datensatz entspricht, den Sie mit Objekten aus Workfront verknüpfen möchten.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf ein Objekt, um es dem ausgewählten Datensatz hinzuzufügen. Objekte werden alphabetisch aufgelistet. Das Objekt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Objekts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Objekt wird automatisch hinzugefügt.

   >[!TIP]
   >
   >Sie können die Seite eines Datensatzes in der Ansicht öffnen, auf das verknüpfte Datensatzfeld doppelklicken oder im Feld auf **Verbinden** klicken, um Objekte aus dem verbundenen Objekttyp hinzuzufügen.

1. (Optional) Wenn Sie ein Objekt zum Verbinden nicht finden und es hinzufügen möchten, klicken Sie auf **+ Hinzufügen** , um ein neues Projekt oder Portfolio zu erstellen und hinzuzufügen.

   Sie können nur Projekte ohne Vorlage oder Portfolios hinzufügen, wenn Sie sie mit Datensätzen der Planung verbinden. Sie können keine neuen Programme, Benutzer oder Unternehmen hinzufügen.

1. (Optional) Klicken Sie auf &quot;**See all**&quot;, um alle Objekte anzuzeigen, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf &quot;**See all**&quot;geklickt haben, wird das Feld **Objekte verbinden** angezeigt.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Geben Sie den Namen eines Workfront-Objekts in das Suchfeld ein und wählen Sie es dann aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Objekte im Feld aus und klicken Sie dann auf **Objekte verbinden**.

   >[!IMPORTANT]
   >
   >* Sie können nur Workfront-Objekte hinzufügen, auf die Sie Zugriff haben.
   >
   >* Nachdem Sie Workfront-Objekte hinzugefügt haben, können alle Benutzer mit der Berechtigung Anzeigen oder höher zum Arbeitsbereich die Workfront-Objekte und ihre Feldinformationen unabhängig von ihren Berechtigungen oder Zugriffsberechtigungen in Workfront anzeigen.

   Folgendes wird hinzugefügt:

   * Die ausgewählten Workfront-Objekte werden dem verknüpften Datensatzfeld hinzugefügt.
   * Wenn Sie sie bei der Verbindung des Datensatztyps mit Workfront hinzugefügt haben, werden die verknüpften Felder (oder die Suchfelder) der Workfront-Objekte automatisch mit Informationen aus Workfront gefüllt.

   Weitere Informationen zum Verbinden von Datensatztypen mit Objekten aus einer anderen Anwendung finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

1. (Optional) Klicken Sie entweder im verknüpften Feld einer Tabellenansicht oder im verknüpften Feld auf der Datensatzseite auf den Namen eines Workfront-Objekts, das mit einem Workfront-Planungsdatensatz verbunden ist.

   Dadurch wird das Workfront-Objekt in Workfront geöffnet, wenn Sie mindestens über Anzeigeberechtigungen für das Objekt verfügen.

   >[!TIP]
   >
   >* Wenn Sie beim Verbinden der Datensatztypen mehrere Datensätze miteinander verbinden möchten, werden die Werte der Lookup-Felder entweder durch Kommas getrennt angezeigt oder entsprechend dem ausgewählten Aggregator aggregiert.
   >
   >* Für die verknüpften Workfront-Objekte in Workfront wird kein verknüpftes Datensatzfeld erstellt.

1. (Optional) Bewegen Sie in der Tabellenansicht des Datensatztyps den Mauszeiger über die Spaltenüberschrift des verknüpften Workfront-Objekts, klicken Sie auf das Dropdown-Menü und klicken Sie dann auf **Suchfelder bearbeiten**.

1. Hinzufügen von Workfront-Objektfeldern aus dem Bereich **Nicht ausgewählte Felder**

   Oder

   Entfernen Sie Workfront-Objektfelder aus dem Bereich **Ausgewählte Felder** .

   Dadurch werden verknüpfte Felder zu den Workfront-Planungsdatensätzen hinzugefügt oder daraus entfernt. Die mit den entfernten Feldern verknüpften Informationen verbleiben in Workfront.


### Verbinden von Workfront-Planungsdatensätzen mit Adobe Experience Manager-Objekten über die Tabellenansicht oder die Registerkarte &quot;Details&quot;der Datensatzseite

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Workfront Planning-Datensätze mit Adobe Experience Manager Assets verbinden zu können.
>
>Wenn Sie Fragen zum Einstieg in Adobe Admin Console haben, lesen Sie die [FAQ zum einheitlichen Erlebnis für Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nachdem Sie eine Verbindung zwischen einem Datensatztyp und Adobe Experience Manager Assets hergestellt haben, können Sie einzelne Datensätze mit Experience Manager-Assets verbinden. Die Asset-Felder, mit denen Sie eine Verbindung aus Experience Manager Assets hergestellt haben, werden automatisch in den Datensatztyp eingetragen, von dem aus Sie die Verbindung hergestellt haben.

>[!NOTE]
>
>Auf die Planung von Datensätzen und deren Feldern kann über Experience Manager Assets zugegriffen werden, wenn der Workfront-Administrator das Metadaten-Mapping über die Integration zwischen Workfront und Adobe Experience Manager Assets konfiguriert. Weitere Informationen finden Sie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

So verbinden Sie Datensätze mit Experience Manager-Assets:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie verbinden möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine **Tabellenansicht** aus dem Dropdown-Menü **Ansicht** in der oberen rechten Ecke der Seite mit dem Datensatztyp aus.

1. (Optional) Klicken Sie auf **Neuer Datensatz** , um dem ausgewählten Datensatztyp neue Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit Experience Manager Assets verbunden haben, wechseln Sie zur verknüpften Objektspalte und bewegen Sie den Mauszeiger über die Zelle, die dem Datensatz entspricht, den Sie mit anderen Objekten aus Experience Manager verknüpfen möchten, und klicken Sie dann auf das Symbol **+** .

   >[!TIP]
   >
   >  Sie können das Symbol **+** im verknüpften Objektfeld auf der Datensatzseite hinzufügen, um Assets mit dem Datensatz zu verbinden.

   Das Feld **Assets auswählen** wird angezeigt. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Klicken Sie auf , um einige der folgenden Asset-Typen auszuwählen:

   * Bilder
   * Ordner

   Sie können mehrere Assets auswählen.

   >[!IMPORTANT]
   >
   > Sie können nur Assets verbinden, auf die Sie Zugriff haben, um sie in Experience Manager anzuzeigen. Nach der Verbindung können alle Benutzer der Workfront-Planung die Assets in der Workfront-Planung anzeigen, unabhängig vom Zugriff auf die Assets in Experience Manager Assets.

1. Klicken Sie auf **Select**. <!-- we might change this to Connect-->

   Folgendes wird hinzugefügt:

   * Die ausgewählten Experience Manager-Assets werden dem verknüpften Datensatzfeld hinzugefügt.
   * Die verknüpften Felder (oder Lookup-Felder) enthalten Informationen aus dem mit dem Experience Manager verbundenen Asset.

     Alle vorhandenen Informationen aus den Feldern der Experience Manager-Assets werden automatisch in den verknüpften Feldern oder Suchfeldern angezeigt.

     >[!TIP]
     >
     >* Wenn Sie beim Verbinden der Datensatztypen mehrere Datensätze miteinander verbinden möchten, werden die Werte der verschiedenen Objekte je nach ausgewähltem Aggregator entweder durch Kommas getrennt oder aggregiert angezeigt.
     >
     >* Für die verknüpften Experience Manager-Assets in der Experience Manager Assets-Anwendung wird kein mit der Workfront-Planung verknüpftes Datensatzfeld erstellt.

1. (Optional) Gehen Sie zu dem mit Experience Manager Assets verknüpften Datensatztyp und klicken Sie im verknüpften Datensatzfeld auf den Namen eines Assets. Die Experience Manager-Details des Assets werden in einem Popup-Fenster angezeigt.

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Die folgenden Felder werden für eine Bilddatei angezeigt:

   * Eine Miniaturansicht des Bildes
   * Der Name der Bilddatei
   * Dimensionen
   * Größe
   * Beschreibung
   * Der Dateipfad im Experience Manager
   * Der Asset-Typ
   * Erstellungsdatum
   * Änderungsdatum

1. (Optional) Um die Datensatzseite für Experience Manager-Assets in Experience Manager zu öffnen, wechseln Sie zur Seite mit dem Datensatztyp des Datensatzes, von dem Sie die Verknüpfung herstellen, klicken Sie auf den Namen eines Assets im verknüpften Datensatzfeld, um das Popup-Fenster zu öffnen, und klicken Sie dann auf das Symbol **In AEM öffnen** ![](assets/open-asset-icon.png) , um das Asset zu öffnen.

   Dadurch wird das Experience Manager-Asset in Adobe Experience Manager Assets geöffnet.

1. (Optional) Bewegen Sie in der Tabellenansicht des Datensatztyps den Mauszeiger über die Spaltenüberschrift des verknüpften Experience Manager-Assets, klicken Sie auf das Dropdown-Menü und klicken Sie dann auf **Suchfelder bearbeiten**.

1. Hinzufügen von Experience Manager Assets-Objektfeldern aus dem Bereich **Nicht ausgewählte Felder**

   Oder

   Entfernen Sie Workfront-Objektfelder aus dem Bereich **Ausgewählte Felder** .

   Dadurch werden verknüpfte Felder aus den Datensätzen hinzugefügt oder entfernt. Die mit den entfernten Feldern verknüpften Informationen verbleiben unter Adobe Experience Assets.

### Verbinden von Workfront-Planungsdatensätzen mit anderen Datensätzen oder Objekten über den Tab Verbindungen der Datensatzseite

1. Navigieren Sie zu einer beliebigen Ansicht eines Datensatztyps, der mit anderen Planungs-Datensatztypen oder -Objekttypen aus anderen Anwendungen verbunden wurde.
1. Führen Sie die in den vorherigen Unterabschnitten beschriebenen Schritte aus, um einen Datensatz in der Ansicht zu finden, der mit anderen Datensätzen oder Objekten verbunden werden soll.
1. Klicken Sie auf den Namen eines Datensatzes.

   Die Vorschauseite wird geöffnet.
1. (Optional) Klicken Sie auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) , um die Seite des Datensatzes zu öffnen.
1. Klicken Sie auf die Registerkarte **Verbindungen** in der Vorschau oder Seite des Datensatzes.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

   Alle Datensätze oder Objekttypen, die mit dem ausgewählten Datensatztyp verknüpft sind, werden als Abschnitte angezeigt. Verbundene Datensätze oder Objekte werden auf den Karten unter den Namen ihrer Datensätze oder Objekttypen angezeigt.

   >[!TIP]
   >
   >    Standardmäßig werden nur verbundene Datensätze angezeigt, für die einzelne Datensätze verbunden sind.

1. (Optional) Klicken Sie auf **Alle Verbindungen anzeigen** , um alle verbundenen Datensatztypen anzuzeigen, einschließlich der Typen ohne verbundene Datensätze.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil links neben einem Abschnitt, um ihn zu reduzieren.

1. (Bedingt) Klicken Sie auf **Verbinden** , um weitere Datensätze oder Objekte desselben Typs hinzuzufügen.
1. Führen Sie die in den vorherigen Abschnitten beschriebenen Schritte aus, um Datensätze aus der Workfront-Planung oder Objekte aus Workfront oder Experience Manager Assets zu verbinden.
Die Datensätze und Objekte werden sofort hinzugefügt.
1. (Optional) Bewegen Sie den Mauszeiger über die verbundene Karte eines Datensatzes oder Objekts und klicken Sie dann auf das Symbol **Datensatz trennen** **-** , um die Verbindung zum ausgewählten Datensatz zu trennen.

   ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   Der Datensatz wird sofort von allen Bereichen der Workfront-Planung oder von anderen Anwendungen getrennt, in denen er als verbunden angezeigt wird. Alle Lookup-Feldwerte werden ebenfalls entfernt.

## Datensätze aus Workfront-Objekten verbinden

Sie müssen über Folgendes verfügen, um Workfront Planning-Datensätze aus Workfront-Objekten zu verbinden:

* Verbindungen zwischen Datensatztypen und Workfront-Objekttypen, die in der Workfront-Planung erstellt werden.
* Ihr Workfront- oder Gruppenadministrator muss den Bereich Planung zu den Workfront-Projekten, -Portfolios und -Programmen in Ihrer Layout-Vorlage hinzufügen.

Weitere Informationen finden Sie unter [Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;von Adobe Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
