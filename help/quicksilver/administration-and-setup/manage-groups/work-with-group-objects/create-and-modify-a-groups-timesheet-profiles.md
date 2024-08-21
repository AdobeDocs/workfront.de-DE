---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Verwalten von Datenblatt-Profilen einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Timesheet-Profile anzeigen und bearbeiten, auf die die Administratoren der Gruppe oder einer ihrer Untergruppen Administratorzugriff haben.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Erstellen und Verwalten von Timesheet-Profilen einer Gruppe

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Timesheet-Profile anzeigen und bearbeiten, auf die die Administratoren der Gruppe oder einer ihrer Untergruppen Administratorzugriff haben.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Gruppenadministrator der Gruppe sein.</p>  <p>Sie müssen auch über Administratorzugriff auf Timesheets verfügen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p>  <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Erstellen und Bearbeiten von Profilen auf Gruppenebene

Sie können Timesheet-Profile für die Verwendung in einer von Ihnen verwalteten Gruppe erstellen und bearbeiten. Anweisungen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Zeitzeichenprofilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Löschen von Timesheet-Profilen auf Gruppenebene

Sie können von einer von Ihnen verwalteten Gruppe verwendete Zeitleistenprofile löschen. Eine Anleitung finden Sie unter [Löschen von Timesheet-Profilen](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Manuelles Generieren von Gruppen-Timesheets

Um Änderungen zu ermöglichen, die Sie an der Gruppierung von Timesheet-Profilen vorgenommen haben, um sie in aktuellen Gruppen-Timesheets widerzuspiegeln, müssen Sie zunächst die vorhandenen Timesheets löschen und dann manuell neue erstellen. Anweisungen finden Sie unter [Manuelles Generieren von Timesheets aus dem Bereich &quot;Timesheets und Stunden&quot;](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Manuelles Generieren von Timesheets](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Weitere Informationen zum Löschen von Gruppen-Timesheets finden Sie unter [Löschen von Timesheets in Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Profile auf Gruppenebene exportieren

{{step-1-to-setup}}

1. Klicken Sie auf **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe mit den zu exportierenden Timesheet-Profilen.
1. Klicken Sie auf **Timesheet-Profile**.
1. Klicken Sie auf **Exportieren** , um die Liste der Zeitleistenprofile für die Gruppe zu exportieren.
