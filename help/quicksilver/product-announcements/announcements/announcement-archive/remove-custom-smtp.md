---
content-type: reference
navigation-topic: announcements
title: Benutzerdefiniertes SMTP als ausgehende E-Mail-Option entfernen
description: Mit der Version 20.3 (die für August 2020 geplant ist) wird Adobe Workfront auf ein neues E-Mail-System umgestellt, das die Zuverlässigkeit Ihres E-Mail-Versands für Workfront-Updates und -Benachrichtigungen deutlich erhöht. Dadurch können Kunden nicht mehr ihren eigenen SMTP-E-Mail-Server verwenden, um ihre E-Mail von der Workfront-Plattform an den gewünschten Empfänger weiterzuleiten. Alle E-Mails werden direkt vom Workfront Mail Server gesendet.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Benutzerdefiniertes SMTP als ausgehende E-Mail-Option entfernen

Mit der Version 20.3 (die für August 2020 geplant ist) wird Adobe Workfront auf ein neues E-Mail-System umgestellt, das die Zuverlässigkeit Ihres E-Mail-Versands für Workfront-Updates und -Benachrichtigungen deutlich erhöht. Dadurch können Kunden nicht mehr ihren eigenen SMTP-E-Mail-Server verwenden, um ihre E-Mail von der Workfront-Plattform an den gewünschten Empfänger weiterzuleiten. Alle E-Mails werden direkt vom Workfront Mail Server gesendet.

Auf diese Funktion können Sie zugreifen, indem Sie sich als Systemadministrator anmelden und zu Einrichtung > E-Mail > Einrichtung navigieren. Im Folgenden finden Sie einen Screenshot, in dem die Funktion hervorgehoben wird:

![](assets/email-server-settings-350x226.png)

Die in diesem Screenshot hervorgehobene Einstellung führt zu einer automatischen Umstellung auf die Workfront Mail Server-Option mit Version 20.3.

Wenn Sie einen benutzerdefinierten SMTP-Mail-Server konfiguriert haben, empfehlen wir dringend, sich an Ihr IT-Team zu wenden **, um sicherzustellen, dass E-Mails von notifications@my.workfront.com nicht für eingehende E-Mails an Ihr System blockiert werden.** Unter Konfigurieren Ihrer Firewall finden Sie auch Informationen dazu, von welchen IP-Adressen unser Traffic und unsere E-Mail stammen.

Wenden Sie sich bei weiteren Fragen oder Bedenken an das [Workfront-Supportteam](https://one.workfront.com/s/support?language=en_US).
