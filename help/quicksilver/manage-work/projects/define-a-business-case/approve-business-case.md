---
navigation-topic: business-case-and-scorecards
title: Geschäftsfall genehmigen
description: Nachdem Sie den Geschäftsfall für eine Projektanforderung abgeschlossen und übermittelt haben, muss der Geschäftsfall genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Geschäftsfall genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und Projekteigentümer halten es möglicherweise nicht für optimal.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Geschäftsfall genehmigen

Nachdem Sie den Geschäftsfall für eine Projektanforderung abgeschlossen und übermittelt haben, muss der Geschäftsfall genehmigt werden. Dies hängt vom Workflow in Ihrer Organisation ab. Ein Projekt kann beginnen, ohne dass der Geschäftsfall genehmigt werden muss, aber Ihr Adobe Workfront-Administrator und Projekteigentümer halten es möglicherweise nicht für optimal.

Weitere Informationen zum Abschließen und Senden eines Geschäftsszenarios finden Sie im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überblick über die Genehmigung von Geschäftsfällen

Beachten Sie bei der Genehmigung eines Geschäftsfalls eines Projekts Folgendes:

* Sie müssen über Verwaltungsberechtigungen für ein Projekt verfügen, um den Geschäftsfall für dieses Projekt zu genehmigen.
* Sie können die Projekte, die auf die Genehmigung des Geschäftsfalls warten, nicht im Widget Meine Genehmigungen in der Startseite sehen.
* Sie müssen manuell zu den einzelnen Projekten wechseln, für die die Genehmigung von Geschäftsfällen erforderlich ist, um zu sehen, dass die Genehmigung aussteht. Es gibt keinen Workfront-Benachrichtigungsmechanismus, der jemanden darauf hinweist, dass er den Geschäftsfall eines Projekts genehmigen muss.
* Sie können die Projekte finden, die auf die Genehmigung des Geschäftsfalls warten, indem Sie entweder einen Projektbericht erstellen oder auf das Portfolio zugreifen, mit dem sie verknüpft sind.

  Weitere Informationen zu Portfolios finden Sie im Artikel [Überblick über Portfolios in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Genehmigen Sie den Geschäftsfall, indem Sie einen Projektbericht erstellen

Sie können einen Bericht für Projekte erstellen, um zu sehen, welche Projekte genehmigt werden müssen.

So erstellen Sie einen Bericht für Projekte, deren Geschäftsszenarios noch nicht genehmigt wurden:

1. Erstellen Sie einen Bericht für Projekte.

   Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie die Registerkarte **Ansicht** des Berichts aus und klicken Sie dann auf **Spalte hinzufügen**.

1. Beginnen Sie mit der Eingabe von &quot;Status&quot;in das Feld **In dieser Spalte anzeigen** und wählen Sie dieses Feld aus, wenn es in der Liste angezeigt wird.

   Diese Spalte zeigt den Status der Projekte an.

1. Wählen Sie die Registerkarte **Filter** des Berichts aus und klicken Sie dann auf **Filterregel hinzufügen**.

1. Beginnen Sie mit der Eingabe von &quot;Status&quot;in das Feld **Nur Projekte anzeigen, in denen das Feld ...** erscheint, und wählen Sie es aus, wenn es in der Liste angezeigt wird.
1. Wählen Sie **Equal** für den Filtermodifikator aus.
1. Beginnen Sie mit der Eingabe von &quot;Angefordert&quot; in das verfügbare Feld.

   Dadurch wird sichergestellt, dass der Bericht nur Projekte enthält, die sich im Status &quot;Angefordert&quot;befinden.

   ![request_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Optional) Klicken Sie auf **Hinzufügen einer weiteren Filterregel**.

   Sie können zusätzliche Filter hinzufügen, um nur Projekte anzuzeigen, bei denen Sie der Projekteigentümer, der Projektsponsor oder der Portfolio-Eigentümer sind.

   Sie können beispielsweise die folgenden Filteranweisungen verwenden:

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   , um Projekte anzuzeigen, bei denen Sie als Projektsponsor benannt sind.

   ```
   Project Owner ID Equals $$USER.ID
   ```

   , um Projekte anzuzeigen, für die Sie als Projekteigentümer bestimmt sind.

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   , um anzuzeigen, wo Sie als Portfolio-Manager benannt sind.

1. Klicken Sie auf **Speichern+Schließen**.

   Beachten Sie, dass sich alle Projekte im Bericht im Status &quot;**Angefordert**&quot;befinden.

1. Klicken Sie auf den Namen eines Projekts im Bericht, um es zu öffnen.
1. Klicken Sie im linken Bereich auf **Geschäftsszenario** .
1. Klicken Sie im Bereich &quot;Zusammenfassung der Geschäftsfälle&quot;auf **Genehmigen** oder **Ablehnen** , um den Geschäftsfall zu genehmigen oder abzulehnen.

   ![](assets/business-case-summary-with-rp-information--1-.png)

   Der Projektstatus wird in &quot;**Genehmigt**&quot; geändert, wenn der Geschäftsfall genehmigt wurde.

   Der Projektstatus wird in **Abgelehnt** geändert, wenn der Geschäftsfall abgelehnt wird.

   >[!NOTE]
   >
   >Es gibt keine Benachrichtigungen, die den Benutzer, der die Genehmigung des Geschäftsfalls eingereicht hat, darauf hinweisen, ob seine Projektanfrage genehmigt oder abgelehnt wurde.

## Genehmigen Sie den Geschäftsfall, indem Sie auf angeforderte Projekte in einem Portfolio zugreifen

Weitere Informationen zum Überprüfen angeforderter Projekte finden Sie im Artikel [Angeforderte Projekte überprüfen](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
