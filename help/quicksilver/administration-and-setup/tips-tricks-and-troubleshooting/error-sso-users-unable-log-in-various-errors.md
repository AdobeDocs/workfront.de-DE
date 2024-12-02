---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehler: SSO-Benutzer können sich aufgrund verschiedener Fehler nicht bei [!DNL Adobe Workfront] anmelden'
description: Wenn Sie einen Anmeldefehler über Federated Single Sign-on erhalten, verwenden Sie Ihre Benutzername-/Passwort-Kombination oder Ihr Zugriff auf die [!DNL Workfront], the problem might be that your [!DNL Workfront] Instanz SSO und Sie versuchen, sich mit einer falschen URL anzumelden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Fehler: SSO-Benutzer können sich aufgrund verschiedener Fehler nicht bei [!DNL Adobe Workfront] anmelden

## Problem

Ich kann mich nicht bei [!DNL Workfront] anmelden und habe einen der folgenden Fehler erhalten:

* Leider können Sie über diesen Anmeldebildschirm nicht auf [!DNL Workfront] zugreifen. [!DNL Workfront] ist für Federated Single Sign-On mit SAML 2.0 eingerichtet. Wenden Sie sich an Ihren [!DNL Workfront] -Administrator.
* Diese Kombination aus Benutzername und Passwort war nicht ganz richtig. Vergewissern Sie sich, dass das Schloss nicht aktiviert ist, und versuchen Sie es erneut.
* Sie haben leider keinen Zugriff auf [!DNL Workfront]. Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um einen Benutzernamen und ein Kennwort zu erhalten.

## Lösung

Ihre [!DNL Workfront] -Instanz verwendet SSO und Sie versuchen, sich über eine falsche URL anzumelden. Stellen Sie sicher, dass Sie sich mit der richtigen URL ohne irgendetwas nach &quot;.com&quot;anmelden.

>[!TIP]
>
>Entfernen Sie alle vorhandenen Lesezeichen mit ungültigen URLs.
