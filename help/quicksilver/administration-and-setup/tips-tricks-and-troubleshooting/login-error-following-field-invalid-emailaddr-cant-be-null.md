---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Login Error: The following fields are invalid: emailAddr cannot be null'
description: Wenn ich versuche, mich bei der URL für meine Domäne anzumelden, werde ich zum SAML-Anmeldungsportal umgeleitet und dann zurück zu  [!DNL Workfront] umgeleitet. Dabei wird ein Fehler ausgegeben, der besagt, dass das Feld emailAddr nicht null sein darf. [!DNL Adobe Workfront]
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# Anmeldefehler: Die folgenden Felder sind ungültig: emailAddr darf nicht null sein

## Problem

Wenn ich versuche, mich mit meiner URL (https://customerdomain.my.workfront.com) bei [!DNL Adobe Workfront] anzumelden, wird ich zum SAML-Anmeldungsportal umgeleitet und dann mit dem folgenden Fehler zurück zu [!DNL Workfront] geleitet:

„Versuchen Sie es erneut. Die folgenden Felder sind ungültig: emailAddr darf nicht null sein.&quot;

## Ursache

Dieser Fehler wird durch ein falsches Element im Bereich Benutzerattribute zuordnen der SAML 2.0-Konfiguration verursacht. Weitere Informationen zum Zuordnen von Benutzerattributen für SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Lösung

Aktualisieren Sie die Attributzuordnung für die E-Mail-Adresse und klicken Sie auf **[!UICONTROL Speichern]**.
