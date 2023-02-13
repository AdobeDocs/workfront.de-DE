---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Sichern Sie Ihre [!DNL Workfront Proof] Daten
description: Sie können eine Sicherungskopie aller Daten anfordern in [!DNL Workfront Proof] die Backup-Funktion verwenden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 0%

---

# Sichern Sie Ihre [!DNL Workfront Proof] Daten

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

## Einführung in Backups

Sie können eine Sicherungskopie aller Daten anfordern in [!DNL Workfront Proof] die Backup-Funktion verwenden.

Das Backup wird Ihnen als ZIP-Datei bereitgestellt. Es enthält einen XML-Export all Ihrer Daten (einschließlich Kommentaren und Antworten für alle Versionen aller Testsendungen). Sie enthält jedoch nicht die Originaldateien, die Sie als Testsendungen hochgeladen haben.

Jede Backup-ZIP-Datei, die für den Download erstellt wurde, hat einen eindeutigen Dateinamen, z. B.:

9789_05_05_2011_61703.zip

Der Dateiname in diesem Beispiel enthält die folgenden Informationen:

* 9789 ist Ihr [!DNL Workfront Proof] Kontokennung
* 05_05_2011 ist das Erstellungsdatum, 5. Mai 2011
* 61703 ist eine zufällige systemzugewiesene Nummer.

Diese Namenskonvention erleichtert es Ihnen, alle Backup-ZIP-Dateien an einem zentralen Speicherort auf Ihrem Computer zu speichern und genau zu wissen, wann jedes Backup für Sie erstellt wurde.

Die [!UICONTROL Backup] -Funktion können Sie festlegen, wie Ihre Ressourcen verwendet werden sollen:

* Ermöglicht Ihnen, Speicherplatz freizugeben, ohne Ihre aktiven oder archivierten Testsendungen zu verlieren. Sie können eine Sicherung anfordern, die Testsendungen löschen und dann die [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Ermöglicht den Zugriff auf alle Dateien, die Sie ursprünglich in hochgeladen haben [!DNL Workfront] Testversand. Sie können sie mit dem [!UICONTROL Originaldatei herunterladen] vor dem Löschen der Testsendungen.

>[!NOTE]
>
>Beachten Sie bei der Verwendung von Backups Folgendes:
>
>* Backups sind für Enterprise- und Unlimited-Pläne verfügbar. Bitte kontaktieren Sie uns [Vertriebsteam](mailto:sales@proofhq.com) für ein Anführungszeichen.
>* Der Datenkodierungstyp ist standardmäßig auf UTF-8 festgelegt. Diese Einstellung wird empfohlen. Dies ist der Kodierungstyp, der am häufigsten von Internetanwendungen verwendet wird.
>* Sie können nur eine [!DNL backup] auf einmal. Wenn Ihre ZIP-Backup-Datei verarbeitet wird, wird der Link Neues Backup anfordern auf der Registerkarte Sicherungen nicht angezeigt und die angezeigte Meldung bleibt unverändert. Informationen zum Anfordern einer Sicherung finden Sie unter [Eine neue Datensicherung anfordern in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>




## Daten sichern

1. Klicken **[!UICONTROL Kontoeinstellungen]** in der oberen rechten Ecke des [!DNL Workfront Proof] -Schnittstelle. (1)
1. Klicken Sie auf **[!UICONTROL Backups]** Registerkarte. (2)
1. Klicken Sie auf **[!UICONTROL Neues Backup anfordern]** link (3)

Wenn das Backup fertig ist, geschieht Folgendes:

* Sie erhalten eine E-Mail von [!DNL Workfront Proof] Sie darüber informieren (&quot;Ihr [!DNL Workfront Proof] Backup ist bereit&quot;). Die E-Mail enthält einen Download-Link für Ihre Backup-Daten.
* Die [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Auf der Registerkarte &quot;Sicherung&quot;wird ein Download-Link für Ihre Sicherungsdaten angezeigt.
* Der Link Neues Backup anfordern (3) wird erneut auf der Registerkarte Sicherungen angezeigt

Ihre Daten können als ZIP-Datei heruntergeladen werden. Sie können die .zip-Backup-Datei entweder von der Benachrichtigungs-E-Mail oder im [!UICONTROL Kontoeinstellungen], wie in den folgenden Abschnitten beschrieben:

* [Herunterladen der .zip-Backup-Datei aus Ihrer E-Mail-Benachrichtigung](#downloading-your-backup-zip-file-from-your-email-notification)
* [Herunterladen der ZIP-Backup-Datei aus den Kontoeinstellungen](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## Herunterladen der .zip-Backup-Datei aus Ihrer E-Mail-Benachrichtigung {#downloading-your-backup-zip-file-from-your-email-notification}

Wenn Ihre .zip-Backup-Datei zum Herunterladen bereit ist, erhalten Sie eine E-Mail von [!DNL Workfront Proof] mit der Betreffzeile &#39;Your [!DNL Workfront Proof] Backup ist bereit.&quot;

So laden Sie die .zip-Sicherungsdatei aus der E-Mail herunter:

1. Klicken Sie auf den Downloadlink in der E-Mail.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   Wenn Sie derzeit nicht angemeldet sind bei [!DNL Workfront Proof], öffnet sich ein neues Browser-Fenster und zeigt die Anmeldeseite an.

## Herunterladen der ZIP-Backup-Datei aus den Kontoeinstellungen {#downloading-your-backup-zip-file-from-the-account-settings}

Wenn Ihre .zip-Backup-Datei heruntergeladen werden kann, muss die [!UICONTROL Backup] gibt dies an, indem ein Downloadlink angezeigt wird. Darüber hinaus wird die [!UICONTROL Neues Backup anfordern] erneut angezeigt.

1. Klicken **[!UICONTROL Kontoeinstellungen]** in der oberen rechten Ecke des [!DNL Workfront Proof] -Schnittstelle. (1)
1. Klicken Sie auf **[!UICONTROL Backups]** Registerkarte. (2)\
   Wenn keine Benutzer in Ihrem Konto Sicherungen angefordert haben, wird die [!UICONTROL Backups] gibt an, dass Sie keine Sicherungen haben. Wenn ein Benutzer eine Sicherung angefordert hat, werden auf der Registerkarte das Erstellungsdatum und der Downloadlink für die letzte Sicherung angezeigt.

1. Klicken Sie auf **[!UICONTROL Backup herunterladen]** Link. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Es wird ein Bildschirm &quot;Datei herunterladen&quot;angezeigt, in dem Sie gefragt werden, ob Sie die Download-Datei öffnen oder speichern möchten.

1. Klicken **[!UICONTROL Speichern]** und wählen Sie dann den Speicherort auf Ihrem Computer aus, auf dem Sie die .zip-Sicherungsdatei speichern möchten.\
   Die Meldung, die das Datum des letzten Backups angibt, bleibt am unteren Rand der [!UICONTROL Backup] bis zum nächsten Mal, wenn Sie ein Backup anfordern. Der Link Backup herunterladen gilt für dieses letzte Backup. Immer [!UICONTROL Neues Backup anfordern] angezeigt wird, können Sie darauf klicken, um ein weiteres Backup anzufordern.

## Grundlegendes zu den Dateien in Ihrer .zip-Sicherungsdatei

Ihre .zip-Backup-Datei enthält sieben CSV-Dateien (kommagetrennte Werte oder kommagetrennte Dateien), die Informationen aus Ihren aktiven und archivierten Testsendungen bis zum Zeitpunkt der Datensicherung enthalten:

* comments.csv - enthält Kommentare zu Testsendungen
* comment_responses.csv - enthält Antworten auf Kommentare zu Testsendungen organization.csv - einschließlich numerischer Kennung und des Namens Ihrer Organisation (Ihres Kontos)
* contact.csv - enthält numerische Kennung, Namen und Organisation für jeden Kontakt
* files.csv - enthält Informationen von der Seite mit den Testversanddetails oder der Seite mit den Dateidetails bei Testsendungen oder Dateien, die in hochgeladen wurden. [!DNL Workfront Proof]
* recipients.csv - enthält numerische ID, Rolle und Entscheidungen jeder Person, die als Prüfer, Prüfer und Genehmiger angegeben wird, usw., wenn Testsendungen zur Überprüfung hochgeladen werden [!DNL Workfront Proof]
* users.csv - enthält numerische IDs und Namen aller Benutzer im Konto

Sie können diese Dateien aus der .zip-Backup-Datei mit dem von Ihnen verwendeten ZIP-Dienstprogramm extrahieren und dann am gewünschten Speicherort auf Ihrem Computer speichern. Nachdem Sie die ZIP-Datei gespeichert und die einzelnen CSV-Dateien extrahiert haben, können Sie die Informationen nach Bedarf für die interne Aufbewahrung von Datensätzen bearbeiten.

Jede Backup-ZIP-Datei, die auf Ihre Anfrage erstellt wird, hat einen eindeutigen Namen, der das Erstellungsdatum der Sicherung enthält, aber die CSV-Dateien, die in jeder Backup-ZIP-Datei enthalten sind, haben immer die gleichen Namen. Möglicherweise möchten Sie eine der folgenden Methoden verwenden, um sicherzustellen, dass Ihre Backup-Dateien sich voneinander unterscheiden:

* Erstellen Sie für jede Backup-ZIP-Datei und die CSV-Dateien, die Sie daraus extrahieren, einen neuen Ordner.
* Benennen Sie jede einzelne CSV-Datei um und fügen Sie das Sicherungsdatum bei, wenn Sie sie aus der ZIP-Datei extrahieren.

>[!NOTE]
>
>Wenn [!DNL Microsoft Excel] auf Ihrem Computer installiert ist, listet Ihr Extrahierungsprogramm möglicherweise den Dateityp für die einzelnen CSV-Dateien auf als [!DNL Microsoft Office Excel] Datei mit kommagetrennten Werten. Sie können eine extrahierte CSV-Datei mit [!DNL Excel] und speichern Sie die Datei als [!DNL Excel] Arbeitsmappe (&#42;.xlsx) oder einem anderen Dateityp.
