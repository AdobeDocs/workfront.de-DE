---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Verwalten der Arbeitszeittabellen-Profile einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Arbeitszeittabellen-Profile anzeigen und mit ihnen arbeiten, für die die Administratoren der Gruppe oder eine ihrer Untergruppen administrativen Zugriff haben.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Erstellen und Verwalten der Arbeitszeittabellen-Profile einer Gruppe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Arbeitszeittabellen-Profile anzeigen und mit ihnen arbeiten, für die die Administratoren der Gruppe oder eine ihrer Untergruppen administrativen Zugriff haben.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</p>
   <p>Sie müssen außerdem administrativen Zugriff auf Arbeitszeittabellen haben.</p></td>
  </tr>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen und Bearbeiten von Arbeitszeittabellen-Profilen auf Gruppenebene

Sie können Arbeitszeittabellen-Profile für die Verwendung in einer von Ihnen verwalteten Gruppe erstellen und bearbeiten. Anweisungen finden Sie [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Arbeitszeittabellen-Profile auf Gruppenebene löschen

Sie können Arbeitszeittabellen-Profile löschen, die von einer von Ihnen verwalteten Gruppe verwendet werden. Anweisungen finden Sie unter [Arbeitszeittabellen-Profile löschen](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Gruppen-Arbeitszeittabellen manuell generieren

Damit Änderungen, die Sie an Gruppen-Arbeitszeittabellen-Profilen vorgenommen haben, auch in aktuellen Gruppen-Arbeitszeittabellen übernommen werden, müssen Sie zunächst die vorhandenen Arbeitszeittabellen löschen und dann manuell neue Arbeitszeittabellen erstellen. Anweisungen finden Sie unter [Manuelles Generieren von Arbeitszeittabellen über den Bereich Arbeitszeittabellen und Stunden](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Manuelles Generieren von Arbeitszeittabellen](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Informationen zum Löschen von Gruppen-Arbeitszeittabellen finden Sie unter [Löschen von Arbeitszeittabellen in Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Arbeitszeittabellen-Profile auf Gruppenebene exportieren

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe mit den Arbeitszeittabellen-Profilen, die Sie exportieren möchten.
1. Klicken Sie **Arbeitszeittabellen-Profile**.
1. Klicken Sie **Exportieren**, um die Liste der Arbeitszeittabellen-Profile für die Gruppe zu exportieren.
