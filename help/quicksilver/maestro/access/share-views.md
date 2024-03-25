---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Verwendung der Adobe Workfront-Planung sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# Ansichten freigeben

{{maestro-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit mit Datensätzen in der Adobe Workfront-Planung sicherzustellen.

Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben.

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
<p>Ihr Unternehmen muss in das Adobe Workfront-Planungsprogramm für die geschlossene Betaversion eingeschrieben sein. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td> Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/maestro/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Berechtigungen für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten mit Verwaltungsberechtigungen freigeben.

>[!NOTE]
>
>Systemadministratoren können keine Ansichten anzeigen oder freigeben, die sie selbst nicht erstellt haben. Sie können nur auf Ansichten zugreifen oder diese freigeben, die für sie freigegeben sind.
>
>Systemadministratoren können nur über Verwaltungsberechtigungen für eine Ansicht verfügen.

{{step1-to-maestro}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte Ansicht den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen der Ansicht klicken Sie auf **Freigeben**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Im **Gewähren des Ansichtszugriffs auf** ein, geben Sie den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann darauf, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. Klicks **Link kopieren** , um einen Link zur Ansicht in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite vom Typ Datensatz zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.
1. Klicken Sie auf **Speichern**.

## Berechtigungen für eine Ansicht entfernen

{{step1-to-maestro}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz. Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Bewegen Sie im Dropdownmenü Ansicht den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen der Ansicht klicken Sie auf **Freigeben**.
1. Suchen Sie den Benutzer oder die Gruppe, den/die Sie entfernen möchten, und klicken Sie dann auf **Entfernen** im Dropdown-Menü Berechtigungen rechts neben dem Namen des Benutzers oder der Gruppe.
1. Klicks **Speichern**.
Der Benutzer oder die Benutzer, die zur entfernten Gruppe gehören, haben keinen Zugriff mehr auf die Ansicht. Es gibt keine Benachrichtigung für die Benutzer, die vom Zugriff auf die Ansicht entfernt wurden.
