---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generieren von Testsendungen in  [!DNL Workfront Proof]
description: Mit Workfront Proof können Sie Testsendungen aus Dokumenten oder Websites erstellen und diese für andere freigeben.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: ec7dc62e23aae7fe09532da47a40438223c32766
workflow-type: tm+mt
source-wordcount: '2257'
ht-degree: 0%

---

# Testsendungen in [!DNL Workfront Proof] generieren

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Mit [!DNL Workfront Proof] können Sie Testsendungen aus Dokumenten oder Websites erstellen und diese für andere freigeben. Die folgenden Schritte beschreiben die verschiedenen verfügbaren Konfigurationsoptionen:

## Erstellen eines Testversands für ein Dokument

1. Führen Sie einen der folgenden Schritte aus, um einen neuen Testversand zu erstellen und die Seite [!UICONTROL Neuer Testversand] anzuzeigen:

   * Klicken Sie auf die grüne Schaltfläche **[!UICONTROL Neuer Testversand]** in der oberen linken Ecke einer beliebigen Seite.
   * Klicken Sie im Bereich **[!UICONTROL Dashboard]** auf der Registerkarte **[!UICONTROL Übersicht]** auf den Link **[!UICONTROL Neuer Testversand]** .

   * Senden über Dropzone (Enterprise-Funktion).
   * Die Seite **[!UICONTROL Neuer Testversand]** wird angezeigt.

1. Fügen Sie zum Testen eines oder mehrerer Dokumente die zu prüfenden Dokumente auf eine der folgenden Arten hinzu (wiederholen Sie diesen Vorgang, um mehrere zu prüfende Dokumente hinzuzufügen):

   * Ziehen Sie ein Dokument aus Ihrem Dateisystem in den Drag-and-Drop-Bereich im Bereich **[!UICONTROL Dateien hinzufügen]** .
   * Klicken Sie im Bereich **[!UICONTROL Dateien hinzufügen]** auf den Drag-and-Drop-Bereich und suchen Sie dann nach dem Dokument, das Sie aus dem Dateisystem auf Ihrer Workstation hochladen möchten, und wählen Sie es aus.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Um eine oder mehrere Websites zu testen, geben Sie die URL der Website, die Sie testen möchten, im Bereich **[!UICONTROL Dateien hinzufügen]** an und drücken Sie dann die Eingabetaste **[!UICONTROL 3}.]**

1. (Optional) Wiederholen Sie diesen Vorgang, um mehrere Websites zum Testversand hinzuzufügen.

   Weitere Informationen zum Testen von Websites finden Sie unter [Erstellen eines Testversands für eine URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Optional) Ändern Sie die Dateinamen aller hochgeladenen Dateien:

   1. Bewegen Sie den Mauszeiger über den Dokumentnamen, den Sie in der Dokumentliste im Bereich **[!UICONTROL Dateien hinzufügen]** ändern möchten, und klicken Sie dann auf das Symbol **[!UICONTROL Bearbeiten]** .

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. Geben Sie im Feld **[!UICONTROL Testversand-Name]** einen neuen Namen ein und klicken Sie dann auf **[!UICONTROL Fertig]**.

   1. (Optional) Um alle hochgeladenen Dateien zu löschen, bewegen Sie den Mauszeiger im Bereich **[!UICONTROL Dateien hinzufügen]** über das Dokument, das Sie löschen möchten, und klicken Sie dann auf das Symbol **[!UICONTROL Löschen]** .

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Optional) Aktivieren Sie die Option **[!UICONTROL Alle kompatiblen Dateien in einem Testversand zusammenführen]**.

      **Wenn diese Option aktiviert ist:** Alle statischen Dateien und Websites sind in einem Testversand verfügbar und Sie können bis zu 50 Dateien gleichzeitig hochladen.

      >[!NOTE]
      >
      >Interaktive Dateien, einschließlich Videos und interaktive Websites, können nicht zu einem Testversand kombiniert werden.

      **Wenn diese Option deaktiviert ist:** Alle Dokumente und Websites werden als einzelne Testsendungen generiert und Sie können bis zu 20 Dateien gleichzeitig hochladen.

      So kombinieren Sie alle hochgeladenen Dateien und Websites zu einem Testversand:

      1. Aktivieren Sie die Option &quot;**[!UICONTROL Kombinieren aller kompatiblen Dateien zu einem Testversand]**&quot;.
      1. Geben Sie im Feld **[!UICONTROL Testversand-Name]** einen neuen Namen für den kombinierten Testversand an.
      1. Ordnen Sie im Bereich **[!UICONTROL Dateien hinzufügen]** die enthaltenen Dateien neu an, indem Sie eine Datei in die gewünschte Reihenfolge ziehen. Die Reihenfolge der Dateien entspricht der Seitenreihenfolge des kombinierten Testversands. Weitere Informationen zum Erstellen kombinierter Testsendungen finden Sie unter [Erstellen eines mehrseitigen Testversands](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Optional) Wenn Sie einen automatisierten Workflow mit mehreren Phasen verwenden möchten, wählen Sie im Abschnitt **[!UICONTROL Workflow]** eine der folgenden Optionen aus:

   * **Einfach:** Wählen Sie diese Option, um Benutzer zu bestimmen, die unmittelbar nach der Erstellung auf den Testversand zugreifen möchten. Sie können den Testversand für mehrere Benutzer freigeben.

     Weitere Informationen zum Freigeben eines Testversands finden Sie unter &quot;Hinzufügen von Benutzern zu einem Testversand&quot;in [Freigeben eines Testversands in  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatisiert:** Wählen Sie diese Option, um Inhaltsüberprüfungen und -genehmigungen zu verwalten, wenn komplexe Überprüfungsprozesse vorliegen oder wenn Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden. Mit einem automatisierten Workflow wechselt der Testversand von Phase zu Phase bis zur endgültigen Genehmigung. Die betroffenen Benutzer werden jedes Mal darüber informiert, dass sie eine Genehmigung vorlegen müssen.

     Weitere Informationen zum Erstellen eines automatisierten Workflows finden Sie unter [Einrichten eines Testversands mit einem automatisierten Workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Wählen Sie aus, ob E-Mail-Benachrichtigungen und eine benutzerdefinierte Nachricht an die Benutzer gesendet werden sollen, die Sie im vorherigen Schritt ausgewählt haben:

   * **Empfänger über diesen Testversand benachrichtigen:** Wählen Sie diese Option, um eine E-Mail-Benachrichtigung an Benutzer zu senden. Wenn im Abschnitt **[!UICONTROL Workflow]** die Option **[!UICONTROL Grundlegende Freigabe]** ausgewählt ist, wird beim Erstellen des Testversands eine E-Mail-Benachrichtigung gesendet. Wenn im Abschnitt **[!UICONTROL Workflow]** die Option **[!UICONTROL Automatisierter Workflow]** ausgewählt ist, wird eine E-Mail-Benachrichtigung gesendet, sobald der Testversand in die Phase des automatisierten Workflows gelangt, mit dem der Benutzer verknüpft ist.

   * **Benutzerdefinierte Nachricht hinzufügen:** Wählen Sie diese Option, um eine benutzerdefinierte Nachricht in die Benachrichtigung einzuschließen. Sie können einen Betreff und einen Nachrichtentext angeben. Der Nachrichtentext kann Rich-Text-Formatierungen wie Fett, Aufzählungszeichen und Hyperlinks enthalten.

1. Wählen Sie eine der folgenden Testversandeinstellungen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anmeldung erforderlich - Testversand kann nur für andere Benutzer freigegeben werden</td> 
      <td> <p><strong>Anmeldung erforderlich - Der Testversand kann nur für andere Benutzer freigegeben werden:</strong> Wenn diese Option aktiviert ist, können nur [!DNL Workfront Proof] Benutzer den Testversand anzeigen.</p> <p>Diese Option ist standardmäßig deaktiviert. Jede Person mit der URL kann den Testversand anzeigen.</p> <p>Wenn diese Option ausgewählt ist:</p> 
       <ul> 
        <li>Benutzer können sich nur dann beim Testversand anmelden, wenn sie zum Testversand hinzugefügt wurden.</li> 
        <li>Abonnements können nicht aktiviert werden.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für diesen Nachweis ist nur eine Entscheidung erforderlich</td> 
      <td> <p>Wenn diese Option ausgewählt ist, wird die Überprüfung abgeschlossen, nachdem einer der Entscheidungsträger seine Entscheidung getroffen hat.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden</td> 
      <td>Benutzer müssen ihren Benutzernamen und ihr Kennwort zum Zeitpunkt der Entscheidung über einen Testversand angeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sperren des Testversands, wenn alle erforderlichen Entscheidungen getroffen werden</td> 
      <td> <p><strong></strong> Wenn diese Einstellung aktiviert ist, wird der Testversandstatus gesperrt, nachdem alle Entscheidungen getroffen wurden. Der Status wird automatisch von entsperrt in gesperrt geändert, wenn der endgültige Genehmiger seine Entscheidung trifft.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Originaldatei herunterladen</td> 
      <td> <p><strong></strong> Wenn diese Option aktiviert ist, können die validierungsverantwortlichen Benutzer die Originaldatei herunterladen, aus der der Testversand erstellt wurde.</p> <p>Wenn diese Option deaktiviert ist, ist das Symbol Herunterladen nicht mehr sichtbar.<br>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigeben eines Testversands über eine öffentliche URL oder einen Einbettungscode</td> 
      <td>Wenn diese Option aktiviert ist, kann der Testversand über eine öffentliche URL oder einen Einbettungscode freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testversand über eine öffentliche URL oder einen Einbettungscode abonnieren</td> 
      <td> <p>Wenn diese Option aktiviert ist, können Personen, die dem Testversand nicht explizit hinzugefügt wurden, den Testversand abonnieren. Die Person, die den Testversand abonniert, erhält die Rolle und E-Mail, die Sie in den folgenden Einstellungen definieren:</p> 
       <ul> 
        <li><strong>Abonnentenrolle</strong>: Die Standardrolle für den Testversand, die allen Validierern zugewiesen ist, die den Testversand abonnieren.</li> 
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten</strong>: Der Standard-E-Mail-Warnhinweis, der allen Validierern zugewiesen wird, die den Testversand abonnieren.</li> 
        <li> <p><strong>Zugriffsnachweis über E-Mail-Link erforderlich für </strong>: Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Testversand erhält. Sie können "<strong>Keine E-Mail</strong>"(E-Mail-Link ist nicht erforderlich, um auf den Testversand zuzugreifen), "<strong>Nur E-Mail-Benachrichtigung versenden</strong>"(der Abonnent erhält einen Link zum Testversand per E-Mail ohne Überprüfung) oder "<strong>E-Mail zur Validierung und zum Testversand"</strong>"(Abonnenten erhalten per E-Mail einen Link und müssen auf den entsprechenden Link klicken, um einen Testversand zu öffnen. E-Mail-Adresse, auf die sie Zugriff haben).</p> <p>Hinweis: Wenn die Testsendungen einen automatisierten Workflow zugeordnet haben, generieren alle Abonnements Bestätigungs-E-Mails an den Testversand-Inhaber, sodass dieser entscheiden kann, zu welcher Stufe die Person hinzugefügt werden soll.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Testversand erstellen]**.

   Workfront beginnt mit der Erstellung eines Testversands der ausgewählten Dokumente oder Websites. Je nach Dateigröße und Typ variiert die Verzögerung beim Hochladen eines Dokuments. Seien Sie geduldig, da die Erzeugung größerer Dateien länger dauert. Sie können von der Seite weg navigieren und Workfront generiert weiterhin Ihre -Datei. Die maximale Größe für den Datei-Upload beträgt 4 GB.

   Nachdem der Testversand erstellt wurde, klicken Sie auf **[!UICONTROL Zum Testversand wechseln]** , um das Testversand-Tool zu starten.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Das Dokument wird im Testwerkzeug angezeigt.

   Benutzer, für die die Testversandfunktion nicht aktiviert wurde, können das Dokument weiterhin ansehen und Kommentare zum Testversand abgeben.

## Erstellen eines Testversands für eine URL {#generate-a-proof-for-a-url}

Sie können zum ersten Mal einen Testversand für eine URL erstellen. Sie können auch eine neue Version eines URL-Testversands generieren, bei dem zuvor ein Testversand erstellt wurde.

>[!NOTE]
>
>Sie können nur dann einen interaktiven Testversand für eine URL generieren, wenn Ihre [!DNL Workfront] -Umgebung in ein [!DNL Workfront Proof] Premium -Konto integriert ist. Wenden Sie sich an Ihren Systemadministrator, wenn Sie die in diesem Abschnitt beschriebenen Testsendungen nicht verwenden können.

So generieren Sie einen Testversand für eine URL:

1. Führen Sie einen der folgenden Schritte aus, um einen neuen Testversand zu erstellen und die Seite [!UICONTROL Neuer Testversand] anzuzeigen:

   * Klicken Sie auf die grüne Schaltfläche **[!UICONTROL Neuer Testversand]** in der oberen linken Ecke einer beliebigen Seite.
   * Klicken Sie im Bereich **[!UICONTROL Dashboard]** auf der Registerkarte **[!UICONTROL Übersicht]** auf den Link **[!UICONTROL Neuer Testversand]** .

   * Senden über Dropzone (Enterprise-Funktion).

1. (Bedingt) Erstellen Sie auf der angezeigten Seite **[!UICONTROL Neuer Testversand]** eine neue Version eines vorhandenen Testversands:

   1. Wählen Sie den URL-Testversand aus, dem Sie eine neue Version hinzufügen möchten.
   1. Klicken Sie oben auf der Seite auf die Schaltfläche **[!UICONTROL Neue Version]** .

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Geben Sie auf der angezeigten Seite Neue Testversand-Version die URL der Website, die Sie testen möchten, im Bereich **[!UICONTROL Dateien hinzufügen]** an und drücken Sie dann die Eingabetaste **[!UICONTROL 3}.]**

1. (Optional) Wiederholen Sie diesen Vorgang, um mehrere Websites zum Testversand hinzuzufügen.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Klicken Sie im Bereich **[!UICONTROL Dateien hinzufügen]** auf die Website in der Dokumentliste.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Geben Sie einen **[!UICONTROL Testversand-Namen]** für den Testversand an.

   Standardmäßig ist der Testversand-Name mit der Site-URL identisch.

1. Wählen Sie die Optionen **[!UICONTROL Site-Inhalte verarbeiten]** aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Screenshot "Capture"</td> 
      <td>Erstellt einen Testversand eines statischen Bildes auf der Titelseite der URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interaktiv</td> 
      <td> <p>Erstellt einen Testversand, der es Benutzern ermöglicht, auf der Site zu navigieren, HTML5-Bilder, Flash-Elemente usw. anzuzeigen.</p> <p>Um einen interaktiven Testversand zu erstellen, muss die Website mit einem sicheren Protokoll (https) gehostet werden. Darüber hinaus können Websites, die nicht in einen iframe eingebettet werden können, nicht als interaktiver Testversand generiert werden (die Einschränkungen für die iframe-Einbettung werden von der Website gesteuert, die Sie einbetten möchten).</p> <p>Nach der Erstellung des anfänglichen Testversands kann diese Einstellung beim Erstellen nachfolgender Versionen nicht mehr geändert werden.</p> <p>Weitere Informationen zum interaktiven Testversand finden Sie unter <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Erstellen eines Testversands für interaktive Inhalte</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Screenshot-Auflösung</td> 
      <td> <p>(Diese Option ist für interaktive Testsendungen nicht verfügbar.) Sie können die Auflösung anpassen, in der Ihr Inhalt angezeigt wird, oder mehrere Auflösungen auswählen.</p> <p>Dadurch können Benutzer den Testversand überprüfen, um zu sehen, wie Inhalte auf verschiedenen Geräten wie Smartphones, Tablets und Monitoren angezeigt werden.</p> <p>Wenn Sie mehrere Auflösungen auswählen, wird für jede ausgewählte Auflösung ein separater Testversand erstellt.</p> <p>Wenn Benutzer einen Kommentar zum Testversand abgeben, wird im Kommentar automatisch die aktuelle Bildschirmauflösung angezeigt, um sicherzustellen, dass andere Benutzer wissen, mit welcher Auflösung der Kommentar verknüpft ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suchen nach Unterseiten</td> 
      <td>(Diese Option ist für interaktive Testsendungen nicht verfügbar.) Wählen Sie diese Option, um durch die Seiten der Website zu navigieren. Sie können die Website von der Hauptseite aus auf zwei Ebenen erweitern. Bewegen Sie den Mauszeiger über eine Seite, um die URL der Seite anzuzeigen. Wählen Sie nur die Seiten aus, die Sie testen möchten. Jede ausgewählte Seite wird standardmäßig als einzelner Testversand erstellt. Alternativ können Sie die Option <strong>Zu Testversand kombinieren</strong> aktivieren, um alle ausgewählten Seiten zu einem Testversand zusammenzuführen.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Konfigurieren Sie alle erweiterten Testversandoptionen, z. B. die Freigabe des Testversands, das Hinzufügen eines automatisierten Workflows oder die Einrichtung von Zugriffs- und Abonnementeinstellungen. Weitere Informationen zu diesen Optionen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Testversands innerhalb von  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Einrichten eines Testversands mit einem automatisierten Workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Zugriffs- und Abonnementeinstellungen für einen Testversand konfigurieren](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicken Sie auf **[!UICONTROL Fertig]**.

   Wenn Sie eine neue Version zu einem vorhandenen URL-Testversand hinzufügen, werden alle Optionen, die für den ursprünglichen Testversand oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten. Wenn Sie eine neue Version zu einem vorhandenen URL-Testversand hinzufügen, werden alle Optionen, die für den ursprünglichen Testversand oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten.

1. Klicken Sie auf **[!UICONTROL Testversand erstellen]**.

## Erstellen eines Testversands für interaktive Inhalte {#generate-a-proof-for-interactive-content}

Für die Verwendung dieser Funktion ist ein Pro-Workfront-Plan oder höher erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

Weitere Informationen zu interaktiven Inhalten finden Sie unter [Übersicht über interaktive Inhaltsanalysen](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Hinzufügen interaktiver Inhalte als URL](#add-interactive-content-as-a-url)
* [Hinzufügen interaktiver Inhalte als ZIP-Datei](#add-interactive-content-as-a-zip-file)

### Hinzufügen interaktiver Inhalte als URL {#add-interactive-content-as-a-url}

Informationen zum Hinzufügen eines interaktiven URL-Testversands finden Sie unter [Erstellen eines Testversands für eine URL](#generate-a-proof-for-a-url).

### Hinzufügen interaktiver Inhalte als ZIP-Datei {#add-interactive-content-as-a-zip-file}

1. Bereiten Sie Ihren Inhalt vor, indem Sie eine ZIP-Bundle-Datei erstellen.

   Informationen zu ZIP-Dateispezifikationen mit Bundles finden Sie unter [Informationen zum Vorbereiten interaktiver Inhalte in einer ZIP-Datei für den Testversand](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) im Artikel [Übersicht über interaktive Inhaltsanalysen](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Führen Sie einen der folgenden Schritte aus, um einen neuen Testversand zu erstellen und die Seite [!UICONTROL Neuer Testversand] anzuzeigen:

   * Klicken Sie auf die grüne Schaltfläche **[!UICONTROL Neuer Testversand]** in der oberen linken Ecke einer beliebigen Seite.
   * Klicken Sie im Bereich **[!UICONTROL Dashboard]** auf der Registerkarte **[!UICONTROL Übersicht]** auf den Link **[!UICONTROL Neuer Testversand]** .

   * Senden über Dropzone (Enterprise-Funktion).

1. Ziehen Sie auf der angezeigten Seite **[!UICONTROL Neuer Testversand]** Ihr interaktives ZIP-Bundle in den Bereich **[!UICONTROL Dateien hinzufügen]** .

1. (Optional) Konfigurieren Sie alle erweiterten Testversandoptionen, z. B. die Freigabe des Testversands, das Hinzufügen eines automatisierten Workflows oder die Einrichtung von Zugriffs- und Abonnementeinstellungen. Weitere Informationen zu diesen Optionen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Testversands innerhalb von  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * im Artikel
   * [Zugriffs- und Abonnementeinstellungen für einen Testversand konfigurieren](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicken Sie auf **[!UICONTROL Testversand erstellen]**.

   Workfront beginnt mit der Erstellung eines Testversands des ZIP-Bundles. Je nach Bundle-Größe variiert die Zeitverzögerung beim Hochladen von Dokumenten. Die Erstellung größerer Dateien dauert länger. Sie können von der Seite weg navigieren und Workfront generiert weiterhin Ihre -Datei. Die maximale Größe für den Datei-Upload beträgt 4 GB.

   Nachdem der Testversand erzeugt wurde, können Sie auf die Schaltfläche **[!UICONTROL Zum Testversand wechseln]** klicken, die angezeigt wird, um den Testversand zu öffnen.
