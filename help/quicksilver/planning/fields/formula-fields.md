---
title: Übersicht über Formelfelder
description: In Adobe Workfront Planning können Sie Formelfelder erstellen, die Funktionen und vorhandene Felder verwenden, um einen neuen benutzerdefinierten Wert zu berechnen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 4%

---

# Übersicht über Formelfelder

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können benutzerdefinierte Felder in Adobe Workfront Planning erstellen, indem Sie auf vorhandene Felder verweisen und sie in einem Feld vom Typ Formel verbinden.

Formelfelder generieren einen neuen Wert anhand vorhandener Werte aus anderen Feldern in einem Datensatztyp und einer Funktion, die angibt, wie die vorhandenen Werte berechnet werden sollen.

Weitere Informationen finden Sie im Abschnitt „Formel“ im Artikel [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

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
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
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
   <td><p> Standard</p>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## Überlegungen zu Formelfeldern

* Formelfelder verweisen auf Felder, die zum selben Datensatztyp gehören.
* Sie können nur dann auf Felder von anderen Datensatztypen verweisen, wenn Sie einen anderen Datensatztyp mit dem verbinden, für den Sie ein Formelfeld erstellen.
* Das Referenzieren von verbundenen Datensatztypen oder deren Lookup-Feldern in einer Formel hängt von Ihren Berechtigungen für die verbundenen Datensatztypen ab. Wenn Sie nicht berechtigt sind, den Datensatztyp anzuzeigen, können Sie dessen Felder nicht in einer Formel referenzieren.
* Der Feldtyp eines Formelfelds kann nach dem Speichern nicht mehr geändert werden.
* Sie können die Berechnung eines Formelfelds nach dem Speichern aktualisieren. Die Ergebnisse der Berechnung werden automatisch für alle Datensätze desselben Typs aktualisiert.
* Sie müssen die Felder, auf die Sie verweisen, in Formeln hinzufügen, die in der Workfront Planning-Benutzeroberfläche angezeigt werden.
* Sie können nur auf Felder verweisen, die in der Tabellenansicht eines Datensatztyps oder auf der Seite mit den Datensatzdetails angezeigt werden.
* Sie können das Format für den Wert einer Formelberechnung definieren, indem Sie aus den folgenden Formatoptionen auswählen:

   * Text
   * Zahl
   * Prozent
   * Währung
   * Tags
   * Datum

  Weitere Informationen finden Sie im Abschnitt „Formel“ im Artikel [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
* Sie können Formelfelder in neuen Formeln referenzieren. Sobald der Wert in einem Feld aktualisiert wird, auf das in einem Formelfeld verwiesen wird, werden alle nachfolgenden Felder, die auf dieses Feld oder Formelfelder verweisen, die dieses Feld enthalten, automatisch aktualisiert.

<div class="preview">

* Wenn Sie ein Formelfeld oder ein Feld aktualisieren, das Auswirkungen darauf haben könnte, werden Sie durch einen Warnhinweis über die Auswirkungen Ihrer Änderung informiert. Der Warnhinweis wird in den folgenden Fällen angezeigt:

   * Wenn Sie ein Formelfeld aktualisieren (mit Ausnahme von Namen- und Beschreibungsänderungen), wenn dieses Feld abhängige Formelfelder oder Suchfelder enthält. Der Warnhinweis listet diese abhängigen Felder auf und fragt Sie, ob Sie fortfahren möchten.

   * Wenn Sie ein Feld löschen, das in einem Formelausdruck oder als Suchfeld verwendet wird. Der Warnhinweis listet die abhängigen Formel- und Lookup-Felder auf und fragt Sie, ob Sie mit der Löschung fortfahren möchten.

</div>



<div class="preview">

## Einschränkungen bei Formelfeldern

* Sie können maximal 20 Formelfelder für einen Datensatztyp hinzufügen.

  Formelsuchfelder, die von verbundenen Datensatztypen hinzugefügt werden, werden nicht auf diese Beschränkung angerechnet.

* Der Formelausdruck darf 50.000 Zeichen nicht überschreiten.

* Formelfelder werden in den folgenden Fällen möglicherweise als `#ERROR!` angezeigt:
   * Wenn ein in einer Formel verwendetes Feld gelöscht wird.
   * Wenn ein in einem aggregierten Suchfeld verwendetes Feld als `#ERROR!` angezeigt wird.

     Beispiel: Sie zeigen ein Suchfeld an, das aggregierte Suchformularfelder enthält, und eines der referenzierten Formelfelder wird als `#ERROR!` angezeigt.
   * Wenn ein Formelwert nicht im ausgewählten Format angezeigt werden kann.

     Wenn ich beispielsweise Zahl für das Format eines Formelfelds auswähle und die in der Formel verwendeten Felder Textfelder sind, die nur nicht numerische Textwerte anzeigen, wird das Formelergebnis als `#ERROR!` angezeigt, da der Text nicht in eine Zahl zerlegt werden kann.

</div>

## Unterstützte Formeln

Adobe Workfront Planning-Formelfelder unterstützen die meisten Ausdrücke aus den berechneten Workfront-Feldern.

>[!NOTE]
>
>Die folgenden Workfront-Ausdrücke werden für Workfront Planning-Formelfelder nicht unterstützt:
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* FORMAT

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Eine vollständige Liste der Workfront-Ausdrücke finden Sie unter [Übersicht über berechnete Datenausdrücke](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Darüber hinaus unterstützen wir die folgenden Ausdrücke für Workfront Planning-Formelfelder. Die folgenden Ausdrücke werden für Workfront-Ausdrücke nicht unterstützt:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erklärung und Beispiel</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Gibt eine verkettete Zeichenfolge mit einem Trennzeichen zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Gibt ein Array mit eindeutigen Werten zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Gibt die ID eines Datensatzes zurück. Jeder Datensatz hat eine eindeutige ID.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Gibt die Daten aus JSON zurück, die durch den bereitgestellten JSONPath bestimmt werden. Wenn der JSONPath nicht in der JSON vorhanden ist, wird ein leeres Ergebnis zurückgegeben. </p> <p>Der Ausdruck ist wie folgt formatiert:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Legt die Zeitzone eines Datums und einer Uhrzeit auf eine bestimmte Zeitzone fest.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>SETTIMEZONE(date,&#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Gibt die Wochenzahl in einem Jahr zurück. Optional können Sie angeben, an welchem Tag die Woche beginnt (verwenden Sie 1 für Sonntag oder 2 für Montag). Wenn nicht angegeben, beginnen Wochen standardmäßig am Sonntag.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>WEEKOFYEAR(Datum,2)</code>
oder
<code>WEEKOFYEAR(Datum)</code>
</p>
   </td></tr>

</table>
