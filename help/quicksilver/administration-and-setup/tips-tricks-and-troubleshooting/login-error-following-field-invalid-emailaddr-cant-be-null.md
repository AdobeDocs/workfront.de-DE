---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Anmeldefehler: Die folgenden Felder sind ungültig: emailAddr darf nicht null sein'
description: Wenn ich versuche, mich bei der  [!DNL Adobe Workfront] -URL für meine Domain anzumelden, werde ich zum SAML-Anmeldeportal weitergeleitet und dann zurück zu  [!DNL Workfront] , wobei ein Fehler angezeigt wird, der besagt, dass das Feld „emailAddr“ nicht null sein darf.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# Anmeldefehler: Die folgenden Felder sind ungültig: emailAddr darf nicht null sein

## Problem

Wenn ich versuche, mich mit meiner URL (https://customerdomain.my.workfront.com) bei [!DNL Adobe Workfront] anzumelden, werde ich zum SAML-Anmeldeportal weitergeleitet und dann mit dem folgenden Fehler zurück zu [!DNL Workfront]:

„Versuchen Sie es erneut. Die folgenden Felder sind ungültig: „emailAddr cannot be null.“

## Ursache

Dieser Fehler wird durch ein falsches Element im Bereich Benutzerattribute zuordnen der SAML 2.0-Konfiguration verursacht. Weitere Informationen zum Zuordnen von Benutzerattributen für SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Lösung

Aktualisieren Sie die Attributzuordnung für die E-Mail-Adresse und klicken Sie auf **[!UICONTROL Speichern]**.
