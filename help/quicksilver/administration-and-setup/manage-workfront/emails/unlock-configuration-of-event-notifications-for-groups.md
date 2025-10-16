---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren
description: Wenn Sie Adobe Workfront-Administrator sind, können Sie die Möglichkeit für Gruppenadministratoren, eine Ereignisbenachrichtigung für von ihnen verwaltete Gruppen der obersten Ebene zu konfigurieren, entsperren oder erneut sperren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 1%

---

# Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren

Wenn Sie Adobe Workfront-Administrator sind, können Sie die Möglichkeit für Gruppenadministratoren, eine Ereignisbenachrichtigung für von ihnen verwaltete Gruppen der obersten Ebene zu konfigurieren, entsperren oder erneut sperren. Bei der Konfiguration einer Ereignisbenachrichtigung wird diese aktiviert oder deaktiviert.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Wenn Admins eine Ereignisbenachrichtigung für eine Gruppe konfigurieren, wirkt sich die Konfiguration auf Benutzende aus, für die diese Gruppe oder eine ihrer Untergruppen ihre Hauptgruppe ist. In ihren Benutzerprofilen sehen diese Benutzer die Ereignisbenachrichtigungen, die für ihre Hauptgruppe aktiviert sind, anstelle der Ereignisbenachrichtigungen, die systemweit aktiviert sind. Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Ein Workfront-Administrator kann die Konfiguration für eine Ereignisbenachrichtigung sowohl in Adobe Workfront Classic als auch in der neuen Adobe Workfront-Version entsperren und erneut sperren. Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann diese Ereignisbenachrichtigung jedoch nur in der neuen Adobe Workfront-Version für eine Gruppe konfigurieren. Gruppenadministratoren, die Adobe Workfront Classic verwenden, können zum neuen Adobe Workfront-Erlebnis wechseln, um entsperrte Ereignisbenachrichtigungen für eine Gruppe zu konfigurieren, und dann zurück zu Adobe Workfront Classic wechseln, um die Änderungen zu sehen.
>* Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen auf Gruppenebene von den darüber liegenden Gruppen der obersten Ebene.
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Die Möglichkeit zum Konfigurieren einer Ereignisbenachrichtigung entsperren oder erneut sperren

>[!IMPORTANT]
>
>Wenn Sie eine Benachrichtigung erneut sperren, erben alle Gruppen im System die Benachrichtigung genau so, wie Sie sie festgelegt haben. Dadurch werden alle Änderungen überschrieben, die Gruppenadministratoren möglicherweise für ihre Gruppen vorgenommen haben. Daher empfiehlt es sich, sich zuerst mit ihnen zu beraten.

{{step-1-to-setup}}

1. Klicken Sie auf **E** > **Benachrichtigungen**.

1. Stellen Sie sicher **dass die Registerkarte** Ereignisbenachrichtigungen“ geöffnet ist.
1. Klicken Sie auf das Symbol rechts neben der Benachrichtigung, um es auf die Position Gesperrtes ![Sperrsymbol](assets/lock-toggle-button.png) oder Entsperrtes ![Entsperrsymbol](assets/unlock-toggle-button.png) zu ändern.

   Oder

   Wenn Sie mehrere Benachrichtigungen gleichzeitig entsperren oder sperren möchten, wählen Sie diese aus und klicken Sie dann auf die Schaltfläche Entsperren ![Entsperrsymbol](assets/unlock-icon-toolbar.png) oder Sperrsymbol ![Sperrsymbol](assets/lock-icon-locked-qs.png), die in der Symbolleiste über der Liste angezeigt wird.

1. Klicken Sie auf **Speichern**.
1. (Optional) Wenn Sie die Ereignisbenachrichtigung für eine Gruppe der obersten Ebene konfigurieren möchten, anstatt diese Aufgabe dem Gruppenadministrator zu überlassen, haben Sie folgende Möglichkeiten:

   * Löschen Sie **Systemereignis** Benachrichtigungen) im Suchfeld über der Benachrichtigungsliste, suchen Sie nach dem Namen der Gruppe der obersten Ebene, um deren Benachrichtigungen aufzulisten, und aktivieren oder deaktivieren Sie dann die entsperrten Benachrichtigungen in der angezeigten Liste.
   * Klicken **im linken** auf „Gruppen“ und dann auf den Namen der Gruppe der obersten Ebene. Klicken Sie **linken Bereich auf** Ereignisbenachrichtigungen“ und konfigurieren Sie dann die entsperrte Ereignisbenachrichtigung, wie in [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe“ ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
