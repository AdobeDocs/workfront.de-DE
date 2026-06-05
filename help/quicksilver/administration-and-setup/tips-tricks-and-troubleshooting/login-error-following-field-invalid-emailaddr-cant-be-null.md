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
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# Anmeldefehler: Die folgenden Felder sind ungültig: emailAddr darf nicht null sein

## Problem

Wenn ich versuche, mich mit meiner URL (https://customerdomain.my.workfront.com) bei [!DNL Adobe Workfront] anzumelden, werde ich zum SAML-Anmeldeportal weitergeleitet und dann mit dem folgenden Fehler zurück zu [!DNL Workfront]:

„Versuchen Sie es erneut. Die folgenden Felder sind ungültig: „emailAddr cannot be null.“

## Ursache

Dieser Fehler wird durch ein falsches Element im Bereich Benutzerattribute zuordnen der SAML 2.0-Konfiguration verursacht. Weitere Informationen zum Zuordnen von Benutzerattributen für SAML 2.0 finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Lösung

Aktualisieren Sie die Attributzuordnung für die E-Mail-Adresse und klicken Sie auf **[!UICONTROL Speichern]**.
