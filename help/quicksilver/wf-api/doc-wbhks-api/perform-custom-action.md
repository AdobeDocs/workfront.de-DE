---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Durchführen einer benutzerdefinierten Aktion
description: Durchführen einer benutzerdefinierten Aktion
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 1%

---


# Durchführen einer benutzerdefinierten Aktion (noch nicht implementiert)

Dieser Endpunkt ermöglicht es einem Adobe Workfront-Benutzer (oder einem automatisierten Workflow-Ereignis), eine Aktion im externen System durchzuführen. Der /customAction-Endpunkt akzeptiert einen „name“-Parameter, mit dem der Webhook-Anbieter mehrere benutzerdefinierte Vorgänge implementieren kann.

Der Webhook-Anbieter registriert benutzerdefinierte Aktionen bei Workfront, indem er die Aktionen in die /serviceInfo-Antwort unter customActions aufnimmt. Workfront lädt diese Liste, wenn Sie den Webhook-Anbieter unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen einrichten oder aktualisieren.

Benutzerinnen und Benutzer können die benutzerdefinierte Aktion mit Triggern versehen, indem sie den Abschnitt unter „Dokumentaktionen“ auswählen

**URL**

GET/customAction

## Abfrageparameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>Die Kennung, die den Typ der auszuführenden Aktion angibt. Dieser Wert entspricht einem der customAction-Werte, die vom Endpunkt /serviceInfo zurückgegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>Die Workfront-Dokument-ID, für die die Aktion ausgeführt wird.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> Die ID der Workfront-Dokumentversion, für die die Aktion ausgeführt wird.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben. Bei einem Fehler (d. h. Status = „Fehler„) zeigt Workfront dem Benutzer die bereitgestellte Fehlermeldung an.

**Beispiel:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

Antwort

```
{
status: "success"
}
```
