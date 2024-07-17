---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden"
description: Wenn ein automatisch bereitgestellter Benutzer versucht, sich zum ersten Mal anzumelden, und einen Fehler erhält, der besagt, dass das System ihm keine Zugriffsstufe zuweist, kann dies daran liegen, dass Ihrem System die mit der Anfragelizenz verknüpften Zugriffsebenen fehlen. Bei der automatischen Bereitstellung wird der Lizenztyp Anforderung verwendet, sodass Sie dieses Problem beheben können, indem Sie eine Zugriffsstufe erstellen, die mit einer Anfragelizenz verknüpft ist.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden

Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, erhält er den folgenden Fehler:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problem

Das System weist dem neuen Benutzer keine Zugriffsebene zu.

Standardmäßig verwendet die automatische Bereitstellung den Lizenztyp Anforderung . Wenn keine Zugriffsebene mit einer Anfragelizenz vorhanden ist, kann das System dem Benutzer keine Zugriffsebene zuweisen.

## Zugriffsanforderungen

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Erstellen Sie eine einfache Zugriffsstufe mit einer Anfragelizenz:

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Zugriffsebenen]**.

1. Klicken Sie auf **[!UICONTROL Neue Zugriffsebene]**.
1. Geben Sie einen **[!UICONTROL Namen]** ein.
1. Wählen Sie im Dropdown-Menü **[!UICONTROL Lizenztyp]** die Option &quot;Anforderung&quot;aus.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

Nachdem Sie eine Zugriffsstufe mit einer Anforderungslizenz erstellt haben, lassen Sie den Benutzer sich mit seinen SSO-Anmeldeinformationen anmelden.


