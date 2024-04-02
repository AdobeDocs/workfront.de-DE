---
title: Erstellen von Datensatztypen
description: Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten Arbeitselemente illustrieren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: eaf1cd4142b83a42d068e2d02fe673fa4dd25769
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Erstellen von Datensatztypen

{{maestro-important-intro}}

Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten arbeitsbezogenen Elemente veranschaulichen.
Datensatztypen können eine der folgenden sein:

Weitere Informationen zu Datensatztypen finden Sie unter [Übersicht über Datensatztypen](../architecture/overview-of-record-types-and-taxonomies.md).

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
<td>
   <p> Produkt</p> </td>
   <td> Adobe Workfront
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
   <p>Aktuell: Plan</p>
   Oder
   <p>Neu: Standard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Für die Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen zum Erstellen von Datensatztypen

* Sie können Datensatztypen in einem Arbeitsbereich wie folgt erstellen:

   * Automatisch:
      * Wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

      * Wenn Sie sie mit einer Excel- oder CSV-Datei importieren.

        >[!IMPORTANT]
        >
        >Diese Funktion ist seit dem 21. März 2024 vorübergehend deaktiviert. Sie wird zu einem späteren Zeitpunkt aktiviert.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * Manuell:

      * Von Grund auf neu.

        In diesem Artikel wird beschrieben, wie Sie neue Datensatztypen erstellen.

* Sie können Datensatztypen innerhalb eines Abschnitts und von einem Abschnitt eines Arbeitsbereichs in einen anderen verschieben. Es ist nicht möglich, Datensatztypen von einem Arbeitsbereich in einen anderen zu verschieben.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Sie können Datensatztypen automatisch erstellen, wenn Sie einen Arbeitsbereich mithilfe einer Workfront-Planungsvorlage erstellen. Jede Vorlage enthält Beispieldatensatztypen.

Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, sind die Datensatztypen in den folgenden Abschnitten gruppiert:

* Betriebsdatentypen
* Taxonomien

Sie können Datensatztypen manuell sowohl in den Abschnitten &quot;Operative Datensatztypen&quot;als auch &quot;Taxonomien&quot;hinzufügen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

Informationen dazu, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Workspace-Vorlagen](../architecture/workspace-templates.md).

## Erstellen eines neuen Datensatztyps

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen erstellen möchten.
1. (Optional) Klicken Sie auf **Abschnitt hinzufügen** , um einen neuen Abschnitt zum Arbeitsbereich hinzuzufügen.
1. Klicks **Datensatztyp hinzufügen**.
1. (Bedingt) Klicken Sie bei der Erstellung von Datensatztypen durch Importieren einer Excel- oder CSV-Datei auf **Von Grund auf**. Andernfalls wird die **Datensatztyp hinzufügen** wird geöffnet.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen:

   * **Name des Datensatztyps**: Ersetzen Sie &quot;Unbenannter operationeller Datensatztyp&quot;durch den Namen Ihres künftigen Datensatztyps.
   * **Erscheinungsbild**: Definieren Sie die Farbe und Form des Symbols, das dem Datensatztyp zugeordnet ist. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um Ihren neuen Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp. Graustufen ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. Klicken Sie außerhalb der **Datensatztyp hinzufügen** zum Speichern des Datensatztyps.

   Die Karte vom Typ Datensatz wird dem ausgewählten Bereich und Arbeitsbereich hinzugefügt.
Die Anzahl der Felder, die der Datensatztyp enthält, wird auf der Karte angezeigt.
1. (Optional) Klicken Sie auf die Karte vom Typ Datensatz , um die Seite vom Typ Datensatz zu öffnen.

   ![](assets/operational-record-type-blank.png)

   Die Seite vom Typ Datensatz wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   >[!TIP]
   >
   >    Wenn Sie einen Datensatztyp aus einer Excel- oder CSV-Datei importieren, werden auch Datensätze importiert.

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operationellen Datensatztyps angezeigt:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf **Mehr** icon ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Umbenennen** , um ihn umzubenennen.

1. (Optional) Klicken Sie auf **+ Neuer Datensatz** , um Datensätze des ausgewählten Datensatztyps hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](../records/create-records.md).
1. (Optional) Klicken Sie auf die **+** rechts oben in der Tabelle, um dem Datensatztyp weitere Felder hinzuzufügen.

   Weitere Informationen zum Erstellen von Feldern finden Sie unter [Felder erstellen](../fields/create-fields.md).

1. (Optional) Klicken Sie in der Kopfzeile auf den nach links zeigenden Pfeil neben dem Namen des Datensatztyps, um zum ausgewählten Arbeitsbereich zurückzukehren.

   Die Karte vom Typ Datensatz zeigt die Anzahl der Felder und Verbindungen an, die der Datensatztyp enthält.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Weitere Informationen zum Hinzufügen von Datensätzen, zum Löschen oder Bearbeiten von Datensatztypen oder zum Aktualisieren der Ansicht auf der Seite mit dem Datensatztyp finden Sie in den folgenden Artikeln:

   * [Datensätze erstellen](../records/create-records.md)
   * [Löschen von Datensatztypen](../architecture/delete-record-types.md)
   * [Datensatztypen bearbeiten](../architecture/edit-record-types.md)
   * [Verwalten von Datensatzansichten](../views/manage-record-views.md)

1. (Optional) Klicken Sie im Arbeitsbereich auf eine Karte vom Typ Datensatz, um den Datensatztyp per Drag-and-Drop an eine gewünschte Stelle zu ziehen oder in einen anderen Bereich zu verschieben.

   Die Änderungen werden automatisch gespeichert.

## Erstellen von Datensatztypen durch Importieren einer Excel- oder CSV-Datei

>[!IMPORTANT]
>
>Diese Funktion ist seit dem 21. März 2024 vorübergehend deaktiviert. Sie wird zu einem späteren Zeitpunkt aktiviert.

Beachten Sie beim Importieren von Datensatztypen mit einer Excel- oder CSV-Datei Folgendes:

* Jedes Blatt der Excel-Datei wird zu einem Datensatztyp.
* Die Spalten der einzelnen Blätter werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für ihre jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit dem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei darf nicht größer sein als:
   * 50.000 Zeilen
   * 500 Spalten
* Die Excel-Datei sollte nicht größer als 5 MB sein.
* Leere Arbeitsblätter werden nicht unterstützt.

So importieren Sie Datensatztypen mithilfe einer Excel-Datei:

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen erstellen möchten.
1. Klicks **Datensatztyp hinzufügen**.
1. Klicks **Excel/CSV**.
1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei in den Arbeitsbereich oder klicken Sie auf **CSV- oder Excel-Datei auswählen** um nach einer zu suchen.
1. Klicks **Daten überprüfen**.

   Das Feld Vorschau und Bearbeitung wird mit den folgenden Informationen angezeigt:

   * Die Namen der Blätter oder der künftigen Datensatztypen werden im linken Bereich angezeigt. Workfront Planning wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
   * Die erste Tabelle oder der erste Datensatztyp wird ausgewählt und die Namen der Felder, die mit ihr verknüpft sind, werden als Spaltenüberschriften angezeigt. Der Feldtyp wird standardmäßig ausgewählt.
   * Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten zehn Datensätze werden im Feld Vorschau und Bearbeitung angezeigt.

   ![](assets/preview-and-edit-box.png)

1. (Optional) Klicken Sie im linken Bereich auf den Namen der einzelnen Blätter, um die darin enthaltenen Informationen zu überprüfen.

   >[!NOTE]
   >
   >    Leere Blätter werden nicht unterstützt und sind abgeblendet.


1. (Optional) Klicken Sie auf die **Zu importierende Tabellen auswählen** Dropdown-Menü aus und heben Sie die Auswahl der Tabellen auf, die Sie nicht importieren möchten.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Sie können die Auswahl der Anzeige mit grauem Hintergrund deaktivieren.

1. Klicks **Import** wenn Sie bereit sind, Ihre Datei zu importieren.

   Die folgenden Informationen werden in die Workfront-Planung importiert:

   * Neue Datensatztypen
   * Neue Felder, die jedem Datensatztyp zugeordnet sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Seiten mit den Datensatztypen beginnen.

   Jeder, der Zugriff auf Workfront Planning hat, kann jetzt die importierten Datensatztypen und ihre Informationen anzeigen und bearbeiten. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->