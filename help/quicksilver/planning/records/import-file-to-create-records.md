---
title: Erstellen von Datensätzen durch Importieren von Informationen aus einer CSV- oder Excel-Datei
description: Datensätze sind einzelne Instanzen von Datensatztypen, die die Objekttypen von Adobe Workfront Planning sind. In Workfront Planning können Sie Datensätze erstellen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---


# Erstellen von Datensätzen durch Importieren von Informationen aus einer CSV- oder Excel-Datei

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Datensätze sind einzelne Instanzen von Datensatztypen, die die Objekttypen von Adobe Workfront Planning sind. In Workfront Planning können Sie Datensätze erstellen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.

Weitere Informationen zum Erstellen von Datensätzen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

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
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen für den Arbeitsbereich und den Datensatztyp bei, in den Sie Datensätze importieren. </p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   </td> 
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Überlegungen zum Importieren von Datensätzen mithilfe einer Excel- oder CSV-Datei

* Die Spaltenüberschriften in jedem Blatt werden zu den Feldern, die mit Datensätzen verknüpft sind.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen zugeordneten Datensatz.
* Wenn die Excel-Datei mehr als ein Blatt enthält, werden nur die Informationen aus einem Blatt importiert, die Sie während des Importvorgangs auswählen.
* Die Datei sollte folgende Werte nicht überschreiten:
   * 25.000 Zeilen
   * 500 Spalten
* Die Datei sollte nicht größer als 5 MB sein.
* Leere Blätter werden nicht unterstützt.
* Felder der folgenden Typen werden nicht unterstützt und können nicht den Feldern im Importblatt zugeordnet werden:

   * Verbindungsfelder zu Workfront- und AEM Assets-Objekttypen. Sie können nur Verbindungsfelder den Planungs-Datensatztypen zuordnen.
   * Nachschlagen von Feldern aus verbundenen Planungsdatensätzen oder Workfront- und AEM Assets-Objekten
   * Formelfelder
   * Erstellungsdatum, Erstellt von
   * Datum der letzten Änderung, letzte Änderung von
   * <span class="preview">Genehmigt am, Genehmigt von</span>
   * Personen
   * Wenn ein Feld mit mehreren oder nur einer Auswahl importiert wird und es mehr Auswahlmöglichkeiten als ein ähnliches Feld in Planning hat, werden die zusätzlichen Optionen während des Imports erstellt. Nur Benutzer mit der Berechtigung Verwalten für den Arbeitsbereich können neue Auswahlmöglichkeiten importieren.

## Erstellen von Datensätzen durch Importieren einer CSV- oder Excel-Datei

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf die Karte des Datensatztyps, in den Sie die Datensätze importieren möchten.
1. Klicken **oben** auf „Neuer Datensatz“.

   ![Wählen Sie aus, wie Datensätze mit drei Schaltflächen hinzugefügt werden sollen](assets/choose-way-to-add-records-three-button-box.png)
1. Klicken Sie **Aus Datei hochladen** und dann **Weiter**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei per Drag-and-Drop oder klicken Sie **CSV- oder Excel-Datei auswählen** um eine Datei zu suchen.
1. Klicken Sie auf **Vorschau und Bearbeitung**.
1. (Bedingt) Wenn die importierte Datei mehr als ein Blatt enthält, wählen Sie das Optionsfeld des zu importierenden Blatts im Feld **Zu importierendes Blatt auswählen** aus und klicken dann auf **Weiter**. Fahren Sie andernfalls mit dem nächsten Schritt fort.

   ![Tabelle zum Importieren von Datensätzen auswählen](assets/select-a-sheet-to-import-box.png)
1. Wählen Sie in **Planfelder den Spaltenüberschriften zuordnen** das Feld **Planung**, das den Informationen in den einzelnen Spalten des Blatts am besten entspricht.

   ![Planfelder beim Importieren von Datensätzen Spalten zuordnen](assets/map-planning-fields-to-columns-when-importing-records.png)

   Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten 10 Datensätze werden im Vorschau- und Bearbeitungsfeld angezeigt.

   >[!TIP]
   >
   >Nicht alle Feldtypen werden unterstützt. Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Importieren von Datensätzen mithilfe einer Excel- oder CSV](#considerations-about-importing-records-using-an-excel-or-csv-file)Datei in diesem Artikel.


1. (Optional und bedingt) Wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, wählen **in der linken unteren Ecke** Bildschirms die Option „Fehlende Optionen erstellen“. Wenn diese Option aktiviert ist, werden die fehlenden Einfach- und Mehrfachauswahlfelder hinzugefügt.

   >[!NOTE]
   >
   >Wenn der ausgewählte Datensatztyp beispielsweise über ein Statusfeld mit einer einzigen Auswahl wie Neu, In Bearbeitung und Geschlossen verfügt und ein aus einer Datei importiertes Statusfeld auch über eine Option für den Status Halten verfügt, wird die Option für den Status Halten ebenfalls hinzugefügt.
   >
   >Wenn Sie keine Verwaltungsberechtigungen für den Arbeitsbereich haben, können Sie Datensätze importieren, die zusätzlichen Auswahlmöglichkeiten werden jedoch nicht erstellt. Stattdessen erhalten Sie die folgende Nachricht in der oberen rechten Ecke des Felds Planungsfelder Ihren Spaltenüberschriften zuordnen : **Die Auswahlmöglichkeiten, die nicht in der Verbindung vorhanden sind, Einfach- oder Mehrfachauswahlfelder werden nicht hinzugefügt**.

1. Klicken Sie **Importieren**.

   Die folgenden Informationen werden in Workfront Planning importiert:

   * Neue Datensätze, die unten in der Tabellenansicht des ausgewählten Datensatztyps angezeigt werden.
   * Neue Feldwerte für vorhandene Felder, die mit jedem Datensatz verknüpft sind.
   * Neue Auswahlmöglichkeiten für ein Mehrfachauswahlfeld oder ein Einzelauswahlfeld, das in Planning nicht vorhanden war.  <!--when we add connected records - add those here too-->

   Sie können mit der Verwaltung von Feldern und Datensätzen auf der Seite „Datensatztypen“ beginnen.

   Alle Personen mit Zugriff auf Workfront Planning und den Arbeitsbereich können jetzt die importierten Datensätze und deren Informationen anzeigen und bearbeiten.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
