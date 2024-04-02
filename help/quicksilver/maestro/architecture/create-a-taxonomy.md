---
title: Erstellen von Taxonomiedatensatztypen
description: Wenn Sie eine Vorlage zum Erstellen eines Arbeitsbereichs verwenden, werden Datensatztypen in den Abschnitten "Operative Datensatztypen"und "Taxonomien"erstellt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Taxonomiedatensatztypen

{{maestro-important-intro}}

Wenn Sie eine Vorlage zum Erstellen eines Arbeitsbereichs verwenden, werden Datensatztypen in den folgenden Abschnitten erstellt:

* Operative Datensatztypen
* Taxonomien

Die Datensatztypen im Abschnitt &quot;Taxonomien&quot;eines Arbeitsbereichs erfassen Attribute zu Datensatztypen im Abschnitt &quot;Betriebliche Datensatztypen&quot;desselben Arbeitsbereichs.

Beispielsweise kann Campaign ein operativer Datensatztyp sein. Im Folgenden finden Sie Taxonomien, die Attribute zum Kampagnen-Datensatztyp erfassen: Region, Zielgruppe, Land.

Weitere Informationen zu Datensatztypen finden Sie unter [Übersicht über Datensatztypen](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Um Datensatztypen mit Experience Manager Assets zu verbinden, müssen Sie über eine Adobe Experience Manager Assets-Lizenz verfügen und die Workfront-Instanz Ihres Unternehmens muss mit der Adobe Business Platform oder der Adobe Admin Console integriert sein.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am geschlossenen Betaprogramm für die Adobe Workfront-Planung teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben
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

* Sie müssen einen Arbeitsbereich mithilfe einer Vorlage erstellen, bevor Sie Datensatztypen im Abschnitt Taxonomien des Arbeitsbereichs erstellen können.

  Weitere Informationen zu Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).
* Sie können einen Datensatztyp im Abschnitt &quot;Taxonomien&quot;eines Arbeitsbereichs erstellen, indem Sie einen der folgenden Schritte ausführen:
   * Erstellen Sie sie automatisch, wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).
   * Erstellen Sie sie manuell von Grund auf im Abschnitt &quot;Taxonomien&quot;eines Arbeitsbereichs.

* Alle neu erstellten Taxonomien verfügen standardmäßig über die folgenden Felder:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

  Darüber hinaus können Sie benutzerdefinierte Felder zu Taxonomien hinzufügen. Weitere Informationen finden Sie unter [Felder erstellen](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Bei Verwendung einer Workspace-Vorlage erstellte Taxonomie-Datensatztypen verfügen über zusätzliche Felder.

## Erstellen eines Taxonomiedatensatztyps

Das Erstellen von Taxonomiedatensätzen ähnelt dem Erstellen von Datensatztypen.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).
