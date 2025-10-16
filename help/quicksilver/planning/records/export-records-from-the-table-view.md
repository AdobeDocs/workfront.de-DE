---
title: Exportieren von Datensätzen aus der Tabellenansicht
description: Sie können Datensätze und ihre Informationen aus der Tabellenansicht in eine CSV- oder Excel-Datei exportieren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 1%

---

# Datensätze aus der Tabellenansicht exportieren

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Datensätze und deren Informationen aus der Tabellenansicht in eine Excel- oder CSV-Datei exportieren.

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
   <td><p>Licht oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich und einen Datensatztyp</p>   
   <p>Anzeigen von oder höheren Berechtigungen für eine Ansicht</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## Datensätze aus der Tabellenansicht exportieren

Beachten Sie beim Exportieren der Tabellenansicht Folgendes:

* Die in eine Excel-Datei exportierten Informationen behalten die Filter, Gruppierungen und Sortierungen bei, die in Workfront Planning auf die Tabellenansicht angewendet wurden. Gruppierungen sind in der CSV-Datei nicht sichtbar.

* Miniaturansichten und benutzerdefinierte Zeilenfarben werden in exportierten Dateien nicht unterstützt.

* Es werden nur Felder exportiert, die in der Workfront-Benutzeroberfläche sichtbar sind. Ausgeblendete Felder werden nicht exportiert.

So exportieren Sie Informationen aus der Tabellenansicht oder einem Datensatztyp:

1. Wechseln Sie zu einer Seite vom Typ Datensatz und klicken Sie auf die Registerkarte Tabellenansicht .
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über den Namen der Registerkarte „Tabellenansicht“ und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Ansichtsnamen und dann auf **Exportieren**.

   ![Menü „Mehr“ in einer Ansicht](assets/view-more-menu-with-duplicate-option.png)

   * Klicken Sie **Freigeben** > **Aktuelle Ansicht exportieren**. Diese Option ist nur verfügbar, wenn die Tabellenansicht angezeigt wird.

   ![Freigabeschaltfläche mit Datensatztyp- und Ansichtsfreigabeoptionen](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Wählen Sie eines der folgenden Formate aus:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Sie können keine Informationen aus der Tabellenansicht exportieren, wenn Sie auf dem Bildschirm eine andere Ansicht anzeigen. Sie müssen die Tabellenansicht anzeigen, die Sie exportieren möchten, um auf die Option Exportieren im Menü Mehr zugreifen zu können.

   Die Datei wird auf Ihren Computer heruntergeladen.

1. (Optional) Gehen Sie zum Ordner Downloads auf Ihrem Computer und suchen Sie die heruntergeladene Datei.

   Der Name der exportierten Datei folgt dem folgenden Format:

   `Name of the view - name of the record type`

   Beispielsweise generiert eine Tabellenansicht für den Datensatztyp Kampagnen eine Datei mit dem Namen `Table view - Campaigns`.

   Die Datei enthält die folgenden Informationen:

   * Die Spaltenüberschriften werden in der Excel-Datei schwarz hervorgehoben
   * Alle in der Workfront-Benutzeroberfläche angezeigten Felder, nach denselben Kriterien sortiert und gefiltert
   * Gruppierungen bleiben in der Excel-Datei erhalten

   Sie können nun die exportierten Dateien für andere freigeben oder sie an eine beliebige Kommunikation anhängen.

</div>
