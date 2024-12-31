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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%

---

# Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden

Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, erhält er die folgende Fehlermeldung:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Dem neuen Benutzer wird keine Zugriffsebene zugewiesen.

Standardmäßig wird bei der automatischen Bereitstellung der Lizenztyp Anfrage verwendet. Wenn keine Zugriffsebenen mit einer Anfragelizenz vorhanden sind, kann das System dem Benutzer keine Zugriffsebene zuweisen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>  
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

Erstellen Sie eine allgemeine Zugriffsebene mit einer Anfragelizenz:

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Zugriffsebenen]**.

1. Klicken Sie **[!UICONTROL Neue Zugriffsebene]**.
1. Geben Sie einen &quot;**[!UICONTROL &quot;]**.
1. Wählen Sie **[!UICONTROL Dropdown-Menü]** Lizenztyp) die Option Anfrage aus.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

Nachdem Sie eine Zugriffsebene mit einer Anfragelizenz erstellt haben, müssen sich Benutzer mit ihren SSO-Anmeldeinformationen anmelden.


