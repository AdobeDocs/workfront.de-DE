---
filename: api-changes-search
content-type: api
keywords: Objekt,Status,Suche,Best,Practice,Antwort
navigation-topic: api-navigation-topic
title: 'Änderungen an der Kern-API: Antworten auf die Statussuche'
description: Änderungen bei der Speicherung von Statusobjekten in Workfront.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Änderungen an der Kern-API: Antworten auf die Statussuche

Die Art und Weise, wie Workfront Statusobjekte speichert, wurde geändert. Diese Änderungen wirken sich nicht auf die Art und Weise aus, wie Statussuchanfragen gestellt werden. Sie wirken sich jedoch auf die Antwort von API-Anfragen aus, die eine Suche nach Statusobjekten durch Rückgabe einer unvollständigen Liste von Gruppenstatus enthalten.

## Best Practices

Um zuverlässig die vollständige Liste der für eine Gruppe verfügbaren Status abzurufen, werden die folgenden Anfragen als Best Practices betrachtet.

>[!NOTE]
>
>Diese Anfragestrukturen werden für alle Benutzer empfohlen, unabhängig davon, ob die Änderungen an der Statussuche für Ihren Cluster vorgenommen wurden oder nicht.

Für den Projektgruppenstatus:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Für den Aufgabengruppenstatus:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Für den Problemgruppenstatus:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Alle drei Endpunkte akzeptieren den Parameter **includeHidden=true**, um die ausgeblendeten Projekt-, Aufgaben- oder Problemstatus einer bestimmten Gruppe abzurufen. Durch die Modellierung Ihrer Statussuchabfragen nach diesen Best Practice-Beispielen wird sichergestellt, dass alle Gruppenstatusinformationen in jeder Antwort enthalten sind.

Im Folgenden finden Sie ein Beispiel für eine Statussuchabfrage an eine Aufgabengruppe, die einen gesperrten Status (**_1)** einen entsperrten Status (**_2)**:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Durch die Verwendung dieses Formats wird sichergestellt, dass Ihre Antwort Folgendes enthält:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Verstehen der Änderungen an der Legacy-Statussuchabfrage

Unter dem alten System würde eine Statussuchabfrage alle Systemstatus kopieren, die für alle in einer Abfrage enthaltenen Gruppen verfügbar sind. Die Legacy-Antwort würde dann alle Systemstatus und Gruppenstatus enthalten, die für jede Gruppe in der Abfrage verfügbar sind.

Beispielsweise diese Abfrage (die nicht den aktuellen empfohlenen Best Practices entspricht):

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

würde die folgende Antwort unter dem alten System haben, das alle Objektstatus enthält:

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Nach den Aktualisierungen der Art und Weise, wie Status gespeichert und verwendet werden, werden sie jedoch nicht für Gruppen kopiert, sondern von jeder Gruppe auf Systemebene übernommen. Daher liest die Abfrage der Such-API nur die Status, die direkt mit einer bestimmten Gruppe verknüpft sind, sodass die Antwort nur den Status Systemgesperrt und entsperrt enthält, aber nur für die Gruppen, die erstellt wurden, nachdem der betreffende Status hinzugefügt wurde.

Wenn Sie die aktualisierten Best-Practice-Methoden nicht verwenden, um nach der Aktualisierung des alten Systems Statussuchabfragen durchzuführen, wird in der Antwort eine unvollständige Liste der Gruppenstatus zurückgegeben.

Im Folgenden finden Sie ein Beispiel dafür, was diese veraltete Anfragestruktur nach der Aktualisierung des alten Systems zurückgibt:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Beachten Sie, dass diese Antwort nur gruppenspezifische Status enthält und jene Status auslässt, die auf Systemebene deklariert wurden:

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
