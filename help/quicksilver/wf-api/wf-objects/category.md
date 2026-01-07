---
content-type: api
navigation-topic: workfront-objects
title: Kategorie
description: Eine Tabelle der für das Kategorieobjekt verfügbaren Felder mit ihren Beschreibungen und Werttypen.
author: Becky
feature: Workfront API
role: Developer
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 30%

---


# Kategorie

<!-- Audited: 5/2025 -->

<!--Fieldsclass: "java.lang.IllegalArgumentException",  
message: "APIModel INTERNAL does not support field projectid (OpTask)"-->

<table style="table-layout:auto"> 
 <col width="100"> 
 <col width="100"> 
 <col width="100"> 
 <col width="240"> 
 <col width="200"> 
 <col width="100"> 
 <thead> 
  <tr> 
   <th>Name</th> 
   <th>Label</th> 
   <th>Typ</th> 
   <th>Beschreibung</th> 
   <th>Mögliche Werte</th> 
   <th>Attribute</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}"><strong>ID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}">ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">Identifizierungs-GUID</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>accessorIDs</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">accessorIDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">Zeichenfolgen-Array</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">Liste der Personen-/Team-IDs, die auf dieses Objekt zugreifen können</td> 
   <td> </td> 
   <td> <p><span class="dtRead">Schreibgeschützt</span> </p> <p><span class="dtLazy">Lazy Read</span> </p> <p><span class="dtDyn">Dynamisch</span> </p> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">Typ</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">Typ des Objekts, mit dem das benutzerdefinierte Formular verknüpft ist</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">Bearbeitbar</span> </p> <p><span class="dtReq">Erforderlich</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">Kunden-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">ID des Kunden</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;description&quot;}"><strong>Beschreibung</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">Beschreibung</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">Beschreibung</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Bearbeitbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;enteredByID&quot;}"><strong>enteredByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Entered By ID&quot;}">Eingegeben von ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">ID des Benutzers, der das benutzerdefinierte Formular hinzugefügt hat</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">Externe Referenz-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">Bearbeitbares Feld des Benutzers, das als Link zu einem externen Objekt verwendet werden soll</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Bearbeitbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">Gruppen-ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">ID der ersten Gruppe mit Zugriff auf das benutzerdefinierte Formular</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Bearbeitbar</span> </p> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedFields</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">Verfügt über berechnete Felder</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">Boolesch</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">Sind dem Formular berechnete Felder zugeordnet?</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdateDate&quot;}"><strong>lastUpdateDate</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Update Date&quot;}">Datum der letzten Aktualisierung</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date/Time&quot;}">Datum/Zeit</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date of when the object was last modified&quot;}">Datum, an dem das Objekt zuletzt geändert wurde</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdatedByID&quot;}"><strong>lastUpdatedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Updated By ID&quot;}">Zuletzt aktualisiert von ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the last user to Update the object&quot;}">ID des letzten Benutzers, der das Objekt aktualisiert hat</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">Nicht gruppierbar</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;name&quot;}"><strong>name</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name&quot;}">Name</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name of the Object&quot;}">Name des Objekts</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">Bearbeitbar</span> </p> <p><span class="dtReq">Erforderlich</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Referenzen

| Name | Label | Typ | Objektcode eingeben |
|---|---|---|---|
| Kundin bzw. Kunde | Kundin bzw. Kunde | Kundin bzw. Kunde | KÜRZEN |
| Eingegeben von | enteredBy | Benutzerin oder Benutzer | BENUTZER |
| Gruppe | Gruppe | Gruppe | GRUPPE |
| Zuletzt aktualisiert von | lastUpdatedBy | Benutzerin oder Benutzer | BENUTZER |


## Sammlungen

| Name | Label | Typ | Objektcode eingeben |
|---|---|---|---|
| Zugriffsregeln | accessRules | Zugriffsregel | VERSIERT |
| Kategoriezugriffsregeln | categoryAccessRules | Kategoriezugriffsregeln | KATAKER |
| Kaskadierende Regeln für Kategorien | categoryCascadeRules | Kaskadierende Regeln für Kategorien | CTCSRL |
| Kategorieparameter | categoryParameters | Kategorieparameter | CTGYPA |
| Andere Gruppen | otherGroups | Gruppe | GRUPPE |


## Aktionen

| Label | Name | Argumente |
|---|---|---|
| Kategorien zuweisen | assignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| Kategorie zuweisen | assignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| Zuweisung von Kategorien aufheben | Zuweisung von Kategorien aufheben | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| Zuweisung der Kategorie aufheben | Zuweisung von Kategorie aufheben | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
