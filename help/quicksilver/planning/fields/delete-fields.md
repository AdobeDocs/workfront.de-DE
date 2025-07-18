---
title: Felder löschen
description: In Adobe Workfront Planning können Sie benutzerdefinierte Felder löschen, die nicht mehr relevant sind.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---



# Felder löschen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning können Sie benutzerdefinierte Felder erstellen, um Informationen über Datensätze zu speichern.

Informationen zum Erstellen benutzerdefinierter Felder in Workfront Planning finden Sie unter [Erstellen von Feldern](/help/quicksilver/planning/fields/create-fields.md).

Sie können Workfront Planning-Felder löschen, die nicht mehr relevant sind.

## Überlegungen zum Löschen von Workfront Planning-Feldern:

* Ein Feld kann nur in der Tabellenansicht vom Typ Datensatz gelöscht werden.
* Das primäre Feld eines Datensatzes kann nicht gelöscht werden.
* Alle im Feld gespeicherten Informationen werden gelöscht und können nicht wiederhergestellt werden.
* Wenn Sie ein verbundenes Datensatzfeld löschen, werden auch alle verbundenen Lookup-Felder aus dem Datensatztyp gelöscht, von dem aus Sie eine Verbindung herstellen. Die verbundenen Datensatzfelder der Datensatztypen, mit denen Sie eine Verbindung herstellen, werden auch aus dem Datensatz gelöscht, mit dem Sie eine Verbindung herstellen.

  Wenn Sie beispielsweise Kampagnen mit einem anderen Datensatztyp namens „Produkt“ verbinden und das Feld „Produktverbindung“ und das Suchfeld „Produktstatus“ aus der Kampagne löschen, werden die folgenden Elemente gelöscht:

   * Das Feld Mit Produkt verbunden der Kampagne
   * Das Suchfeld „Produktstatus“ in der Kampagne
   * Das Feld der mit dem Produkt verbundenen Kampagne.

  Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p></td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   Das Feld wird gelöscht, kann nicht wiederhergestellt werden und kann mit keinen Datensätzen mehr verknüpft werden.
