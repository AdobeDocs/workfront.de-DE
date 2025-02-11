---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Diagnose zum Auslösen automatisierter Prozesse verwenden
description: Sie können Diagnostics verwenden, um automatisierte Prozesse wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen manuell in Trigger zu setzen.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 9%

---

# Diagnose zum Auslösen automatisierter Prozesse verwenden

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Sie können Diagnostics verwenden, um automatisierte Prozesse wie zeitbasierte Skripte, Neuberechnungen oder E-Mail-Benachrichtigungen manuell in Trigger zu setzen.

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
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Trigger automatisierter Prozesse mit Diagnosefunktionen

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Erweitern Sie **System** und klicken Sie dann auf **Diagnose**.
1. Wählen Sie eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Versäumnisnachrichten senden</td> 
      <td> <p>sendet die automatischen Erinnerungsbenachrichtigungen für überfällige Aufgaben und Probleme manuell. </p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Einrichten automatischer Erinnerungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frühzeitige Benachrichtigungen senden</td> 
      <td> <p>sendet die automatischen Erinnerungsbenachrichtigungen für Aufgaben und Probleme, die sich ihrem Fälligkeitsdatum nähern, manuell.</p> <p>Weitere Informationen zum Einrichten automatischer Erinnerungen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Einrichten automatischer Erinnerungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten senden</td> 
      <td> <p>sendet Erinnerungsnachrichten manuell. </p> <p>Weitere Informationen zum Einrichten von Erinnerungsnachrichten finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsnachrichten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle POP-Konten prüfen</td> 
      <td> <p>Sucht nach neuen E-Mails, die an mit Workfront verknüpfte POP-Konten gesendet wurden. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timelines erneut berechnen</td> 
      <td> <p>Berechnet die Zeitleiste neu für alle Projekte in Workfront mit dem Status „Aktuell“. </p> <p>Weitere Informationen zur automatischen oder manuellen Berechnung der Zeitleiste von Projekten, jeweils ein Projekt, finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Neuberechnen von Projektzeitleisten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardkundenberichte wiederherstellen</td> 
      <td>Stellt die Standardberichte wieder her, die ursprünglich mit Workfront bereitgestellt wurden, sodass sie für alle Benutzenden im Abschnitt <strong>Berichte</strong> angezeigt werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitszeittabellen erstellen</td> 
      <td>Erzeugt Arbeitszeittabellen für Benutzer basierend auf ihren Profilen mit wiederkehrenden Arbeitszeittabellen. Diese Option muss nur ausgeführt werden, wenn das Arbeitszeittabellen-Profil nach der Zuweisung an Benutzende erheblich geändert wurde, und nur, nachdem alle aktuellen und künftigen Arbeitszeittabellen gelöscht wurden.</td> 
     </tr> 
    </tbody> 
   </table>
