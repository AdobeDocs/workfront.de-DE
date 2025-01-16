---
title: Datensatztypen erstellen
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1394'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# Datensatztypen erstellen

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die arbeitsbezogenen Elemente veranschaulichen, die im Lebenszyklus Ihres Unternehmens benötigt werden.

Weitere Informationen zu Datensatztypen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

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
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>. </p> 
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
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
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

      * Wenn Sie sie mithilfe einer Excel- oder CSV-Datei importieren.

     >[!TIP]
     >
     >Wenn Sie einen Datensatztyp aus einer Excel- oder CSV-Datei importieren, können Sie auch Datensätze und Felder importieren.

   * Manuell:

      * Von Grund auf.

        In diesem Artikel wird beschrieben, wie Sie Datensatztypen von Grund auf neu erstellen.

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
1. Klicken Sie **Datensatztyp hinzufügen** und dann auf **Neu**.

   Das Feld Datensatztyp hinzufügen wird geöffnet.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen:

   * Ersetzen Sie „Unbenannter Datensatztyp“ durch den Namen Ihres zukünftigen Datensatztyps. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschreibung**: Fügen Sie weitere Informationen über den Datensatztyp hinzu.
   * Wählen Sie eine Farbe und eine Form für das Symbol aus, das mit dem Datensatztyp verknüpft ist. Gehen Sie folgendermaßen vor:
      * Farbe zur Identifizierung des neuen Datensatztyps auswählen. Dies ist die Farbe des Symbols für den Datensatztyp. Grau ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. Klicken Sie auf **Erstellen**.

   Die Karte Datensatztyp wird dem ausgewählten Abschnitt und Arbeitsbereich hinzugefügt.
Die Beschreibung des Datensatztyps wird auf der Karte angezeigt.

   ![](assets/record-type-card-with-description.png)

1. (Optional) Zeigen Sie mit der Maus auf die Karte für den Datensatztyp und klicken Sie auf das Symbol **Mehr** oben rechts ![](assets/more-menu.png) und dann auf **Bearbeiten**, um Informationen zum Datensatztyp zu ändern.
1. (Optional) Klicken Sie auf die Karte „Datensatztyp“, um die Seite „Datensatztyp“ zu öffnen.

   ![](assets/operational-record-type-blank.png)

   Die Seite „Datensatztyp“ wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operativen Datensatztyps angezeigt:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf das **Mehr**-Symbol ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten**, um ihn umzubenennen oder die zugehörigen Informationen zu ändern. Weitere Informationen finden Sie unter [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

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

## Erstellen von Datensatztypen durch Importieren einer Excel- oder CSV-Datei

Beachten Sie beim Importieren von Datensatztypen mit einer Excel- oder CSV-Datei Folgendes:

* Jedes Blatt der Excel-Datei wird zu einem Datensatztyp. Der Name des Blatts wird zum Namen des Datensatztyps.
* Wenn nur ein Blatt vorhanden ist oder Sie eine CSV-Datei importieren, wird der Name der Datei zum Namen des Datensatztyps.
* Die Spaltenüberschriften der einzelnen Tabellen werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für die jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit seinem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei sollte Folgendes nicht überschreiten:
   * 10.000 Zeilen
   * 500 Spalten
* Die Excel-Datei sollte nicht größer als 5 MB sein.
* Leere Blätter werden nicht unterstützt.

So importieren Sie Datensatztypen mithilfe einer Excel- oder CSV-Datei:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensatztypen erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie **Datensatztyp hinzufügen**.
1. Klicken Sie auf **Aus Datei**.
1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei per Drag-and-Drop oder klicken Sie **CSV- oder Excel-Datei auswählen** um eine Datei zu suchen.
1. Klicken Sie auf **Vorschau und Bearbeitung**.

   Das **„Vorschau und**&quot; wird mit den folgenden Informationen angezeigt:

   * Die Namen der Tabellen oder der zukünftigen Datensatztypen werden im linken Bereich angezeigt. Workfront Planning wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
   * Das erste Blatt oder der erste Datensatztyp wird ausgewählt, und die Namen der mit ihm verknüpften Felder werden als Spaltenüberschriften angezeigt. Der Typ jedes Felds ist standardmäßig ausgewählt.
   * Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten 10 Datensätze werden im Vorschau- und Bearbeitungsfeld angezeigt.

   ![](assets/preview-and-edit-box.png)

1. (Optional) Klicken Sie auf den Namen der einzelnen Blätter im linken Bereich, um die darin enthaltenen Informationen zu überprüfen.

   >[!NOTE]
   >
   >Leere Blätter werden nicht unterstützt und sind abgeblendet.

1. (Optional) Deaktivieren Sie im linken Bereich die Auswahl der Blätter, die Sie nicht importieren möchten.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blättert, wenn Sie die Auswahl aufgehoben haben, wird die Anzeige mit grauem Hintergrund angezeigt.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben der Spaltenüberschrift, um eine der folgenden Aktionen durchzuführen:

   * Eines der Felder umbenennen
   * Ändern des **Feldtyps**
   * Aktualisieren Sie das Feld **Beschreibung**

1. (Bedingt) Klicken Sie nach dem Aktualisieren der Feldinformationen auf **Speichern**.

1. Klicken Sie **Importieren** wenn Sie bereit sind, Ihre Datei zu importieren.

   Die folgenden Informationen werden in Workfront Planning importiert:

   * Neue Datensatztypen
   * Neue Felder, die mit jedem Datensatztyp verknüpft sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Datensatztypseiten beginnen.

   Alle Personen mit Zugriff auf Workfront Planning können jetzt die importierten Datensatztypen und deren Informationen anzeigen und bearbeiten.
