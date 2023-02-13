---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren
description: Gruppen in Ihrer Organisation benötigen möglicherweise eine andere Projektreferenz, die für ihre individuellen Workflows unterschiedlich konfiguriert ist. Sie können die Voreinstellung für alle Gruppen in der Organisation freigeben, damit sie sie selbst konfigurieren können.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise eine andere Projektreferenz, die für ihre individuellen Workflows unterschiedlich konfiguriert ist. Sie können die Voreinstellung für alle Gruppen in der Organisation freigeben, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt ist und der Gruppenadministrator sie ändert, erhalten die mit der Gruppe verknüpften Projekte die Konfiguration für diese Voreinstellung aus der Gruppeneinstellung und nicht aus der Einstellung auf Systemebene.

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Über gesperrte und entsperrte Voreinstellungen

Durch das Sperren der von Ihnen auf Systemebene konfigurierten Projekt-, Aufgaben- oder Problemvoreinstellungen wird sichergestellt, dass alle dieselbe Einstellung für diese Voreinstellung verwenden. Obwohl Sie eine Voreinstellung, die Sie sperren, weiterhin neu konfigurieren können, können Gruppenadministratoren sie nicht für ihre Gruppen neu konfigurieren.

Umgekehrt ermöglicht das Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung Gruppenadministratoren mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen neu konfigurieren.

Anweisungen zum Sperren oder Entsperren von Projekten, Aufgaben oder Problemeinstellungen auf Systemebene finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Nach [!DNL Workfront] Administrator entsperrt eine Voreinstellung auf Systemebene, kann jeder Gruppenadministrator sie konfigurieren und dann sperren, um sicherzustellen, dass alle Mitglieder ihrer Gruppe und der Untergruppen unten dieselbe Konfiguration verwenden. Dies entspricht der Fähigkeit, dass ein [!DNL Workfront] -Administrator muss eine Voreinstellung für alle Benutzer im System konfigurieren und sperren. Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Entsperren Sie eine Projektvoreinstellung, damit sie von Gruppen konfiguriert werden kann.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Projektvoreinstellungen]** Klicken Sie auf **[!UICONTROL Projekte]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie. ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

      >[!IMPORTANT]
      >
      >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Gruppen im System übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Einstellungen, die von Gruppenadministratoren vorgenommen wurden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
