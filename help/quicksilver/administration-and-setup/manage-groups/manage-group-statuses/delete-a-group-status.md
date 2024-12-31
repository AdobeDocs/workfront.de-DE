---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Gruppenstatus löschen
description: Als Gruppenadministrator können Sie einen Status für eine von Ihnen verwaltete Gruppe löschen, wenn diese nicht als erforderlicher oder gesperrter Status auf Systemebene oder für eine höhere Gruppe in der Hierarchie konfiguriert ist.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Gruppenstatus löschen

Als Gruppenadministrator können Sie einen Status für eine von Ihnen verwaltete Gruppe löschen, wenn diese nicht als erforderlicher oder gesperrter Status auf Systemebene oder für eine höhere Gruppe in der Hierarchie konfiguriert ist.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>Folgendes kann nicht gelöscht werden:
>
>* Der integrierte Status „Planung“, „Aktuell“ und „Abgeschlossen“. Sie können ihre Namen aktualisieren, ihre Farben bearbeiten und sie sperren oder entsperren, aber sie können nicht gelöscht werden.
>* Status, die sich für mindestens ein mit der Gruppe oder einer ihrer Untergruppen verknüpftes Objekt in einem ausstehenden Genehmigungsstatus befinden.

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

## Gruppenstatus löschen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen**.
1. Klicken Sie auf den Namen der Gruppe der obersten Ebene.
1. Klicken Sie im linken Bedienfeld auf **Status**.
1. Bewegen Sie in der angezeigten Statusliste den Mauszeiger über den Status, den Sie löschen möchten, und klicken Sie dann auf **Löschen**, wenn er ganz rechts angezeigt wird.

   ![](assets/hover-click-delete.jpg)

1. Wählen Sie in dem angezeigten Feld einen Status aus, um einen Ersatzstatus für Objekte (Projekte, Aufgaben, Probleme und Genehmigungsprozesse) festzulegen, die den Status verwendet haben, den Sie löschen möchten.

   Es sind nur Status verfügbar, die dem Status entsprechen, den Sie löschen möchten. Wenn Sie beispielsweise einen Status löschen, der dem aktuellen entspricht, können Sie nur Status sehen, die dem aktuellen entsprechen.

   Außerdem hängen die angezeigten Status davon ab, ob der Status, den Sie löschen möchten, entsperrt oder gesperrt ist:

   * **Wenn er entsperrt ist**: Nicht ausgeblendete, gesperrte und entsperrte Status sind verfügbar.

     Neben den Status, die für die Untergruppe erstellt wurden, sind auch Status enthalten, die von Gruppen der Systemebene und der oberen Ebene übernommen wurden.

   * **Wenn es gesperrt ist**: Eine der folgenden Bedingungen ist erfüllt:

      * Wenn andere gesperrte, nicht ausgeblendete Status vorhanden sind, sind nur diese verfügbar.
      * Wenn es keinen gesperrten, nicht ausgeblendeten Status gibt, ist der standardmäßige Workfront-Status verfügbar, auch wenn er ausgeblendet oder entsperrt ist.

        Informationen zu den standardmäßigen Workfront-Status finden Sie unter [Zugriff auf die Liste der Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Zugriff auf die Liste der Systemaufgabenstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) und die Informationen zu den vier erforderlichen Problemstatus in [Zugriff auf die Liste der Systemanfragestatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Klicken Sie **Status löschen**.

   Wenn der gelöschte Status der Standardstatus für diesen Typ in der Gruppe war, wird der Ersatzstatus ersetzt.

   Wenn der gelöschte Status in den Projektvoreinstellungen als standardmäßiger Projektstatus festgelegt wurde, ist die Voreinstellung jetzt auf den Ersatzstatus festgelegt.

## Wenn eine Gruppe gelöscht wird

Wenn eine Gruppe gelöscht und durch eine andere Gruppe ersetzt wird, werden alle eindeutigen Status der gelöschten Gruppe zu den Status der Ersatzgruppe hinzugefügt. Weitere Informationen finden Sie unter [Benutzerdefinierte Status in einer Gruppe, die verschoben oder gelöscht wird](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
