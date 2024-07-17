---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Voreinstellung für Zeitblatt und Stunde einer Gruppe sperren oder entsperren
description: Wenn Sie Gruppenadministrator sind, können Sie die Voreinstellung für ein Zeitblatt und eine Stunde für Ihre Gruppe konfigurieren und sperren, nachdem ein Workfront-Administrator sie auf Systemebene entsperrt hat.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Voreinstellung für Zeitblatt und Stunde einer Gruppe sperren oder entsperren

Wenn Sie Gruppenadministrator sind, können Sie die Voreinstellung für ein Zeitblatt und eine Stunde für Ihre Gruppe konfigurieren und sperren, nachdem ein Workfront-Administrator sie auf Systemebene entsperrt hat.

Durch das Sperren einer Adobe Workfront-Voreinstellung wird sichergestellt, dass alle Mitglieder Ihrer Gruppe und ihrer Untergruppen dieselbe Einstellung für diese Voreinstellung verwenden. Obwohl Sie eine Voreinstellung, die Sie sperren, weiterhin neu konfigurieren können, können Gruppenadministratoren dies für niedrigere Untergruppen nicht tun.

Umgekehrt ermöglicht es das Entsperren einer Voreinstellung auf Gruppenebene den Administratoren der Untergruppe mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für diese Untergruppen neu konfigurieren.

Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System sperren oder entsperren muss.

Informationen dazu, wie ein Workfront-Administrator eine Zeitblatt- und Stundenvoreinstellung für alle Gruppen im System sperren oder entsperren kann, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen zum Konfigurieren eines Zeitplans und einer Stunde für eine Gruppe finden Sie unter [Konfigurieren der Voreinstellungen für das Zeitblatt und die Stunde für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* Die Konfiguration einer entsperrten Voreinstellung für eine Gruppe wirkt sich nicht auf diese Voreinstellung für Untergruppen unter der Gruppe aus.
>
>  Wenn jedoch eine neue Untergruppe erstellt wird, übernimmt sie die Voreinstellungen und den Status &quot;gesperrt&quot;oder &quot;entsperrt&quot;der Gruppe direkt darüber.
>
>* Wenn Sie eine Gruppe unter eine Gruppe verschieben, die über eine gesperrte Voreinstellung verfügt, erbt die verschobene Gruppe diese Voreinstellung und ist für die verschobene Gruppe gesperrt.
>* Wenn Sie eine Gruppe unter eine Gruppe verschieben, die über eine entsperrte Voreinstellung verfügt, wirkt sich diese Voreinstellung nicht auf die verschobene Gruppe aus.
>
>  Wenn die Voreinstellung in der verschobenen Gruppe zum Zeitpunkt des Verschiebevorgangs gesperrt ist, bleibt sie gesperrt. Der Gruppenadministrator kann sie jedoch jetzt entsperren, da sie für die übergeordnete Gruppe entsperrt ist.
>

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

## Voreinstellung für Zeitblatt und Stunde einer Gruppe sperren oder entsperren

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie &quot;Einrichtung&quot;> &quot;Zeitblatt und Stunden&quot;> &quot;Voreinstellungen&quot;aufrufen und dann im Feld oben auf der Seite nach dem Gruppennamen suchen.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe, deren Voreinstellung für Timesheets und Stunden gesperrt oder entsperrt werden soll.
1. Klicken Sie im linken Bereich auf **Voreinstellungen für Timesheets und Stunden**.

1. Führen Sie auf der angezeigten Seite einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen unterhalb Ihrer Voreinstellung Ihre Konfiguration verwenden, stellen Sie sicher, dass sie ![](assets/lock-toggle-button.png) gesperrt ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es ist wichtig, mit den Administratoren und Benutzern in Gruppen unter Ihnen zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Untergruppen unten übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration diejenigen, die von Gruppenadministratoren in niedrigeren Untergruppen vorgenommen wurden.

1. Klicken Sie auf **Speichern**.
