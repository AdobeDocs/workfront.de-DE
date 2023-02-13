---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Verknüpfte Ordner werden für DOCU-Objekte nicht unterstützt
description: Verknüpfte Ordner werden für DOCU-Objekte nicht unterstützt
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# Die Verwendung der API zum Hinzufügen eines verknüpften Ordners wird nicht unterstützt

Die Verwendung der API zum Hinzufügen eines verknüpften Ordners zum Ordner-Array für ein Document (DOCU)-Objekt wird nicht unterstützt. Die Anfrage wird erfolgreich sein, aber das Dokument kann von einigen externen Anbietern aus dem System entfernt werden. Dies liegt daran, dass das externe System als letzte Quelle der Wahrheit verwendet wird. Wenn das Dokument daher aus dem externen Anbieter entfernt wird, wird davon ausgegangen, dass es nicht mehr vorhanden ist. Alle Dokumente, die nicht im verknüpften (externen) Ordner gefunden werden, können automatisch aus [!DNL Workfront] keine Möglichkeit, sie wiederherzustellen.
