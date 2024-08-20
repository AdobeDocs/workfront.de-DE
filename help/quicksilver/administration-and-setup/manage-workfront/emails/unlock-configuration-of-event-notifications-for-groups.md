---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen
description: Wenn Sie Adobe Workfront-Administrator sind, können Sie Gruppenadministratoren die Möglichkeit erschließen oder erneut sperren, eine Ereignisbenachrichtigung für von ihnen verwaltete Gruppen der obersten Ebene zu konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen

Wenn Sie Adobe Workfront-Administrator sind, können Sie Gruppenadministratoren die Möglichkeit erschließen oder erneut sperren, eine Ereignisbenachrichtigung für von ihnen verwaltete Gruppen der obersten Ebene zu konfigurieren. Die Konfiguration einer Ereignisbenachrichtigung besteht darin, sie zu aktivieren oder zu deaktivieren.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Wenn ein Administrator eine Ereignisbenachrichtigung für eine Gruppe konfiguriert, wirkt sich die Konfiguration auf Benutzer aus, für die diese Gruppe oder eine ihrer Untergruppen ihre Startseite ist. In ihren Benutzerprofilen sehen diese Benutzer die Ereignisbenachrichtigungen, die für ihre Startseite aktiviert sind, anstelle der systemweit aktivierten Ereignisbenachrichtigungen. Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Ein Workfront-Administrator kann die Konfiguration für eine Ereignisbenachrichtigung sowohl in Adobe Workfront Classic als auch im neuen Adobe Workfront-Erlebnis entsperren und erneut sperren. Ein Gruppenadministrator kann diese Ereignisbenachrichtigung für eine Gruppe jedoch nur im neuen Adobe Workfront-Erlebnis konfigurieren. Gruppenadministratoren, die Adobe Workfront Classic verwenden, können zum neuen Adobe Workfront-Erlebnis wechseln, um entsperrte Ereignisbenachrichtigungen für eine Gruppe zu konfigurieren, und dann zurück zu Adobe Workfront Classic wechseln, um die Änderungen zu sehen.
>* Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen auf Gruppenebene von den übergeordneten Gruppen, die über ihnen stehen.
>

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
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Die Möglichkeit, eine Ereignisbenachrichtigung zu konfigurieren, entsperren oder erneut sperren

>[!IMPORTANT]
>
>Wenn Sie eine Benachrichtigung erneut sperren, erben alle Gruppen im System die Benachrichtigung genau so, wie Sie sie festgelegt haben. Dadurch werden alle Änderungen überschrieben, die Gruppenadministratoren möglicherweise für ihre Gruppen vorgenommen haben. Daher ist es empfehlenswert, sie zuerst zu konsultieren.

{{step-1-to-setup}}

1. Klicken Sie auf **E-Mail** > **Benachrichtigungen**.

1. Stellen Sie sicher, dass die Registerkarte **Ereignisbenachrichtigungen** geöffnet ist.
1. Klicken Sie auf das Symbol rechts neben der Benachrichtigung, um sie zur gesperrten Position ![Sperrsymbol](assets/lock-toggle-button.png) oder entsperrten ![Entsperrungssymbol](assets/unlock-toggle-button.png) zu wechseln.

   Oder

   Wenn Sie mehrere Benachrichtigungen gleichzeitig entsperren oder sperren möchten, wählen Sie sie aus und klicken Sie dann auf die Schaltfläche Entsperren ![Entsperren](assets/unlock-icon-toolbar.png) oder Sperren ![Sperrsymbol](assets/lock-icon-locked-qs.png) , die in der Symbolleiste über der Liste angezeigt wird.

1. Klicken Sie auf **Speichern**.
1. (Optional) Wenn Sie die Ereignisbenachrichtigung für eine Gruppe der obersten Ebene konfigurieren möchten, anstatt diese Aufgabe dem Gruppenadministrator zu überlassen, können Sie einen der folgenden Schritte ausführen:

   * Löschen Sie **Systemereignisbenachrichtigungen** im Suchfeld über der Benachrichtigungsliste, suchen Sie nach dem Namen der Gruppe der obersten Ebene, um deren Benachrichtigungen aufzulisten, und wählen Sie ihn aus. Aktivieren oder deaktivieren Sie dann die entsperrten Benachrichtigungen in der angezeigten Liste.
   * Klicken Sie im linken Menü auf **Gruppen** und dann auf den Namen der Gruppe der obersten Ebene. Klicken Sie im linken Bereich auf **Ereignisbenachrichtigungen** und konfigurieren Sie dann die Benachrichtigung zum entsperrten Ereignis, wie unter [Ereignisbenachrichtigungen für eine Gruppe anzeigen und konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md) beschrieben.
