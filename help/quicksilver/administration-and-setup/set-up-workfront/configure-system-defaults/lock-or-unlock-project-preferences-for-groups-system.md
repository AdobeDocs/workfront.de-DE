---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Projekteinstellungen für alle Gruppen im System sperren oder entsperren
description: Gruppen in Ihrer Organisation benötigen möglicherweise eine andere Projektreferenz, die für ihre individuellen Workflows unterschiedlich konfiguriert ist. Sie können die Voreinstellung für alle Gruppen in der Organisation freigeben, damit sie sie selbst konfigurieren können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise eine andere Projektreferenz, die für ihre individuellen Workflows unterschiedlich konfiguriert ist. Sie können die Voreinstellung für alle Gruppen in der Organisation freigeben, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt ist und der Gruppenadministrator sie ändert, erhalten die mit der Gruppe verknüpften Projekte die Konfiguration für diese Voreinstellung aus der Gruppeneinstellung und nicht aus der Einstellung auf Systemebene.

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
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td>
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über gesperrte und entsperrte Voreinstellungen

Durch das Sperren der von Ihnen auf Systemebene konfigurierten Projekt-, Aufgaben- oder Problemvoreinstellungen wird sichergestellt, dass alle dieselbe Einstellung für diese Voreinstellung verwenden. Obwohl Sie eine Voreinstellung, die Sie sperren, weiterhin neu konfigurieren können, können Gruppenadministratoren sie nicht für ihre Gruppen neu konfigurieren.

Umgekehrt ermöglicht das Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung Gruppenadministratoren mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen neu konfigurieren.

Wenn für ein Feld kein Umschalter zum Sperren/Entsperren vorhanden ist, kann es für Gruppenadministratoren nicht entsperrt werden, um Einstellungen auf Gruppenebene zu konfigurieren. Die Konfiguration ist nur auf Systemebene verfügbar.

Anweisungen zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung auf Systemebene finden Sie unter [Konfigurieren von systemweiten Aufgaben und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] -Administrator eine Voreinstellung auf Systemebene entsperrt hat, kann jeder Gruppenadministrator sie konfigurieren und sie dann sperren, um sicherzustellen, dass alle Mitglieder ihrer Gruppe und der unten stehenden Untergruppen dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein [!DNL Workfront] -Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Konfigurieren von Projekteigenschaften für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Sperren oder Entsperren von Projekten, Aufgaben oder Problemeinstellungen für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Entsperren Sie eine Projektvoreinstellung, damit sie von Gruppen konfiguriert werden kann.

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** und dann auf **[!UICONTROL Projekte]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Gruppen im System übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Einstellungen, die von Gruppenadministratoren vorgenommen wurden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
