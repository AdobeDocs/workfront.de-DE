---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Diagnose zum Auslösen automatisierter Prozesse verwenden
description: Mithilfe von Diagnostics können Sie automatisierte Prozesse, wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen, manuell Trigger durchführen.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 9%

---

# Diagnose zum Auslösen automatisierter Prozesse verwenden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Mithilfe von Diagnostics können Sie automatisierte Prozesse, wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen, manuell Trigger durchführen.

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

## Verwenden Sie die Diagnose für den Trigger automatisierter Prozesse.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Erweitern Sie **System** und klicken Sie dann auf **Diagnose**.
1. Wählen Sie eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Versäumnisnachrichten senden</td> 
      <td> <p>Sendet die automatischen Erinnerungsbenachrichtigungen für überfällige Aufgaben und Probleme manuell. </p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Einrichten automatischer Erinnerungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frühzeitige Benachrichtigungen senden</td> 
      <td> <p>Sendet die automatischen Erinnerungsbenachrichtigungen für Aufgaben und Probleme, die sich ihrem Fälligkeitsdatum nähern.</p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Einrichten automatischer Erinnerungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten senden</td> 
      <td> <p>Sendet Erinnerungsbenachrichtigungen manuell. </p> <p>Weitere Informationen zum Einrichten von Erinnerungsbenachrichtigungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsbenachrichtigungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle POP-Konten prüfen</td> 
      <td> <p>Prüft neue E-Mails, die an mit Workfront verknüpfte POP-Konten gesendet wurden. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitleisten erneut berechnen</td> 
      <td> <p>Berechnet die Timeline für alle Projekte in Workfront mit dem Status "Aktuell". </p> <p>Weitere Informationen zum automatischen oder manuellen Berechnen der Zeitleiste von Projekten finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Aktualisieren der Projektzeitpläne</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardkundenberichte wiederherstellen</td> 
      <td>Stellt die Standardberichte wieder her, die ursprünglich mit Workfront bereitgestellt wurden, sodass sie für alle Benutzer im Abschnitt <strong>Berichte</strong> sichtbar sind.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen erstellen</td> 
      <td>Erstellt Timesheets für Benutzer basierend auf ihren wiederkehrenden Timesheet-Profilen. Diese Option muss nur ausgeführt werden, wenn das Timesheet-Profil nach der Zuweisung an Benutzer erheblich geändert wurde, und erst, nachdem alle aktuellen und künftigen Timesheets gelöscht wurden.</td> 
     </tr> 
    </tbody> 
   </table>
