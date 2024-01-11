---
title: Felder löschen
description: In Adobe Maestro können Sie benutzerdefinierte Felder löschen, die nicht mehr relevant sind.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1ae60512c337d778939ef6c48fd2eda8b279dcce
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Felder löschen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro können Sie benutzerdefinierte Felder erstellen, um Informationen zu Datensätzen zu speichern.

Informationen zum Erstellen von benutzerdefinierten Feldern in Maestro finden Sie unter [Felder erstellen](../fields/create-fields.md).

Sie können nicht mehr relevante Maestro-Felder löschen.

## Überlegungen zum Löschen von Maestro-Feldern:

* Sie können ein Feld nur in der Tabellenansicht des Datensatztyps löschen.
* Das primäre Feld eines Datensatzes kann nicht gelöscht werden.
* Alle im Feld gespeicherten Informationen werden gelöscht und können nicht abgerufen werden.
* Wenn Sie ein verknüpftes Datensatzfeld löschen, werden auch alle verknüpften Suchfelder aus dem Datensatztyp gelöscht, aus dem Sie eine Verknüpfung herstellen. Die verknüpften Datensatzfelder der Datensatztypen, mit denen Sie eine Verknüpfung herstellen, werden nicht gelöscht.

  Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
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

{{step1-to-maestro}}

Dadurch wird der zuletzt aufgerufene Arbeitsbereich in Maestro geöffnet.
1. Klicken Sie auf die Karte eines Datensatztyps, dessen Felder Sie löschen möchten.
1. (Bedingt) Wählen Sie eine **Tabellenansicht** aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.
1. Suchen Sie das zu löschende Feld in den Spaltenüberschriften, bewegen Sie den Mauszeiger über die Spaltenüberschrift und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicks **Löschen**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klicks **Löschen** zur Bestätigung.

   Das Feld wird gelöscht, kann nicht wiederhergestellt werden und kann keinem Datensatz mehr zugeordnet werden.
