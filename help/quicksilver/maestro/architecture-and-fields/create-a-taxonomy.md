---
title: Erstellen von Taxonomiedatensatztypen
description: Taxonomien sind eine Art wiederverwendbarer Datensatztypen, die Attribute über einen operationellen Datensatztyp in Adobe Workfront Maestro erfassen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Taxonomiedatensatztypen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Taxonomien sind Datensatztypen, die Attribute über betriebliche Datensatztypen in Adobe Maestro erfassen.

Beispielsweise kann Campaign ein operativer Datensatztyp sein. Im Folgenden finden Sie Taxonomien, die Attribute zum Kampagnen-Datensatztyp erfassen: Region, Zielgruppe, Land.

Weitere Informationen zu Maestro-Datensatztypen finden Sie unter [Übersicht über Datensatztypen und Taxonomien](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## Überlegungen zum Erstellen von Taxonomien

* Sie müssen einen Arbeitsbereich erstellen, bevor Sie Taxonomien im Arbeitsbereich erstellen können.

  Weitere Informationen zu Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).
* Sie können einen Taxonomie-Datensatztyp erstellen, indem Sie einen der folgenden Schritte ausführen:
   * Erstellen Sie sie automatisch, wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).
   * Erstellen Sie sie manuell von Grund auf neu.
   * Erstellen Sie sie manuell, indem Sie Informationen aus einer externen Liste einfügen.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Alle neu erstellten Taxonomien enthalten die folgenden Felder:

   * Name <!--if there won't be any more fields, consider rephrasing this-->

  Darüber hinaus können Sie benutzerdefinierte Felder zu Taxonomien hinzufügen. Weitere Informationen finden Sie unter [Felder erstellen](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    Bei Verwendung einer Workspace-Vorlage erstellte Taxonomien verfügen über zusätzliche Felder.

## Erstellen einer Taxonomie

Das Erstellen von Taxonomien ähnelt dem Erstellen eines operationellen Datensatztyps von Grund auf oder aus einer Workspace-Vorlage.

Weitere Informationen finden Sie im Artikel unter &quot;Erstellen eines neuen Datensatztyps&quot; [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

Informationen zum automatischen Erstellen von Taxonomien beim Erstellen eines Arbeitsbereichs aus einer Vorlage finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).
