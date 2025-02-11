---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Projekteinstellungen für alle Gruppen im System sperren oder entsperren
description: Gruppen in Ihrer Organisation benötigen möglicherweise eine Projektvoreinstellung, die für ihre spezifischen Workflows anders konfiguriert ist. Sie können die Voreinstellung für alle Gruppen im gesamten Unternehmen entsperren, damit sie sie selbst konfigurieren können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Projekteinstellungen für alle Gruppen im System sperren oder entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise eine Projektvoreinstellung, die für ihre spezifischen Workflows anders konfiguriert ist. Sie können die Voreinstellung für alle Gruppen im gesamten Unternehmen entsperren, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt wird und der Gruppenadministrator sie ändert, erhalten die mit der Gruppe verknüpften Projekte die Konfiguration für diese Voreinstellung über die Einstellung auf Gruppenebene anstelle über die Einstellung auf Systemebene.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td>
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über gesperrte und entsperrte Voreinstellungen

Durch das Sperren eines Projekts, einer Aufgabe oder eines Problems, das bzw. das Sie auf Systemebene konfiguriert haben, wird sichergestellt, dass für alle Benutzer dieselbe Einstellung verwendet wird. Sie können eine Voreinstellung zwar immer noch neu konfigurieren, die Sie sperren, Gruppenadministratoren können sie jedoch nicht für ihre Gruppen neu konfigurieren.

Umgekehrt können Gruppenadministratoren durch das Entsperren von Projekt-, Aufgaben- oder Problemeinstellungen flexibler die Art und Weise verwalten, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen neu konfigurieren.

Wenn ein Feld keinen Umschalter zum Sperren/Entsperren hat, kann es von Gruppenadministratoren nicht entsperrt werden, um Einstellungen auf Gruppenebene zu konfigurieren. Die Konfiguration ist nur auf Systemebene verfügbar.

Anweisungen zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung auf Systemebene finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] eine Voreinstellung auf Systemebene entsperrt hat, kann sie jeder Gruppenadministrator konfigurieren und dann sperren, um sicherzustellen, dass alle Benutzer in seiner Gruppe und den Untergruppen unten dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein [!DNL Workfront]-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Sperren oder Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Projektvoreinstellungen entsperren, damit Gruppen sie konfigurieren können

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** und dann auf **[!UICONTROL Projekte]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![Umschalter Entsperren](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen in der Art und Weise berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie ihn sperren, wird die entsprechende Konfiguration von allen Gruppen im System übernommen. Und wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Konfigurationen, die Gruppenadministratoren möglicherweise vorgenommen haben.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
