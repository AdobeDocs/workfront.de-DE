---
content-type: api
navigation-topic: general-api
title: Versionierung von Ereignisabonnements
description: Ereignisabonnement-API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 0%

---

# Versionierung von Ereignisabonnements

Workfront verfügt über zwei Versionen von Ereignisabonnements. Dieser Artikel beschreibt die Unterschiede zwischen ihnen.

Die neue Version ist keine Änderung der Workfront-API, sondern eine Änderung der Ereignisabonnementfunktion.

Die Möglichkeit, Ereignisabonnements zu aktualisieren oder herabzustufen, stellt sicher, dass vorhandene Abonnements nicht beschädigt werden, wenn Änderungen an der Ereignisstruktur vorgenommen werden, sodass Sie ohne Lücke in Ihrem Ereignisabonnement testen und auf die neue Version aktualisieren können.


Wenn Sie Ihr Ereignisabonnement auf eine andere Version aktualisieren oder herunterstufen, erhalten Sie nach der Versionsänderung für jeden Ereignisversand für ein Zeitfenster von fünf Minuten doppelte Ereignisse. Die Duplikate enthalten je eines der Ereignisabonnements, Version 1 und Version 2. Dadurch wird sichergestellt, dass Sie keine Ereignisse aufgrund einer Änderung der Ereignisabonnementversion verpassen.

Informationen zu den Endpunkten, die zum Aktualisieren oder Herunterstufen von Ereignisabonnements verwendet werden, finden Sie [Ereignisabonnement-Versionierung](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) im Artikel Ereignisabonnement-API.

>[!IMPORTANT]
>
>Die folgenden Versionen wirken sich auf die Versionierung von Ereignisabonnements aus:
>
>* **25.2 Version** (10. April 2025): Alle neuen Abonnements, die nach der Version 25.2 erstellt wurden, werden als Version 2 erstellt.
>* **25.3 Version** (17. Juli 2025): Abonnements können nach der Version 25.3 nicht mehr auf Version 1 heruntergestuft werden.
>* **15. Januar 2026**: Alle verbleibenden Version 1-Abonnements werden auf Version 2 migriert.

## Änderungen zwischen Version 1 und Version 2

Die folgenden Änderungen wurden für Ereignisabonnements Version 2 vorgenommen:


### Allgemeine Änderungen


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Betroffene Felder</b></p> </th> 
   <th> <p><b>Version 1 (vorheriges Verhalten)</b></p> </th> 
   <th> <p><b>Version 2 (Änderung)</b></p> </th> 
   <th> <p><b>Korrekturmaßnahme</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Berechnete Parameterwerte</p> </td> 
   <td> <p>Jedes Objekt, das aus einer Vorlage erstellt wurde, die ein benutzerdefiniertes Formular mit berechneten Parameterwerten enthielt, wird ein <code>CREATE</code>-Ereignis gesendet und anschließend wird ein <code>UPDATE</code> mit den Parameterwerten (einschließlich berechneter Felder und ihrer Werte) gesendet. </p> </td> 
   <td> <p>Wenn ein Objekt aus einer Vorlage erstellt wird, die ein benutzerdefiniertes Formular mit berechneten Parameterwerten enthält, wird nur ein <code>CREATE</code> gesendet, das Parameterwerte einschließlich berechneter Felder enthält.</p> </td> 
   <td> <p>Wenn Sie über ein Abonnement für <code>UPDATE</code> Ereignisse verfügen und ein <code>UPDATE</code> Ereignis erwarten, nachdem ein Objekt mit berechneten Parameterwerten erstellt wurde, erhalten Sie dieses <code>UPDATE</code> Ereignis nicht mehr. Wenn Sie berechnete Parameterwerte bei der Objekterstellung anzeigen möchten, müssen Sie ein zusätzliches <code>CREATE</code> erstellen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Felder vom Typ „Mehrfachauswahl“</p> </td> 
   <td> <p>Für jeden Ereignistyp, der eine Änderung an einem Feld vom Typ Mehrfachauswahl enthält, würde das Feld, wenn es nur einen Wert enthält, in konvertiert und als Zeichenfolge gesendet. Andernfalls wird es als Array gesendet. </p><p>Beispiele:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> wird konvertiert und als <code>myMultiSelectField: "oneValue"</code> gesendet.</li><li><code>myMultiSelectField: ["first", "second"]</code> wird als <code>myMultiSelectField: ["first", "second"]</code> gesendet.</li></ul> </td> 
   <td> <p>Unabhängig davon, wie viele Werte sich im Array befinden, wird es als Array gesendet. </p><p>Beispiele:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> wird als <code>myMultiSelectField: ["oneValue"]</code> gesendet.</li><li><code>myMultiSelectField: ["first", "second"]</code> wird als <code>myMultiSelectField: ["first", "second"]</code> gesendet.</li></ul> </td> 
   <td> <p>Wenn Sie über ein Abonnement mit einem Filter für ein Mehrfachauswahlfeld verfügen und den Wert als Zeichenfolge haben, müssen Sie ein neues Abonnement mit demselben Filter erstellen, der den Wert als Array hat. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Objektspezifische Änderungen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Objektcode</b> </th> 
   <th> <b>Betroffene Felder</b> </th> 
   <th> <b>Version 1 (vorheriges Verhalten)</b></th> 
   <th> <b>Version 2 (Änderung)</b> </th> 
   <th> <b>Behebungsaktion</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ZUWEISEN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code>-Ereignis manchmal fälschlicherweise die betroffenen Felder an, die sich von <code>null</code> zu <code>ID value</code> ändern.</td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für die betroffenen Felder an.</td> 
   <td>Keine. Wenn Sie über einen Filter für die betroffenen Felder verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich diese Felder tatsächlich geändert haben, nicht jedoch, wenn sich ein anderer Wert geändert hat.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOKU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Wenn ein Parameterwert für dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code> fälschlicherweise die betroffene Feldänderung von <code>null</code> zu <code>object id</code> an. </td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für die betroffenen Felder an.</td> 
   <td>Keine. Wenn Sie über einen Filter für die betroffenen Felder verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich diese Felder tatsächlich geändert haben, nicht jedoch, wenn sich ein anderer Wert geändert hat.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Beim Löschen eines Dokuments zeigte das <code>DELETE</code>-Ereignis das betroffene Feld im Status Vor fälschlicherweise als leeres Array an.    </td> 
   <td>Das <code>DELETE</code>-Ereignis zeigt das betroffene Feld im Status Vor korrekt an.</td> 
   <td>Keine. Das <code>DELETE</code> wird weiterhin gesendet, zeigt aber jetzt die korrekten Daten für das betroffene Feld an. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt aktualisiert wird, werden zwei <code>UPDATE</code>-Ereignisse gesendet. Die erste umfasste nicht die betroffenen Felder, während das zweite Ereignis dies tat.</td> 
   <td>Alle Feldaktualisierungen einschließlich der betroffenen Felder sind nur in einem <code>UPDATE</code> Ereignis vorhanden, und ein zweites unnötiges Ereignis wird nicht gesendet.     </td> 
   <td>Keine. Wenn Sie über einen Filter für die betroffenen Felder verfügen, werden die Ereignisse im ersten Ereignis gesendet. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">AUSGABEN</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Wenn ein Parameterwert für eine Ausgabe aktualisiert wurde, zeigte das <code>UPDATE</code>-Ereignis fälschlicherweise die TopReferenceObjCode-Änderung von <code>EXPNS</code> zu <code>PROJ</code> und <code>referenceObjectName</code> Änderung von <code>null</code> zu <code>string value of project name</code> an.      </td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für die betroffenen Felder an.</td> 
   <td>Keine. Wenn Sie über einen Filter für die betroffenen Felder verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich diese Felder tatsächlich geändert haben, nicht jedoch, wenn sich ein anderer Wert geändert hat.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Beim Löschen eines Ausgabenobjekts wurde ein <code>UPDATE</code> gesendet, durch das die betroffenen Felder in null geändert wurden, bevor das <code>DELETE</code> gesendet wurde.    </td> 
   <td>Das zusätzliche <code>UPDATE</code> wird nicht gesendet. Das <code>DELETE</code>-Ereignis hat korrekte Werte für die betroffenen Felder im Status Vor . </td> 
   <td>Wenn Sie über einen Filter für die betroffenen Felder für <code>UPDATE</code> Ereignisse verfügen und erwarten, ihn zu erhalten, wenn das Objekt gelöscht wird, erhalten Sie dieses <code>UPDATE</code> Ereignis nicht mehr. Wenn diese Felder beim Löschen des Objekts angezeigt werden sollen, müssen Sie ein zusätzliches <code>DELETE</code>-Abonnement erstellen.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt gelöscht wurde, wurden die betroffenen Felder im <code>DELETE</code>-Ereignis fälschlicherweise wie im Status Vor <code>null</code> angezeigt. </td> 
   <td>Das <code>DELETE</code>-Ereignis zeigt die betroffenen Felder im Status Vor korrekt an.</td> 
   <td>Keine. Das <code>DELETE</code> wird weiterhin gesendet, zeigt aber jetzt die korrekten Daten für die betroffenen Felder an. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Wenn ein Parameterwert für dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code> fälschlicherweise die betroffene Feldänderung von <code>null</code> zu <code>ID value</code> an. </td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für das betroffene Feld an.</td> 
   <td>Keine. Wenn Sie über einen Filter für das betroffene Feld verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich dieses Feld tatsächlich geändert hat, nicht jedoch, wenn sich ein anderer Parameterwert geändert hat.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code>-Ereignis manchmal fälschlicherweise die betroffenen Felder an, die sich von <code>null</code> zu <code>ID value</code> ändern.</td> 
   <td>Bei allen <code>UPDATE</code> Ereignissen wird der richtige Wert für die betroffenen Felder angezeigt.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Wenn ein Parameterwert für dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code> fälschlicherweise die betroffene Feldänderung von <code>null</code> zu <code>ID value</code> an. </td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für das betroffene Feld an.</td> 
   <td>Keine. Wenn Sie über einen Filter für das betroffene Feld verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich dieses Feld tatsächlich geändert hat, nicht jedoch, wenn sich ein anderer Parameterwert geändert hat.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code>-Ereignis manchmal fälschlicherweise die betroffenen Felder an, die sich von <code>null</code> zu <code>ID value</code> ändern.</td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für das betroffene Feld an.</td> 
   <td>Keine. Wenn Sie über einen Filter für das betroffene Feld verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich dieses Feld tatsächlich geändert hat, nicht jedoch, wenn sich ein anderer Parameterwert geändert hat.
  </tr> 
  <tr> 
   <th rowspan="2">AUFGABE</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Wenn ein Parameterwert für dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code> fälschlicherweise die betroffene Feldänderung von <code>null</code> zu <code>ID value</code> an. </td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für das betroffene Feld an.</td> 
   <td>Keine. Wenn Sie über einen Filter für das betroffene Feld verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich dieses Feld tatsächlich geändert hat, nicht jedoch, wenn sich ein anderer Parameterwert geändert hat.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Wenn dieses Objekt aktualisiert wurde, zeigte das <code>UPDATE</code>-Ereignis manchmal fälschlicherweise die betroffenen Felder an, die sich von <code>null</code> zu <code>ID value</code> ändern.</td> 
   <td>Alle <code>UPDATE</code> Ereignisse zeigen den richtigen Wert für das betroffene Feld an.</td> 
   <td>Keine. Wenn Sie über einen Filter für das betroffene Feld verfügen, erhalten Sie nur dann ein <code>UPDATE</code>, wenn sich dieses Feld tatsächlich geändert hat, nicht jedoch, wenn sich ein anderer Parameterwert geändert hat.
 </tbody> 
</table>


## Aktualisieren der Ereignisabonnementversion in einem Workfront Fusion-Szenario

Workfront Fusion verwendet Ereignisabonnements, um auf Änderungen in Szenarien mit Workfront-Triggern zu achten. Sie können die Ereignisabonnementversion, die Fusion direkt in einem Szenario verwendet, mithilfe des Payload-Versionsmoduls Workfront > Ereignisse aktualisieren aktualisieren .

Anweisungen zur Verwendung dieses Moduls finden Sie unter [Workfront-Module](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) in der Dokumentation zu Workfront Fusion.
