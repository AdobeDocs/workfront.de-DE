---
title: Datensätze bearbeiten
description: Sie können Datensatzinformationen in Adobe Maestro bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensätze bearbeiten

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines geschlossenen Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Datensatzinformationen in Adobe Maestro bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

&lt;!— Erwähnen Sie hier, dass die Felder in der Detailansicht mit denen in der Tabellenansicht identisch sind. Dieser Artikel ist über die Option Datensatzansichten verwalten verknüpft, um auf diese Informationen zu verweisen.—>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Beliebig</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Beliebig</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
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

## Überlegungen zum Bearbeiten von Datensätzen

* Sie können von Ihnen oder einem anderen Benutzer erstellte Datensätze bearbeiten. <!--will change with access levels-->
* Wenn die bearbeiteten Datensätze mit anderen Datensätzen verknüpft sind, spiegeln sich die neuen Informationen der bearbeiteten Datensätze in den verknüpften Datensätzen wider.
* Datensätze können nicht stapelweise bearbeitet werden. <!--this will probably change-->

## Datensätze bearbeiten

Sie können einen Datensatz aus den folgenden Bereichen bearbeiten:

* [Auf der Detailseite eines Datensatzes](#edit-a-record-from-the-records-details-page)
* [Aus der Tabellenansicht eines Datensatztyps](#edit-a-record-from-the-record-type-table-view)

### Datensatz auf der Detailseite des Datensatzes bearbeiten

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke oder **Hauptmenü** ![](assets/main-menu-shell.png) in der oberen linken Ecke, sofern verfügbar, klicken Sie auf Maestro.

   Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.
   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Ansicht**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicken Sie in einer Timeline-Ansicht auf eine Datensatzleiste.

   Der Datensatz **Details** Seite geöffnet.

1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Datensatznamen klicken Sie auf **Bearbeiten**

   Oder

   Klicken Sie auf der Detailseite in ein beliebiges bearbeitbares Feld, um die Informationen zu bearbeiten.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    Verknüpfte Felder oder Felder, die Berechnungen enthalten oder vom System generiert werden, können nicht bearbeitet werden.


1. Klicks **Änderungen speichern**. <!--logged a bug for this - this needs to be "Save"-->

### Datensatz in der Tabellenansicht des Datensatztyps bearbeiten

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Aus der **Ansicht** aus dem Dropdown-Menü oben rechts in der Tabelle eine Tabellenansicht auswählen. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Timeline-Ansicht angezeigt, als Sie zuletzt darauf zugegriffen haben.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie in die Zeile eines Datensatzes, um Informationen über den Datensatz inline zu bearbeiten, und drücken Sie dann die Eingabetaste **Eingabe** auf der Tastatur, um Ihre Änderungen zu speichern. Die Änderungen werden automatisch gespeichert.

   >[!TIP]
   >
   >Verknüpfte Felder können nicht bearbeitet werden. Die Informationen für diese Felder werden automatisch aus den verknüpften Datensätzen ausgefüllt. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).



