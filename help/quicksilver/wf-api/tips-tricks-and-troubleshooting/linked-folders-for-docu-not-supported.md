---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Verknüpfte Ordner werden für das DOCU-Objekt nicht unterstützt
description: Verknüpfte Ordner werden für das DOCU-Objekt nicht unterstützt
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 9%

---

# Die Verwendung der API zum Hinzufügen eines verknüpften Ordners wird nicht unterstützt

Die Verwendung der -API zum Hinzufügen eines verknüpften Ordners zum Ordner-Array für ein Dokument-(DOCU-)Objekt wird nicht unterstützt. Die Anfrage wird erfolgreich sein, aber das Dokument kann von einigen externen Anbietern aus dem System entfernt werden. Dies liegt daran, dass das externe System als letzte Quelle der Wahrheit verwendet wird. Wenn das Dokument daher vom externen Anbieter entfernt wird, wird davon ausgegangen, dass das Dokument nicht mehr vorhanden ist. Alle Dokumente, die nicht im verknüpften (externen) Ordner gefunden wurden, können automatisch aus [!DNL Workfront] entfernt werden, ohne dass eine Möglichkeit besteht, sie wiederherzustellen.
