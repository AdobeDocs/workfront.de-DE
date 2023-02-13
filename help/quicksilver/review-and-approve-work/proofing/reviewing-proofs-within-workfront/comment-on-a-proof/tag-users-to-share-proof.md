---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Benutzer zum Freigeben eines Testversands taggen
description: Wenn Sie einen Testversand im Testversand-Viewer kommentieren, können Sie andere Benutzer mit Tags versehen, um ihnen per E-Mail auf Ihren Kommentar aufmerksam zu machen und ihn zum Testversand-Workflow hinzuzufügen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Benutzer zum Freigeben eines Testversands taggen

Wenn Sie einen Testversand im Testversand-Viewer kommentieren, können Sie andere Benutzer mit Tags versehen, um ihnen per E-Mail auf Ihren Kommentar aufmerksam zu machen und ihn zum Testversand-Workflow hinzuzufügen.

Beim Tagging von Benutzern in Kommentaren zu einem Testversand können die Benutzer, die Sie taggen können, abhängig von verschiedenen Faktoren wie individuellen Benutzerberechtigungen und Ihrer Mitgliedschaft in der Organisation unterschiedlich sein:

* Wenn Sie der Ersteller oder Eigentümer eines Testversands sind oder bestimmte Berechtigungen aktiviert haben, können Sie Benutzer außerhalb des Testversand-Workflows taggen und den Testversand für sie freigeben.
* Wenn Sie als externer Benutzer zum Testversand hinzugefügt wurden und Mitglied einer anderen Umgebung mit einem anderen Testversandkonto sind, können Sie nur diese Benutzer aus Ihrer ursprünglichen Umgebung mit Tags versehen. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Zugriffsanforderungen {#access-requirements}

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proof role</td> 
   <td>Autor, Moderator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Supervisor oder Administrator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Benutzer zum Freigeben eines Testversands taggen

Benutzer mit der Rolle &quot;Testberechtigungsprofil&quot;oder &quot;Testversand&quot;, die im Abschnitt [Zugriffsanforderungen](#access-requirements) -Abschnitt oben können Benutzer taggen, um standardmäßig einen Testversand freizugeben. Sie können Benutzer auch so taggen, dass sie einen Testversand unabhängig vom Profil für Testberechtigungen oder der Rolle Testversand freigeben können, wenn Sie Testversand-Besitzer oder -Ersteller sind. Sie können Benutzern mit den Rollen &quot;Profil für Testversandberechtigungen&quot;oder &quot;Testversand&quot;die Möglichkeit geben, Benutzer beim Erstellen eines Testversands mit Tags für einen Testversand zu versehen. Weitere Informationen finden Sie unter [Workflow konfigurieren und Überprüfer hinzufügen](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) im Abschnitt [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) Artikel.

>[!NOTE]
>
>Sie können einen externen Mitarbeiter nur dann mit seiner E-Mail-Adresse taggen, wenn eine der folgenden Voraussetzungen erfüllt ist:>
>* Ein Benutzer im Workfront-Konto Ihres Unternehmens hat die E-Mail-Adresse des Mitarbeiters bereits einem Testversand hinzugefügt.
>* Der Mitarbeiter hat zuvor die E-Mail-Adresse verwendet, um einen Testversand im Workfront-Konto Ihres Unternehmens zu abonnieren.
>


So taggen Sie jemanden und geben einen Testversand in einem Kommentar frei:

1. Wenn Sie einen Testversand kommentieren, geben Sie ein at -Zeichen (@) ein, gefolgt vom Namen oder der E-Mail-Adresse der Person. Wenn Sie mit der Eingabe beginnen, werden die verfügbaren Namen in einer Dropdown-Liste angezeigt.
1. Wählen Sie den Namen der Person aus, wenn Sie ihn in der Dropdown-Liste sehen.

   >[!TIP]
   >
   >Wenn Sie die Dropdownliste schließen möchten, ohne einen anderen auszuwählen, können Sie die **Esc** oder klicken Sie auf eine beliebige Stelle außerhalb der Liste.

1. Wiederholen Sie die Schritte 1 bis 2 für alle anderen Benutzer, die Sie im Kommentar taggen möchten.
1. Schließen Sie den Kommentar ab und klicken Sie auf **Post**.
1. (Bedingt) Wenn Sie Personen mit Tags versehen haben, die noch nicht zum Testversand hinzugefügt wurden, geben Sie eine **Proof role** und **E-Mail-Warnungen** für jeden Benutzer festlegen, der im angezeigten Feld aufgeführt ist, und klicken Sie dann auf **Personen hinzufügen und Kommentare posten**.

   ![](assets/add-people-to-proof-350x220.png)

   Informationen zu Testversandrollen finden Sie unter . Informationen zu Testversand-E-Mail-Warnungen finden Sie im Abschnitt im Artikel [E-Mail-Benachrichtigungseinstellungen in Workfront Testversand konfigurieren](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Wenn der Testversand über einen automatisierten Workflow verfügt, werden die Benutzer, die Sie taggen, der Bühne hinzugefügt, in der Sie sich befinden. Weitere Informationen finden Sie unter [Übersicht über den automatisierten Workflow](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Jeder, den Sie taggen, erhält eine Benachrichtigungs-E-Mail über Ihren Testversandkommentar, unabhängig von den von ihm verwendeten Benachrichtigungseinstellungen beim Testversand per E-Mail:

   * Wenn der Benutzer eine tägliche Zusammenfassung oder eine stündliche Zusammenfassungs-E-Mail erhält, sendet Workfront die Benachrichtigung separat und enthält in der Zusammenfassungs-E-Mail Informationen zu Ihrem Testkommentar.
   * Wenn der Benutzer Warnhinweise für alle Aktivitäten oder für Antworten auf seine Kommentare erhält, ersetzt die Benachrichtigung die Benachrichtigungen über diese Kommentare und Antworten.

Weitere Informationen zu anderen Möglichkeiten, Benutzer zu einem Testversand hinzuzufügen, finden Sie unter [Freigeben eines Testversands in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
