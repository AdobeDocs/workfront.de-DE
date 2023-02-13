---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Gruppenadministratoren müssen einen höheren Zugriff haben als die von ihnen verwalteten
description: Wenn ein Gruppenadministrator über Berechtigungen in seiner Zugriffsstufe verfügt, die niedriger sind als die von ihm verwalteten, kann er keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Gruppenadministratoren müssen einen höheren Zugriff haben als die von ihnen verwalteten

Wenn ein Gruppenadministrator über Berechtigungen in seiner Zugriffsstufe verfügt, die niedriger sind als die von ihm verwalteten, kann er keine niedrigeren Zugriffsebenen anzeigen, ändern oder zuweisen.

## Problem

Wenn einem Gruppenadministrator eine geänderte Zugriffsstufe &quot;Planer&quot;mit Ansichtsberechtigungen für Teams zugewiesen wurde, bestimmten Benutzern jedoch die Zugriffsstufe &quot;Worker&quot;mit Bearbeitungsberechtigungen für Teams zugewiesen wurde, kann der Gruppenadministrator nicht mit der geänderten Zugriffsstufe &quot;Worker&quot;interagieren.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Diese Logik gilt auch für das Dropdown-Menü Einstellungen optimieren . Beide Zugriffsebenen können Zugriff auf &quot;Bearbeiten&quot;haben, aber die Einstellungen im Dropdown-Menü Einstellungen anpassen müssen für den Gruppenadministrator höher sein.
> ![](assets/fine-tune-your-settings.png)

## Lösung

Gruppenadministratoren müssen in allen Bereichen der Zugriffsebene über höhere Berechtigungen verfügen als die von ihnen verwalteten.