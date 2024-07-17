---
content-type: api
keywords: API,data,sync,journal,entry,object
navigation-topic: general-api
title: Verwenden der API zum Synchronisieren von Daten für Programme und Dienste
description: Verwenden der API zum Synchronisieren von Daten für Programme und Dienste
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Verwenden der API zum Synchronisieren von Daten für Programme und Dienste

Dies sind einige gängige Methoden, mit denen Sie die API zum Synchronisieren von Daten für Programme und Dienste verwenden können.

## Nahezu alle Echtzeitaktualisierungen

Adobe Workfront verwendet &quot;Ereignisabos&quot;(auch häufig als Webhooks bezeichnet), um über die API nahezu Echtzeitaktualisierungen zu unterstützten Objekten und Aktionen an Ihren gewünschten Endpunkt bzw. Ihre gewünschten Endpunkte zu senden. Sie können innerhalb von 5 Sekunden mit einer Aktualisierung neuer Objekte und Aktionen rechnen, aber im Durchschnitt werden Aktualisierungen in etwa 1 Sekunde angezeigt. Weitere Informationen dazu, welche Objekttypen unterstützt werden, welche Aktionstypen unterstützt werden, technische Details und Beispiele zum Einrichten von Ereignisanmeldungen finden Sie unter [API für die Ereignisabonnement-API](../../wf-api/general/event-subs-api.md) und [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).

## Batch-Aktualisierungen

Mit Batch-Aktualisierungen können Sie Ihr System für Aktualisierungen konfigurieren, indem Sie regelmäßige Anfragen an Workfront-Server richten. Es gibt viele Möglichkeiten, dies zu tun. Im Allgemeinen besteht der Prozess jedoch darin, dass Ihr Dienst eine Anfrage an die Workfront-API-Server sendet und nach Objekten sucht, die seit dem letzten Anfrageaufruf erstellt oder geändert wurden. Weitere Informationen zu potenziellen Anforderungsaufrufen und hilfreichen Parametern finden Sie im Abschnitt [Verhalten der GET](../../wf-api/general/api-basics.md#get-behavior) im Artikel [API-Grundlagen](../../wf-api/general/api-basics.md) .

Beachten Sie beim Einrichten Ihres Dienstes für Batch-Aktualisierungen Folgendes:

### Eintrittstage

Einstiegsdaten werden im ISO 8601-Format gespeichert. Dieser Standard umfasst Informationen zu Datum, Uhrzeit und Zeitzone.

**Beispiel:** Datumsformat nach ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

Sowohl das Datum, an dem ein Objekt erstellt wird, als auch das Datum, an dem das Objekt zuletzt geändert wurde, werden als &quot;entryDate&quot;bzw. &quot;lastUpdateDate&quot;gespeichert. Ausführliche Informationen zu Workfront-Objekten, den zugehörigen Feldern und Feldnamen finden Sie im [API-Explorer](../../wf-api/general/api-explorer.md). Beachten Sie, dass sich das entryDate für ein bestimmtes Workfront-Objekt nicht ändert, wobei sich lastUpdatedDate jedes Mal ändert, wenn das Objekt geändert wird.

**Beispiel:** GET-Anfrage für ein Ausgabenobjekt unter Verwendung des Felds **lastUpdateDate** . Diese Anfrage gibt alle Probleme zurück, die seit dem angegebenen Datum aktualisiert wurden.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Journaleintragsobjekt

Wenn Sie Änderungen an einem bestimmten Feld eines Objekts erhalten möchten, können Sie das Objekt &quot;Journaleintrag&quot;abfragen. Das Workfront Journal Entry-Objekt kann so eingerichtet werden, dass bei jeder Änderung dieser Felder Informationen über bestimmte Objektfelder protokolliert werden. Weitere Informationen finden Sie unter [Systemaktualisierungen konfigurieren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) .

Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird bei jeder Änderung dieses Felds ein entsprechender Journaleintrag erstellt. Anschließend können Sie das Journaleintragsobjekt mithilfe eines API-Aufrufs abfragen, der dem folgenden ähnelt:

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot;wird verwendet, um einen Journaleintrag einer Änderung zu betrachten, anstatt das geänderte Objekt selbst zu betrachten.
