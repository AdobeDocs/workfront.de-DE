---
title: Felder bearbeiten
description: In Adobe Maestro können Sie die Feldeinstellungen für bereits erstellte Felder bearbeiten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 908a3136b2537310305f282b7a76d8f09cae3836
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Felder bearbeiten

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können die Feldeinstellungen für bereits erstellte Felder bearbeiten.

Informationen zum Erstellen von Adobe Maestro-Feldern finden Sie unter [Felder erstellen](../architecture-and-fields/create-fields.md).

Dieser Artikel beschreibt, wie Sie die Einstellungen für Maestro-Felder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Maestro-Datensätze finden Sie unter [Datensätze bearbeiten](../records/edit-records.md).

## Überlegungen zum Bearbeiten von Feldinformationen

* Sie können von Ihnen erstellte Felder oder von anderen Benutzern erstellte Felder bearbeiten. <!--this will change with access levels/ permissions-->
* Sie können ein Feld in der Tabelle vom Typ Datensatz bearbeiten.
* Nach dem Speichern des Felds können Sie den Feldtyp nicht mehr bearbeiten.
* Die Auswahl der zuvor ausgewählten Einstellung Negative Zahlen zulassen für ein Feld vom Typ Zahl, Prozentsatz oder Währung kann nicht aufgehoben werden, wenn bereits negative Werte in den Datensätzen gespeichert sind, an die das Feld angehängt ist.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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

## Felder bearbeiten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen löschen möchten.

   Der Arbeitsbereich wird geöffnet und die damit verbundenen Datensatztypen und Taxonomien werden angezeigt.
1. Klicken Sie auf die Karte für den Datensatztyp oder die Taxonomie, deren Felder Sie bearbeiten möchten.

   Dadurch wird die Seite des Datensatztyps geöffnet.
1. (Bedingt) Wählen Sie eine **Tabellenansicht** aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicks **Feld bearbeiten**, aktualisieren Sie dann die Informationen über das Feld und klicken Sie auf **Speichern**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Nach dem Speichern des Felds kann der Feldtyp nicht mehr aktualisiert werden.


1. (Bedingt) Klicken Sie für verknüpfte Datensatzfelder auf **Suchfelder bearbeiten** und fügen Sie eines der Felder aus dem verknüpften Datensatztyp hinzu oder entfernen Sie es.

   Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).
