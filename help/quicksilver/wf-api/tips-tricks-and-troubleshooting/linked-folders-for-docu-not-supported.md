---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Verknüpfte Ordner werden für DOCU-Objekte nicht unterstützt
description: Verknüpfte Ordner werden für DOCU-Objekte nicht unterstützt
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Die Verwendung der API zum Hinzufügen verknüpfter Ordner wird nicht unterstützt

Die Verwendung der API zum Hinzufügen eines verknüpften Ordners zum Ordner-Array für ein Document (DOCU)-Objekt wird nicht unterstützt. Die Anfrage wird erfolgreich sein, aber das Dokument kann von einigen externen Anbietern aus dem System entfernt werden. Dies liegt daran, dass das externe System als letzte Quelle der Wahrheit verwendet wird. Wenn das Dokument daher aus dem externen Anbieter entfernt wird, wird davon ausgegangen, dass es nicht mehr vorhanden ist. Alle Dokumente, die nicht im verknüpften (externen) Ordner gefunden wurden, können automatisch aus [!DNL Workfront] entfernt werden, ohne dass eine Wiederherstellung möglich ist.
