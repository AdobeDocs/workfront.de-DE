---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]
description: Als  [!DNL Workfront Proof]  können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zu Dropzone finden Sie unter The Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Konfigurieren des Ablagebereichs in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] können Sie die Dropzone-Einstellungen Ihrer Benutzer festlegen, anzeigen und bearbeiten. Weitere Informationen zu Dropzone finden Sie unter [Die Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Klicken Sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** und öffnen Sie dann die Registerkarte **[!UICONTROL Dropzone]**.

1. Nehmen Sie im Abschnitt **[!UICONTROL Details der Dropzone]** eine der folgenden Änderungen vor:

   * **[!UICONTROL Web Dropzone]**: Aktiviert oder deaktiviert die Dropzone.
   * **[!UICONTROL Web Dropzone URL]**: Die URL, die Sie in Ihren Browser eingeben müssen, um Testsendungen über die Dropzone durchzuführen.
   * **[!UICONTROL E-Mail-Ablagebereich]**: Aktivieren oder Deaktivieren der E-Mail-Ablagebereich.

     >[!NOTE]
     >
     >Das Senden von E-Mails an Ablagebereiche wird nicht mehr unterstützt.

   * **[!UICONTROL Inhaber der Dropzone]**: Legen Sie den Inhaber der Dropzone fest oder bearbeiten Sie ihn. Dies ist die Person, die über neue Übermittlungen an den Ablagebereich benachrichtigt wird. Um als Besitzer der Dropzone festgelegt zu werden, muss der Benutzer ein Supervisor, Admin, Abrechnungs-Admin oder der Ersteller des Kontos sein. Weitere Informationen finden Sie unter [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Standardrolle für Ersteller]**: Alle Absender werden dem Korrekturabzug mit dieser Rolle als Standard hinzugefügt.
   * **[!UICONTROL E-Mail-Benachrichtigung für alle Ersteller]**: Hier können Sie die Voreinstellung für E-Mail-Warnungen für Ersteller von Korrekturabzügen (Absender) festlegen. Weitere [&#x200B; zu den verschiedenen verfügbaren Warnhinweiseinstellungen finden Sie unter  [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) von E-Mail-Benachrichtigungseinstellungen in .

   * **[!UICONTROL Neue Versionsfunktion]**: Aktivieren und deaktivieren Sie die Funktion „Neue Version“ im Ablagebereich. Dadurch erhalten oder werden Benutzer die Möglichkeit entfernt, neue Versionen von Testsendungen über den Ablagebereich einzureichen.
   * **[!UICONTROL Entwurf von Korrekturabzügen löschen nach (Tagen)]**: Geben Sie die Anzahl der Tage an, nach denen der Entwurf eines Korrekturabzugs gelöscht wird. Korrekturabzüge verbleiben im Entwurfsstatus, wenn die Übermittlung im Ablagebereich nach dem Hochladen der Datei in den Ablagebereich nicht abgeschlossen ist.
   * **[!UICONTROL Reviewer-Rolle ausblenden]**: Blendet das Feld für die Reviewer-Rolle aus, wenn Personen zur Dropzone hinzugefügt werden.
   * **[!UICONTROL Testversandnachricht bei Aktivierung senden]**: Konfigurieren Sie [!DNL Workfront Proof] so, dass die Benachrichtigungs-E-Mails für Testsendungen bei Aktivierung eines Testversands automatisch an die Validierungsverantwortlichen gesendet werden.
   * **[!UICONTROL Testversand bei Übermittlung aktivieren]**: Konfigurieren Sie [!DNL Workfront Proof] so, dass Testsendungen automatisch bei der Übermittlung aktiviert werden (Korrekturabzüge müssen nicht mehr manuell aktiviert werden).

   * Wenn ein Korrekturabzug aus der Ablagezone verschoben wird (z. B. in einen anderen Ordner in Ihrem Konto), gelten die Einstellungen für die Ablagezone nicht mehr für den Korrekturabzug. Dies ist besonders wichtig in Bezug auf E-Mail-Warnhinweiseinstellungen.

1. Nehmen Sie im Abschnitt **[!UICONTROL Dropzone-Felder]** Änderungen vor, um festzulegen, welche Felder im Abschnitt [!UICONTROL Testversanddetails] der Seite Übermittlung in der Dropzone angezeigt werden, wenn Testsendungen über die Dropzone gesendet werden.
1. Geben Sie im Abschnitt **[!UICONTROL Zugelassene Domains]** die Domains an, für die Sie die Dropzone verwenden dürfen.

   * Sie können auf **[!UICONTROL Domain hinzufügen]** klicken, um eine Domain hinzuzufügen. Nachdem Sie die Domain-Details hinzugefügt haben, klicken Sie auf **[!UICONTROL Speichern]**.

   * Sie können **[!UICONTROL Bearbeiten]** und **[!UICONTROL Löschen]** alle vorhandenen Domains auswählen, die Sie zuvor hinzugefügt haben.

1. Geben **[!UICONTROL unter „Zu benachrichtigende Personen]** die Personen an, die zusammen mit dem Ablagebereichsinhaber benachrichtigt werden sollen, wenn neue Korrekturabzüge in der Ablagezone eingereicht werden [Der Ablagebereich](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Klicken Sie **[!UICONTROL Personen hinzufügen]**, geben Sie die Empfängerdetails ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

   * **[!UICONTROL Löschen]** zuvor hinzugefügte Personen.
