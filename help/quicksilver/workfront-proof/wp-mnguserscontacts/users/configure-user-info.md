---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Benutzerinformationen konfigurieren mithilfe von [!DNL Workfront Proof]
description: Benutzerinformationen konfigurieren mithilfe von [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Benutzerinformationen konfigurieren mithilfe von [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testing](../../../review-and-approve-work/proofing/proofing.md).

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines Benutzers wie unter [Benutzer erstellen mithilfe von [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Geben Sie die folgenden Informationen an:

   * Im **[!UICONTROL Persönliche Daten]** Abschnitt:

      * **Email Address:** Die E-Mail-Adresse des Benutzers.
      * **Vorname:** Der Vorname des Benutzers.
      * **Nachname:** Der Nachname des Benutzers.
      * **Funktion:** Die Position des Benutzers im Unternehmen.
      * **Berechtigungsprofil:** Die Berechtigungen des Benutzers für das Testkonto.
      * **Sprache:** Die Primärsprache des Benutzers.
      * **Zeitzone:** Wählen Sie die Zeitzone des Benutzers aus.
      * **Datumsformat:** Wählen Sie das vom Benutzer bevorzugte Datumsformat aus.
      * **Opt-in - Produkt- und Marketing-E-Mails:** Wählen Sie aus, ob der Benutzer für Produkt- und Marketing-E-Mails angemeldet werden soll.
      * **Nur API:** Ermöglicht dem Benutzer die Anmeldung nur über die API.

   * Im **[!UICONTROL Benutzerdetails]** Geben Sie die Kontaktinformationen des Benutzers ein, z. B. die Straße und die Telefonnummer.
   * Im **[!UICONTROL Standardmäßige Testversand-Einstellungen]** konfigurieren Sie die Einstellungen, die sich auf die Art und Weise auswirken, wie der Benutzer Testsendungen erstellt oder bearbeitet.

      * **Standardmäßige Testversand-Rolle:** Wählen Sie eine standardmäßige Testversand-Rolle für den Benutzer aus. Rollenoptionen sind **[!UICONTROL Schreibgeschützt]**, **[!UICONTROL Überprüfer]**, **[!UICONTROL Genehmiger]**, **[!UICONTROL Überprüfer und Genehmiger]**, **[!UICONTROL Autor]** oder **[!UICONTROL Moderator]**.

        Weitere Informationen zu Testversandrollen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Sperren Sie den Testversand, wenn alle Entscheidungen getroffen werden:** Sperrt den Testversand automatisch vor weiteren Änderungen, nachdem alle Entscheidungen über den Testversand getroffen wurden.
      * **Anmeldung erforderlich. Der Testversand kann nur für andere Benutzer freigegeben werden:** Stellt den Testversand nur Benutzern mit zur Verfügung [!DNL Workfront Proof] Anmeldedaten.
      * **Nur eine Entscheidung erforderte:** Erfordert nur eine Entscheidung über einen Beweis.
      * **Herunterladen der Originaldatei:** Ermöglicht dem Benutzer das Herunterladen der Originaldatei für einen Testversand. Diese Option ist standardmäßig aktiviert.

        Weitere Informationen zum Herunterladen von Originaldateien finden Sie unter [Herunterladen von in gespeicherten Dateien [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Personen können sich über die öffentliche URL oder den Einbettungscode für den Testversand anmelden:** Ermöglicht es externen Validierern der Organisation, sich über die öffentliche URL oder den Einbettungscode für den Testversand zu registrieren.

        Wenn diese Option ausgewählt ist, **Abonnenten müssen auf einen Link in einer E-Mail klicken, um einen Testversand zu erhalten** ist auch verfügbar. Wählen Sie diese Option aus, damit der externe Validierer auf einen Link in der E-Mail klicken muss, um auf den Testversand zugreifen zu können.
Diese Option ist standardmäßig aktiviert, wenn die Variable **Öffentliche Freigabe** ausgewählt ist.

      * **Standardrolle für neue Gastreviewer:** Wählen Sie eine standardmäßige Testversand-Rolle für Gastreviewer aus. Die Optionen entsprechen denen unter **Standardmäßige Testversand-Rolle**, mit Ausnahme von Moderator und Autor.

   * Im **[!UICONTROL Standard-E-Mail-Warnhinweiseinstellungen]** Abschnitt:

      * **Standard-E-Mail-Warnung:** Wählen Sie aus, wie häufig der Benutzer E-Mail-Aktualisierungen erhält. Auswählen **Alle Aktivitäten, Antworten auf meine Kommentare, Entscheidungen, endgültige Entscheidung, Stündliche Zusammenfassung, Tägliche Zusammenfassung,** oder **Behinderte**.

        Weitere Informationen zu den standardmäßigen E-Mail-Warnhinweisoptionen finden Sie unter [E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Standard-E-Mail-Warnung für neue Gastreviewer:** Wählen Sie aus, wie häufig Gastreviewer E-Mail-Aktualisierungen erhalten. Die Optionen entsprechen denen für **Standard-E-Mail-Warnhinweis.**

      * **Senden Sie eine E-Mail-Bestätigung, wenn Testsendungen abgeschlossen sind:** Wählen Sie diese Option, um dem Benutzer automatisch eine Bestätigungs-E-Mail zu senden, wenn die Testsendungen fertig sind.
      * **Format der an diesen Benutzer gesendeten E-Mails:** Auswählen **[!UICONTROL HTML]** oder **[!UICONTROL Nur Text]** als Standardformat für E-Mails, die an den Benutzer gesendet werden.

   * Im **[!UICONTROL Benutzerdefinierte Nachrichteneinstellungen]** Abschnitt: Erstellen Sie Einstellungen für Testversandvorlagen.

     Weitere Informationen zu Vorlagen finden Sie unter:

      * **Vorlage für Testversand-Betreff:** Erstellen Sie eine Vorlage für einen Testversand-Betreff.
      * **Vorlage für Testnachrichten:** Erstellen Sie eine Vorlage für eine Testnachricht und deren Format.
