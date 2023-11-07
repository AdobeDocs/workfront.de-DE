---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Benutzerdefinierte Aktion ausführen
description: Benutzerdefinierte Aktion ausführen
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# Benutzerdefinierte Aktion ausführen (noch nicht implementiert)

Dieser Endpunkt ermöglicht es einem Adobe Workfront-Benutzer (oder einem automatisierten Workflow-Ereignis), eine Aktion im externen System durchzuführen. Der Endpunkt /customAction akzeptiert einen Parameter &quot;name&quot;, der es dem Webhook-Provider ermöglicht, mehrere benutzerdefinierte Vorgänge zu implementieren.

Der Webhook-Provider registriert benutzerdefinierte Aktionen bei Workfront, indem er die Aktionen in die Antwort /serviceInfo unter customActions einbezieht. Workfront lädt diese Liste beim Einrichten oder Aktualisieren des Webhook-Providers unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen.

Benutzer können die benutzerdefinierte Aktion durch Auswahl des Bereichs unter &quot;Dokumentaktionen&quot;Trigger haben.

**URL**

GET /customAction

## Abfrageparameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>Die Kennung, die die Art der auszuführenden Aktion angibt. Dieser Wert entspricht einem der customAction -Werte, die vom Endpunkt /serviceInfo zurückgegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>Die Dokument-ID der Arbeitsfläche, für die die Aktion ausgeführt wird.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> Die Kennung der Dokumentversion, für die die Aktion ausgeführt wird.</td> 
  </tr> 
 </tbody> 
</table>

 

## Antwort

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben. Bei einem Fehler (d. h. Status = &quot;Fehler&quot;) zeigt Workfront die bereitgestellte Fehlermeldung an.

**Beispiel:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: "success"
}
```
