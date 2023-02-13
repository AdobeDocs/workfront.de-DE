---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Abrufen von Währungsinformationen für ein Projekt, wenn die Währung null ist
description: Abrufen von Währungsinformationen für ein Projekt, wenn die Währung null ist
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Abrufen von Währungsinformationen für ein Projekt, wenn die Währung null ist (nicht zugewiesen)

Das Projektobjekt mit dem Währungsfeld kann mit der folgenden Anfrage abgerufen werden:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Dadurch wird der folgende Antworttext zurückgegeben:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Wenn die Währung nicht für das Projekt festgelegt ist, enthält diese Antwort eine Währung mit dem Wert `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Wenn Sie die Währung für das Projekt benötigen (z. B. für Berechnungen), können Sie die Standardwährung für den Kunden abrufen:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

Die Antwort enthält die Währung, die der Benutzer als Standard festgelegt hat, die von allen Projekten für diesen Kunden verwendet wird, für die die Währung nicht festgelegt ist:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
