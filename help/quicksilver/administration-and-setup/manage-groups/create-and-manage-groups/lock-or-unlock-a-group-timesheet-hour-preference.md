---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Arbeitszeittabelle und Stundeneinstellungen einer Gruppe sperren oder entsperren
description: Wenn Sie Gruppenadministrator sind, können Sie eine Arbeitszeittabelle und Stundeneinstellungen für Ihre Gruppe konfigurieren und dann sperren, nachdem ein Workfront-Administrator diese auf Systemebene entsperrt hat.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Arbeitszeittabelle und Stundeneinstellungen einer Gruppe sperren oder entsperren

Wenn Sie Gruppenadministrator sind, können Sie eine Arbeitszeittabelle und Stundeneinstellungen für Ihre Gruppe konfigurieren und dann sperren, nachdem ein Workfront-Administrator diese auf Systemebene entsperrt hat.

Das Sperren einer Adobe Workfront-Voreinstellung stellt sicher, dass alle Personen in Ihrer Gruppe und ihren Untergruppen dieselbe Einstellung für diese Voreinstellung verwenden. Sie können eine Voreinstellung zwar immer noch neu konfigurieren, die Sie sperren, Gruppenadministratoren können dies jedoch nicht für untere Untergruppen tun.

Umgekehrt ermöglicht das Entsperren einer Voreinstellung auf Gruppenebene Untergruppenadministratoren mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für diese Untergruppen neu konfigurieren.

Dies geschieht parallel zu der Fähigkeit, die ein Workfront-Administrator hat, eine Voreinstellung für alle im System zu sperren oder zu entsperren.

Informationen dazu, wie ein Workfront-Administrator eine Arbeitszeittabelle und Stundenvoreinstellungen für alle Gruppen im System sperren oder entsperren kann, finden Sie unter [Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen zum Konfigurieren einer Arbeitszeittabelle und der Stundeneinstellungen für eine Gruppe finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Das Konfigurieren einer entsperrten Einstellung für eine Gruppe wirkt sich nicht auf diese Einstellung für Untergruppen unter der Gruppe aus.
>
>  Wenn jedoch eine neue Untergruppe erstellt wird, erbt sie die Voreinstellungen und den gesperrten oder entsperrten Status der Gruppe direkt darüber.
>
>* Wenn Sie eine Gruppe in eine Gruppe verschieben, die über eine gesperrte Voreinstellung verfügt, übernimmt die verschobene Gruppe diese Voreinstellung und wird für die verschobene Gruppe gesperrt.
>* Wenn Sie eine Gruppe in eine Gruppe verschieben, die über eine entsperrte Einstellung verfügt, ist die verschobene Gruppe von dieser Einstellung nicht betroffen.
>
>  Wenn die Voreinstellung in der verschobenen Gruppe zum Zeitpunkt des Verschiebevorgangs gesperrt ist, bleibt sie gesperrt, aber der Gruppenadministrator kann sie jetzt entsperren, da sie für die übergeordnete Gruppe entsperrt ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabelle und Stundeneinstellungen einer Gruppe sperren oder entsperren

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einstellungen > Arbeitszeittabelle und Stunden > Voreinstellungen wechseln und dann im Feld oben auf der Seite nach dem Namen der Gruppe suchen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe, für die Sie eine Arbeitszeittabelle und die Stundeneinstellungen sperren oder entsperren möchten.
1. Klicken Sie im linken Bedienfeld auf **Arbeitszeittabellen und**).

1. Führen Sie auf der angezeigten Seite einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![Umschalter Entsperren](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen unter Ihnen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist ![Umschalter sperren](assets/lock-toggle-button.png) (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es ist wichtig, mit den Administratoren und Benutzern in den Gruppen unter Ihnen zu kommunizieren, um sicherzustellen, dass alle Anforderungen auf die Weise berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird ihre Konfiguration für sie von allen Untergruppen unter übernommen. Und wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Gruppen-Administratoren in niedrigeren Untergruppen, die möglicherweise vorgenommen haben.

1. Klicken Sie auf **Speichern**.
