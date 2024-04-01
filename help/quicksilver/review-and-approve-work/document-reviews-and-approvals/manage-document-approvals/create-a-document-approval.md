---
product-area: documents
navigation-topic: approvals
title: Erstellen einer Dokumentgenehmigung
description: Sie können die Genehmigung von anderen Benutzern für ein Dokument in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: 6a02a7bdb21e79a6b91f81e71b42968d6262cd05
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Anforderung einer Dokumentgenehmigung erstellen

Sie können die Genehmigung von anderen Benutzern oder Teams für ein Dokument in Adobe Workfront anfordern oder anfordern, dass diese ein Dokument überprüfen, ohne es genehmigen zu müssen.

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf die aktualisierte Funktion zur Dokumentgenehmigung, die nur für bestimmte Konten verfügbar ist. Informationen zu Standardgenehmigungsverfahren finden Sie in den Artikeln unter [Arbeitsgenehmigungen](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards und Kalender, Dokumente anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Objekt verwalten, das mit dem Anforderungszugriff oder der Genehmigung verknüpft ist </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen einer Dokumentgenehmigung über die Dokumentseite

1. Klicken Sie auf die Dokumentseite, um auf den Namen des Dokuments zu klicken, und wählen Sie dann die Version des Dokuments aus, für das Sie im Dropdown-Menü Version eine Genehmigung erstellen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Auswählen **Genehmigungen** im linken Bereich.

1. Um einen Genehmiger hinzuzufügen, stellen Sie sicher, dass das **Genehmiger** das Kontrollkästchen aktiviert ist und die Eingabe im **Überprüfer** Textfeld. Sie können Workfront-Benutzer oder -Teams anhand des Namens hinzufügen. Wenn Sie stattdessen einen Validierer hinzufügen möchten, deaktivieren Sie einfach die **Genehmiger** vor der Eingabe aktivieren.

1. Wiederholen Sie den vorherigen Schritt, um weitere Genehmiger oder Validierer hinzuzufügen.

## Erstellen einer Dokumentgenehmigung über den Bereich Dokumentzusammenfassung

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das benötigte Dokument. Daraufhin wird der Bereich Dokumentzusammenfassung für dieses Dokument geöffnet.

1. Wählen Sie im Versions-Dropdown-Menü die Version des Dokuments aus, für das Sie eine Genehmigung erstellen möchten. Standardmäßig wird die neueste Version ausgewählt.

1. Scrollen Sie nach unten zum **Genehmigungen** im Bereich &quot;Document Summary&quot;. Um einen Genehmiger hinzuzufügen, stellen Sie sicher, dass das **Genehmiger** das Kontrollkästchen aktiviert ist und die Eingabe im **Überprüfer** Textfeld. Sie können Workfront-Benutzer oder -Teams anhand des Namens hinzufügen. Wenn Sie stattdessen einen Validierer hinzufügen möchten, deaktivieren Sie einfach die **Genehmiger** vor der Eingabe aktivieren.

1. Wiederholen Sie den vorherigen Schritt, um weitere Genehmiger oder Validierer hinzuzufügen.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
