---
product-area: documents
navigation-topic: approvals
title: Entfernen von genehmigenden Personen oder Prüfenden aus einem Dokumentgenehmigungs-Workflow
description: Sie können einzelne genehmigende Personen oder Prüfende Personen aus einem Dokument entfernen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b3c8559ddac934cc41461f88503b2fa71abaf452
workflow-type: tm+mt
source-wordcount: '538'
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
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe von Adobe Enterprise-Speicher</p>  </td> 
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

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Workfront-Speicher im Vergleich zu Adobe Enterprise-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

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

Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Massenspeicher für Unternehmen](/help/quicksilver/review-and-approve-work/esm-overview.md).

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