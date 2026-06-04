---
navigation-topic: business-case-and-scorecards
title: Genehmigen eines Business-Case
description: Nachdem Sie den Business Case für eine Projektanfrage abgeschlossen und gesendet haben, muss der Business Case genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Business Case genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und die Projektbesitzer halten es möglicherweise nicht für ideal, dies zu tun.
author: Becky
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
TQID: https://experienceleague.adobe.com/DCLPGdt9b-7jkg7ajSbaRJRO968yAdetzVvOXpNI9nc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 682
ht-degree: 6%

---

# Genehmigen eines Business-Case

<!--Audit: 6/2025-->

Nachdem Sie den Business Case für eine Projektanfrage abgeschlossen und gesendet haben, muss der Business Case genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Business Case genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und die Projektbesitzer halten es möglicherweise nicht für ideal, dies zu tun.

Weitere Informationen zum Abschließen und Senden eines Business Case finden Sie im Artikel [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
   <p>Prime oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Standard </p> 
   <p>Abo </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt</p> <p>Anzeigen oder Erweitern von Berechtigungen für ein Portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

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

1. Beginnen Sie mit der Eingabe *Status* in das Feld **In dieser Spalte anzeigen** und wählen Sie dieses Feld aus, wenn es in der Liste angezeigt wird.

   In dieser Spalte wird der Status der Projekte angezeigt.

1. Wählen Sie **Registerkarte** Filter“ des Berichts aus und klicken Sie dann auf **Filterregel hinzufügen**.

1. Beginnen Sie mit der Eingabe *Status* in das Feld **Nur Projekte anzeigen, in denen …** angezeigt wird, und wählen Sie es aus, wenn es in der Liste angezeigt wird.
1. Wählen Sie **Filtermodifikator &quot;**&quot; aus.
1. Beginnen Sie *angefordert* in das verfügbare Feld einzugeben.

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

<!-- ![Business case](assets/business-case-summary-with-rp-information--1-.png) -->

Der Projektstatus wird in &quot;**&quot; geändert** wenn der Business Case genehmigt wurde.

Der Projektstatus ändert sich in **Abgelehnt** wenn der Business-Case abgelehnt wird.

>[!NOTE]
>
>Es gibt keine Benachrichtigungen, die den Benutzer, der die Genehmigung des Business-Case eingereicht hat, darüber informieren, ob seine Projektanforderung genehmigt oder abgelehnt wurde.

## Genehmigen des Business Case durch Zugriff auf angeforderte Projekte in einem Portfolio

Weitere Informationen zur Überprüfung angeforderter Projekte finden Sie im Artikel [angeforderte Projekte überprüfen](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
