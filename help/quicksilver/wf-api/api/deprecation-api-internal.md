---
content-type: api
navigation-topic: api-navigation-topic
title: Einstellung von API-intern
description: Einstellung von API-intern
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

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
