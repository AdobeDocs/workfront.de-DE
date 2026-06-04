---
product-area: documents
navigation-topic: approvals
title: Entfernen von genehmigenden Personen oder Prüfenden aus einem Dokumentgenehmigungs-Workflow
description: Sie können einzelne genehmigende Personen oder Prüfende Personen aus einem Dokument entfernen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zSKSGDHN8vNwozS4R-GYqsxP52Iob6SqcY0G32-3FyQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 544
ht-degree: 6%

---

# Entfernen von genehmigenden Personen oder Prüfenden aus einem Dokumentgenehmigungs-Workflow

Sie können einzelne genehmigende Personen oder Prüfende Personen aus einem Asset oder Dokument entfernen, nachdem sie zugewiesen wurden.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zur Verwaltung von Genehmigungen unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Überprüfen oder höher</p>
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten des Zugriffs auf das Objekt, das mit der Zugriffsanforderung oder Genehmigung verknüpft ist </p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++


## Entfernen Sie genehmigende Personen oder Prüfende Personen aus einem Genehmigungs-Workflow im Bereich für veraltete Dokumente

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

So entfernen Sie genehmigende Personen oder Prüfende Personen aus einem Genehmigungs-Workflow:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das gewünschte Dokument, und das Bedienfeld Dokumentzusammenfassung für dieses Dokument wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** im Bedienfeld Dokumentzusammenfassung.

1. Klicken Sie **Workflow bearbeiten**.

1. Suchen Sie den Teilnehmer, den Sie entfernen möchten, und klicken Sie auf das Symbol **Entfernen** neben seinem Namen.

   Die Genehmigungs- oder Überprüfungsanfrage wird entfernt und die genehmigende Person erhält eine Benachrichtigung, dass ihre Genehmigung nicht mehr erforderlich ist. Ihr genehmigungsbezogener Freigabezugang wird ebenfalls entfernt.

   ![Genehmigungs-Workflow bearbeiten](assets/edit-approval-in-legacy.png)

1. (Optional) Um die Rolle einer genehmigenden Person in eine prüfende Person zu ändern oder umgekehrt, klicken Sie auf das Dropdown-Menü neben dem Benutzernamen und wählen Sie die neue Rolle aus.

1. Wiederholen Sie den vorherigen Schritt, um alle zusätzlichen genehmigenden Personen oder Prüfer zu entfernen.

</div>


## Entfernen von genehmigenden Personen oder Prüfenden aus einem Genehmigungs-Workflow im Bereich „Neue Dokumente“

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

So erstellen Sie einen Validierungs-Workflow:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das Dokument und dann auf **Genehmigungen** rechts auf der Seite.

   ![Genehmigende Personen in der Dokumentzusammenfassung hinzufügen](assets/approvals-icon-new.png)


1. Klicken Sie **Workflow bearbeiten**.

1. Suchen Sie den Teilnehmer, den Sie entfernen möchten, und klicken Sie auf das Symbol **Entfernen** neben seinem Namen.

   Die Genehmigungs- oder Überprüfungsanfrage wird entfernt und die genehmigende Person erhält eine Benachrichtigung, dass ihre Genehmigung nicht mehr erforderlich ist.

1. (Optional) Um die Rolle einer genehmigenden Person in eine prüfende Person zu ändern oder umgekehrt, klicken Sie auf das Dropdown-Menü neben dem Benutzernamen und wählen Sie die neue Rolle aus.

1. Wiederholen Sie den vorherigen Schritt, um alle zusätzlichen genehmigenden Personen oder Prüfer zu entfernen.

   ![Teilnehmer von einer Phase entfernen](assets/add-or-remove-participants.png)

1. Klicken Sie auf **Speichern**.