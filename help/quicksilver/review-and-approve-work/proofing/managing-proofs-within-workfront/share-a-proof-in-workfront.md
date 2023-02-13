---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Freigeben eines Testversands in Adobe Workfront
description: Sie können ein freigegebenes Dokument in Adobe Workfront freigeben, indem Sie es freigeben oder dem Testversand Benutzer hinzufügen.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Freigeben eines Testversands in Adobe Workfront

Sie können ein freigegebenes Dokument in Adobe Workfront freigeben, indem Sie es freigeben oder dem Testversand Benutzer hinzufügen.

Wenn Sie den Testversand wie in diesem Artikel beschrieben freigeben, hat Ihr Empfänger denselben Zugriff auf das Dokument und den Testversand. Zusätzlich können Sie die Validierung des Testversands beim Empfänger anfordern.

>[!TIP]
>
>Sie können einen Testversand auch aus dem Testversand-Viewer freigeben. Anweisungen finden Sie unter [Freigeben eines Testversands aus dem Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Select oder Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle "Testversand"</td> 
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Testversand-Link freigeben

Durch die Freigabe eines Testversand-Links erhalten Workfront-Benutzer, die Zugriff darauf erhalten. Benutzer können den Testversand kommentieren und E-Mail-Benachrichtigungen für den Testversand mit ihren Workfront-Anmeldedaten abonnieren. Benutzer, die keine Prüfung durchführen, können mit einer E-Mail-Adresse und einem Anzeigenamen Kommentare abgeben und sich für diese anmelden.

>[!IMPORTANT]
>
>Die Einstellung Freigeben eines Testversands über öffentliche URLs oder Einbettungscodes zulassen muss aktiviert sein.

1. Wählen Sie das Dokument aus, das den Testversand enthält, den Sie für Benutzer freigeben möchten.

   Sie können nur ein Dokument auswählen. Sie können den Link nicht für mehrere Dokumente gleichzeitig freigeben.

1. Klicken **Freigeben** > **Testlink**.
1. Im **Link zum Testversand** das angezeigt wird, führen Sie einen der folgenden Schritte aus:

   * Um den Link in die Zwischenablage zu kopieren, klicken Sie auf **Link kopieren**.

      Sie können den Link nun über ein Tool eines Drittanbieters verteilen, z. B. einen Chat oder eine E-Mail-Anwendung.

   * Gehen Sie wie folgt vor, um den Link direkt von Adobe Workfront per E-Mail zu versenden:

      1. Im **Oder E-Mail-Link zu** eingeben und den Namen Ihres Empfängers auswählen. Oder geben Sie die E-Mail-Adresse eines externen Benutzers an, für den Sie freigeben möchten.

         >[!NOTE]
         >
         >Wenn bei der Freigabe eines Testversands eine Alias-E-Mail angezeigt wird, erstellen Sie keinen neuen Gastbenutzer, indem Sie die ursprüngliche E-Mail eingeben, sofern eine Alias-E-Mail vorhanden ist.

      1. Wählen Sie aus den folgenden Optionen aus:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Öffentlichen Link senden</td>
            <td><p>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, über die Benutzer zum Testversand innerhalb des von ihnen verwendeten Testversand-Viewers weitergeleitet werden und der Zugriff auf die Ansicht gewährt wird.</p><p>Wenn <strong>Testversand über öffentliche URL oder Einbettungscode abonnieren</strong> für den Testversand deaktiviert ist, können sich Benutzer mit ihren Workfront-Anmeldedaten anmelden, um dem Testversand Kommentare hinzuzufügen. Ist diese Option aktiviert, kann jeder, der seine E-Mail-Adresse und seinen Namen (kein Passwort erforderlich) angibt, den Testversand signieren und Kommentare hinzufügen.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Downloadlink senden</td>
            <td>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, über die Benutzer zu einer Download-Seite weitergeleitet werden, auf der Dateidetails, Dateiname und Dateigröße sowie die Datei inline angezeigt werden. Benutzer können auf der Downloadseite auf den Link Download klicken, um die Datei herunterzuladen.</td>
           </tr>
           <tr>
            <td role="rowheader">Benutzerdefinierte Nachricht hinzufügen</td>
            <td>Hiermit können Sie einen benutzerdefinierten Betreff und Text für die E-Mail-Benachrichtigung angeben.</td>
           </tr>
          </tbody>
         </table>

      1. Klicken **Senden**.

         Ihre Empfänger erhalten eine E-Mail-Benachrichtigung mit Informationen zum Testversand und den von Ihnen ausgewählten Schaltflächen.

         ![](assets/proof-share-email-350x87.png)

## Benutzer zu Testversand hinzufügen

Sie können einen beliebigen Workfront-Benutzer zum Testversand hinzufügen, wenn Sie für den Testversand über die Berechtigung zum Bearbeiten verfügen. Wenn der Testversand mehrere Phasen umfasst, fügen Sie den Benutzer einer einzelnen Phase hinzu

>[!NOTE]
>
>Beachten Sie Folgendes, wenn Sie einen veralteten Workfront-Plan verwenden, in dem die Prüfung für einen Benutzer aktiviert und deaktiviert werden kann:
>
>* Für Ihre Empfänger ist die Aktivierung des Testversands nicht erforderlich.
>* Wenn der automatisierte Workflow aktiviert ist und Sie einen Benutzer zum Testversand hinzufügen, für den die Testversand-Funktion in Workfront nicht aktiviert ist, wird im automatisierten Workflow eine neue Phase erstellt. Der Benutzer, den Sie hinzufügen, wird automatisch zu dieser neuen Phase hinzugefügt, wenn er den Testversand zum ersten Mal anzeigt. (Weitere Informationen finden Sie unter [Übersicht über den automatisierten Workflow](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).
>


### Hinzufügen von Benutzern zu einem vorhandenen Testversand über die Registerkarte &quot;Dokumente&quot;

1. Wählen Sie das Dokument aus, das den Testversand enthält, dem Sie Benutzer hinzufügen möchten.
1. Wenn der Testversand keinen automatisierten Workflow (Phasen) aufweist, klicken Sie auf die Schaltfläche **Mehr** in der oberen rechten Ecke des Bereichs Phase 1 und klicken Sie dann auf **Freigeben** im Dropdown-Menü.

   Oder

   Wenn der Testversand einen automatisierten Workflow aufweist, klicken Sie auf die Schaltfläche **Mehr** in der oberen rechten Ecke der Phase, in der Sie den Validierer hinzufügen möchten, klicken Sie auf **Freigeben** im Dropdown-Menü.

1. Im **Diese Version freigeben** Feld, das angezeigt wird, unter **Freigeben**, geben Sie den Namen oder die E-Mail-Adresse eines Benutzers ein, für den Sie den Testversand freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

1. (Optional) Wiederholen Sie diesen Schritt, um dem Testversand mehrere Benutzer hinzuzufügen.
1. (Optional) Legen Sie einen Termin für die Validierungsverantwortlichen fest.
1. (Optional) Stellen Sie sicher, dass **Personen per E-Mail benachrichtigen** ausgewählt ist, wenn Sie den Validierungsverantwortlichen mitteilen möchten, dass sie zum Testversand hinzugefügt wurden.
1. (Optional) **Benutzerdefinierte Nachricht hinzufügen** an die E-Mail.
1. Wenn Sie alle Validierungsverantwortlichen hinzugefügt haben, klicken Sie auf **Freigeben**.

### Hinzufügen von Benutzern zu einem vorhandenen Testversand aus dem Testversand-Viewer

Sie können Benutzer zu einem Testversand hinzufügen, während Sie einen Testversand im Web Proofing Viewer und im Desktop Proofing Viewer durchführen.

Weitere Informationen finden Sie unter [Freigeben eines Testversands durch Hinzufügen von Benutzern](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) im Artikel [Freigeben eines Testversands aus dem Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Bericht über die Validierung von Testsendungen

Sie können einen Bericht erstellen, der Berichte zu den in Workfront freigegebenen Testversandgenehmigungen enthält. Dieser Bericht enthält die folgenden Informationen zur Testversandvalidierung in Ihrem System:

* Dokument, das zur Genehmigung eingereicht wurde
* Name des Genehmigers
* Testversion
* Korrekturabzugs-ID
* Erstellungsdatum des Testversands

Sie können auf diese Validierung zugreifen, wenn Sie einen Bericht basierend auf einem Objekt erstellen, wie in [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Weitere Informationen zum Objektbericht für Testsendungen finden Sie in der [Berichte zu Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) Abschnitt in [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Freigegebenen Testversand genehmigen

Wenn ein Benutzer Sie zu einem Testversand hinzufügt und entweder die Rolle &quot;Genehmiger&quot;oder die Rolle &quot;Genehmiger und Genehmiger&quot;mithilfe des automatisierten Workflows gewährt, wird die Genehmigungsanfrage auf der Registerkarte &quot;Genehmigungen&quot;in Ihrer Startseite oder im Arbeitsbereich angezeigt. Sie können den Testversand ansehen und direkt in Workfront eine Validierungsentscheidung für den Testversand treffen.

Informationen dazu, wie Sie Genehmigungsentscheidungen im Bereich &quot;Meine Arbeit&quot;treffen, finden Sie unter [Genehmigen Sie die Arbeit vom Startbereich aus.](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) oder [Validierung der Arbeit](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [Validierung der Arbeit](../../../review-and-approve-work/manage-approvals/approving-work.md).
