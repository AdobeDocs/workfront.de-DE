---
title: Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.

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
<p>Oder</p>
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
</table>-->


## Überlegungen zum Importieren von Datensatztypen mithilfe einer Excel- oder CSV-Datei

* Jedes Blatt der Excel-Datei wird zu einem Datensatztyp. Der Name des Blatts wird zum Namen des Datensatztyps.
* Wenn nur ein Blatt vorhanden ist oder Sie eine CSV-Datei importieren, wird der Name der Datei zum Namen des Datensatztyps.
* Die Spaltenüberschriften in jedem Blatt werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für die jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit seinem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei sollte Folgendes nicht überschreiten:
   * 25.000 Zeilen
   * 500 Spalten
* Die Datei sollte nicht größer als 5 MB sein.
* Leere Blätter werden nicht unterstützt.
* Felder der folgenden Typen werden nicht unterstützt und können nicht den Feldern im Importblatt zugeordnet werden:

   * Verbindungsfelder zu Workfront- und AEM Assets-Objekttypen.
   * Nachschlagen von Feldern aus verbundenen Planungsdatensätzen oder Workfront- und AEM Assets-Objekten
   * Formelfelder
   * Erstellungsdatum, Erstellt von
   * Datum der letzten Änderung, letzte Änderung von
   * Genehmigt am, Genehmigt von
   * Personen

So importieren Sie Datensatztypen mithilfe einer Excel- oder CSV-Datei:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensatztypen erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie **Datensatztyp hinzufügen**.
1. Klicken Sie **Aus Datei hochladen**.
1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei per Drag-and-Drop oder klicken Sie **CSV- oder Excel-Datei auswählen** um eine Datei zu suchen, und wählen Sie sie aus.
1. Klicken Sie auf **Vorschau und Bearbeitung**.

   Das **„Vorschau und**&quot; wird mit den folgenden Informationen angezeigt:

   * Die Namen der Tabellen oder der zukünftigen Datensatztypen werden im linken Bereich angezeigt. Workfront Planning wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
   * Das erste Blatt oder der erste Datensatztyp wird ausgewählt, und die Namen der mit ihm verknüpften Felder werden als Spaltenüberschriften angezeigt. Der Typ jedes Felds ist standardmäßig ausgewählt.
   * Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten 10 Datensätze werden im Vorschau- und Bearbeitungsfeld angezeigt.

   ![Vorschau und Bearbeitungsfeld](assets/preview-and-edit-box.png)

1. (Optional) Klicken Sie auf den Namen der einzelnen Blätter im linken Bereich, um die darin enthaltenen Informationen zu überprüfen.

   >[!NOTE]
   >
   >Leere Blätter werden nicht unterstützt und sind abgeblendet.

1. (Optional) Deaktivieren Sie im linken Bereich die Auswahl der Blätter, die Sie nicht importieren möchten.

   ![Dropdown-Liste Zu importierende Tabellen auswählen mit nicht ausgewählter Option](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blättert, wenn Sie die Auswahl aufgehoben haben, wird die Anzeige mit grauem Hintergrund angezeigt.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben einer Spaltenüberschrift, um auf der Registerkarte **Feld** eine der folgenden Aktionen auszuführen:

   ![Registerkarte „Feld“ im Importfeld „Datensatztyp-Zuordnung“](assets/field-tab-on-record-type-import-mapping-box.png)

   * Eines der Felder umbenennen
   * Ändern des **Feldtyps**
   * Aktualisieren Sie das Feld **Beschreibung**

1. (Optional) Klicken Sie auf die **Verbindung**, um die Informationen in der Spalte einem verbundenen Feld von anderen Datensatztypen zuzuordnen.

   ![Registerkarte „Verbindung“ im Feld „Datensatztyp-Import-Mapping“](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Sie können nur Felder aus Workfront Planning-verbundenen Datensätzen zuordnen. Sie können keine Felder von Workfront- oder AEM Assets-Verbindungen zuordnen. Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Importieren von Datensatztypen mithilfe einer Excel- oder CSV](#considerations-about-importing-record-types-using-an-excel-or-csv-file)Datei in diesem Artikel.

1. (Bedingt) Klicken Sie nach dem Aktualisieren der Feldinformationen auf **Speichern**.

1. Klicken Sie **Importieren** wenn Sie bereit sind, Ihre Datei zu importieren.

   Die folgenden Informationen werden in Workfront Planning importiert:

   * Neue Datensatztypen
   * Neue Felder, die mit jedem Datensatztyp verknüpft sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Datensatztypseiten beginnen.

   Alle Personen mit Zugriff auf Workfront Planning und den Arbeitsbereich können jetzt die importierten Datensatztypen und deren Informationen anzeigen und bearbeiten.
