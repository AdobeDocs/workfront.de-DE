---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Tagging von Benutzern für die Freigabe eines Korrekturabzugs
description: Wenn Sie einen Korrekturabzug im Proofing Viewer kommentieren, können Sie andere Benutzende taggen, um ihre Aufmerksamkeit auf Ihren Kommentar per E-Mail zu lenken und sie zum Workflow des Korrekturabzugs hinzuzufügen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Tagging von Benutzern für die Freigabe eines Korrekturabzugs

Wenn Sie einen Korrekturabzug im Proofing Viewer kommentieren, können Sie andere Benutzende taggen, um ihre Aufmerksamkeit auf Ihren Kommentar per E-Mail zu lenken und sie zum Workflow des Korrekturabzugs hinzuzufügen.

Beim Tagging von Benutzern in Kommentaren zu einem Korrekturabzug können die Benutzenden, die Sie taggen können, je nach verschiedenen Faktoren unterschiedlich sein, z. B. individuelle Benutzerberechtigungen und Ihre Mitgliedschaft in der Organisation:

* Wenn Sie der Ersteller oder Inhaber eines Korrekturabzugs sind oder bestimmte Berechtigungen aktiviert haben, können Sie Benutzer außerhalb des Korrekturabzugs-Workflows taggen und den Korrekturabzug für sie freigeben.
* Wenn Sie als externer Benutzer zum Korrekturabzug hinzugefügt wurden und Mitglied einer anderen Umgebung mit einem anderen Korrekturabzugskonto sind, können Sie nur diese Benutzer aus Ihrer ursprünglichen Umgebung taggen. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Zugriffsanforderungen {#access-requirements}

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Autor, Moderator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Verantwortlicher oder Administrator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Tagging von Benutzern für die Freigabe eines Korrekturabzugs

Benutzende mit dem im Abschnitt [Zugriffsanforderungen“ oben beschriebenen Profil für Korrekturabzugsberechtigungen oder der Rolle für &#x200B;](#access-requirements) können Benutzende taggen, damit sie einen Korrekturabzug standardmäßig freigeben. Sie können Benutzende auch taggen, um einen Korrekturabzug unabhängig vom Profil der Korrekturabzugsberechtigung oder von der Rolle des Korrekturabzugs freizugeben, wenn Sie der Inhaber oder Ersteller des Korrekturabzugs sind. Sie können Benutzern mit einem niedrigeren Profil für Korrekturabzugsberechtigungen oder Korrekturabzugsrollen die Möglichkeit geben, bei der Erstellung eines Korrekturabzugs einen Korrekturabzug für andere Benutzer freizugeben. Weitere Informationen finden Sie im Abschnitt [Konfigurieren des Workflows und Hinzufügen von Reviewern](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) im Artikel [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Sie können einen externen Mitarbeiter nur dann mit seiner E-Mail-Adresse taggen, wenn einer der folgenden Punkte zutrifft:>
>* Ein(e) Benutzende(r) im Workfront-Konto Ihres Unternehmens hat die E-Mail-Adresse des/r Mitwirkenden zuvor zu einem Korrekturabzug hinzugefügt.
>* Der Mitarbeiter hat die E-Mail-Adresse verwendet, um einen Testversand im Workfront-Konto Ihres Unternehmens zu abonnieren.
>

So taggen Sie jemanden und geben einen Korrekturabzug in einem Kommentar frei:

1. Wenn Sie einen Korrekturabzug kommentieren, geben Sie ein Zeichen (@) gefolgt vom Namen oder der E-Mail-Adresse der Person ein. Wenn Sie mit der Eingabe beginnen, werden verfügbare Namen in einer Dropdown-Liste angezeigt.
1. Wählen Sie den Namen der Person aus, wenn Sie ihn in der Dropdown-Liste sehen.

   >[!TIP]
   >
   >Wenn Sie die Dropdown-Liste schließen möchten, ohne jemanden auszuwählen, können Sie die **Esc**-Taste drücken oder auf eine beliebige Stelle außerhalb der Liste klicken.

1. Wiederholen Sie die Schritte 1 bis 2 für alle anderen Benutzer, die Sie im Kommentar taggen möchten.
1. Schließen Sie den Kommentar ab und klicken Sie dann auf **Posten**.
1. (Bedingt) Wenn Sie eine Person getaggt haben, die dem Korrekturabzug noch nicht hinzugefügt wurde, geben Sie für jeden Benutzer, der in dem angezeigten Feld aufgeführt ist, eine **Rolle des** und **E-Mail-**). Klicken Sie dann auf **Personen hinzufügen und einen Kommentar posten**.

   ![Personen zum Korrekturabzug hinzufügen](assets/add-people-to-proof-350x220.png)

   Informationen zu Korrekturabzug-Rollen finden Sie unter . Informationen zu E-Mail-Warnhinweisen bei Korrekturabzügen finden Sie im Abschnitt im Artikel [Konfigurieren von E-Mail-Benachrichtigungseinstellungen in Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Wenn der Korrekturabzug einen automatisierten Workflow hat, werden die Benutzenden, die Sie taggen, zu dem Schritt hinzugefügt, an dem Sie sich befinden. Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Jeder, den Sie taggen, erhält eine Benachrichtigungs-E-Mail zu Ihrem Korrekturabzugskommentar, unabhängig von den Einstellungen für die E-Mail-Benachrichtigung zum Korrekturabzug, die er verwendet:

   * Wenn der/die Benutzende eine E-Mail mit einer täglichen oder stündlichen Zusammenfassung erhält, sendet Workfront die Benachrichtigung separat. Außerdem enthält die E-Mail mit der Zusammenfassung Informationen zu Ihrem Korrekturabzugskommentar.
   * Wenn der/die Benutzende Warnhinweise für alle Aktivitäten oder für Antworten auf seine/ihre Kommentare erhält, ersetzt die Benachrichtigung die Benachrichtigungen über diese Kommentare und Antworten.

Informationen zu anderen Möglichkeiten, Benutzende zu einem Korrekturabzug hinzuzufügen, finden Sie unter [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
