---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Wenn eine authentifizierte E-Mail aufgrund der DMARC-Richtlinie der Domäne nicht akzeptiert wird
description: Wenn eine E-Mail von der [!DNL Workfront] aufgrund der DMARC-Richtlinie der Domain nicht akzeptiert wird, kann Ihr E-Mail-Administrator das Problem beheben, indem er Ihr E-Mail-System so konfiguriert, dass alle E-Mails von workfront.com zugelassen werden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Nicht authentifizierte E-Mails werden aufgrund der DMARC-Richtlinie der Domain nicht akzeptiert.

## Anfrage

[Test] Ich habe die folgende Bounce-back-E-Mail erhalten:

550-5.7.1 Nicht authentifizierte E-Mail von &quot;customer domain.com&quot;wird aufgrund von\
DMARC-Richtlinie der Domain 550-5.7.1. Wenden Sie sich an den Administrator von &quot;customer domain.com&quot;.\
550-5.7.1 Domain, wenn es sich um eine legitime E-Mail handelt. Besuch\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) Informationen zu DMARC\
550 5.7.1 Initiative.

## Lösung

DMARC ist im E-Mail-System Ihres Unternehmens konfiguriert und ist nicht Teil von [!DNL Adobe Workfront]. Wenn Sie diese E-Mail erhalten, müssen Sie sich an Ihren E-Mail-Administrator wenden.

Ihr E-Mail-Administrator sollte Ihr E-Mail-System so konfigurieren, dass E-Mails von noreply@workfront.com zugelassen/vertrauenswürdig sind oder vorzugsweise alle E-Mails von workfront.com erhalten.

Weitere Informationen zu DMARC finden Sie unter [https://support.google.com/mail/answer/2451690](https://support.google.com/mail/answer/2451690)
