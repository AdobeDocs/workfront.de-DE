---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Tracking von Stundenkatalogen mit der Adobe Workfront-API
description: Wenn Ihr Unternehmen Adobe Workfront verwendet, um Arbeitsstunden einzugeben, aber ein anderes Tool als Datensatzsystem für diese Daten verwendet, können Sie die Workfront-API verwenden, um Daten zwischen den beiden Systemen zu synchronisieren.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Tracking von Stundenkatalogen mit der Adobe Workfront-API

Wenn Ihr Unternehmen Adobe Workfront verwendet, um Arbeitsstunden einzugeben, aber ein anderes Tool als Datensatzsystem für diese Daten verwendet, können Sie die Workfront-API verwenden, um Daten zwischen den beiden Systemen zu synchronisieren.

Das einfache Tracking des Stundendatensatzes ist nicht möglich, da bei Entfernung des Stundeneintrags der gesamte Datensatz gelöscht wird. Dazu müssen Sie den gesamten Datensatz abrufen und ihn mit dem alten Datensatz vergleichen. Glücklicherweise werden alle Stundentransaktionen in Workfront Journal Entries aufgezeichnet.

Nachdem Sie einen ersten Satz aller aktuellen Stunden im System abgerufen haben, können Sie alle Änderungen über die Journaleinträge verfolgen.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "STUNDE",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "STUNDE",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "STUNDE",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "STUNDE",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Im Folgenden finden Sie eine Beschreibung der enthaltenen Felder:

* **changeType:** Die Art der Objektänderung:

   * **A:** Hinzufügen

   * **E:** Bearbeiten

   * **D:** Löschen

* **aux2:** Der Name des Benutzers, für den der Stundendatensatz gilt.

* **newNumberVal:** Neuer Wert des Stundendatensatzes (dieser Wert ist null, wenn changeType D ist).

* **oldNumberVal:** Vorheriger Wert des Stundendatensatzes.

* **subObjCode:** Typ des zu ändernden Datensatzes (Sollte immer HOUR sein).

* **subObjID:** Kennung des Stundendatensatzes.

Anhand dieser Informationen können Sie ermitteln, welche Stundendatensätze geändert, bearbeitet oder gelöscht wurden. Sie können dann die subObjID verwenden, um bei Bedarf weitere Informationen aus den Stundendatensätzen abzurufen.
