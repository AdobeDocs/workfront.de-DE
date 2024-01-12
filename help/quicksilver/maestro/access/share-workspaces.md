---
title: Freigeben von Arbeitsbereichen
description: Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Maestro sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 2%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Freigeben von Arbeitsbereichen

Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Maestro sicherzustellen.

>[!NOTE]
>
>Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben. Weitere Informationen finden Sie unter [Anzeigen freigeben](/help/quicksilver/maestro/access/share-views.md).


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
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich zu Ihrer Layoutvorlage hinzufügen. </p>  
</td>
  </tr>
 </tbody>
</table>

## Freigeben von Berechtigungen für einen Arbeitsbereich

Die folgenden Benutzer können einen Arbeitsbereich für andere Benutzer freigeben:

* Systemadministratoren können alle Arbeitsbereiche gemeinsam nutzen, auch jene, die sie nicht erstellt haben.
* Alle anderen Benutzer können nur Arbeitsbereiche freigeben, für die sie über Verwaltungsberechtigungen verfügen.

So geben Sie einen Arbeitsbereich für andere frei:

{{step1-to-maestro}}

1. Öffnen Sie den freizugebenden Arbeitsbereich und klicken Sie auf **Freigeben** in der oberen rechten Ecke des Bildschirms.

   ![](assets/share-button-on-workspace-top-right.png)

1. Im **Gewähren von Workspace-Zugriff auf** ein, geben Sie den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann darauf, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Mitwirken
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Freigabe von Berechtigungen in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Klicken Sie auf **Speichern**.


## Berechtigungen für einen Arbeitsbereich entfernen


{{step1-to-maestro}}

1. Öffnen Sie den Arbeitsbereich, für den Sie Berechtigungen entfernen möchten, und klicken Sie auf **Freigeben** in der oberen rechten Ecke des Bildschirms.
1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen eines Benutzers oder einer Gruppe und klicken Sie dann auf **Entfernen**.
1. Klicken Sie auf **Speichern**.

   Der Benutzer oder die Benutzer, die zur entfernten Gruppe gehören, haben keinen Zugriff mehr auf den Arbeitsbereich oder die zugehörigen Objekte.