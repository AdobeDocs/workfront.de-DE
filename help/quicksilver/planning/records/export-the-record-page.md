---
title: Exportieren der Datensatzseite
description: Sie können die Vorschau- oder Detailseite des Datensatzes nach Word exportieren.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 1%

---

# Datensatzdetails exportieren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).</span>-->


Um effizienter mit anderen zusammenzuarbeiten, die möglicherweise kein Workfront-Konto haben, können Sie die Details eines Datensatzes in eine Datei exportieren und für diese freigeben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
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
   <td> <p>Standard</p>
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
   <td>   <p>Anzeigen oder höherer Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Exportieren von Datensatzdetails:

* Sie können die Details eines Datensatzes in die folgenden Dateiformate exportieren:

   * .docx Word
   * .pdf

* Sie können nur den Tab Details einer Datensatzseite oder eines Vorschaubereichs exportieren.

* Die exportierte Datei behält das Layout der Datensatzseite bei, einschließlich der Miniaturansicht und der Titelbilder.

## Datensatzdetails exportieren

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite mit dem Datensatztyp wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Das Vorschaufeld des Datensatzes wird geöffnet.

1. (Optional) Klicken Sie auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) , um die Seite des Datensatzes zu öffnen.

1. Wählen Sie die Registerkarte **Details** aus. Die Registerkarte Details sollte standardmäßig geöffnet werden.

1. Klicken Sie entweder in der Vorschau oder auf der Datensatzseite auf das Menü **Exportieren** und dann auf eine der folgenden Optionen:![](assets/export-icon-in-record-details-page.png)

   * **Microsoft Word**
   * **Adobe PDF**

   Eine Word-Datei (.docx) oder eine PDF-Datei wird heruntergeladen und auf Ihrem Computer gespeichert.

   Der Name der exportierten Datei ist das Primäre Feld des Datensatzes.

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Zusätzliche Informationen, die nicht auf der Seite angezeigt werden und nur sichtbar sind, nachdem Sie im Bereich mit den Datensatzdetails auf Mehr anzeigen geklickt haben, werden nicht in der exportierten PDF angezeigt. In der exportierten Datei werden nur die auf der Seite sichtbaren Informationen angezeigt.


1. (Optional) Gehen Sie zur heruntergeladenen Datei, öffnen Sie sie und bearbeiten Sie sie (falls es sich um eine Word-Datei handelt) oder geben Sie sie für andere frei.

