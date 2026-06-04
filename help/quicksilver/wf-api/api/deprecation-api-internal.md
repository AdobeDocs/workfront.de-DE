---
content-type: api
navigation-topic: api-navigation-topic
title: Einstellung von API-intern
description: Einstellung von API-intern
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
TQID: https://experienceleague.adobe.com/LGyk8MIATMQj6JHqKmjkeL2pXW-b6xtxo2heMd4h0y4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 4%

---

# Einstellung von API-intern

API-intern ist eine Version der Adobe Workfront-API, die aufgrund ihres Designs und Zwecks nicht unterstützt wird. Obwohl es die neuesten Aktualisierungen der Workfront-API enthält, kann es sich ohne Vorankündigung ändern und sollte daher bei Produktionsintegrationen mit Vorsicht verwendet werden. Workfront empfiehlt dringend, alle API-internen Integrationen auf eine versionierte API zu aktualisieren.

Weitere Informationen zu unterstützten Versionen der Workfront-API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

**Verwendung von API-nicht unterstützt**

Wenn Ihre Integrationen Funktionen erfordern, die nicht in einer versionierten API verfügbar sind, empfiehlt Workfront die Verwendung von API-Nicht unterstützt . Ähnlich wie API-intern wird API-Unsupported nicht unterstützt. „API-Nicht unterstützt“ umfasst auch die neuesten Änderungen an der Workfront-API und kann ohne Vorankündigung geändert werden. Workfront empfiehlt die Verwendung von API-Nicht unterstützt in Ihrer Testumgebung, in der Sie neue Funktionen erkunden und sicherstellen können, dass die API frei von Fehlern ist.

**Bestimmen der verwendeten API-Version**

Sie können die API-Version ermitteln, die Ihre Integrationen verwenden, indem Sie REST verwenden, um einen URI zu erstellen, der einen Aufruf über HTTPS an Workfront sendet und dann eine JSON-Antwort zurückgibt.

Das folgende Beispiel zeigt einen URI, der API-intern aufruft:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

Das folgende Beispiel zeigt einen URI, der API-Unsupported aufruft:

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>Bei nicht unterstützten API-Aufrufen wird der `/api` Abschnitt der URL weggelassen.

Das folgende Beispiel zeigt einen URI, der Version 15.0 der API aufruft:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
