---
title: Löschen von Arbeitsbereichen
description: Sie können Arbeitsbereiche löschen, die nicht mehr relevant sind.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Löschen von Arbeitsbereichen

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Sie können nicht mehr relevante Arbeitsbereiche löschen.

Es wird empfohlen, einige oder alle Datensatztypen, Datensätze, Felder und Ansichten, die mit dem Arbeitsbereich verknüpft sind, den Sie löschen möchten, neu zu erstellen, bevor Sie ihn löschen.

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
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p>
   <p>Aktuell: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Überlegungen zum Löschen von Arbeitsbereichen

* Beim Löschen von Arbeitsbereichen werden auch alle Datensatztypen, Datensätze, Felder und Ansichten gelöscht.
* Gelöschte Arbeitsbereiche und die darin enthaltenen Informationen können nicht wiederhergestellt werden.

## Löschen eines Arbeitsbereichs

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, den Sie löschen möchten.

   Die Workspace-Seite wird angezeigt.

1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) neben dem Workspace-Namen klicken Sie dann auf **Löschen**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Typ &quot;**delete**&quot; in der vorgesehenen Platzierung und klicken Sie dann auf **Dauerhaftes Löschen**. Dabei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der Arbeitsbereich wird gelöscht und kann nicht wiederhergestellt werden. Alle Datensatztypen, Datensätze, Felder und Ansichten, die mit ihnen verknüpft sind, werden ebenfalls gelöscht. <!--ensure this is right at or before GA-->
