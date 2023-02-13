---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error: SSO-Benutzer können sich nicht bei anmelden [!DNL Adobe Workfront] Aufgrund verschiedener Fehler'
description: Wenn Sie einen Anmeldefehler über Federated Single Sign-On, Ihre Benutzername/Kennwort-Kombination oder Ihren Zugriff auf [!DNL Workfront], the problem might be that your [!DNL Workfront] -Instanz verwendet SSO und Sie versuchen, sich mit einer falschen URL anzumelden. Stellen Sie sicher, dass Sie sich mit der richtigen URL ohne irgendetwas nach ".com"anmelden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# Fehler: SSO-Benutzer können sich nicht bei anmelden [!DNL Adobe Workfront] Aufgrund verschiedener Fehler

## Problem

Ich kann mich nicht bei [!DNL Workfront] und einen der folgenden Fehler erhalten haben:

* Leider können Sie nicht auf [!DNL Workfront] durch diesen Anmeldebildschirm. [!DNL Workfront] ist für Federated Single Sign-On mit SAML 2.0 eingerichtet. Bitte kontaktieren Sie Ihren [!DNL Workfront] Administrator.
* Diese Kombination aus Benutzername/Kennwort war falsch. Stellen Sie sicher, dass die Feststelltaste ausgeschaltet ist.
* Leider haben Sie keinen Zugriff auf [!DNL Workfront]. Bitte kontaktieren Sie Ihre [!DNL Workfront] Administrator , um einen Benutzernamen und ein Kennwort zu erhalten.

## Lösung

Ihre [!DNL Workfront] -Instanz verwendet SSO und Sie versuchen, sich über eine falsche URL anzumelden. Vergewissern Sie sich, dass Sie sich mit der richtigen URL ohne irgendetwas nach &quot;.com&quot;anmelden.

>[!TIP]
>
>Entfernen Sie alle vorhandenen Lesezeichen mit ungültigen URLs.
