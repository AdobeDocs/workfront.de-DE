---
title: Datensätze löschen
description: Sie können von Ihnen oder einem anderen Benutzer erstellte Datensätze löschen. Gelöschte Datensätze können nicht wiederhergestellt werden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Datensätze löschen

{{maestro-important-intro}}

Sie können Datensätze löschen, die in den Planungsfunktionen von Adobe Workfront nicht mehr relevant sind.

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am geschlossenen Betaprogramm für Planungsfunktionen der Adobe Workfront teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p>
   </td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsmöglichkeiten für Adobe Workfront-Planungsfunktionen </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Beitragen oder höhere Berechtigungen zu einem Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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

{{step1-to-maestro}}

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

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.

1. Klicken Sie auf einen Datensatztyp.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Aus der **Ansicht** aus dem Dropdown-Menü oben links in der Tabelle eine Tabellenansicht auswählen. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Timeline-Ansicht angezeigt, als Sie zuletzt darauf zugegriffen haben.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Rechtsklicken Sie auf eine Datensatzzeile und klicken Sie dann auf **Löschen**.
   * Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Datensatznamen klicken Sie auf **Löschen**

   ![](assets/contextual-menu-for-record-row.png)
   <!--* Click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to open the Details box, and click **More** ![](assets/more-menu.png) to the right of the record name, then **Delete**. -->

   Der Datensatz wird gelöscht und kann nicht wiederhergestellt werden.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Löschen eines Datensatzes rückgängig zu machen oder wiederherzustellen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung
