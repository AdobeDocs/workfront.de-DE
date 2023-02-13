---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden."
description: Wenn ein automatisch bereitgestellter Benutzer versucht, sich zum ersten Mal anzumelden, und einen Fehler erhält, der besagt, dass das System ihm keine Zugriffsstufe zuweist, kann dies daran liegen, dass Ihrem System die mit der Anfragelizenz verknüpften Zugriffsebenen fehlen. Bei der automatischen Bereitstellung wird der Lizenztyp Anforderung verwendet, sodass Sie dieses Problem beheben können, indem Sie eine Zugriffsstufe erstellen, die mit einer Anfragelizenz verknüpft ist.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Fehler: Automatisch bereitgestellter Benutzer kann sich nicht anmelden

Wenn ein automatisch bereitgestellter Benutzer zum ersten Mal versucht, sich anzumelden, erhält er den folgenden Fehler:

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
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Erstellen Sie eine einfache Zugriffsstufe mit einer Anfragelizenz:

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Zugriffsebenen]**.

1. Klicken **[!UICONTROL Neue Zugriffsebene]**.
1. Geben Sie einen **[!UICONTROL Name]**.
1. Im **[!UICONTROL Lizenztyp]** im Dropdown-Menü die Option Anforderung auswählen.
1. Klicken **[!UICONTROL Änderungen speichern]**.

Nachdem Sie eine Zugriffsstufe mit einer Anforderungslizenz erstellt haben, lassen Sie den Benutzer sich mit seinen SSO-Anmeldeinformationen anmelden.
