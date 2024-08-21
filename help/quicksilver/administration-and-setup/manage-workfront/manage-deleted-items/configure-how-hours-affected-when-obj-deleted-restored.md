---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Auswirkungen auf Stunden konfigurieren, wenn ein Objekt gelöscht und wiederhergestellt wird
description: Sie können konfigurieren, was passiert, wenn ein Benutzer ein Projekt, eine Aufgabe oder ein Problem löscht, gegen das die Stunden protokolliert werden. Die gewählte Option bestimmt auch, was mit den Stunden geschieht, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter Gelöschte Elemente wiederherstellen .)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Auswirkungen auf die Stunden konfigurieren, in denen ein Objekt gelöscht und wiederhergestellt wird

Sie können konfigurieren, was passiert, wenn ein Benutzer ein Projekt, eine Aufgabe oder ein Problem löscht, gegen das die Stunden protokolliert werden. Die gewählte Option bestimmt auch, was mit den Stunden geschieht, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Konfigurieren der Verwaltung von Stunden beim Löschen und Wiederherstellen eines Elements

{{step-1-to-setup}}

1. Erweitern Sie **Timesheets und Stunden** und klicken Sie dann auf **Voreinstellungen**.

1. Suchen Sie den Abschnitt **Voreinstellungen für Projekt-, Aufgaben- oder Problemlöschungen** .
1. (Bedingt) Um zu konfigurieren, wie Stunden beim Löschen eines Projekts verwaltet werden, wählen Sie eine der folgenden Optionen im Abschnitt **Beim Löschen von Projekten** aus:

   * Behalten Sie bereits zu Timesheets hinzugefügte protokollierte Stunden als allgemeine Stunden bei (wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, bleiben die Stunden auf dem Timesheet).\
     Diese Option ist standardmäßig ausgewählt.
   * Löschen Sie alle protokollierten Stunden (wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, werden die protokollierten Stunden im Projekt wiederhergestellt).

1. (Bedingt) Um zu konfigurieren, wie Stunden beim Löschen einer Aufgabe oder eines Problems verwaltet werden, wählen Sie eine der folgenden Optionen im Abschnitt **Beim Löschen von Aufgaben oder Problemen** aus:

   * Verschieben Sie die protokollierten Stunden in das Projekt, in dem sich die Aufgabe oder das Problem befindet (wenn diese Aufgabe oder dieses Problem zu einem späteren Zeitpunkt wiederhergestellt wird, bleiben die Stunden im Projekt erhalten).\
     Diese Option ist standardmäßig ausgewählt.
   * Löschen Sie alle protokollierten Stunden (wenn diese Aufgabe oder dieses Problem zu einem späteren Zeitpunkt wiederhergestellt wird, werden die protokollierten Stunden für die Aufgabe oder das Problem wiederhergestellt).

1. Klicken Sie auf **Speichern**.
