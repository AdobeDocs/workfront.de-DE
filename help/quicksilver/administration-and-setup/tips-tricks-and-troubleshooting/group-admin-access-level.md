---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gruppenadministratoren müssen über einen höheren Zugriff verfügen als die von ihnen verwalteten
description: Wenn ein Gruppenadministrator über Berechtigungen in der Zugriffsstufe verfügt, die niedriger sind als die von ihm verwalteten, kann er keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Gruppenadministratoren müssen einen höheren Zugriff haben als die von ihnen verwalteten

Wenn ein Gruppenadministrator über Berechtigungen in der Zugriffsstufe verfügt, die niedriger sind als die von ihm verwalteten, kann er keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.

## Problem

Wenn einem Gruppenadministrator eine geänderte Zugriffsstufe &quot;Planer&quot;mit Ansichtsberechtigungen für Teams zugewiesen wurde, bestimmten Benutzern jedoch die Zugriffsstufe &quot;Worker&quot;mit Bearbeitungsberechtigungen für Teams zugewiesen wurde, kann der Gruppenadministrator nicht mit der geänderten Zugriffsstufe &quot;Worker&quot;interagieren.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Diese Logik gilt auch für das Dropdown-Menü Einstellungen optimieren . Beide Zugriffsebenen können Zugriff auf &quot;Bearbeiten&quot;haben, aber die Einstellungen im Dropdown-Menü Einstellungen anpassen müssen für den Gruppenadministrator höher sein.
> ![](assets/fine-tune-your-settings.png)

## Lösung

Gruppenadministratoren müssen in allen Bereichen der Zugriffsebene über höhere Berechtigungen verfügen als die von ihnen verwalteten.
