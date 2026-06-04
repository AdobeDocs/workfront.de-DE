---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden'
description: Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, und eine Fehlermeldung erhält, dass ihm das System keine Zugriffsebene zuweist, kann dies daran liegen, dass Ihrem System Zugriffsebenen fehlen, die mit der Anfragelizenz verknüpft sind.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 16%

---

# Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden

Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, erhält er die folgende Fehlermeldung:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Dem neuen Benutzer wird keine Zugriffsebene zugewiesen.

Standardmäßig wird bei der automatischen Bereitstellung der Lizenztyp Anfrage verwendet. Wenn keine Zugriffsebenen mit einer Anfragelizenz vorhanden sind, kann das System dem Benutzer keine Zugriffsebene zuweisen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Lösung

Erstellen Sie eine allgemeine Zugriffsebene mit einer Anfragelizenz:

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Zugriffsebenen]**.

1. Klicken Sie **[!UICONTROL Neue Zugriffsebene]**.
1. Geben Sie einen &quot;**[!UICONTROL &quot;]**.
1. Wählen Sie **[!UICONTROL Dropdown-Menü]** Lizenztyp) die Option Anfrage aus.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

Nachdem Sie eine Zugriffsebene mit einer Anfragelizenz erstellt haben, müssen sich Benutzer mit ihren SSO-Anmeldeinformationen anmelden.


