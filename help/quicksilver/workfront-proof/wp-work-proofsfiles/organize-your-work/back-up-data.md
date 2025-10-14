---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 'Sichern Sie Ihre  [!DNL Workfront Proof] '
description: Mit der Backup-Funktion können Sie eine Sicherung aller  [!DNL Workfront Proof]  Daten in anfordern.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# [!DNL Workfront Proof] sichern

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Einführung in Backups

Mit der Sicherungsfunktion können Sie eine Sicherung aller Daten in [!DNL Workfront Proof] anfordern.

Das Backup wird Ihnen als ZIP-Datei bereitgestellt. Es enthält einen XML-Export aller Ihrer Daten (einschließlich Kommentaren und Antworten für alle Versionen aller Korrekturabzüge), jedoch nicht die Originaldateien, die Sie als Korrekturabzüge hochgeladen haben.

Jede Backup-ZIP-Datei, die zum Herunterladen erstellt wurde, verfügt über einen eindeutigen Dateinamen, z. B.:

9789_05_05_2011_61703.zip

Der Dateiname in diesem Beispiel enthält die folgenden Informationen:

* 9789 ist Ihre [!DNL Workfront Proof] Kontokennung
* 05_05_2011 ist das Erstellungsdatum, 5. Mai 2011
* 61703 ist eine zufällige, vom System zugewiesene Zahl

Diese Namenskonvention erleichtert es Ihnen, alle ZIP-Sicherungsdateien an einem einzigen Speicherort auf Ihrem Computer zu speichern und genau zu wissen, wann die Sicherung für Sie erstellt wurde.

Mit [!UICONTROL Backup]-Funktion können Sie entscheiden, wie Sie Ihre Ressourcen verwenden:

* So können Sie Speicherplatz freigeben, ohne Ihre aktiven oder archivierten Korrekturabzüge zu verlieren. Sie können eine Sicherung anfordern, die Testsendungen löschen und dann die Datei [Wiederherstellen und Papierkorb leeren [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Ermöglicht den Zugriff auf alle Dateien, die Sie ursprünglich in [!DNL Workfront] Korrekturabzug hochgeladen haben. Sie können sie mit der Funktion [!UICONTROL Originaldatei herunterladen] herunterladen, bevor Sie die Korrekturabzüge löschen.

>[!NOTE]
>
>Beachten Sie bei der Verwendung von Backups Folgendes:
>
>* Backups sind für Pläne des Typs „Enterprise“ und „Unlimited“ verfügbar. Bitte kontaktieren Sie unser [Vertriebsteam](mailto:sales@proofhq.com) für ein Angebot.
>* Für den Datenkodierungstyp ist standardmäßig UTF-8 festgelegt. Wir empfehlen diese Einstellung. Dies ist der Kodierungstyp, der am häufigsten von Internetanwendungen verwendet wird.
>* Sie können jeweils nur eine [!DNL backup] anfordern. Wenn Ihre ZIP-Sicherungsdatei verarbeitet wird, wird der Link Neues Backup anfordern auf der Registerkarte Backups nicht angezeigt und die angezeigte Meldung bleibt unverändert. Informationen zum Anfordern einer Sicherung finden Sie unter [Anfordern einer neuen Datensicherung in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>



## Sichern von Daten

1. Klicken **[!UICONTROL oben rechts]** der [!DNL Workfront Proof] auf „Kontoeinstellungen“. 1)
1. Klicken Sie auf **[!UICONTROL Registerkarte]** Sicherungen“. 2)
1. Klicken Sie auf **[!UICONTROL Link „Neues Backup anfordern]** (3)

Wenn das Backup fertig ist, geschieht Folgendes:

* Sie erhalten eine E-Mail von [!DNL Workfront Proof], in der Sie darüber informiert werden („Ihr [!DNL Workfront Proof]-Backup ist bereit„). Die E-Mail enthält einen Download-Link für Ihre Sicherungsdaten.
* Auf [&#x200B; Registerkarte &#x200B;](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)Kontoeinstellungen“ wird ein Download-Link für Ihre Sicherungsdaten angezeigt.
* Der Link Neues Backup anfordern (3) wird erneut auf der Registerkarte Backups angezeigt

Ihre Daten können als ZIP-Datei heruntergeladen werden. Sie können die ZIP-Sicherungsdatei entweder über die Benachrichtigungs-E-Mail oder in den [!UICONTROL Kontoeinstellungen] herunterladen, wie in den folgenden Abschnitten beschrieben:

* [Herunterladen der ZIP-Sicherungsdatei aus der E-Mail-Benachrichtigung](#downloading-your-backup-zip-file-from-your-email-notification)
* [Herunterladen der ZIP-Sicherungsdatei über die Kontoeinstellungen](#downloading-your-backup-zip-file-from-the-account-settings)

![request_backup.png](assets/request-backup-350x167.png)

## Herunterladen der ZIP-Sicherungsdatei aus der E-Mail-Benachrichtigung {#downloading-your-backup-zip-file-from-your-email-notification}

Wenn Ihre ZIP-Sicherungsdatei zum Herunterladen bereit ist, erhalten Sie eine E-Mail von [!DNL Workfront Proof] mit der Betreffzeile „Ihr [!DNL Workfront Proof] Backup ist bereit“.

So laden Sie die ZIP-Sicherungsdatei aus der E-Mail herunter:

1. Klicken Sie auf den Download-Link in der E-Mail.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   Wenn Sie derzeit nicht bei [!DNL Workfront Proof] angemeldet sind, wird ein neues Browser-Fenster geöffnet, in dem die Anmeldeseite angezeigt wird.

## Herunterladen der ZIP-Sicherungsdatei über die Kontoeinstellungen {#downloading-your-backup-zip-file-from-the-account-settings}

Wenn Ihre ZIP-Sicherungsdatei zum Herunterladen bereit ist, wird dies auf der Registerkarte [!UICONTROL Sicherung] durch einen Download-Link angezeigt. Darüber hinaus wird erneut der [!UICONTROL Neues Backup anfordern] angezeigt.

1. Klicken **[!UICONTROL oben rechts]** der [!DNL Workfront Proof] auf „Kontoeinstellungen“. 1)
1. Klicken Sie auf **[!UICONTROL Registerkarte]** Sicherungen“. 2)\
   Wenn kein(e) Benutzende(r) in Ihrem Konto Sicherungskopien angefordert hat, zeigt die Registerkarte [!UICONTROL Sicherungskopien] an, dass Sie keine Sicherungskopien haben. Wenn ein Benutzer eine Sicherung angefordert hat, zeigt die Registerkarte das Erstellungsdatum und den Download-Link für die letzte Sicherung an.

1. Klicken Sie auf den **[!UICONTROL Sicherung herunterladen]**. 3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Ein Bildschirm zum Herunterladen von Dateien wird angezeigt, in dem Sie gefragt werden, ob Sie die heruntergeladene Datei öffnen oder speichern möchten.

1. Klicken Sie **[!UICONTROL Speichern]** und wählen Sie dann den Speicherort auf Ihrem Computer aus, an dem Sie die ZIP-Sicherungsdatei speichern möchten.\
   Die Meldung, die das Datum Ihres letzten Backups angibt, wird bis zum nächsten Backup unten auf [!UICONTROL Backup]-Seite angezeigt. Der Link Sicherung herunterladen gilt für diese letzte Sicherung. Sobald der Link [!UICONTROL Neues Backup anfordern] angezeigt wird, können Sie darauf klicken, um ein weiteres Backup anzufordern.

## Grundlegendes zu den Dateien in Ihrer ZIP-Sicherungsdatei

Ihre ZIP-Backup-Datei enthält sieben CSV-Dateien (kommagetrennte Werte oder kommagetrennte Dateien), die Informationen aus Ihren aktiven und archivierten Korrekturabzügen bis zum Zeitpunkt der Sicherung Ihrer Daten enthalten:

* comments.csv - Enthält Kommentare zu Korrekturabzügen
* comment_responses.csv - enthält Antworten auf Kommentare zu Korrekturabzügen in Organisation.csv - enthält die numerische Kennung und den Namen Ihrer Organisation (Ihres Kontos)
* Kontakte.csv - Enthält numerische Kennung, Namen und Organisation für jeden Kontakt
* files.csv - Enthält Informationen auf der Seite „Korrekturabzugsdetails“ oder der Seite „Dateidetails“ zu Korrekturabzügen oder Dateien, die in [!DNL Workfront Proof] hochgeladen wurden
* recipients.csv - Enthält numerische Kennungen, Rollen und Entscheidungen jeder Person, die als Prüfer, Prüfer und genehmigende Person usw. angegeben ist, wenn Testsendungen zur Überprüfung in die [!DNL Workfront Proof] hochgeladen werden
* users.csv - Enthält numerische Kennungen und Namen aller Benutzer im Konto

Sie können diese Dateien aus der ZIP-Sicherungsdatei mit dem von Ihnen verwendeten ZIP-Dienstprogramm extrahieren und dann an einem Speicherort Ihrer Wahl auf Ihrem Computer speichern. Nachdem Sie die ZIP-Datei gespeichert und die einzelnen CSV-Dateien extrahiert haben, können Sie die Informationen nach Bedarf für Ihre interne Datensatzaufbewahrung bearbeiten.

Jede auf Ihre Anfrage hin erstellte ZIP-Sicherungsdatei hat einen eindeutigen Namen, der das Erstellungsdatum des Backups enthält, aber die in jeder ZIP-Sicherungsdatei enthaltenen CSV-Dateien haben immer dieselben Namen. Sie können eine der folgenden Methoden verwenden, um sicherzustellen, dass sich Ihre Backup-Dateien voneinander unterscheiden:

* Erstellen Sie für jede Backup-ZIP-Datei und die daraus extrahierten CSV-Dateien einen neuen Ordner.
* Benennen Sie jede einzelne CSV-Datei um, um das Backup-Datum einzuschließen, wenn Sie sie aus der ZIP-Datei extrahieren.

>[!NOTE]
>
>Wenn [!DNL Microsoft Excel] auf Ihrem Computer installiert ist, listet Ihr Extrahierungs-Dienstprogramm möglicherweise den Dateityp für die einzelnen CSV-Dateien als [!DNL Microsoft Office Excel] Datei mit kommagetrennten Werten auf. Sie können eine extrahierte CSV-Datei mithilfe von [!DNL Excel] öffnen und die Datei als [!DNL Excel] Arbeitsmappe (&#42;.xlsx) oder einen anderen Dateityp speichern.
