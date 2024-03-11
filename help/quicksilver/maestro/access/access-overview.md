---
title: Zugriffsübersicht
description: Für die Verwendung von Adobe Maestro-Funktionen gibt es Lizenzbeschränkungen und Freigabeberechtigungen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Zugriffsübersicht

{{maestro-important-intro}}

Für die Verwendung von Adobe Maestro-Funktionen gibt es Lizenzbeschränkungen und Freigabeberechtigungen.

## Zugriffsanforderungen

Sie müssen über die folgenden Einstellungen verfügen, um Adobe Maestro zu verwenden:

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
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. </p>
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
   <p>Alle</p>
   <p>Um Arbeitsbereiche zu erstellen, benötigen Sie die folgende Lizenz:</p>
   <ul>
   <li>
   Neu: Standard
   </li>
   <li>
   Aktuell: Worker oder höher
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Es gibt keine Steuerelemente für die Zugriffsstufe für Maestro-Objekte</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Sie können Arbeitsbereiche und Ansichten, die Sie nicht erstellt haben, um sie zu bearbeiten, zu löschen und freizugeben sowie Datensatztypen und -datensätze zu erstellen, zu bearbeiten oder zu löschen, mit oder über höhere Berechtigungen versehen.</p>
    <p>Systemadministratoren können nicht erstellte Arbeitsbereiche und Ansichten verwalten </p>
   <p>Informationen zum Freigeben von Berechtigungen für Maestro-Objekte finden Sie unter  
   <a href="../access/sharing-permissions-overview.md">Übersicht über die Freigabe von Berechtigungen in Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Maestro-Bereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/maestro/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Maestro-Bereich im Hauptmenü für andere freigeben

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Nachdem sich Ihr Unternehmen für das Betaprogramm Maestro angemeldet hat, können Sie den Bereich Maestro zum Hauptmenü aller Benutzer hinzufügen, indem Sie eine Layoutvorlage verwenden.

1. Anmelden bei **Workfront** als Workfront-Administrator.

1. Fügen Sie die **Maestro** icon ![](assets/maestro-icon.png) der **Hauptmenü** mithilfe einer **Layout-Vorlage**.

   Weitere Informationen finden Sie unter [Hauptmenü mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Weisen Sie die Layoutvorlage den Benutzern zu, die Zugriff auf Maestro erhalten sollen.

   Weitere Informationen finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alle Benutzer, die der Vorlage zugewiesen sind, können jetzt im Hauptmenü auf Maestro zugreifen.

   Benutzer können damit beginnen, Arbeitsbereiche, Datensatztypen, Datensätze und Felder zu erstellen.

## Zugriff erteilen

Es gibt keine Zugriffskontrollen für Maestro.

Benutzer mit einer beliebigen Lizenz können auf Maestro zugreifen.

Informationen zur Gewährung von Zugriff in Workfront finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Berechtigungen erteilen

Sie müssen Benutzern, die keine Systemadministratoren sind, Berechtigungen für Arbeitsbereiche und Ansichten erteilen, die Sie erstellen, damit sie darauf zugreifen können.

Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Maestro](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Maestro-Berechtigungen zusammen, um Ihnen Zugriff auf Maestro-Objekte zu gewähren, diese anzuzeigen, einzubringen oder zu verwalten.

Informationen dazu, wie Lizenztypen die Berechtigungsstufen für Maestro-Objekte beeinflussen, finden Sie unter [Übersicht über den Lizenztyp bei Verwendung der Planungsfunktionen von Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


