---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Konfigurieren von Benutzerinformationen mit  [!DNL Workfront Proof]
description: Konfigurieren von Benutzerinformationen mit  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Benutzerinformationen mit [!DNL Workfront Proof] konfigurieren

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines Benutzers, wie unter [Benutzer mit  [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md) erstellen beschrieben.
1. Geben Sie die folgenden Informationen an:

   * Im Abschnitt **[!UICONTROL Persönliche Details]** :

      * **E-Mail-Adresse:** Die E-Mail-Adresse des Benutzers.
      * **Vorname:** Der Vorname des Benutzers.
      * **Nachname:** Der Nachname des Benutzers.
      * **Position:** Die Position des Benutzers im Unternehmen.
      * **Berechtigungsprofil:** Die Berechtigungen des Benutzers für das Testkonto.
      * **Sprache:** Die primäre Sprache des Benutzers.
      * **Zeitzone:** Wählen Sie die Zeitzone des Benutzers aus.
      * **Datumsformat:** Wählen Sie das bevorzugte Datumsformat des Benutzers aus.
      * **Opt-in - Produkt- und Marketing-E-Mails:** Wählen Sie aus, ob der Benutzer für Produkt- und Marketing-E-Mails angemeldet werden soll.
      * Nur **API:** Ermöglicht dem Benutzer die Anmeldung nur über die API.

   * Geben Sie im Abschnitt **[!UICONTROL Benutzerdetails]** die Kontaktinformationen des Benutzers ein, z. B. die Straße und die Telefonnummer.
   * Konfigurieren Sie im Abschnitt **[!UICONTROL Standardmäßige Testversand-Einstellungen]** die Einstellungen, die sich auf die Art und Weise auswirken, wie der Benutzer Testsendungen erstellt oder bearbeitet.

      * **Standardmäßige Testversand-Rolle:** Wählen Sie eine standardmäßige Testversandrolle für den Benutzer aus. Rollenoptionen sind **[!UICONTROL Schreibgeschützt]**, **[!UICONTROL Überprüfer]**, **[!UICONTROL Genehmiger]**, **[!UICONTROL Überprüfer und Genehmiger]**, **[!UICONTROL Autor]** oder **[!UICONTROL Moderator]**.

        Weitere Informationen zu Proof-Rollen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Sperren Sie den Testversand, wenn alle Entscheidungen getroffen werden:** Sperrt den Testversand automatisch für weitere Änderungen, nachdem alle Entscheidungen zum Testversand getroffen wurden.
      * **Anmeldung erforderlich. Der Testversand kann nur für andere Benutzer freigegeben werden:** Stellt den Testversand nur Benutzern mit [!DNL Workfront Proof] Anmeldedaten zur Verfügung.
      * **Nur eine Entscheidung erforderlich:** Erfordert nur eine Entscheidung über einen Testversand.
      * **Herunterladen der Originaldatei:** Ermöglicht dem Benutzer, die Originaldatei für einen Testversand herunterzuladen. Diese Option ist standardmäßig aktiviert.

        Weitere Informationen zum Herunterladen von Originaldateien finden Sie unter [Herunterladen von in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md) gespeicherten Dateien.

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Personen können sich über die öffentliche URL oder den Einbettungscode für den Testversand anmelden:** Ermöglicht externen Validierern, sich über die öffentliche URL oder den Einbettungscode für den Testversand zu registrieren.

        Wenn diese Option aktiviert ist, muss der **Abonnent auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können.** ist ebenfalls verfügbar. Wählen Sie diese Option aus, damit der externe Validierer auf einen Link in der E-Mail klicken muss, um auf den Testversand zugreifen zu können.
Diese Option ist standardmäßig aktiviert, wenn die Option **Öffentliche Freigabe** ausgewählt ist.

      * **Standardrolle für neue Gastreviewer:** Wählen Sie eine standardmäßige Testversandrolle für Gastreviewer aus. Die Optionen sind mit denen in **Standardmäßige Testversand-Rolle** identisch, mit Ausnahme von Moderator und Autor.

   * Im Abschnitt **[!UICONTROL Standard-E-Mail-Warnhinweiseinstellungen]** :

      * **Standard-E-Mail-Warnung:** Wählen Sie aus, wie oft der Benutzer E-Mail-Aktualisierungen erhält. Wählen Sie **Alle Aktivitäten, Antworten auf meine Kommentare, Entscheidungen, endgültige Entscheidung, stündliche Zusammenfassung, tägliche Zusammenfassung,** oder **Deaktiviert**.

        Weitere Informationen zu den standardmäßigen E-Mail-Warnhinweisoptionen finden Sie unter [E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) .

      * **Standard-E-Mail-Warnung für neue Gastreviewer:** Wählen Sie aus, wie oft Gastreviewer E-Mail-Aktualisierungen erhalten. Die Optionen entsprechen denen für den standardmäßigen E-Mail-Warnhinweis **.**

      * **E-Mail-Bestätigung senden, wenn Testsendungen fertig sind:** Wählen Sie diese Option aus, um dem Benutzer automatisch eine Bestätigungs-E-Mail zu senden, wenn Testsendungen abgeschlossen sind.
      * **Format der an diesen Benutzer gesendeten E-Mails:** Wählen Sie **[!UICONTROL HTML]** oder **[!UICONTROL Klartext]** als Standardformat für an den Benutzer gesendete E-Mails aus.

   * Erstellen Sie im Abschnitt **[!UICONTROL Benutzerdefinierte Nachrichteneinstellungen]** Einstellungen für Testversandvorlagen.

     Weitere Informationen zu Vorlagen finden Sie unter:

      * **Betreffvorlage &quot;Testversand&quot;:** Erstellen Sie eine Vorlage für einen Testversand-Betreff.
      * **Vorlage für Testversand-Nachricht:** Erstellen Sie eine Vorlage für eine Testnachricht und deren Format.
