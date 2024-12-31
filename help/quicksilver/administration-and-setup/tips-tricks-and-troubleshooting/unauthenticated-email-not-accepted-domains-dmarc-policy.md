---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Nicht authentifizierte E-Mails werden aufgrund der DMARC-Richtlinie der Domain nicht akzeptiert
description: Wenn eine vom System gesendete E [!DNL Workfront] Mail aufgrund der DMARC-Richtlinie der Domain nicht akzeptiert wird, kann Ihr E-Mail-Administrator das Problem beheben, indem er Ihr E-Mail-System so konfiguriert, dass alle E-Mails von workfront.com zugelassen werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Nicht authentifizierte E-Mails werden aufgrund der DMARC-Richtlinie der Domain nicht akzeptiert

## Problem

[Test] Ich habe die folgende Bounce-E-Mail erhalten:

550-5.7.1 Nicht authentifizierte E-Mail von „customer domain.com“ wird aus folgenden Gründen nicht akzeptiert\
DMARC-Richtlinie der Domain 550-5.7.1. Bitte wenden Sie sich an den Administrator von „customer domain.com“\
550-5.7.1 Domain, wenn es sich um eine legitime E-Mail handelte. Please visit\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) für weitere Informationen zu DMARC\
550 5.7.1-Initiative.

## Lösung

DMARC wird im E-Mail-System Ihres Unternehmens konfiguriert und ist nicht Teil von [!DNL Adobe Workfront]. Wenn Sie diese E-Mail erhalten, müssen Sie sich an Ihren E-Mail-Administrator wenden.

Ihr E-Mail-Administrator sollte Ihr E-Mail-System so konfigurieren, dass E-Mails von noreply@workfront.com oder vorzugsweise alle E-Mails von workfront.com zugelassen/vertrauenswürdig sind.

Weitere Informationen zu DMARC finden Sie unter [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
