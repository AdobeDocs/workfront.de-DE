---
title: Exportieren von Datensätzen aus der Tabellenansicht
description: Sie können Datensätze und ihre Informationen aus der Tabellenansicht in eine CSV- oder Excel-Datei exportieren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 2%

---

# Datensätze aus der Tabellenansicht exportieren

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning können Sie Datensätze und deren Informationen aus der Tabellenansicht in eine Excel- oder CSV-Datei exportieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
   <td><p> Licht oder höher </p>
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
   <td>   <p>Anzeigen von oder höheren Berechtigungen für eine Ansicht</p>  
   </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
