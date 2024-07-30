---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Verwendung der Adobe Workfront-Planung sicherzustellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# Ansichten freigeben

{{planning-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit mit Datensätzen in der Adobe Workfront-Planung sicherzustellen.

Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben.

Wenn Sie eine Ansicht freigeben, gewähren Sie anderen Berechtigungen für den Zugriff auf alle Elemente der Ansicht. Wenn Sie ihnen beispielsweise Berechtigungen zum Verwalten für eine Ansicht erteilen, können sie die Gruppierung, den Filter, die Sortierung oder das Erscheinungsbild der Leiste ändern.


Sie können eine Ansicht für die folgenden Entitäten freigeben:

* Workfront-Benutzer
* Workfront-Gruppen
<!--* Publicly, with users outside Workfront
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>  
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

+++

## Berechtigungen für eine Ansicht freigeben <!--internally-->

Sie können von Ihnen erstellte Ansichten oder Ansichten mit der Berechtigung &quot;Verwalten&quot;für <!--with users or groups in Workfront--> freigeben.

>[!NOTE]
>
>Systemadministratoren können keine Ansichten anzeigen oder freigeben, die sie selbst nicht erstellt haben. Sie können nur auf Ansichten zugreifen oder diese freigeben, die für sie freigegeben sind.
>
>Systemadministratoren können nur über Verwaltungsberechtigungen für eine Ansicht verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte &quot;Ansicht&quot;den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Ansichtsnamen und klicken Sie dann auf **Freigeben** .

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. (Optional) Wählen Sie aus den folgenden Optionen aus, um die Ansicht freizugeben:

   * **Nur eingeladene Personen können auf** zugreifen: Sie müssen Benutzer oder Gruppen angeben, für die Sie die Ansicht freigeben möchten. Dies ist die Standardoption.
   * **Alle Benutzer im Arbeitsbereich können anzeigen**: Alle Benutzer mit der Berechtigung &quot;Ansicht&quot;oder höher für Arbeitsbereiche können auf die Ansicht zugreifen.

1. Geben Sie im Feld **Gewähren des Ansichtszugriffs auf** den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann auf diesen, wenn er in der Liste angezeigt wird.  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Berechtigungen für die Freigabe in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratoren erhalten immer Berechtigungen zum Verwalten von Ansichten, die für sie freigegeben sind.

1. Klicken Sie auf **Link kopieren** , um einen Link in die Ansicht in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite vom Typ Datensatz zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.
1. Klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >   Für Sie freigegebene Ansichten haben neben dem Ansichtssymbol einen Personenindikator ![](assets/view-shared-with-others-people-icon.png). Ansichten ohne Personen-Indikator sind Ansichten, die Sie erstellt haben.

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-planning}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## Berechtigungen für eine Ansicht entfernen

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie die Freigabe stoppen möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz. Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Bewegen Sie den Mauszeiger über den Registerkartennamen der Ansicht, von der Sie die Freigabe entfernen möchten, und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Freigeben**.
1. Suchen Sie den Benutzer oder die Gruppe, den/die Sie entfernen möchten, und klicken Sie dann im Dropdown-Menü für Berechtigungen rechts neben dem Namen des Benutzers oder der Gruppe auf **Entfernen** .
1. Klicken Sie auf **Speichern**.
Der Benutzer oder die Benutzer, die zur entfernten Gruppe gehören, haben keinen Zugriff mehr auf die Ansicht. Es gibt keine Benachrichtigung für die Benutzer, die nicht mehr auf die Ansicht zugreifen konnten, dass sie diesen Zugriff verloren haben.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-planning}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->