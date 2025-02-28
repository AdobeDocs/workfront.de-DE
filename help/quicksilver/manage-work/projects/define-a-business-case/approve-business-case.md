---
navigation-topic: business-case-and-scorecards
title: Business Case genehmigen
description: Nachdem Sie den Business Case für eine Projektanfrage abgeschlossen und gesendet haben, muss der Business Case genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Business Case genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und die Projektbesitzer halten es möglicherweise nicht für ideal, dies zu tun.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Business Case genehmigen

Nachdem Sie den Business Case für eine Projektanfrage abgeschlossen und gesendet haben, muss der Business Case genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Business Case genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und die Projektbesitzer halten es möglicherweise nicht für ideal, dies zu tun.

Weitere Informationen zum Abschließen und Senden eines Business Case finden Sie im Artikel [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Überblick über die Business Case-Genehmigung

Beachten Sie bei der Genehmigung eines Business Case für ein Projekt Folgendes:

* Sie müssen über Verwaltungsberechtigungen für ein Projekt verfügen, um den Business Case dafür zu genehmigen.
* Die Projekte, die auf die Genehmigung des Business Case warten, werden nicht unter dem Widget Meine Genehmigungen auf der Startseite angezeigt.
* Sie müssen die einzelnen Projekte, für die eine Business Case-Genehmigung erforderlich ist, manuell aufrufen, um zu sehen, dass sie noch nicht genehmigt wurden. Es gibt keinen Workfront-Benachrichtigungsmechanismus, der jemanden darauf hinweist, dass er den Business Case eines Projekts genehmigen muss.
* Sie können die Projekte finden, die auf die Genehmigung des Business Case warten, indem Sie entweder einen Projektbericht erstellen oder auf das Portfolio zugreifen, dem sie zugeordnet sind.

  Weitere Informationen zu Portfolios finden Sie im Artikel [Übersicht über Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Genehmigen des Business Case durch Erstellen eines Projektberichts

Sie können einen Bericht für Projekte erstellen, um zu sehen, für welche Projekte ein Business Case genehmigt werden muss.

So erstellen Sie einen Bericht für Projekte, für die die Genehmigung ihrer Business Cases aussteht:

1. Erstellen Sie einen Bericht für Projekte.

   Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie die **Ansicht** des Berichts aus und klicken Sie dann auf **Spalte hinzufügen**.

1. Beginnen Sie, „Status“ in das Feld **In dieser Spalte anzeigen** einzugeben, und wählen Sie dieses Feld aus, wenn es in der Liste angezeigt wird.

   In dieser Spalte wird der Status der Projekte angezeigt.

1. Wählen Sie **Registerkarte** Filter“ des Berichts aus und klicken Sie dann auf **Filterregel hinzufügen**.

1. Beginnen Sie mit der Eingabe von „Status **in das Feld „Nur Projekte anzeigen, in denen …** und wählen Sie es aus, wenn es in der Liste angezeigt wird.
1. Wählen Sie **Filtermodifikator &quot;**&quot; aus.
1. Beginnen Sie, „Angefordert“ in das verfügbare Feld einzugeben.

   Dadurch wird sichergestellt, dass der Bericht nur Projekte mit dem Status Angefordert enthält.

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Optional) Klicken Sie auf **Weitere Filterregel hinzufügen**.

   Sie können zusätzliche Filter hinzufügen, um nur Projekte anzuzeigen, bei denen Sie Projektinhaber oder Projektsponsor oder Portfolio-Inhaber sind.

   Sie können beispielsweise die folgenden Filteranweisungen verwenden:

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   , um Projekte anzuzeigen, für die Sie als Projektsponsor angegeben sind

   ```
   Project Owner ID Equals $$USER.ID
   ```

   So zeigen Sie Projekte an, für die Sie als Projektbesitzer festgelegt sind

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   , um anzuzeigen, wo Sie als Portfolio-Manager festgelegt sind.

1. Klicken Sie **Speichern+Schließen**.

   Beachten Sie, dass alle Projekte im Bericht den Status &quot;**&quot;**.

1. Klicken Sie auf den Namen eines Projekts im Bericht, um es zu öffnen.
1. Klicken Sie **linken Bedienfeld** Business Case“.
1. Klicken Sie **Bereich** Genehmigen“ oder **Ablehnen**, um den Business Case zu genehmigen oder abzulehnen.

   ![Business Case](assets/business-case-summary-with-rp-information--1-.png)

   Der Projektstatus wird in &quot;**&quot; geändert** wenn der Business Case genehmigt wurde.

   Der Projektstatus ändert sich in **Abgelehnt** wenn der Business-Case abgelehnt wird.

   >[!NOTE]
   >
   >Es gibt keine Benachrichtigungen, die den Benutzer, der die Genehmigung des Business-Case eingereicht hat, darüber informieren, ob seine Projektanforderung genehmigt oder abgelehnt wurde.

## Genehmigen des Business Case durch Zugriff auf angeforderte Projekte in einem Portfolio

Weitere Informationen zur Überprüfung angeforderter Projekte finden Sie im Artikel [angeforderte Projekte überprüfen](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
