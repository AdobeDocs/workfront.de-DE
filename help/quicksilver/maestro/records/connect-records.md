---
title: Datensätze verbinden
description: Nachdem Sie Verbindungen zwischen Datensatztypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '2356'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Datensätze verbinden

{{maestro-important-intro}}

Sie können Adobe Workfront Planning-Datensätze miteinander oder mit Objekten aus anderen Anwendungen verbinden.

Zuerst müssen Sie zwei Datensatztypen miteinander verbinden oder einen Datensatztyp mit einem Objekttyp aus einer anderen Anwendung verbinden. Dadurch werden verknüpfte Datensatzfelder erstellt. Mithilfe der verknüpften Datensatzfelder können Sie dann Datensätze miteinander oder Datensätze mit anderen Objekten aus anderen Anwendungen verbinden.

Das Verbinden von Datensätzen ähnelt dem Verbinden von Datensätzen mit Objekten aus einer anderen Anwendung.

Informationen zum Verbinden von Datensatztypen untereinander oder mit Objekttypen aus anderen Anwendungen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

Ein Beispiel für das Verbinden von Datensatztypen finden Sie unter [Beispiel für das Verbinden von Datensatztypen und Datensätzen](../architecture/example-connect-record-types-and-records.md).

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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Um Adobe Workfront Planning-Datensätze mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit dem Adobe Unified Experience integriert sein. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am geschlossenen Betaprogramm für die Adobe Workfront-Planung teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich zum Verbinden von Datensätzen verwalten </p>  
   <p>Zeigen Sie die Berechtigungen für einen Arbeitsbereich oder höher an, um alle Verbindungen zu Objekten und Feldern aus anderen Anwendungen anzuzeigen, unabhängig von Ihrem Zugriff in einer anderen Anwendung. </p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Datensätze verbinden

### Überlegungen zum Verbinden von Datensätzen

* Nachdem Sie die Datensatztypen miteinander verbunden haben, werden die verbundenen Datensatztypen in der Tabelle der Datensatztypen, von denen sie verknüpft sind, und auf den Datensatzseiten als verknüpfte Datensatzfelder angezeigt.
* Sie können Datensätze und Objekte der verknüpften Datensätze und Objekttypen aus den verknüpften Datensatzfeldern durchsuchen und hinzufügen.
* Sie können Felder der verknüpften Datensatztypen zur Tabelle des Datensatztyps hinzufügen, von dem Sie die Verknüpfung herstellen.
* Die Werte verknüpfter Felder in den Datensätzen, aus denen Sie die Relation herstellen, können nicht manuell aktualisiert werden.

  Die Werte der verknüpften Felder der verknüpften Datensätze füllen den Workfront Planning-Datensatz aus, den Sie automatisch aus dem ursprünglichen Datensatz oder Objekt verknüpfen.

* Jeder, der Zugriff auf die Workfront-Planung und -Ansicht oder höhere Berechtigungen für den Arbeitsbereich hat, kann die Verbindungen sehen, die Sie zwischen Datensätzen oder zwischen Datensätzen und Objekten anderer Anwendungen herstellen. Sie können verbundene Datensätze und Objekte unabhängig von ihren Berechtigungen in den Anwendungen anzeigen, mit denen Sie eine Verbindung herstellen.
* Sie können die Verbindungen aller anderen Benutzer anzeigen und bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, in dem die verbundenen Datensätze gespeichert sind.
* Sie können einen Datensatz mit einem oder mehreren Objekten aus einer anderen Anwendung verbinden.
* Um Datensätze mit anderen Datensätzen oder Objekten zu verknüpfen, ist Folgendes erforderlich:

   * Mindestens ein Arbeitsbereich, ein Datensatztyp und ein Datensatz.

     Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md)
      * [Erstellen von Datensatztypen](../architecture/create-record-types.md)
      * [Datensätze erstellen](../records/create-records.md)

   * Verbindungen zwischen Datensatztypen oder zwischen Datensatztypen und Objekten aus anderen Anwendungen. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md)

### Adobe Workfront-Planungsdatensätze verbinden

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensätze verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine **Verzeichnis** Ansicht von **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. (Optional) Fügen Sie dem ausgewählten Datensatztyp durch Hinzufügen einer neuen Zeile zur Tabelle Datensätze hinzu. Weitere Informationen finden Sie unter [Datensätze erstellen](../../maestro/records/create-records.md).
1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit einem anderen Datensatztyp verbunden haben, wechseln Sie zur verknüpften Datensatzspalte und doppelklicken Sie auf die Zelle, die dem Datensatz entspricht, den Sie mit anderen Datensätzen verknüpfen möchten.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf den Namen eines verbundenen Datensatzes, um ihn zum ausgewählten Datensatz hinzuzufügen. Der Datensatz wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Datensatzes ein und klicken Sie darauf, wenn er in der Liste angezeigt wird. Der Datensatz wird automatisch hinzugefügt.
   * Klicks **Alle anzeigen** , um alle Datensätze anzuzeigen.

1. (Bedingt) Wenn Sie auf **Alle auswählen** im vorherigen Schritt die Variable **Objekte verbinden** angezeigt.

   ![](assets/connected-objects-table-for-records.png)

1. Geben Sie den Namen eines Datensatzes in das Suchfeld ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Datensätze im Feld aus und klicken Sie auf **Objekte verbinden** in der oberen rechten Ecke des Felds &quot;Objekte verbinden&quot;ein.

   >[!TIP]
   >
   >    Sie können die Seite eines Datensatzes öffnen, das verknüpfte Datensatzfeld suchen und auf **Datensätze verbinden** im Feld, um Datensätze aus dem verbundenen Datensatz oder Objekttyp hinzuzufügen.
   >
   >![](assets/connect-records-from-record-page-field.png)

   Folgendes wird hinzugefügt:

   * Die verknüpften Datensätze werden im verknüpften Datensatzfeld des Datensatzes angezeigt, den Sie in Schritt 6 ausgewählt haben. <!--accurate?-->
   * Die verknüpften Felder werden mit den Informationen aus den verknüpften Datensätzen ausgefüllt, wenn Sie verknüpfte Suchfelder hinzugefügt haben, als Sie die Datensatztypen verbunden haben.

   Durch die Aktualisierung der verknüpften Datensätze werden die verknüpften Felder für die Datensätze aktualisiert, von denen Sie automatisch eine Verknüpfung herstellen. Verknüpfte Felder können nicht manuell bearbeitet werden.

   >[!TIP]
   >
   >* &quot;Verknüpfte Felder&quot;und &quot;Suchfelder&quot;werden synonym verwendet.
   >
   >* Wenn Sie die **Mehrere Datensätze zulassen** festlegen, wenn Sie die Datensatztypen miteinander verbunden haben, werden die Feldwerte für mehrere ausgewählte Objekte entweder durch Kommas getrennt angezeigt oder entsprechend dem ausgewählten Aggregator aggregiert.

1. (Optional) Schließen Sie die Seite mit dem Datensatztyp und wechseln Sie zum ausgewählten Arbeitsbereich.
1. Klicken Sie auf die Karte des Datensatztyps, mit dem Sie verknüpft sind.

   Wenn Sie beispielsweise die **Kampagne** mit dem Produktdatensatz aufzeichnen, klicken Sie auf die **Produkt** Karte.

   Die Karte vom Typ Datensatz sollte in der Tabellenansicht geöffnet werden. Wenn nicht, wählen Sie eine Tabellenansicht aus.

   Beachten Sie, dass **Kampagne** Das Feld für verknüpfte Datensätze zeigt die Namen der Kampagnen an, die Sie mit Produkten verknüpft haben, auf der Seite Produktdatensatz-Typ . Durch die Aktualisierung der Campaign-Informationen wird das Campaign-verknüpfte Datensatzfeld für den Produktdatensatz-Typ automatisch aktualisiert.

### Verbinden von Adobe Workfront-Planungsprotokollen mit Workfront-Objekten

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

Nachdem Sie eine Verbindung zwischen einem Datensatztyp und einem Workfront-Objekttyp hergestellt haben, können Sie einzelne Datensätze mit Objekten in Workfront verbinden. Die Workfront-Felder, mit denen Sie eine Verbindung herstellen, werden automatisch in die Datensätze eingefügt, aus denen die Objekte verknüpft werden.

>[!NOTE]
>
>Sie können Workfront-Objekte nicht mit Datensätzen der Workfront-Planung aus Workfront verbinden.


{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensätze verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine **Verzeichnis** Ansicht von **Ansicht** Dropdown-Menü.

1. Klicks **Neuer Datensatz**  , um dem ausgewählten Datensatztyp einzelne Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](../../maestro/records/create-records.md).
1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit einem Workfront-Objekttyp verbunden haben, wechseln Sie zur verknüpften Objektspalte und doppelklicken Sie auf die Zelle, die dem Datensatz entspricht, den Sie mit Objekten aus Workfront verknüpfen möchten.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Liste auf ein Objekt, um es dem ausgewählten Datensatz hinzuzufügen. Objekte werden alphabetisch aufgelistet. Das Objekt wird automatisch hinzugefügt.
   * Geben Sie den Namen eines Objekts ein und klicken Sie darauf, wenn es in der Liste angezeigt wird. Das Objekt wird automatisch hinzugefügt.
   * Klicks **Alle anzeigen** , um alle Objekte anzuzeigen, für die Sie mindestens über die entsprechenden Berechtigungen verfügen.

1. (Bedingt) Wenn Sie auf **Alle anzeigen** im vorherigen Schritt die Variable **Objekte verbinden** angezeigt.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Geben Sie den Namen eines Workfront-Objekts in das Suchfeld ein und wählen Sie es dann aus, wenn es in der Liste angezeigt wird

   Oder

   Wählen Sie den Namen eines oder mehrerer Objekte im Feld aus und klicken Sie dann auf **Objekte verbinden** in der oberen rechten Ecke des Felds &quot;Objekte verbinden&quot;ein.

   >[!IMPORTANT]
   >
   >* Sie können nur Workfront-Objekte hinzufügen, auf die Sie Zugriff haben.
   >
   >* Nachdem Sie Workfront-Objekte hinzugefügt haben, können alle Benutzer mit der Berechtigung Anzeigen oder höher zum Arbeitsbereich die Workfront-Objekte und ihre Feldinformationen unabhängig von ihren Berechtigungen oder Zugriffsberechtigungen in Workfront anzeigen.

   Folgendes wird hinzugefügt:

   * Die ausgewählten Workfront-Objekte werden dem verknüpften Datensatzfeld hinzugefügt.
   * Wenn Sie sie bei der Verbindung des Datensatztyps mit Workfront hinzugefügt haben, werden die verknüpften Felder (oder die Suchfelder) der Workfront-Objekte automatisch mit Informationen aus Workfront gefüllt.

   >[!TIP]
   >
   >Sie können die Seite eines Datensatzes öffnen, das verknüpfte Datensatzfeld suchen und auf das **+** im Feld, um Objekte aus dem verbundenen Objekttyp hinzuzufügen.

   Weitere Informationen zum Verbinden von Datensatztypen mit Objekten aus einer anderen Anwendung finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

1. (Optional) Klicken Sie entweder im verknüpften Feld einer Tabellenansicht oder im verknüpften Feld auf der Datensatzseite auf den Namen eines Workfront-Objekts, das mit einem Workfront-Planungsdatensatz verbunden ist.

   Dadurch wird die schreibgeschützte Datensatzseite für die Workfront-Planung für das verknüpfte Workfront-Objekt geöffnet. Die Felder, die Sie als Suchfelder ausgewählt haben, als Sie den Datensatztyp mit der Workfront-Objektanzeige auf der Datensatzseite Workfront-Planung verbunden haben.

   >[!TIP]
   >
   >* Wenn Sie die Einstellung Mehrere Datensätze zulassen aktivieren, werden die Werte der Lookup-Felder entweder durch Kommas getrennt angezeigt oder entsprechend dem ausgewählten Aggregator aggregiert.
   >
   >* Für die verknüpften Workfront-Objekte in Workfront wird kein verknüpftes Datensatzfeld erstellt.

1. (Optional) Um das verknüpfte Workfront-Objekt in Workfront zu öffnen, klicken Sie auf **Zu Quelle wechseln** in der rechten oberen Ecke der Datensatzseite des Workfront-Objekts.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Dadurch wird die Workfront-Objektseite geöffnet, wenn Sie zumindest über Anzeigeberechtigungen für das Objekt verfügen. Sie können Informationen zum Workfront-Objekt bearbeiten, sofern Sie dazu berechtigt sind.

1. (Optional) Bewegen Sie in der Tabellenansicht des Datensatztyps den Mauszeiger über die Spaltenüberschrift des verknüpften Workfront-Objekts, klicken Sie auf das Dropdown-Menü und klicken Sie auf **Suchfelder bearbeiten**.

1. Fügen Sie Workfront-Objektfelder aus der **Nicht ausgewählte Felder** area

   Oder

   Entfernen Sie Workfront-Objektfelder aus dem **Ausgewählte Felder** Bereich.

   Dadurch werden verknüpfte Felder zu den Workfront-Planungsdatensätzen hinzugefügt oder daraus entfernt. Die mit den entfernten Feldern verknüpften Informationen verbleiben in Workfront.


### Verbinden von Workfront-Planungsprotokollen mit Adobe Experience Manager-Objekten

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Sie müssen über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein, um Workfront Planning-Datensätze mit Adobe Experience Manager Assets verbinden zu können.
>
>Wenn Sie Fragen zum Einstieg in die Adobe Admin Console haben, lesen Sie den Abschnitt [Häufig gestellte Fragen zu Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Nachdem Sie eine Verbindung zwischen einem Datensatztyp und Adobe Experience Manager Assets hergestellt haben, können Sie einzelne Datensätze mit Experience Manager-Assets verbinden. Die Asset-Felder, mit denen Sie eine Verbindung aus Experience Manager Assets hergestellt haben, werden automatisch in den Datensatztyp eingetragen, von dem aus Sie die Verbindung hergestellt haben.

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, aus dem Sie Datensätze verbinden möchten.
1. Klicken Sie auf die Karte eines Datensatztyps, um die Seite vom Typ Datensatz zu öffnen.
1. Wählen Sie eine **Verzeichnis** Ansicht von **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.

1. (Optional) Klicken Sie auf **Neuer Datensatz** , um dem ausgewählten Datensatztyp neue Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](../../maestro/records/create-records.md).
1. (Bedingt) Nachdem Sie den ausgewählten Datensatztyp mit Experience Manager Assets verbunden haben, wechseln Sie zur verknüpften Objektspalte und bewegen Sie den Mauszeiger über die Zelle, die dem Datensatz entspricht, den Sie mit anderen Objekten aus Experience Manager verknüpfen möchten. Klicken Sie dann auf die Schaltfläche **+** Symbol.

   >[!TIP]
   >
   >  Klicken Sie auf das **+** im Feld verknüpftes Objekt auf der Datensatzseite, um Assets mit dem Datensatz zu verbinden.

   Die **Auswählen von Assets** angezeigt. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. Klicken Sie auf , um einige der folgenden Asset-Typen auszuwählen:

   * Bilder
   * Ordner

   Sie können mehrere Assets auswählen.

   >[!IMPORTANT]
   >
   > Sie können nur Assets verbinden, auf die Sie Zugriff haben, um sie in Experience Manager anzuzeigen. Nach der Verbindung können alle Benutzer der Workfront-Planung die Assets in der Workfront-Planung anzeigen, unabhängig vom Zugriff auf die Assets in Experience Manager Assets.

1. Klicks **Auswählen**. <!-- we might change this to Connect-->

   Folgendes wird hinzugefügt:

   * Die ausgewählten Experience Manager-Assets werden dem verknüpften Datensatzfeld hinzugefügt.
   * Die verknüpften Felder (oder Lookup-Felder) enthalten Informationen aus dem mit dem Experience Manager verbundenen Asset.

     Alle vorhandenen Informationen aus den Feldern der Experience Manager-Assets werden automatisch in den verknüpften Feldern oder Suchfeldern angezeigt.

     >[!TIP]
     >
     >* Wenn Sie die Einstellung Mehrere Datensätze zulassen aktiviert haben, werden die Werte der verschiedenen Objekte je nach ausgewähltem Aggregator entweder durch Kommas getrennt oder aggregiert angezeigt.
     >
     >* Für die verknüpften Experience Manager-Assets in der Experience Manager Assets-Anwendung wird kein mit der Workfront-Planung verknüpftes Datensatzfeld erstellt.

1. (Optional) Gehen Sie zu dem mit Experience Manager Assets verknüpften Datensatztyp und klicken Sie im verknüpften Datensatzfeld auf den Namen eines Assets. Die Experience Manager-Details des Assets werden in einem Popup-Fenster angezeigt. <!--update screen shot with hi-rez picture-->

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

1. (Optional) Um die Datensatzseite für Experience Manager-Assets in Experience Manager zu öffnen, wechseln Sie zur Seite mit dem Datensatztyp des Datensatzes, von dem Sie die Verknüpfung herstellen, klicken Sie auf den Namen eines Assets im verknüpften Datensatzfeld, um das Popup-Fenster zu öffnen, und klicken Sie dann auf das **Öffnen** icon ![](assets/open-asset-icon.png) , um das Asset zu öffnen.

   Dadurch wird das Experience Manager-Asset in Adobe Experience Manager Assets geöffnet.

1. (Optional) Bewegen Sie in der Tabellenansicht des Datensatztyps den Mauszeiger über die Spaltenüberschrift des verknüpften Experience Manager-Assets, klicken Sie auf das Dropdown-Menü und klicken Sie auf **Suchfelder bearbeiten**.

1. Fügen Sie Experience Manager Assets-Objektfelder aus der **Nicht ausgewählte Felder** area

   Oder

   Entfernen Sie Workfront-Objektfelder aus dem **Ausgewählte Felder** Bereich.

   Dadurch werden verknüpfte Felder aus den Datensätzen hinzugefügt oder entfernt. Die mit den entfernten Feldern verknüpften Informationen verbleiben unter Adobe Experience Assets.
