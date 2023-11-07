---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Deaktivieren eines Benutzers über die API
description: Deaktivieren eines Benutzers über die API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Deaktivieren eines Benutzers über die API

Wenn ein Benutzer Ihre Organisation verlässt, können Sie ihn deaktivieren, indem Sie seine Adobe Workfront-Lizenz einem anderen Benutzer zur Verfügung stellen und verhindern, dass ihm versehentlich Arbeitsaufgaben zugewiesen werden. Durch die Deaktivierung eines Benutzers behalten Sie seinen Arbeitsverlauf bei, einschließlich der Arbeitsaufgaben und der Verknüpfung mit Notizen, Stunden und Dokumenten.

Weitere Informationen zum Deaktivieren eines Benutzers finden Sie unter [Benutzer deaktivieren oder reaktivieren](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Informationen zur Verwendung der Core-API finden Sie unter [API-Grundlagen](../../wf-api/general/api-basics.md).

So deaktivieren Sie einen Benutzer über die API:

1. Generieren Sie mithilfe der folgenden API-Anfrage einen API-Schlüssel:

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Suchen Sie die GUID für den Benutzer, den Sie deaktivieren möchten.

   1. Verwenden Sie die folgende API-Anfrage, um die GUID für alle Benutzer in Ihrem System abzurufen. Beachten Sie, dass die Variable **isActive** Feldanzeigen **true** für Benutzer, die derzeit aktiv sind, und **false** für Benutzer, die deaktiviert wurden:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Suchen Sie die GUID für den Benutzer, den Sie deaktivieren möchten, und verwenden Sie Folgendes **PUT** Anforderung zum Ändern der **isActive** Feldwert zu **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. Die Antwort zeigt, dass die **isActive** Der Feldwert hat sich geändert von **true** nach **false** gibt an, dass der Benutzer deaktiviert wurde:

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
