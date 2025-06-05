---
product-area: projects
navigation-topic: manage-issues
title: Probleme löschen
description: Sie können Probleme oder Anfragen in Adobe Workfront löschen, wenn Sie dazu über die erforderlichen Zugriffsrechte und Berechtigungen verfügen.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 1%

---

# Probleme löschen

<!--Audited: 05/2025-->

Sie können Probleme oder Anfragen in Adobe Workfront löschen, wenn Sie dazu über die erforderlichen Zugriffsrechte und Berechtigungen verfügen.

>[!TIP]
>
>„Probleme“ und „Anfragen“ werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um unvorhergesehene Arbeiten anzuzeigen, die bearbeitet werden müssen. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anfrage-Warteschlange bezeichnet wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   <p>Aktuell: Anforderung oder höher</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Anzeigen oder Hochladen des Zugriffs auf Projekte und Aufgaben</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> <p>Mitwirken an oder höhere Berechtigungen für das Projekt oder die Aufgabe</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Löschen von Problemen

* Ihr Workfront-Administrator oder ein Gruppenadministrator muss das Löschen von Anfragen in einem Projekt mit dem Status „Abgeschlossen“ in Ihrem Bereich Projektvoreinstellungen aktivieren.

  Informationen zum Einrichten von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn das Problem über protokollierte Stunden verfügt, muss der Workfront-Administrator oder ein Gruppenadministrator das Löschen dieser Probleme zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in Ihrer Workfront-Instanz konfiguriert. Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, bei denen Probleme mit protokollierten Stunden bestehen.

  Weitere Informationen zum Aktivieren des Löschens von Problemen, bei denen Stunden protokolliert werden, finden Sie im Abschnitt „Löschen“ in [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).


## Die Auswirkungen des Löschens von Problemen

Wenn Sie ein Problem löschen, wirkt sich dies auf andere mit dem Problem verknüpfte Objekte aus.

Die folgenden an ein Problem angehängten Objekte werden auch gelöscht, wenn Sie ein Problem löschen:

* Dokumente

  Sie können ein Problem, an das ein ausgechecktes Dokument angehängt wurde, nicht löschen. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

* Notizen
* Genehmigungen

Je nachdem, wie Ihr Workfront- oder Gruppen-Administrator die Einstellungen für die Löschung von Projekten, Aufgaben oder Problemen in den **Arbeitszeittabellen- und**) Ihrer Workfront-Instanz konfiguriert, werden die für die Probleme protokollierten Stunden beim Löschen eines Problems auf eine der folgenden Arten gehandhabt:

* Verschieben Sie in das Projekt und wird bei dem Problem nicht wiederhergestellt, wenn das Problem später wiederhergestellt wird.
* wird gelöscht und bei dem Problem wiederhergestellt, wenn das Problem später wiederhergestellt wird.

  Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, in denen Aufgaben mit Stunden protokolliert sind.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert sind, finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Die Benutzer, die dem Problem oder der Problemgenehmigung zugewiesen sind, bleiben im Projektteam.\
  Weitere Informationen zu Projektteams finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Probleme löschen

### Gleichzeitiges Löschen mehrerer Probleme in einem Projekt  {#delete-multiple-issues-in-a-project-simultaneously}

1. Navigieren Sie zum **Hauptmenü**.
1. Klicken Sie auf **Projekte**.
1. Klicken Sie auf den Projektnamen, der die Probleme enthält, die Sie löschen möchten.
1. Klicken Sie **linken** auf „Probleme“.

   Rechts wird eine Liste der mit dem ausgewählten Projekt verknüpften Probleme angezeigt.
1. Wählen Sie ein oder mehrere Probleme in der Liste aus und klicken Sie dann oben in **Liste auf** Löschen![Symbol &quot;](assets/delete.png)&quot;.

1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Löschen**.

   Ihr Workfront-Administrator erlaubt möglicherweise nicht das Löschen von Anfragen, bei denen Stunden protokolliert werden.\
   Weitere Informationen zu den Zugriffsrechten und Berechtigungen, die zum Löschen eines Problems erforderlich sind, finden Sie im Abschnitt [Überlegungen zum Löschen von Problemen](#considerations-for-deleting-issues) in diesem Artikel.

### Einzelnes Problem löschen {#delete-a-single-issue}

{{step1-to-projects}}

1. Klicken Sie auf den Projektnamen, der das Problem enthält, das Sie löschen möchten.
1. Klicken Sie **linken** auf „Probleme“.

   ![Abschnitt „Probleme“ im linken Bedienfeld](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Klicken Sie auf den Namen des Problems, das Sie löschen möchten.
1. Klicken Sie auf das **Mehr**-Menü rechts neben dem Problemnamen.

   ![Menü „Problem Mehr“](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Klicken Sie **Problem löschen**.
1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Löschen**.

   Ihr Workfront-Administrator erlaubt möglicherweise nicht das Löschen von Anfragen, bei denen Stunden protokolliert werden.\
   Weitere Informationen zu den Zugriffsrechten und Berechtigungen, die zum Löschen eines Problems erforderlich sind, finden Sie im Abschnitt [Überlegungen zum Löschen von Problemen](#considerations-for-deleting-issues) in diesem Artikel.

## Gelöschte Anfragen wiederherstellen

Ein Workfront- oder Gruppen-Administrator kann Probleme innerhalb von 30 Tagen nach dem Löschen wiederherstellen.

Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
