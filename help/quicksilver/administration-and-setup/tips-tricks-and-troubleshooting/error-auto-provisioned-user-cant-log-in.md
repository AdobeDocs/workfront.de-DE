---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden'
description: Wenn ein automatisch bereitgestellter Benutzer versucht, sich zum ersten Mal anzumelden, und einen Fehler erhält, der besagt, dass das System ihm keine Zugriffsstufe zuweist, kann dies daran liegen, dass Ihrem System die mit der Anfragelizenz verknüpften Zugriffsebenen fehlen.
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

Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, erhält er den folgenden Fehler:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Das System weist dem neuen Benutzer keine Zugriffsebene zu.

Standardmäßig verwendet die automatische Bereitstellung den Lizenztyp Anforderung . Wenn keine Zugriffsebene mit einer Anfragelizenz vorhanden ist, kann das System dem Benutzer keine Zugriffsebene zuweisen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>  
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

Erstellen Sie eine einfache Zugriffsstufe mit einer Anfragelizenz:

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Zugriffsebenen]**.

1. Klicken Sie auf **[!UICONTROL Neue Zugriffsebene]**.
1. Geben Sie einen **[!UICONTROL Namen]** ein.
1. Wählen Sie im Dropdown-Menü **[!UICONTROL Lizenztyp]** die Option &quot;Anforderung&quot;aus.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

Nachdem Sie eine Zugriffsstufe mit einer Anforderungslizenz erstellt haben, lassen Sie den Benutzer sich mit seinen SSO-Anmeldeinformationen anmelden.


