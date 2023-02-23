---
content-type: api
navigation-topic: api-navigation-topic
title: Veraltete API-interne
description: Veraltete API-interne
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Veraltete API-interne

API-intern ist eine Version der Adobe Workfront-API, die aufgrund ihres Designs und Zwecks nicht unterstützt wird. Obwohl es die neuesten Aktualisierungen der Workfront-API enthält, kann es ohne Vorankündigung geändert werden und sollte daher bei Produktionsintegrationen mit Vorsicht verwendet werden. Workfront empfiehlt dringend, alle API-internen Integrationen auf eine versionierte API zu aktualisieren.

Weitere Informationen zu unterstützten Versionen der Workfront-API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

**Verwenden von API-Nicht unterstützt**

Wenn Ihre Integrationen Funktionen erfordern, die in einer versionierten API nicht verfügbar sind, empfiehlt Workfront die Verwendung von API-Nicht unterstützt. Ähnlich wie API-intern wird API-Unsupported nicht unterstützt. API-Nicht unterstützt enthält auch die neuesten Änderungen an der Workfront-API und kann ohne Vorankündigung geändert werden. Workfront empfiehlt Ihnen, API-Nicht unterstützt in Ihrer Testumgebung zu verwenden, um neue Funktionen zu erkunden und sicherzustellen, dass die API keine Fehler enthält.

**Bestimmen der verwendeten API-Version**

Sie können die Version der API, die Ihre Integrationen verwenden, mithilfe von REST ermitteln, um einen URI zu erstellen, der einen Aufruf über HTTPS an Workfront sendet und dann eine JSON-Antwort zurückgibt.

Das folgende Beispiel zeigt einen URI, der API-intern aufruft:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

Das folgende Beispiel zeigt einen URI, der API-Unsupported aufruft:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

Das folgende Beispiel zeigt einen URI, der Version 15.0 der API aufruft:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
