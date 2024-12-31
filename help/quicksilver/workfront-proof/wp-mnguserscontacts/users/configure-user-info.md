---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Konfigurieren von Benutzerinformationen mithilfe von [!DNL Workfront Proof]
description: Konfigurieren von Benutzerinformationen mithilfe von [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Konfigurieren von Benutzerinformationen mithilfe von [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

1. Erstellen oder bearbeiten Sie einen Benutzer wie in [Benutzer erstellen mit [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md) beschrieben.
1. Geben Sie die folgenden Informationen an:

   * Im Abschnitt **[!UICONTROL Persönliche]**):

      * **E-Mail-Adresse** Die E-Mail-Adresse des Benutzers.
      * **Vorname:** Vorname der Benutzerin oder des Benutzers.
      * **Nachname:** Der Nachname des Benutzers.
      * **Position:** Die Position des Benutzers im Unternehmen.
      * **Berechtigungsprofil** Die Berechtigungen des Benutzers für das Korrekturabzugskonto.
      * **Language:** Die primäre Sprache des Benutzers.
      * **Zeitzone:** Sie die Zeitzone des Benutzers aus.
      * **Datumsformat** Wählen Sie das bevorzugte Datumsformat des Benutzers aus.
      * **Opt-in - Produkt- und Marketing-E-Mails:** Wählen Sie aus, ob der Benutzer sich für Produkt- und Marketing-E-Mails anmelden soll.
      * **Nur API:** Erlaubt dem Benutzer, sich nur über die API anzumelden.

   * Geben Sie **[!UICONTROL Abschnitt &quot;]**&quot; die Kontaktinformationen des Benutzers ein, z. B. Straße und Telefonnummer.
   * Konfigurieren Sie im Abschnitt **[!UICONTROL Standardeinstellungen für]** die Einstellungen, die sich auf die Art und Weise auswirken, wie Benutzende Korrekturabzüge erstellen oder bearbeiten.

      * **Standard-Korrekturabzugsrolle** Wählen Sie eine Standard-Korrekturabzugsrolle für den Benutzer aus. Die Rollenoptionen sind **[!UICONTROL Schreibgeschützt]**, **[!UICONTROL Prüfende]**, **[!UICONTROL Genehmigende]**, **[!UICONTROL Prüfende und genehmigende Person]**, **[!UICONTROL Autor]** oder **[!UICONTROL Moderator]**.

        Weitere Informationen zu Korrekturabzug-Rollen finden Sie unter [Verwalten von Korrekturabzug-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Korrekturabzug sperren, wenn alle Entscheidungen getroffen werden:** Sperrt den Korrekturabzug automatisch für weitere Änderungen, nachdem alle Entscheidungen über den Korrekturabzug getroffen wurden.
      * **Anmeldung erforderlich. Der Korrekturabzug kann nur für andere Benutzer freigegeben werden** Stellt den Korrekturabzug nur Benutzenden mit [!DNL Workfront Proof] Anmeldedaten zur Verfügung.
      * **Nur eine Entscheidung erforderlich:** Erfordert nur eine Entscheidung zu einem Korrekturabzug.
      * **Originaldatei herunterladen:** Ermöglicht dem Benutzer, die Originaldatei für einen Korrekturabzug herunterzuladen. Diese Option ist standardmäßig aktiviert.

        Weitere Informationen zum Herunterladen von Originaldateien finden Sie unter [Herunterladen von in gespeicherten Dateien [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement Personen können sich über die öffentliche URL oder den Einbettungs-Code für den Korrekturabzug anmelden:** Ermöglicht externen Prüfern, sich über die öffentliche URL oder den Einbettungs-Code für den Korrekturabzug zu registrieren.

        Wenn diese Option ausgewählt ist **ist auch „Abonnent muss auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen** verfügbar. Wählen Sie diese Option aus, damit der externe Prüfer auf einen Link in der E-Mail klicken muss, um auf den Korrekturabzug zuzugreifen.
Diese Option ist standardmäßig aktiviert, wenn die Option **Öffentliche Freigabe** ausgewählt ist.

      * **Standardrolle für neue Gast-Reviewer:** Wählen Sie eine Standardrolle für Korrekturabzüge für Gast-Reviewer aus. Die Optionen sind mit denen in der **Standardrolle für Korrekturabzüge** identisch, mit Ausnahme von Moderator und Autor.

   * Im Abschnitt **[!UICONTROL Standardeinstellungen für E-Mail]**:

      * **Standard-E-Mail-Warnhinweis** Wählen Sie aus, wie oft Benutzende E-Mail-Updates erhalten sollen. Wählen Sie **Alle Aktivitäten, Antworten auf meine Kommentare, Entscheidungen, Endgültige Entscheidung, Stündliche Zusammenfassung, Tägliche Zusammenfassung** oder **Deaktiviert** aus.

        Weitere Informationen zu den Standardoptionen für E-Mail-Warnhinweise finden Sie unter [Konfigurieren von E-Mail-Benachrichtigungseinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Standard-E-Mail-Warnhinweis für neue Gast-Reviewer:** Wählen Sie aus, wie oft Gast-Reviewer E-Mail-Aktualisierungen erhalten sollen. Die Optionen sind die gleichen wie bei **E-Mail-Warnhinweis.**

      * **Senden einer E-Mail-Bestätigung, wenn Testsendungen fertig sind:** Wählen Sie diese Option, um dem Benutzer automatisch eine Bestätigungs-E-Mail zu senden, wenn Testsendungen bereit sind.
      * **Format der an diesen Benutzer gesendeten E-Mails:** Wählen Sie **[!UICONTROL HTML]** oder **[!UICONTROL Nur Text]** als Standardformat für E-Mails, die an den Benutzer gesendet werden.

   * Im Abschnitt **[!UICONTROL Benutzerdefinierte Nachrichteneinstellungen]**: Erstellen Sie Einstellungen für Korrekturabzugsvorlagen.

     Weitere Informationen zu Vorlagen finden Sie unter:

      * **Vorlage für einen Testversand:** Sie eine Vorlage für einen Testversand-Betreff.
      * **Testversandnachrichtenvorlage:** Sie eine Vorlage für eine Testversandnachricht und ihr Format.
