---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Verwenden der Diagnose für den Trigger automatisierter Prozesse
description: Mithilfe von Diagnostics können Sie automatisierte Prozesse, wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen, manuell Trigger durchführen.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 6%

---

# Verwenden der Diagnose für den Trigger automatisierter Prozesse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Mithilfe von Diagnostics können Sie automatisierte Prozesse, wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen, manuell Trigger durchführen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a> </td> 
   <td> <p>Plan </p>Sie müssen Workfront-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Verwenden Sie die Diagnose für den Trigger automatisierter Prozesse

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Erweitern **System** Klicken Sie auf **Diagnose**.
1. Wählen Sie eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Versäumnisnachrichten senden</td> 
      <td> <p>Sendet die automatischen Erinnerungsbenachrichtigungen für überfällige Aufgaben und Probleme manuell. </p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Automatische Erinnerungen einrichten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frühzeitige Benachrichtigungen senden</td> 
      <td> <p>Sendet die automatischen Erinnerungsbenachrichtigungen für Aufgaben und Probleme, die sich ihrem Fälligkeitsdatum nähern.</p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Automatische Erinnerungen einrichten</a>.</p> </td> 
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
      <td> <p>Berechnet die Timeline für alle Projekte in Workfront mit dem Status "Aktuell". </p> <p>Weitere Informationen zur automatischen oder manuellen Berechnung der Zeitleiste von Projekten finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Projektzeitpläne neu berechnen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardkundenberichte wiederherstellen</td> 
      <td>Stellt die Standardberichte wieder her, die ursprünglich mit Workfront bereitgestellt wurden, damit sie im <strong>Berichte</strong> für alle Benutzer.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen erstellen</td> 
      <td>Erstellt Timesheets für Benutzer basierend auf ihren wiederkehrenden Timesheet-Profilen. Diese Option muss nur ausgeführt werden, wenn das Timesheet-Profil nach der Zuweisung an Benutzer erheblich geändert wurde, und erst, nachdem alle aktuellen und künftigen Timesheets gelöscht wurden.</td> 
     </tr> 
    </tbody> 
   </table>
