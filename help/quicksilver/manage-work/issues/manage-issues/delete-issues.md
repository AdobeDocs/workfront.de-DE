---
product-area: projects
navigation-topic: manage-issues
title: Probleme löschen
description: Sie können Probleme oder Anforderungen in Adobe Workfront löschen, wenn Sie über die entsprechenden Berechtigungen und Zugriffsrechte verfügen.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 1%

---

# Probleme löschen

<!--Audited: 01/2024-->

Sie können Probleme oder Anforderungen in Adobe Workfront löschen, wenn Sie über die entsprechenden Berechtigungen und Zugriffsrechte verfügen.

>[!TIP]
>
>&quot;Probleme&quot;und &quot;Anforderungen&quot;werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um auf unvorhergesehene Arbeit hinzuweisen, die behoben werden muss. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anforderungswarteschlange bezeichnet wird.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Mitarbeiter oder höher</p>
   <p>Aktuell: Anforderung oder höher</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p>  <p>Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen zum Problem verwalten</p> <p>Contribute oder höhere Berechtigungen für das Projekt oder die Aufgabe</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Löschen von Problemen

* Ihr Workfront-Administrator oder ein Gruppenadministrator muss das Löschen von Problemen in einem Projekt aktivieren, dessen Status im Bereich &quot;Projekteinstellungen&quot;den Status Fertig stellen aufweist. Weitere Informationen zum Einrichten von Projektvoreinstellungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn das Problem Stunden protokolliert hat, muss der Workfront-Administrator oder ein Gruppenadministrator das Löschen dieser Probleme zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in Ihrer Workfront-Instanz konfiguriert. Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, bei denen Probleme mit Stunden aufgetreten sind.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Weitere Informationen zum Aktivieren des Löschens von Problemen, bei denen Stunden protokolliert werden, finden Sie im Abschnitt &quot;Löschung&quot;unter [Systemweite Aufgabe konfigurieren und Ausgabevoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Auswirkungen des Löschens von Problemen

Wenn Sie ein Problem löschen, wirkt sich dies auf andere Objekte aus, die mit dem Problem verknüpft sind.

Die folgenden Objekte, die an ein Problem angehängt sind, werden auch beim Löschen eines Problems gelöscht:

* Dokumente

  Sie können ein Problem nicht löschen, bei dem ein ausgechecktes Dokument angehängt ist. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Dokumente auschecken](../../../documents/managing-documents/check-out-documents.md).

* Notizen
* Genehmigungen

Je nachdem, wie Ihr Workfront- oder Gruppenadministrator die Voreinstellungen zum Projekt, zur Aufgabe oder zur Problemlöschung in den Voreinstellungen für das Timesheet und die Stunde **Ihrer Workfront-Instanz konfiguriert, werden die Stunden, die für die Probleme protokolliert werden, beim Löschen eines Problems auf eine der folgenden Arten behandelt:**

* Wechseln Sie zum Projekt und werden beim Problem nicht wiederhergestellt, wenn das Problem später wiederhergestellt wird.
* Wird gelöscht und wird zum Problem wiederhergestellt, wenn das Problem später wiederhergestellt wird.

  Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, bei denen Aufgaben mit aufgezeichneten Stunden ausgeführt werden.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert werden, finden Sie unter [Konfigurieren von Voreinstellungen für Zeitblätter und Stunden](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Die Benutzer, die dem Problem oder der Problemgenehmigung zugewiesen sind, verbleiben im Projektteam.\
  Weitere Informationen zu Projektteams finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Probleme löschen

* [Mehrere Probleme in einem Projekt gleichzeitig löschen](#delete-multiple-issues-in-a-project-simultaneously)
* [Löschen eines einzelnen Problems](#delete-a-single-issue)

### Mehrere Probleme gleichzeitig in einem Projekt löschen  {#delete-multiple-issues-in-a-project-simultaneously}

1. Wechseln Sie zum **Hauptmenü**.
1. Klicken Sie auf **Projekte**.
1. Klicken Sie auf den Projektnamen, der die zu löschenden Probleme enthält.
1. Klicken Sie im linken Bereich auf **Probleme** .
1. Wählen Sie ein Problem aus und klicken Sie dann oben in der Liste auf das Symbol **Löschen** ![](assets/delete.png) .

1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Ja, löschen Sie ihn**.\
   Möglicherweise lässt Ihr Workfront-Administrator das Löschen von Problemen, bei denen Stunden protokolliert werden, nicht zu.\
   Weitere Informationen zu Zugriff und Berechtigungen, die zum Löschen eines Problems erforderlich sind, finden Sie unter [Löschprobleme](#access-and-permissions-needed).

### Löschen eines einzelnen Problems {#delete-a-single-issue}

{{step1-to-projects}}

1. Klicken Sie auf den Projektnamen, der das zu löschende Problem enthält.
1. Klicken Sie im linken Bereich auf **Probleme** .

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Klicken Sie auf den Namen des Problems, das Sie löschen möchten.
1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Problems.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Klicken Sie auf **Problem löschen**.
1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Ja, löschen Sie ihn**.

   Möglicherweise lässt Ihr Workfront-Administrator das Löschen von Problemen, bei denen Stunden protokolliert werden, nicht zu.\
   Weitere Informationen zu Zugriff und Berechtigungen, die zum Löschen eines Problems erforderlich sind, finden Sie unter [Löschprobleme](#access-and-permissions-needed).

## Gelöschte Probleme wiederherstellen

Ein Workfront- oder Gruppenadministrator kann Probleme innerhalb von 30 Tagen nach dem Löschen wiederherstellen. Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
