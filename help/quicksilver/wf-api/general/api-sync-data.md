---
content-type: api
keywords: API,Daten,Synchronisierung,Journal,Eintrag,Objekt
navigation-topic: general-api
title: Verwenden der API zum Synchronisieren von Daten für Programme und Services
description: Verwenden der API zum Synchronisieren von Daten für Programme und Services
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
TQID: https://experienceleague.adobe.com/7ozt2OXI0CWlPmtkJGlaD-n6pekapA0X-GBpwDhFZ4Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 478
ht-degree: 2%

---

# Verwenden der API zum Synchronisieren von Daten für Programme und Services

Dies sind einige gängige Möglichkeiten, die API zum Synchronisieren von Daten für Programme und Services zu verwenden.

## Fast Echtzeit-Updates

Adobe Workfront verwendet „Ereignisabonnements“ (auch allgemein als Webhooks bezeichnet), um nahezu in Echtzeit Aktualisierungen zu unterstützten Objekten und Aktionen über die API an Ihre gewünschten Endpunkte zu senden. Sie können davon ausgehen, dass Sie innerhalb von 5 Sekunden ein Update zu neuen Objekten und Aktionen erhalten, aber im Durchschnitt werden Aktualisierungen in etwa 1 Sekunde eintreffen. Weitere Informationen dazu, welche Objekttypen unterstützt werden, welche Aktionstypen unterstützt werden, technische Details und Beispiele zum Einrichten von Ereignisabonnements finden Sie unter [Ereignisabonnement-](../../wf-api/general/event-subs-api.md) und [Bereitstellungsanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).

## Batch-Aktualisierungen

Batch-Aktualisierungen stellen eine Möglichkeit dar, Ihr System für Aktualisierungen zu konfigurieren, indem Sie regelmäßig Anfragen an Workfront-Server senden. Dazu gibt es viele Möglichkeiten, aber im Allgemeinen besteht der Prozess darin, dass Ihr Service eine Anfrage an die Workfront-API-Server sendet und nach Objekten sucht, die seit dem letzten Anforderungsaufruf erstellt oder geändert wurden. Informationen zu potenziellen -Aufrufen und hilfreichen Parametern finden Sie im Abschnitt [Verhalten abrufen](../../wf-api/general/api-basics.md#get-behavior) im Artikel [API-Grundlagen](../../wf-api/general/api-basics.md) .

Beim Einrichten des Service für Batch-Aktualisierungen sollten Sie folgende wichtige Punkte beachten:

### Eingabedaten

Eingabedaten werden mit ISO 8601-Formatierung gespeichert. Dieser Standard enthält Informationen zu Datum, Uhrzeit und Zeitzone.

**Beispiel:** ISO 8601-Datumsformat

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Sowohl das Datum, an dem ein Objekt erstellt wird, als auch das letzte Datum, an dem das Objekt geändert wurde, werden als „entryDate“ bzw. „lastUpdateDate“ gespeichert. Detaillierte Informationen zu Workfront-Objekten, ihren zugehörigen Feldern und Feldnamen finden Sie im [API-Explorer](../../wf-api/general/api-explorer.md). Beachten Sie, dass sich das entryDate für ein bestimmtes Workfront-Objekt nicht ändert, wobei sich das lastUpdatedDate jedes Mal ändert, wenn das Objekt geändert wird.

**Beispiel** GET-Anfrage für ein Anfrageobjekt, die das Feld **lastUpdateDate** verwendet. Diese Anfrage gibt alle Probleme zurück, die seit diesem angegebenen Datum aktualisiert wurden.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Tagebucheintragsobjekt

Wenn Sie Änderungen zu einem bestimmten Feld eines Objekts erhalten möchten, können Sie das Objekt „Journaleintrag“ abfragen. Das Workfront-Journaleintragsobjekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Weitere Informationen finden [&#x200B; unter „Konfigurieren von &#x200B;](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)&quot;.

Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt. Anschließend können Sie das Journaleintragsobjekt mit einem API-Aufruf ähnlich dem folgenden abfragen:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>„entryDate“ wird verwendet, um einen Journaleintrag einer Änderung anzuzeigen, anstatt das geänderte Objekt selbst zu betrachten.
