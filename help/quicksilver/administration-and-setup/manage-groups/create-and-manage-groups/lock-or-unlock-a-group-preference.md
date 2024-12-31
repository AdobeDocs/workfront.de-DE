---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Voreinstellungen zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen
description: Als Gruppenadministrator können Sie eine Projekt-, Aufgaben- oder Problemeinstellung konfigurieren und dann sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Voreinstellungen für Projekte, Aufgaben oder Probleme für Untergruppen sperren oder entsperren

Als Gruppenadministrator können Sie eine Projekt-, Aufgaben- oder Problemeinstellung konfigurieren und dann sperren, wenn ein Workfront-Administrator sie auf Systemebene entsperrt hat.

Durch das Sperren einer Projekt-, Aufgaben- oder Problem-Voreinstellung, die Sie auf der Ebene konfiguriert haben, wird sichergestellt, dass alle Personen in Ihrer Gruppe und in ihren Untergruppen dieselbe Einstellung für diese Voreinstellung verwenden. Sie können eine Voreinstellung, die Sie für Ihre Gruppe sperren, zwar neu konfigurieren, Gruppenadministratoren können sie jedoch nicht für Gruppen neu konfigurieren.

Umgekehrt können Gruppenadministratoren durch das Entsperren von Projekt-, Aufgaben- oder Problemeinstellungen flexibler die Art und Weise verwalten, wie ihre Gruppen mit diesen Elementen arbeiten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für diese Untergruppen neu konfigurieren.

Dies geschieht parallel zu der Fähigkeit, die ein Workfront-Administrator hat, eine Voreinstellung für alle im System zu sperren oder zu entsperren.

Informationen dazu, wie Workfront-Admins eine Voreinstellung für alle Gruppen im System sperren oder entsperren können, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voreinstellungen für Gruppenprojekte, Aufgaben oder Probleme sperren oder entsperren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe, für die Sie eine Projektvoreinstellung sperren oder entsperren möchten.
1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** oder **Voreinstellungen für Aufgaben und Probleme**.

1. Führen Sie auf der angezeigten Seite eine der folgenden Aktionen für eine Voreinstellung aus, die auf Systemebene entsperrt wurde, oder für eine Gruppe oberhalb Ihrer Gruppe:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie diese ![](assets/unlock-toggle-button.png).
   * Wenn alle Gruppen unter Ihnen Ihre Konfiguration für eine Voreinstellung verwenden sollen, stellen Sie sicher, dass sie ![](assets/lock-toggle-button.png) gesperrt ist.

     >[!IMPORTANT]
     >
     >Es ist wichtig, mit den Administratoren und Benutzern in den Gruppen unter Ihnen zu kommunizieren, um sicherzustellen, dass alle Anforderungen auf die Weise berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird ihre Konfiguration für sie von allen Untergruppen unter übernommen. Und wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Gruppen-Administratoren in niedrigeren Untergruppen, die möglicherweise vorgenommen haben.

1. Klicken Sie auf **Speichern**.
