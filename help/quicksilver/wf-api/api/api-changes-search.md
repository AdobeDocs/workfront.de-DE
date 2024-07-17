---
filename: api-changes-search
content-type: api
keywords: object,status,search,best,practice,response
navigation-topic: api-navigation-topic
title: "Core API changes: Status search responses"
description: Änderungen in der Art und Weise, wie Workfront Statusobjekte speichert.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Core-API-Änderungen: Status-Suchantworten

Es wurden Änderungen an der Art und Weise vorgenommen, wie Workfront Statusobjekte speichert. Diese Änderungen wirken sich nicht darauf aus, wie Statussuchanfragen ausgeführt werden, sondern beeinflussen die Antwort, die von API-Anfragen zurückgegeben wird, die eine Suche nach Statusobjekten enthalten, indem eine unvollständige Liste der Gruppenstatus zurückgegeben wird.

## Best Practices

Um zuverlässig die vollständige Liste der für eine Gruppe verfügbaren Status abzurufen, gelten die folgenden Anforderungen als Best Practices.

>[!NOTE]
>
>Diese Anfragestrukturen werden für alle Benutzer empfohlen, unabhängig davon, ob die Statussuchänderungen an Ihrem Cluster vorgenommen wurden oder nicht.

Für den Projektgruppenstatus:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Für Aufgabengruppenstatus:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Für den Status der Problemgruppe:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Alle drei Endpunkte akzeptieren den Parameter **includeHidden=true** , um den Status des ausgeblendeten Projekts/der Aufgabe/des Problems einer bestimmten Gruppe abzurufen. Durch die Modellierung Ihrer Statussuchabfragen nach diesen Best-Practice-Beispielen wird sichergestellt, dass alle Gruppenstatusinformationen in jeder Antwort enthalten sind.

Im Folgenden finden Sie ein Beispiel für eine Statussuchabfrage, die an eine Aufgabengruppe gesendet wird, die einen auf Systemebene gesperrten Status **Benutzerdefiniert_1** und einen entsperrten Status **Benutzerdefiniert_2** aufweist:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Durch Verwendung dieses Formats wird sichergestellt, dass Ihre Antwort alle folgenden Elemente enthält:

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

## Grundlegendes zu den Änderungen an der alten Statussuchabfrage

Unter dem alten System kopiert eine Statussuchabfrage alle Systemstatus, die für alle in einer Abfrage enthaltenen Gruppen verfügbar sind. Die veraltete Antwort würde dann alle Systemstatus und Gruppenstatus enthalten, die für jede in der Abfrage enthaltene Gruppe verfügbar sind.

Beispielsweise diese Abfrage (die nicht den aktuellen empfohlenen Best Practices entspricht):

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

hätte die folgende Antwort unter dem alten System, das alle Objektstatus enthält:

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

Nach den Aktualisierungen, die an der Speicherung und Verwendung von Status vorgenommen wurden, werden die Status jedoch nicht für Gruppen kopiert und von jeder Gruppe auf Systemebene übernommen. Daher liest die Abfrage der Such-API nur die Status, die einer bestimmten Gruppe direkt zugeordnet sind. Daher enthält die Antwort systemgesperrte und entsperrte Status, jedoch nur für die Gruppen, die nach dem Hinzufügen des betreffenden Status erstellt wurden.

Wenn Sie die aktualisierten Best Practice-Methoden nicht zum Erstellen von Statussuchabfragen verwenden, nachdem das alte System aktualisiert wurde, wird in der Antwort eine unvollständige Liste der Gruppenstatus zurückgegeben.

Im Folgenden finden Sie ein Beispiel dafür, was diese veraltete Anforderungsstruktur nach der Aktualisierung des Legacy-Systems zurückgibt:

>**Beispiel:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Beachten Sie, dass diese Antwort nur gruppenspezifische Status enthält und die Status auslässt, die auf Systemebene deklariert wurden:

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
