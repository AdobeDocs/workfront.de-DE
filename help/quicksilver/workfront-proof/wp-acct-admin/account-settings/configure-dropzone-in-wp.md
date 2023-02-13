---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]
description: Als [!DNL Workfront Proof] Administrator können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zur Dropzone finden Sie in der Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] Administrator können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zur Dropzone finden Sie unter [Die Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**, und öffnen Sie dann die **[!UICONTROL Dropzone]** Registerkarte.

1. Nehmen Sie eine der folgenden Änderungen in der **[!UICONTROL Dropzone-Details]** Abschnitt:

   * **[!UICONTROL Web-Dropzone]**: Aktivieren oder deaktivieren Sie die Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: Die URL, die Sie in Ihren Browser eingeben müssen, um Testsendungen über die Dropzone durchzuführen.
   * **[!UICONTROL E-Mail-Dropzone]**: Aktivieren oder deaktivieren Sie die Dropzone E-Mail .

      >[!NOTE]
      >
      >Das Senden von E-Mails an Dropzones wird nicht mehr unterstützt.

   * **[!UICONTROL Dropzone Owner]**: Legen Sie den Inhaber der Dropzone fest oder bearbeiten Sie ihn. Dies ist die Person, die über neue Einsendungen in die Dropzone benachrichtigt wird. Um als Inhaber der Dropzone festgelegt zu werden, muss der Benutzer ein Supervisor, Administrator, Abrechnungsadministrator oder Kontoersteller sein. Weitere Informationen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Standardrolle für Ersteller]**: Alle Übermittler werden dem Testversand hinzugefügt, wobei diese Rolle standardmäßig verwendet wird.
   * **[!UICONTROL E-Mail-Benachrichtigung für alle Ersteller]**: Legen Sie hier die E-Mail-Benachrichtigungseinstellung für Testversand-Ersteller (Einsender) fest. Siehe [E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) für Informationen zu den verschiedenen verfügbaren Warnhinweiseinstellungen.

   * **[!UICONTROL Neue Versionsfunktion]**: Aktivieren und deaktivieren Sie die Funktion Neue Version in der Dropzone. Dadurch erhalten oder entfällt die Möglichkeit, neue Testsendungen über die Dropzone durchzuführen.
   * **[!UICONTROL Testsendungsentwürfe löschen nach (Tagen)]**: Geben Sie die Anzahl der Tage an, nach denen ein Testversand-Entwurf gelöscht wird. Testsendungen verbleiben im Entwurfsstatus, wenn die Übermittlung der Dropzone nach dem Hochladen der Datei in die Dropzone nicht abgeschlossen ist.
   * **[!UICONTROL Überprüferrolle ausblenden]**: Blenden Sie beim Hinzufügen von Personen zur Dropzone das Feld für die Überprüferrolle aus.
   * **[!UICONTROL Testversandnachricht bei Aktivierung senden]**: Konfigurieren [!DNL Workfront Proof] , um den Validierungsverantwortlichen bei der Aktivierung eines Testversands automatisch eine Benachrichtigungs-E-Mail zu senden.
   * **[!UICONTROL Testversand bei Übermittlung aktivieren]**: Konfigurieren [!DNL Workfront Proof] , um Testsendungen automatisch bei der Übermittlung zu aktivieren (sodass sie nicht mehr manuell aktiviert werden müssen).

   * Wenn ein Testversand aus der Dropzone (z. B. in einen anderen Ordner in Ihrem Konto) verschoben wird, gelten die Dropzone-Einstellungen nicht mehr für den Testversand. Dies ist besonders wichtig in Bezug auf die Einstellungen für E-Mail-Warnhinweise.

1. Nehmen Sie Änderungen an der **[!UICONTROL Dropzone-Felder]** -Abschnitt, um anzugeben, welche Felder in der [!UICONTROL Testversanddetails] auf der Dropzone-Übermittlungsseite, wenn Testsendungen über die Dropzone gesendet werden.
1. Im **[!UICONTROL Zulässige Domänen]** Geben Sie Domänen an, die Sie in der Dropzone verwenden dürfen möchten.

   * Sie können auf **[!UICONTROL Domain hinzufügen]** , um eine Domäne hinzuzufügen. Wenn Sie die Domänendetails hinzugefügt haben, klicken Sie auf **[!UICONTROL Speichern]**.

   * Sie können **[!UICONTROL Bearbeiten]** und **[!UICONTROL Löschen]** alle vorhandenen Domänen, die Sie zuvor hinzugefügt haben.

1. under **[!UICONTROL Benachrichtigung]**, geben Sie die Personen an, die Sie mit dem Dropzone-Eigentümer benachrichtigen möchten, wenn neue Testsendungen an die Dropzone gesendet werden [Die Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Klicken **[!UICONTROL Personen hinzufügen]**, geben Sie die Details des Empfängers ein und klicken Sie auf **[!UICONTROL Speichern]**.

   * **[!UICONTROL Löschen]** Personen, die Sie bereits hinzugefügt haben.
