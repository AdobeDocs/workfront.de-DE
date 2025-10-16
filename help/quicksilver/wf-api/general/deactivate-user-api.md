---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Deaktivieren von Benutzern über die API
description: Deaktivieren von Benutzern über die API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: f9a154fa92217810b762ac48169512bc0bca7305
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# Deaktivieren von Benutzern über die API

Wenn ein(e) Benutzende(r) Ihre Organisation verlässt, können Sie den/die Benutzende(n) deaktivieren, indem Sie dessen/deren Adobe Workfront-Lizenz einem/r anderen Benutzenden zur Verfügung stellen und so verhindern, dass ihm/ihr versehentlich Arbeit zugewiesen wird. Durch die Deaktivierung eines Benutzers behalten Sie seinen Arbeitsverlauf bei, einschließlich der Arbeitszuweisungen und ihrer Zuordnung zu Notizen, Stunden und Dokumenten.

Weitere Informationen zur Deaktivierung von Benutzenden finden Sie unter &quot;[Deaktivieren oder Reaktivieren von Benutzenden](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Informationen zur Verwendung der Kern-API finden Sie unter [API-Grundlagen](../../wf-api/general/api-basics.md).

So deaktivieren Sie einen Benutzer über die API:

1. Generieren Sie einen API-Schlüssel mithilfe der folgenden API-Anfrage:

   ```
   <domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
   ```

1. Suchen Sie die GUID für den Benutzer, den Sie deaktivieren möchten.

   Verwenden Sie die folgende API-Anfrage, um die GUID für alle Benutzer in Ihrem System abzurufen. Beachten Sie, dass das Feld **isActive** für derzeit aktive Benutzer **true** und für **deaktivierte Benutzer false** anzeigt:

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
   ```

1. Verwenden Sie die folgende **PUT**-Anfrage, um den Feldwert **isActive** des Benutzers in &quot;**&quot;** ändern:

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
   ```

1. Die Antwort zeigt an, dass der Wert des **isActive**-Felds von **true** in **false** geändert wurde. Dies bedeutet, dass der Benutzer deaktiviert wurde:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
