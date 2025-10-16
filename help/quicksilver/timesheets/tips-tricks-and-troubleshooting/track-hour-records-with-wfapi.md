---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Nachverfolgen von Stundeneinträgen mit der Adobe Workfront-API
description: Wenn Ihr Unternehmen zur Eingabe der Arbeitsstunden Adobe Workfront verwendet, aber ein anderes Tool als Aufzeichnungssystem für diese Daten verwendet, können Sie die Workfront-API verwenden, um Daten zwischen den beiden Systemen zu synchronisieren.
author: Lisa
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Nachverfolgen von Stundeneinträgen mit der Adobe Workfront-API

Wenn Ihr Unternehmen zur Eingabe der Arbeitsstunden Adobe Workfront verwendet, aber ein anderes Tool als Aufzeichnungssystem für diese Daten verwendet, können Sie die Workfront-API verwenden, um Daten zwischen den beiden Systemen zu synchronisieren.

Das einfache Nachverfolgen des Stundendatensatzes ist nicht möglich, da beim Entfernen des Stundeneintrags der gesamte Datensatz gelöscht wird, sodass Sie den gesamten Datensatz abrufen und mit dem alten Datensatz vergleichen müssen. Glücklicherweise werden alle Stundenbuchungen in Workfront-Journaleinträgen erfasst.

Nachdem Sie einen ersten Satz aller aktuellen Stunden im System abgerufen haben, können Sie alle Änderungen über die Journaleinträge verfolgen.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>„data“: [<br>{<br>„ID“: „5785406d008d93dd35665f14d90d4929“,<br>„objCode“: „JRNLE“,<br>„changeType“: „A“,<br>„aux2“: „Brad Littler“,<br>„newNumberVal“: 1,<br>„oldNumberVal“: null,<br>„subObjCode“: „STUNDE“,<br>„subObjID“: „5785406d008d93dce3f7f2e0e8eda4ea“<br>},<br>{<br>„ID“: „57854124008da2b9f372c01f8b9054bf“,<br>„objCode“: „JRNLE“,<br>„changeTypeD“:<br>„aux2“,Brad d dLittler“,newNumberVal:„null“<br>„oldNumberVal“: 1,<br>"<br>Code“: „STUNDE“,<br>„subObjID“: „5785406d003dce3f7e0e8eda„ea“,ID0„ID005db05ecode“: „JRNLE“,A00type„a05ecode„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a„a „STUNDE“,<br>„subObjID“: "<br>f005db05d9d2925c12b10f521„ID“},{id}d„db22fe974b„ea62b2„objCode:„JRNLE“,<br>Type: „E“,5785416„aux2“: „Brad Littler“,934663Number“ 2,968366„oldNumberVal“: 1,<br>„subjCode“: „STUNDE“,<br>„subObjID“: "<br>f008db9d2925c12b10f52f“<br>}<br> <br> <br> 5785416 <br> <br> <br> 57854176008 <br> <br> <br> <br> <br> <br> <br> 5785416 <br> <br> <br>}</pre>Im Folgenden finden Sie eine Beschreibung der eingeschlossenen Felder:

* **changeType:** Der Typ der Änderung, die am Objekt vorgenommen wird:

   * **a:** hinzufügen

   * **E:** Bearbeiten

   * **d:** Löschen

* **aux2:** Der Name des Benutzers, für den der Stundeneintrag bestimmt ist.

* **newNumberVal:** Neuer Wert des Stundeneintrags (dieser ist null, wenn changeType auf D gesetzt ist).

* **oldNumberVal** Vorheriger Wert des Stundeneintrags.

* **subObjCode:** Typ des zu ändernden Datensatzes (sollte immer STUNDE sein).

* **subObjID:** ID des Stundeneintrags.

Anhand dieser Informationen können Sie ermitteln, welche Stundeneinträge geändert, bearbeitet oder gelöscht wurden. Anschließend können Sie ggf. mit der subObjID weitere Informationen aus den Stundeneinträgen abrufen.
