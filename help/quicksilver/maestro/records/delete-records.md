---
title: Datensätze löschen
description: Sie können von Ihnen oder einem anderen Benutzer erstellte Datensätze löschen. Gelöschte Datensätze können nicht wiederhergestellt werden.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Datensätze löschen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Einträge löschen, die in Adobe Maestro nicht mehr relevant sind.

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

## Überlegungen zum Löschen von Datensätzen

* Sie können von Ihnen oder einem anderen Benutzer erstellte Datensätze löschen.
* Gelöschte Datensätze können nicht wiederhergestellt werden. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber auch die Informationen aus dem gelöschten Datensatz werden gelöscht.
* Es ist nicht möglich, Datensätze stapelweise zu löschen. <!--this will probably change-->
* Datensätze können nicht aus der Timeline-Ansicht gelöscht werden.

## Datensätze löschen

Sie können einen Datensatz aus den folgenden Bereichen löschen:

* [Auf der Detailseite eines Datensatzes](#delete-a-record-from-the-records-details-page)
* [Aus der Tabellenansicht eines Datensatztyps](#delete-a-record-from-the-record-type-table-view)

### Datensatz von der Detailseite des Datensatzes löschen

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke oder **Hauptmenü** ![](assets/main-menu-shell.png) in der oberen linken Ecke, sofern verfügbar, klicken Sie auf Maestro.

   Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.
1. Klicken Sie auf einen Datensatztyp.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.
   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Ansicht**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicken Sie in einer Timeline-Ansicht auf eine Datensatzleiste.

   Der Datensatz **Details** Seite geöffnet.

1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Datensatznamen klicken Sie auf **Löschen**, dann **Löschen** erneut zu bestätigen.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Der Datensatz wird gelöscht und kann nicht wiederhergestellt werden.

### Datensatz aus der Tabellenansicht des Datensatztyps löschen

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke oder **Hauptmenü** ![](assets/main-menu-shell.png) in der oberen linken Ecke, sofern verfügbar, klicken Sie auf **Maestro**.

   Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.
1. Klicken Sie auf einen Datensatztyp.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Aus der **Ansicht** aus dem Dropdown-Menü oben rechts in der Tabelle eine Tabellenansicht auswählen. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Timeline-Ansicht angezeigt, als Sie zuletzt darauf zugegriffen haben.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Rechtsklicken Sie auf eine Datensatzzeile und klicken Sie dann auf **Löschen**.

   ![](assets/contextual-menu-for-record-row.png)

   Der Datensatz wird gelöscht und kann nicht wiederhergestellt werden.
