---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurieren der Dropzone in [!DNL Workfront Proof]
description: Als [!DNL Workfront Proof] Administrator können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zur Dropzone finden Sie in der Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Konfigurieren der Dropzone in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] -Administrator können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zur Dropzone finden Sie unter [Die Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** und öffnen Sie dann die Registerkarte **[!UICONTROL Dropzone]**.

1. Nehmen Sie eine der folgenden Änderungen im Abschnitt **[!UICONTROL Details der Dropzone]** vor:

   * **[!UICONTROL Web Dropzone]**: Aktivieren oder deaktivieren Sie die Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: Die URL, die Sie in Ihren Browser eingeben müssen, um Testsendungen über die Dropzone durchzuführen.
   * **[!UICONTROL E-Mail-Dropzone]**: Aktivieren oder deaktivieren Sie die E-Mail-Dropzone.

     >[!NOTE]
     >
     >Das Senden von E-Mails an Dropzones wird nicht mehr unterstützt.

   * **[!UICONTROL Besitzer der Dropzone]**: Legen Sie den Besitzer der Dropzone fest oder bearbeiten Sie ihn. Dies ist die Person, die über neue Einsendungen in die Dropzone benachrichtigt wird. Um als Inhaber der Dropzone festgelegt zu werden, muss der Benutzer ein Supervisor, Administrator, Abrechnungsadministrator oder Kontoersteller sein. Weitere Informationen finden Sie unter [Profile für Testberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Standardrolle für Ersteller]**: Alle Übermittler werden dem Testversand hinzugefügt, wobei diese Rolle standardmäßig verwendet wird.
   * **[!UICONTROL E-Mail-Benachrichtigung für alle Ersteller]**: Legen Sie hier die E-Mail-Warnhinweispräferenz für Ersteller von Testsendungen (Übermittler) fest. Informationen zu den verschiedenen verfügbaren Warnhinweiseinstellungen finden Sie unter [E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) .

   * **[!UICONTROL Neue Versionsfunktion]**: Aktivieren und deaktivieren Sie die Funktion &quot;Neue Version&quot;in der Dropzone. Dadurch erhalten oder entfällt die Möglichkeit, neue Testsendungen über die Dropzone durchzuführen.
   * **[!UICONTROL Testsendungen löschen nach (Tagen)]**: Geben Sie die Anzahl der Tage an, nach denen ein Testversand-Entwurf gelöscht wird. Testsendungen verbleiben im Entwurfsstatus, wenn die Übermittlung der Dropzone nach dem Hochladen der Datei in die Dropzone nicht abgeschlossen ist.
   * **[!UICONTROL Überprüferrolle ausblenden]**: Blendet das Feld für die Überprüferrolle aus, wenn Personen zur Dropzone hinzugefügt werden.
   * **[!UICONTROL Testversand bei Aktivierung durchführen]**: Konfigurieren Sie [!DNL Workfront Proof], um den Validierern bei Aktivierung eines Testversands automatisch E-Mails mit der Testversand-Benachrichtigung zu senden.
   * **[!UICONTROL Testversand bei Übermittlung aktivieren]**: Konfigurieren Sie [!DNL Workfront Proof], um Testsendungen bei der Übermittlung automatisch zu aktivieren (sodass diese nicht mehr manuell aktiviert werden müssen).

   * Wenn ein Testversand aus der Dropzone (z. B. in einen anderen Ordner in Ihrem Konto) verschoben wird, gelten die Dropzone-Einstellungen nicht mehr für den Testversand. Dies ist besonders wichtig in Bezug auf die Einstellungen für E-Mail-Warnhinweise.

1. Nehmen Sie Änderungen im Abschnitt **[!UICONTROL Dropzone fields]** vor, um festzulegen, welche Felder im Abschnitt [!UICONTROL Testversand-Details] der Dropzone-Übermittlungsseite angezeigt werden, wenn Testsendungen über die Dropzone gesendet werden.
1. Geben Sie im Abschnitt **[!UICONTROL Zulässige Domänen]** die Domänen an, die die Dropzone verwenden dürfen sollen.

   * Sie können auf **[!UICONTROL Domäne hinzufügen]** klicken, um eine Domäne hinzuzufügen. Wenn Sie die Domänendetails hinzugefügt haben, klicken Sie auf **[!UICONTROL Speichern]**.

   * Sie können alle bereits hinzugefügten Domänen **[!UICONTROL bearbeiten]** und **[!UICONTROL löschen]**.

1. Geben Sie unter &quot;**[!UICONTROL Personen, die]** benachrichtigen sollen, die Personen an, die Sie zusammen mit dem Dropzone-Inhaber benachrichtigt werden möchten, wenn neue Testsendungen an die Dropzone gesendet werden [Die Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Klicken Sie auf **[!UICONTROL Personen hinzufügen]**, geben Sie die Details des Empfängers ein und klicken Sie auf **[!UICONTROL Speichern]**.

   * **[!UICONTROL Löschen]** Personen, die Sie zuvor hinzugefügt haben.
