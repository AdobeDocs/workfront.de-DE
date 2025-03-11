---
title: Exportieren der Datensatzseite
description: Sie können die Vorschau oder Detailseite des Datensatzes nach Word exportieren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Exportieren der Details eines Datensatzes

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


Um effizienter mit Personen zusammenzuarbeiten, die möglicherweise kein Workfront-Konto haben, können Sie die Details eines Datensatzes in eine Datei exportieren und für diese freigeben.

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
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Standard</p>
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
   <td>   <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Exportieren der Datensatzdetails:

* Sie können die Details eines Datensatzes in die folgenden Dateiformate exportieren:

   * .docx-Wort
   * .pdf

* Sie können nur die Registerkarte Details der Seite oder des Vorschaubereichs eines Datensatzes exportieren.

* Die exportierte Datei behält das Layout der Datensatzseite bei, einschließlich der Miniatur und der Titelbilder.

## Exportieren der Details eines Datensatzes

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet, und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite „Datensatztyp“ wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Das Vorschaufeld des Datensatzes wird geöffnet.

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![](assets/open-details-in-a-new-tab-icon.png), um die Seite des Datensatzes zu öffnen.

1. Wählen Sie die **Details** aus. Die Registerkarte Details sollte standardmäßig geöffnet sein.

1. Klicken Sie auf **Menü** Exportieren“ ![](assets/export-icon-in-record-details-page.png) entweder in der Vorschau oder auf der Seite des Datensatzes und dann auf eine der folgenden Aktionen:

   * **Microsoft Word**
   * **Adobe PDF**

   Ein Word-Dokument (.docx) oder eine PDF-Datei wird heruntergeladen und auf Ihrem Computer gespeichert.

   Der Name der exportierten Datei ist das Primäre Feld des Datensatzes.

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Zusätzliche Informationen, die nicht auf der Seite angezeigt werden und erst angezeigt werden, nachdem im Bereich Datensatzdetails auf Mehr anzeigen geklickt wurde, werden nicht in der exportierten PDF-Datei angezeigt. In der exportierten Datei werden nur die auf der Seite sichtbaren Informationen angezeigt.


1. (Optional) Wechseln Sie zur heruntergeladenen Datei, öffnen Sie sie und bearbeiten Sie sie (wenn es sich um eine Word-Datei handelt) oder geben Sie sie für andere frei.

