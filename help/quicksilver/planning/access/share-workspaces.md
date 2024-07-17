---
title: Freigeben von Arbeitsbereichen
description: Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit an der Adobe Workfront-Planung sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 2%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Planning as a product ??-->

# Freigeben von Arbeitsbereichen

{{planning-important-intro}}

Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit an der Adobe Workfront-Planung sicherzustellen.

>[!NOTE]
>
>Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben. Weitere Informationen finden Sie unter [Anzeigen freigeben](/help/quicksilver/planning/access/share-views.md).


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
   Oder
   <p>Aktuell: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Freigeben von Berechtigungen für einen Arbeitsbereich

Die folgenden Benutzer können einen Arbeitsbereich für andere Benutzer freigeben:

* Systemadministratoren können alle Arbeitsbereiche gemeinsam nutzen, auch jene, die sie nicht erstellt haben.
* Alle anderen Benutzer können nur Arbeitsbereiche freigeben, für die sie über Verwaltungsberechtigungen verfügen.

So geben Sie einen Arbeitsbereich für andere frei:

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, den Sie freigeben möchten, und klicken Sie dann oben rechts im Bildschirm auf **Freigeben** .

   ![](assets/share-button-on-workspace-top-right.png)

1. Geben Sie im Feld **Workspace Zugriff auf** gewähren den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann auf diesen, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Mitwirken
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Berechtigungen für die Freigabe in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klicken Sie auf **Link kopieren** , um einen Link in den Arbeitsbereich in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich zugreifen zu können.
1. Klicken Sie auf **Speichern**.


## Berechtigungen für einen Arbeitsbereich entfernen


{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, für den Sie Berechtigungen entfernen möchten, und klicken Sie dann oben rechts im Bildschirm auf **Freigeben** .
1. Klicken Sie auf das Dropdown-Menü rechts neben einem Benutzer- oder Gruppennamen und dann auf **Entfernen**.
1. Klicken Sie auf **Speichern**.

   Der Benutzer oder die Benutzer, die zur entfernten Gruppe gehören, haben keinen Zugriff mehr auf den Arbeitsbereich oder die zugehörigen Objekte.