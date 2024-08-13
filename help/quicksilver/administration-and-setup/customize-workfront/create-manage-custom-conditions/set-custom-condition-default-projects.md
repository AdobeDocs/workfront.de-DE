---
title: Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wenn der Bedingungstyp eines Projekts auf Fortschrittsstatus anstelle von Manuell festgelegt ist, zeigt Adobe Workfront automatisch eine von drei integrierten Standardbedingungen für das Projekt (On Target, At Risk oder In Trouble) an, während es weitergeht, wie unter Übersicht über Projektbedingungen und Bedingungstyp beschrieben.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte

Wenn der Bedingungstyp eines Projekts auf Fortschrittsstatus anstelle von Manuell festgelegt ist, zeigt Adobe Workfront automatisch eine von drei integrierten Standardbedingungen für das Projekt (On Target, At Risk oder In Trouble) an, während es weitergeht, wie unter [Übersicht über Projektbedingungen und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md) erläutert.

![](assets/condition-in-project-header-nwe.png)

Sie können Ihre benutzerdefinierten Bedingungen als Standardbedingungen festlegen, anstatt diese drei integrierten Standardbedingungen zu verwenden. Sie können beispielsweise die Standardbedingung On Target ändern und in allen Projekten als Tracking Well anzeigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Legen Sie eine benutzerdefinierte Bedingung als Standardbedingung für alle Projekte fest:

{{step-1-to-setup}}

1. Klicken Sie auf **Projekteinstellungen** > **Bedingungen**.

1. Klicken Sie auf die Registerkarte **Projekt** .
1. Klicken Sie auf **Standardbedingungen festlegen**.
1. Klicken Sie im Dropdown-Menü neben der Standardbedingung, die Sie ändern möchten, auf die benutzerdefinierte Bedingung, die Sie stattdessen verwenden möchten.
1. Wiederholen Sie den vorherigen Schritt für alle anderen Standardbedingungen, die Sie ändern möchten.
1. Klicken Sie auf **Speichern**.

Informationen zum Festlegen einer benutzerdefinierten Bedingung als Standardbedingung für Aufgaben und Probleme finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Informationen zum Einrichten eines Projekts, sodass Benutzer seine Bedingung manuell aktualisieren können, finden Sie unter [Bedingung für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Weitere Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
