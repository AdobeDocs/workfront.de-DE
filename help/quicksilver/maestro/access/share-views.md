---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Maestro sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 72d044541f8e061c51c4483672a89ce20e4f30d9
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---


<!--*****************ADD TO TOC AND MINITOC WHEN RELEASING*********************-->

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Ansichten freigeben

{{maestro-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Maestro sicherzustellen.

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
   <td> Es gibt keine Zugriffskontrollen für Adobe Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich zu Ihrer Layoutvorlage hinzufügen. </p>  
</td>
  </tr>
 </tbody>
</table>

## Berechtigungen für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten mit Verwaltungsberechtigungen freigeben.

>[!NOTE]
>
>Systemadministratoren können keine Ansichten anzeigen oder freigeben, die sie selbst nicht erstellt haben. Sie können nur Ansichten anzeigen oder freigeben, die für sie freigegeben sind.


So geben Sie eine Ansicht für andere frei:

{{step1-to-maestro}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf die Karte Datensatztyp .

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie im Dropdownmenü Ansicht den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen der Ansicht klicken Sie auf **Freigeben**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Im **Gewähren des Ansichtszugriffs auf** ein, geben Sie den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann darauf, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Freigabe von Berechtigungen in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Klicks **Link kopieren** , um einen Link zur Ansicht in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite vom Typ Datensatz zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.
1. Klicken Sie auf **Speichern**.


## Berechtigungen für eine Ansicht entfernen


{{step1-to-maestro}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf die Karte Datensatztyp .

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie im Dropdownmenü Ansicht den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen der Ansicht klicken Sie auf **Freigeben**.

1. Suchen Sie den Benutzer oder die Gruppe, den/die Sie entfernen möchten, und klicken Sie auf **Entfernen** im Dropdown-Menü Berechtigungen rechts neben dem Namen des Benutzers oder der Gruppe.

1. Klicken Sie auf **Speichern**.

   Der Benutzer oder die Benutzer, die zur entfernten Gruppe gehören, haben keinen Zugriff mehr auf die Ansicht.