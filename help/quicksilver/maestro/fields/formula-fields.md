---
title: Übersicht über Formelfelder
description: In Adobe Maestro können Sie Formelfelder erstellen, die Funktionen und vorhandene Felder verwenden, um einen neuen benutzerdefinierten Wert zu berechnen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---


# Übersicht über Formelfelder

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO miniTOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können benutzerdefinierte Felder in Adobe Maestro erstellen, indem Sie auf bestehende Felder verweisen und sie durch eine Formel verbinden. Erstellen Sie dazu ein benutzerdefiniertes Feld vom Typ Formel .

Formelfelder generieren einen neuen Wert anhand vorhandener Werte aus anderen Feldern eines Datensatztyps und einer Funktion, die angibt, wie die vorhandenen Werte berechnet werden sollen.

Weitere Informationen finden Sie unter [Felder erstellen](../fields/create-fields.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
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
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## Überlegungen zu Formelfeldern

* Formularfelder verweisen auf Felder, die zum selben Datensatztyp gehören. Beim Erstellen eines Formelfelds können Sie keine Felder aus anderen Datensatztypen referenzieren. <!--is this still accurate??-->
* Sie können den Feldtyp eines Formelfelds nicht mehr ändern, nachdem Sie es gespeichert haben.
* Sie können die Berechnung eines Formelfelds nach dem Speichern aktualisieren und die Ergebnisse der Berechnung werden automatisch für alle Datensätze desselben Typs aktualisiert.
* Sie müssen die Felder, auf die Sie verweisen, in Formeln hinzufügen, wie sie in der Maestro-Benutzeroberfläche angezeigt werden.
* Die Verwendung von Suchfeldern aus verknüpften Datensatztypen in einer Formel ist zu einem späteren Zeitpunkt verfügbar.

## Unterstützte Formeln

Maestro-Formelfelder unterstützen alle Ausdrücke aus den berechneten Workfront-Feldern. Weitere Informationen finden Sie unter [Übersicht über berechnete Datenausdrücke](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Darüber hinaus unterstützen wir die folgenden Ausdrücke für Maestro-Formelfelder:


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ausdruck</th> 
   <th>Erläuterung und Beispiel</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Gibt verkettete Zeichenfolge als Trennzeichen zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Gibt ein Array mit eindeutigen Werten zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>ARRAYUNIQUE(Array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Gibt die Kennung eines Datensatzes zurück.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>{ID}</code>
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
   <td> <p>Gibt die Wochenzahl eines Jahres zurück. Optional können Sie angeben, an welchem Tag die Woche beginnt (1 für Sonntag oder 2 für Montag). Wenn diese Option deaktiviert ist, beginnen die Wochen standardmäßig am Sonntag.</p> <p>Der Ausdruck ist wie folgt formatiert:

<code>WEEKOFYEAR(Datum,2)</code>
oder
<code>WEEKOFYEAR(Datum)</code>
</p>
   </td></tr>

</table>





