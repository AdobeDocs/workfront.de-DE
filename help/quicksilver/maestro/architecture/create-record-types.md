---
title: Erstellen von operationellen Datensatztypen
description: Datensatztypen sind die Objekttypen von Adobe Maestro. In Maestro können Sie benutzerdefinierte Datensatztypen erstellen, die die Arbeitselemente illustrieren, die im Lebenszyklus Ihres Unternehmens benötigt werden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Erstellen von operationellen Datensatztypen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Datensatztypen sind die Objekttypen von Adobe Maestro. In Maestro können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten arbeitsbezogenen Elemente veranschaulichen.

Datensatztypen können eine der folgenden sein:

* **Betriebsdatentypen**
* **Taxonomien**

Weitere Informationen zu Maestro-Datensatztypen finden Sie unter [Übersicht über Datensatztypen und Taxonomien](../architecture/overview-of-record-types-and-taxonomies.md).

Das Erstellen operativer Datensatztypen ähnelt dem Erstellen von Taxonomie-Datensatztypen. In diesem Artikel wird beschrieben, wie Sie betriebliche Datensatztypen erstellen.

Informationen zum Erstellen von Taxonomien finden Sie unter [Erstellen von Taxonomiedatensatztypen](../architecture/create-a-taxonomy.md).

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
   <td>
   <p> Adobe Workfront</p> <p>Um Maestro-Record-Typen mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen zum Erstellen von Datensatztypen

* Sie können Datensatztypen in einem Arbeitsbereich erstellen, indem Sie einen der folgenden Schritte ausführen:

   * Automatisch:
      * Wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).
      * Wenn Sie sie mit einer Excel- oder CSV-Datei importieren. Dies ist nicht für Taxonomie-Datensatztypen verfügbar.
      * Wenn Sie eine Verbindung zu Objekttypen aus einer anderen Anwendung erstellen, wenn Sie Felder zu einem Datensatztyp hinzufügen. Dadurch wird in Maestro ein schreibgeschützter Datensatztyp erstellt, der mit Objektarten aus der Originalanwendung verbunden ist.

     Informationen zum Verbinden von Objekttypen mit Maestro-Datensätzen finden Sie unter [Datensätze verbinden](../records/connect-records.md).
   * Manuell:

      * Von Grund auf neu.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Sie können Datensatztypen automatisch erstellen, wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen. Jede Maestro-Vorlage enthält Beispiel-Betriebs- und Taxonomiedatensatztypen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

Informationen dazu, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Workspace-Vorlagen](../architecture/workspace-templates.md).

## Erstellen eines neuen Datensatztyps

In diesem Artikel wird beschrieben, wie Sie von Grund auf betriebliche Datensatztypen erstellen. Das Erstellen neuer betrieblicher Datensatztypen ist mit dem Erstellen von Taxonomien vergleichbar.

Weitere Informationen zu Taxonomien finden Sie unter [Erstellen einer Taxonomie](../architecture/create-a-taxonomy.md).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront oder **Hauptmenü** icon ![](assets/main-menu-shell.png)  in der oberen linken Ecke, falls verfügbar, klicken Sie auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen erstellen möchten.
1. Klicks **Datensatztyp hinzufügen**.
1. (Bedingt) Wenn Sie einen operationellen Datensatztyp erstellen, klicken Sie auf **Von Grund auf**. Diese Option ist beim Erstellen von Taxonomien nicht verfügbar.

   Das Feld Datensatztyp hinzufügen wird geöffnet.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Wählen Sie die folgenden Informationen aus:

   * **Name des Eintrags**: Ersetzen Sie &quot;Unbenannter operationeller Datensatztyp&quot;durch den Namen Ihres künftigen Datensatztyps. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Erscheinungsbild**: Definieren Sie die Farbe und Form des Symbols, das dem Datensatztyp zugeordnet ist. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um Ihren neuen Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp. Graustufen ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. Klicken Sie außerhalb der **Datensatztyp hinzufügen** zum Speichern des Datensatzes.

   Die Karte vom Typ Datensatz wird dem ausgewählten Arbeitsbereich hinzugefügt.
Die Anzahl der Felder, die der Datensatztyp enthält, wird auf der Karte angezeigt.
1. (Optional) Klicken Sie auf die Karte vom Typ Datensatz , um die Seite vom Typ Datensatz zu öffnen.

   ![](assets/operational-record-type-blank.png)

   Die Seite mit dem Datensatztyp wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operationellen Datensatztyps angezeigt:

   * Name

     Das Feld Name ist das einzige Feld, das automatisch für Taxonomien erstellt wird.
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf **Mehr** icon ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Umbenennen** , um ihn umzubenennen.

1. (Optional) Klicken Sie auf **+ Neu &lt; Name des Datensatztyps >** , um Datensätze des ausgewählten Datensatztyps hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](../records/create-records.md).
1. (Optional) Klicken Sie auf die **+** rechts oben in der Tabelle, um dem Datensatztyp weitere Felder hinzuzufügen. Weitere Informationen finden Sie unter [Felder erstellen](../fields/create-fields.md).
1. (Optional) Klicken Sie auf den linken Pfeil neben dem Namen des Datensatztyps, um zum ausgewählten Arbeitsbereich zurückzukehren.

   Die Karte vom Typ Datensatz zeigt die Anzahl der Felder und Verbindungen an, die der Datensatztyp enthält.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Weitere Informationen zum Hinzufügen von Datensätzen, zum Löschen oder Bearbeiten von Datensatztypen oder zum Aktualisieren der Ansicht auf der Seite mit dem Datensatztyp finden Sie in den folgenden Artikeln:

   * [Datensätze erstellen](../records/create-records.md)
   * [Löschen von Datensatztypen](../architecture/delete-record-types.md)
   * [Datensatztypen bearbeiten](../architecture/edit-record-types.md)
   * [Verwalten von Datensatzansichten in Adobe Maestro](../views/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## Erstellen von Datensatztypen durch Importieren einer Excel- oder CSV-Datei

Beachten Sie beim Importieren von Datensatztypen mit einer Excel- oder CSV-Datei Folgendes:

* Jedes Blatt der Excel-Datei wird in Maestro zu einem Datensatztyp.
* Die Spalten der einzelnen Blätter werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für ihre jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit dem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei darf nicht größer sein als:
   * 10.000 Zeilen
   * 500 Spalten
* Die Excel-Datei sollte nicht größer als 5 MB sein.
* Leere Arbeitsblätter werden nicht unterstützt.

So importieren Sie Datensatztypen mithilfe einer Excel-Datei:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen erstellen möchten.
1. Klicks **Datensatztyp hinzufügen**.
1. (Bedingt) Wenn Sie einen operationellen Datensatztyp erstellen, klicken Sie auf **Excel/CSV**.

   >[!NOTE]
   >
   >    Diese Option ist beim Erstellen von Taxonomie-Datensatztypen nicht verfügbar.

1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei in den Arbeitsbereich oder klicken Sie auf **CSV- oder Excel-Datei auswählen** um nach einer zu suchen.
1. Klicks **Daten überprüfen**.

   Das Feld Vorschau und Bearbeitung wird mit den folgenden Informationen angezeigt:

   * Die Namen der Blätter oder der künftigen Datensatztypen werden im linken Bereich angezeigt. Maestro wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
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

   Die folgenden Informationen werden in Maestro importiert:

   * Neue Datensatztypen
   * Neue Felder, die jedem Datensatztyp zugeordnet sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Seiten mit den Datensatztypen beginnen.

   Jeder mit Zugriff auf Maestro kann jetzt die importierten Datensatztypen und ihre Informationen anzeigen und bearbeiten. <!--this will change with permissions-->

## Verbinden von Datensatztypen mit Objekttypen aus einer anderen Anwendung

Sie können Datensatztypen importieren, wenn Sie eine Verbindung zwischen einem Maestro-Record-Typ und einem Objekttyp aus einer anderen Anwendung herstellen. Dadurch wird in Maestro ein schreibgeschützter Datensatztyp erstellt, der dem Objekttyp in der Drittanbieteranwendung entspricht.

Sie können beispielsweise Datensatztypen erstellen, indem Sie Maestro-Datensatztypen mit Workfront-Projekten verbinden. Daher wird der Workfront-Projektobjekttyp als schreibgeschützter Datensatztyp in Maestro importiert. Standardmäßig erhält der Datensatztyp den Namen &quot;Workfront Project&quot;. <!--has this name changed? Lusine wanted to change it at some point-->

Sie können die folgenden Objekte aus den folgenden Anwendungen importieren:

* In Workfront:

   * Projekte
   * Portfolios
   * Programme
   * Firma
   * Gruppe

Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).
