---
title: Löschen von Arbeitsbereichen
description: Sie können Arbeitsbereiche löschen, die nicht mehr relevant sind.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Löschen von Arbeitsbereichen

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Sie können nicht mehr relevante Arbeitsbereiche löschen.

Es wird empfohlen, einige oder alle Datensatztypen, Datensätze, Felder und Ansichten, die mit dem Arbeitsbereich verknüpft sind, den Sie löschen möchten, neu zu erstellen, bevor Sie ihn löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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

*Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Überlegungen zum Löschen von Arbeitsbereichen

* Beim Löschen von Arbeitsbereichen werden auch alle Datensatztypen, Datensätze, Felder und Ansichten gelöscht.
* Gelöschte Arbeitsbereiche und die darin enthaltenen Informationen können nicht wiederhergestellt werden.

## Löschen eines Arbeitsbereichs

{{step1-to-planning}}

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf **Arbeitsbereiche, die ich verwende, um auf die erstellten Arbeitsbereiche zuzugreifen, oder auf** Andere Arbeitsbereiche **, um auf Arbeitsbereiche zuzugreifen, die für Sie freigegeben wurden.**

1. (Optional) Klicken Sie auf **Alle anzeigen** , um weitere Arbeitsbereiche anzuzeigen. Der Link **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Workspace-Karten haben.
1. (Optional) Klicken Sie auf K **Anzeigen weniger** , um die Anzahl der auf dem Bildschirm angezeigten Arbeitsbereiche zu begrenzen.
1. Um einen Arbeitsbereich zu löschen, führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Workspace-Karte und klicken Sie dann oben rechts auf der Karte auf das Menü **Mehr** ![](assets/more-menu.png) .
Oder
   * Klicken Sie auf eine Workspace-Karte, um den Arbeitsbereich zu öffnen, und klicken Sie dann auf das Menü **Mehr** rechts neben dem Arbeitsbereichnamen.![](assets/more-menu.png)
1. Klicken Sie auf **Löschen**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Geben Sie &quot;**delete**&quot;in den verfügbaren Bereich ein und klicken Sie dann auf **Permanentes Löschen**. Dabei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der Arbeitsbereich wird gelöscht und kann nicht wiederhergestellt werden. Alle Datensatztypen, Datensätze, Felder und Ansichten, die mit ihnen verknüpft sind, werden ebenfalls gelöscht. <!--ensure this is right at or before GA-->
