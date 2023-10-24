---
title: Felder löschen
description: In Adobe Maestro können Sie benutzerdefinierte Felder löschen, die nicht mehr relevant sind.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 908a3136b2537310305f282b7a76d8f09cae3836
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Felder löschen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro können Sie benutzerdefinierte Felder erstellen, um Informationen zu Datensätzen zu speichern.

Informationen zum Erstellen von benutzerdefinierten Feldern in Maestro finden Sie unter [Felder erstellen](../architecture-and-fields/create-fields.md).

Sie können nicht mehr relevante Maestro-Felder löschen.

## Überlegungen zum Löschen von Maestro-Feldern:

* Sie können von Ihnen erstellte Felder oder von anderen Benutzern erstellte Felder löschen. <!--this will change with access levels/ permissions-->
* Sie können ein Feld nur in der Tabelle vom Typ Datensatz löschen.
* Alle im Feld gespeicherten Informationen werden gelöscht und können nicht abgerufen werden.
* Wenn Sie ein verknüpftes Datensatzfeld löschen, werden auch alle verknüpften Suchfelder aus dem Datensatztyp gelöscht, aus dem Sie eine Verknüpfung herstellen. Die verknüpften Datensatzfelder der Datensatztypen, mit denen Sie eine Verknüpfung herstellen, werden nicht gelöscht.

  Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture-and-fields/connect-record-types.md).
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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

## Felder löschen

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Dadurch wird der zuletzt aufgerufene Arbeitsbereich in Maestro geöffnet.
1. Klicken Sie auf die Karte eines Datensatztyps, dessen Felder Sie löschen möchten.
1. (Bedingt) Wählen Sie eine **Tabellenansicht** aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Suchen Sie das zu löschende Feld in den Spaltenüberschriften, bewegen Sie den Mauszeiger über die Spaltenüberschrift und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicks **Löschen**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klicks **Löschen** zur Bestätigung.

   Das Feld wird gelöscht, kann nicht wiederhergestellt werden und kann keinem Datensatz mehr zugeordnet werden.
