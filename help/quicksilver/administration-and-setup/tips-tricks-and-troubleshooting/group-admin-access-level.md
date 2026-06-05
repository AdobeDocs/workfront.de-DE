---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gruppenadmins müssen über höhere Zugriffsrechte verfügen als die von ihnen verwalteten
description: Wenn ein Gruppenadministrator bzw. eine Gruppenadministratorin in niedrigere Zugriffsberechtigungen hat als die, die er bzw. sie verwaltet, kann er bzw. sie keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
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
source-wordcount: 157
ht-degree: 7%

---

# Gruppenadmins müssen über höhere Zugriffsrechte verfügen als die von ihnen verwalteten

Wenn ein Gruppenadministrator bzw. eine Gruppenadministratorin in niedrigere Zugriffsberechtigungen hat als die, die er bzw. sie verwaltet, kann er bzw. sie keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.

## Problem

Wenn einem Gruppenadministrator die Zugriffsebene Geänderter Planer mit den Anzeigeberechtigungen für Teams zugewiesen ist, aber bestimmten Benutzern die Zugriffsebene Arbeiter mit den Bearbeitungsberechtigungen für Teams zugewiesen ist, kann der Gruppenadministrator nicht mit der Zugriffsebene Geänderter Arbeiter interagieren.

![Gruppenadministrator hat Zugriff geändert](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Diese Logik gilt auch für das Dropdown-Menü Einstellungen optimieren . Beide Zugriffsebenen können Bearbeitungszugriff haben, aber die Einstellungen im Dropdown-Menü Einstellungen optimieren müssen für den Gruppenadministrator höher sein.
> ![Optimieren Sie Ihre Einstellungen](assets/fine-tune-your-settings.png)

## Lösung

Gruppenadmins müssen in allen Bereichen der Zugriffsebene über höhere Berechtigungen verfügen als die von ihnen verwalteten.
