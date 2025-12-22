---
title: Felder löschen
description: In Adobe Workfront Planning können Sie benutzerdefinierte Felder löschen, die nicht mehr relevant sind.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---



# Felder löschen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning können Sie benutzerdefinierte Felder erstellen, um Informationen über Datensätze zu speichern.

Informationen zum Erstellen benutzerdefinierter Felder in Workfront Planning finden Sie unter [Erstellen von Feldern](/help/quicksilver/planning/fields/create-fields.md).

Sie können Workfront Planning-Felder löschen, die nicht mehr relevant sind.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
ODER
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>

<p><span class="preview">So löschen Sie Felder aus globalen Datensatztypen:</span></p>
<ul><li><p><span class="preview">Beliebiges Workfront-Paket und Planning Plus-Paket</span></p></li>
ODER
<li><p><span class="preview">Beliebige Workflow- und Planungspakete für Prime und Ultimate</span></p></li></ul>

<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Überlegungen zum Löschen von Workfront Planning-Feldern:

* Ein Feld kann nur in der Tabellenansicht vom Typ Datensatz gelöscht werden.
* Das primäre Feld eines Datensatzes kann nicht gelöscht werden.
* Alle im Feld gespeicherten Informationen werden gelöscht und können nicht wiederhergestellt werden.
* Wenn Sie ein verbundenes Datensatzfeld löschen, werden auch alle verbundenen Lookup-Felder aus dem Datensatztyp gelöscht, von dem aus Sie eine Verbindung herstellen. Die verbundenen Datensatzfelder der Datensatztypen, mit denen Sie eine Verbindung herstellen, werden auch aus dem Datensatz gelöscht, mit dem Sie eine Verbindung herstellen.

  Wenn Sie beispielsweise Kampagnen mit einem anderen Datensatztyp namens „Produkt“ verbinden und das Feld „Produktverbindung“ und das Suchfeld „Produktstatus“ aus der Kampagne löschen, werden die folgenden Elemente gelöscht:

   * Das Feld Mit Produkt verbunden der Kampagne
   * Das Suchfeld „Produktstatus“ in der Kampagne
   * Das Feld für die mit dem Produkt verbundene Kampagne

  Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* <span class="preview">Sie können keine Felder aus globalen Datensätzen löschen, die einem sekundären Arbeitsbereich aus den sekundären Arbeitsbereichen hinzugefügt wurden.</span>

## Felder löschen

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatzfelder Sie löschen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

1. (Bedingt) Klicken Sie, falls noch nicht ausgewählt, auf der Seite „Datensatztyp **auf die Registerkarte** Tabellenansicht“.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.

1. Suchen Sie das Feld, das Sie löschen möchten, in den Spaltenüberschriften, bewegen Sie den Mauszeiger über die Spaltenüberschrift und klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen.

   ![Pfeilmenü nach dem Feldnamen in der Tabellenkopfzeile hervorgehoben](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Klicken Sie **Löschen**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Klicken Sie **Löschen** zur Bestätigung.

   Gelöschte Felder können nicht wiederhergestellt werden.

   Je nachdem, welchen Typ von Feld Sie gelöscht haben, geschieht Folgendes:

   * Wenn Sie ein Feld löschen, das zu dem von Ihnen ausgewählten Datensatz gehört, wird das Feld gelöscht und kann mit keinem Datensatz mehr verknüpft werden. Wenn dieses Feld als Suchfeld in anderen Datensätzen hinzugefügt wird, werden diese Felder ebenfalls gelöscht.
   * Wenn Sie ein Verbindungsfeld löschen, wird das Feld aus dem ausgewählten Datensatz gelöscht. Außerdem wird das entsprechende Verbindungsfeld aus seinem ursprünglichen Datensatz ebenfalls gelöscht.
   * Wenn Sie ein Suchfeld löschen, das aus einem verbundenen Datensatz hinzugefügt wurde, wird das Feld aus dem ausgewählten Datensatztyp gelöscht, bleibt jedoch vom ursprünglichen Datensatztyp.
   * <span class="preview">Wenn Sie ein Feld aus einem globalen Datensatztyp in seinem primären Arbeitsbereich löschen, wird es aus allen Arbeitsbereichen gelöscht, in denen dieser Datensatztyp hinzugefügt wurde. Sie können keine Felder aus globalen Datensatztypen aus ihren sekundären Arbeitsbereichen löschen.</span>
