---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen
description: Als Gruppenadministrator können Sie die Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem konfigurieren und sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen

Als Gruppenadministrator können Sie die Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem konfigurieren und sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.

Durch das Sperren einer Projekt-, Aufgaben- oder Problemvoreinstellung, die Sie auf der Ebene der Gruppe konfiguriert haben, stellen Sie sicher, dass alle Mitglieder Ihrer Gruppe und ihrer Untergruppen dieselbe Einstellung für diese Voreinstellung verwenden. Obwohl Sie eine Voreinstellung, die Sie für Ihre Gruppe sperren, weiterhin neu konfigurieren können, können Gruppenadministratoren sie nicht für Gruppen neu konfigurieren.

Umgekehrt ermöglicht das Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung Gruppenadministratoren mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für diese Untergruppen neu konfigurieren.

Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System sperren oder entsperren muss.

Informationen dazu, wie ein Workfront-Administrator eine Voreinstellung für alle Gruppen im System sperren oder entsperren kann, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Gruppenprojekt, -aufgabe oder -präferenz sperren oder entsperren

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe, in der Sie eine Projektvoreinstellung sperren oder entsperren möchten.
1. Klicken Sie im linken Bereich auf **Projektvoreinstellungen** oder **Voreinstellungen für Aufgaben und Probleme**.

1. Führen Sie auf der angezeigten Seite einen der folgenden Schritte aus, um eine Voreinstellung zu erhalten, die auf Systemebene entsperrt ist, oder für eine Gruppe über Ihrer Gruppe:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie. ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen unter Ihren Einstellungen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist. ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >Es ist wichtig, mit den Administratoren und Benutzern in Gruppen unter Ihnen zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Untergruppen unten übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration diejenigen, die von Gruppenadministratoren in niedrigeren Untergruppen vorgenommen wurden.

1. Klicken Sie auf **Speichern**.
