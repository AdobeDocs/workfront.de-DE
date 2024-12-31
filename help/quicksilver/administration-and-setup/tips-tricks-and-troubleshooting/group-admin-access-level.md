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
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Gruppenadmins müssen über höhere Zugriffsrechte verfügen als die von ihnen verwalteten

Wenn ein Gruppenadministrator bzw. eine Gruppenadministratorin in niedrigere Zugriffsberechtigungen hat als die, die er bzw. sie verwaltet, kann er bzw. sie keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.

## Problem

Wenn einem Gruppenadministrator die Zugriffsebene Geänderter Planer mit den Anzeigeberechtigungen für Teams zugewiesen ist, aber bestimmten Benutzern die Zugriffsebene Arbeiter mit den Bearbeitungsberechtigungen für Teams zugewiesen ist, kann der Gruppenadministrator nicht mit der Zugriffsebene Geänderter Arbeiter interagieren.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Diese Logik gilt auch für das Dropdown-Menü Einstellungen optimieren . Beide Zugriffsebenen können Bearbeitungszugriff haben, aber die Einstellungen im Dropdown-Menü Einstellungen optimieren müssen für den Gruppenadministrator höher sein.
> ![](assets/fine-tune-your-settings.png)

## Lösung

Gruppenadmins müssen in allen Bereichen der Zugriffsebene über höhere Berechtigungen verfügen als die von ihnen verwalteten.
