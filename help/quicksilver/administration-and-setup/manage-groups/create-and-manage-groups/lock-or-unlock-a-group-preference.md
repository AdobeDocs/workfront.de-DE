---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Sperren oder Entsperren von Projekten, Aufgaben oder Problemeinstellungen für Untergruppen
description: Als Gruppenadministrator können Sie die Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem konfigurieren und sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen

Als Gruppenadministrator können Sie die Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem konfigurieren und sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.

Durch das Sperren einer Projekt-, Aufgaben- oder Problemvoreinstellung, die Sie auf der Ebene der Gruppe konfiguriert haben, stellen Sie sicher, dass alle Mitglieder Ihrer Gruppe und ihrer Untergruppen dieselbe Einstellung für diese Voreinstellung verwenden. Obwohl Sie eine Voreinstellung, die Sie für Ihre Gruppe sperren, weiterhin neu konfigurieren können, können Gruppenadministratoren sie nicht für Gruppen neu konfigurieren.

Umgekehrt ermöglicht das Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung Gruppenadministratoren mehr Flexibilität bei der Verwaltung der Art und Weise, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für diese Untergruppen neu konfigurieren.

Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System sperren oder entsperren muss.

Informationen dazu, wie ein Workfront-Administrator eine Voreinstellung für alle Gruppen im System sperren oder entsperren kann, finden Sie unter [Sperren oder Entsperren von Projektanforderungen für alle Gruppen im System](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppenprojekt, -aufgabe oder -präferenz sperren oder entsperren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe, in der Sie eine Projektvoreinstellung sperren oder entsperren möchten.
1. Klicken Sie im linken Bereich auf **Projekteinstellungen** oder **Voreinstellungen für Aufgaben und Probleme**.

1. Führen Sie auf der angezeigten Seite einen der folgenden Schritte aus, um eine Voreinstellung zu erhalten, die auf Systemebene entsperrt ist, oder für eine Gruppe über Ihrer Gruppe:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen unter Ihren Einstellungen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie ![](assets/lock-toggle-button.png) gesperrt ist.

     >[!IMPORTANT]
     >
     >Es ist wichtig, mit den Administratoren und Benutzern in Gruppen unter Ihnen zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Untergruppen unten übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration diejenigen, die von Gruppenadministratoren in niedrigeren Untergruppen vorgenommen wurden.

1. Klicken Sie auf **Speichern**.
