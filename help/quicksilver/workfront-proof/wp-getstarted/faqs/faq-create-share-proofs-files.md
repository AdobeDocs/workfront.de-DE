---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Häufig gestellte Fragen - Erstellen und Freigeben von Testsendungen und Dateien
description: Ein Testversand ist eine statische, Audio- oder Videodatei, die im Testversand-Viewer zur Überprüfung verfügbar ist. Prüfer, die zu einem Testversand hinzugefügt wurden, verfügen über eine Reihe von Werkzeugen, mit denen sie Kommentare und Entscheidungen zum Testversand treffen können.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 1%

---

# Häufig gestellte Fragen - Erstellen und Freigeben von Testsendungen und Dateien

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testing](../../../review-and-approve-work/proofing/proofing.md).

## Was ist ein Beweis?

### Antwort

Ein Testversand ist eine statische, Audio- oder Videodatei, die im Testversand-Viewer zur Überprüfung verfügbar ist. Prüfer, die zu einem Testversand hinzugefügt wurden, verfügen über eine Reihe von Werkzeugen, mit denen sie Kommentare und Entscheidungen zum Testversand treffen können.

## Welche Dateitypen werden unterstützt?

### Antwort

Testsendungen können aus statischen, Audio- und Videodateien erstellt werden. Sie können keine Dateien hochladen, die größer als 4 GB sind. [!DNL Workfront] unterstützt mehr als 150 Dateitypen (siehe [Unterstützte Testing-Dateitypen und Größenbeschränkungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) für eine vollständige Liste).

## Was ist der Unterschied zwischen einem Testversand und einer Datei?

### Antwort

Wenn Sie eine Datei in [!DNL Workfront Proof], speichert das System die Datei in Ihrer [!DNL Workfront Proof] -Konto. Wenn Sie es freigeben, [!DNL Workfront Proof] E-Mail-Adressen an Empfänger senden, auf die sie klicken können, um die Datei herunterzuladen. Sie können beliebige Dateitypen freigeben.

Beim Erstellen eines Testversands aus einer Datei, die Sie in hochgeladen haben [!DNL Workfront Proof], können Sie die Datei im Testversand-Viewer zur Überprüfung bereitstellen. Überprüfer erhalten eine E-Mail mit einem Link zum Testversand. Wenn sie den Testversand öffnen, sehen sie das Testversandbild und können Kommentare hinzufügen und Entscheidungen dazu treffen. Sie können Testsendungen mithilfe von Dateien aus der Liste der unterstützten Dateitypen durchführen. Sie können auch Testsendungen mithilfe von URLs für Websites und andere Webinhalte durchführen.

Eine vollständige Liste der unterstützten Dateitypen finden Sie unter [Unterstützte Testing-Dateitypen und Größenbeschränkungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Wie erstelle ich einen Testversand?

### Antwort

Sie können Testsendungen aus statischen Dateien, Audiodateien, Videodateien und URLs erstellen (siehe ).

Um einen Testversand im Konto zu erstellen, müssen Sie ein Benutzer mit dem richtigen Berechtigungsprofil sein (siehe [[!UICONTROL Profile für Testberechtigungen] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Wenn Sie mehrere Dateien gleichzeitig hochladen, erstellen Sie mehrere Testsendungen, die Sie mit einer E-Mail an dieselbe Gruppe von Validierern senden können. Wenn Ihr Unternehmen über [!UICONTROL Unternehmen] oder [!UICONTROL Unbegrenzt] -Konto können Sie Dateien zu einem Testversand zusammenfassen (siehe [Erstellen eines mehrseitigen Testversands](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Was sind Testversandrollen und E-Mail-Warnungen?

### Antwort

Proof-Rollen definieren, welche Aktionen ein Validierer für einen Testversand ausführen muss. Es gibt verschiedene Rollenoptionen, die Sie für Prüfer verwenden können, wenn Sie einen Testversand erstellen, je nachdem, ob Sie möchten, dass sie Kommentare abgeben, Entscheidungen treffen können usw. Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Mit E-Mail-Warnungen werden die validierungsverantwortlichen Benutzer über den Fortschritt eines Testversands aktualisiert (sie unterscheiden sich von neuen Testversandbenachrichtigungen und Benachrichtigungen zu verspäteten Testsendungen). Je nach der Rolle der einzelnen Validierer beim Testversand können Sie für verschiedene Validierungsverantwortliche unterschiedliche Optionen auswählen. Weitere Informationen finden Sie unter [Erstellen Sie einen erweiterten Testversand mit einer [!UICONTROL Automatisierter Workflow]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Kann ich einen Testversand aus mehreren Dateien erstellen?

### Antwort

Die Kombination mehrerer Dateien zu einem Testversand ist eine Funktion, die unter [!UICONTROL Unternehmen] und [!UICONTROL Unbegrenzt] Bearbeitungspläne. Diese Option ist nur für statische Dateien möglich, nicht für Videodateien. Weitere Informationen finden Sie unter  [Erstellen eines mehrseitigen Testversands](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Kann ich Testsendungen über URLs erstellen?

### Antwort

Ja, Sie können Testsendungen von Websites und anderen Webinhalten erstellen. Wenn Sie eine URL hinzufügen, um einen Testversand zu erstellen, können Sie angeben, ob Sie einen statischen Testversand oder einen interaktiven Testversand durchführen möchten:

* In einem interaktiven Testversand können Prüfer wie gewohnt mit der Website oder anderen Webinhalten wie Anzeigen mit Streaming-Video oder -Audio navigieren und interagieren. [!DNL Flash] -Elemente in einer Anzeige, HTML-Animationen und interaktiven Bannern. Weitere Informationen finden Sie unter [Erstellen eines Testversands für interaktive Inhalte in einer ZIP-Datei](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).
* Für einen statischen Testversand: [!DNL Workfront] erstellt einen Screenshot der von Ihnen angegebenen Seiten und Unterseiten. Hyperlinks befinden sich im Testversand, sodass Sie testen können, ob sie zum richtigen Ziel führen oder nicht. Weitere Informationen finden Sie unter [Erstellen eines statischen Testversands für eine Website oder andere Webinhalte](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Sie können mehrere URLs gleichzeitig hinzufügen, wenn Sie sie durch ein Leerzeichen trennen. Beachten Sie, dass die Kombination nur in verfügbar ist. [!UICONTROL Unternehmen] und [!UICONTROL Unbegrenzt] Bearbeitungspläne.

## Können Personen, die keine Anmeldung haben, Testsendungen in meinem Konto erstellen?

### Antwort

Sie benötigen Anmeldedaten, um Testsendungen direkt in einem [!DNL Workfront Proof] -Konto.

## Was bedeutet die Freigabe eines Testversands?

### Antwort

Durch die Freigabe eines Testversands erhalten die Prüfer Zugriff darauf, sodass sie Kommentare und Markierungen hinzufügen und Entscheidungen dazu treffen können. Gastreviewer greifen auf Testsendungen aus der E-Mail-Benachrichtigung zu, die sie erhalten. Validierungsverantwortliche [!DNL Workfront Proof] -Konto kann auf Testsendungen im [!UICONTROL Dashboard].

## Wie gebe ich einen Testversand frei?

### Antwort

Wenn Sie einen Testversand erstellen, können Sie Überprüfer im [!UICONTROL Workflow] Abschnitt [!UICONTROL Neuer Testversand] Seite. Wenn der Testversand fertig ist, [!DNL Workfront Proof] sendet eine E-Mail an die validierungsverantwortlichen Benutzer, die einen Link zum Testversand enthalten.

Wenn Sie über ausreichende Berechtigungen für einen Testversand verfügen, können Sie den Testversand-Viewer, Ihre [!UICONTROL Dashboard]oder einer der Listenansichten, um einem vorhandenen Testversand Überprüfer hinzuzufügen (siehe [Testversand freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Seite in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

Das Hinzufügen von Validierungsverantwortlichen ist die gängigste Möglichkeit, Testsendungen gemeinsam zu nutzen. Weitere verfügbare Optionen finden Sie unter:

* [Freigeben von Testlinks in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Öffentliche URL freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Abonnieren eines Testversands in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Erstellen Sie einen Mini-Testversand in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Müssen Sie Benutzer sein, um einen Testversand zu überprüfen?

### Antwort

Nein. Gastreviewer (Personen ohne [!DNL Workfront Proof] Anmeldedaten) können über die Testversand-E-Mail-Benachrichtigung, die sie erhalten, auf einen Testversand zugreifen. Sie können einen Testversand mit beliebig vielen Gästen teilen.

Es ist möglich, die Freigabe von Testsendungen für Personen mit [!DNL Workfront Proof] Anmeldedaten. Dadurch wird Ihren Testsendungen eine weitere Sicherheitsschicht hinzugefügt. Für mehr Sicherheit benötigen Systemadministratoren von Organisationen mit [!UICONTROL Unternehmen] und [!UICONTROL Unbegrenzt] Pläne können diese Anforderung für alle in der Organisation erstellten Testsendungen konfigurieren.

Weitere Informationen zur erforderlichen Anmeldung finden Sie unter [Sicherheitsnachweis in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Wenn Ihr Unternehmen von den Validierern verlangt, Testsendungen elektronisch zu signieren, müssen Sie sich anmelden. [!DNL Workfront Proof], können Benutzer Testsendungen nur für registrierte Benutzer freigeben. Diese ist verfügbar unter [!UICONTROL Unternehmen] und [!UICONTROL Unbegrenzt] Bearbeitungspläne. Weitere Informationen finden Sie unter [Grundlagen zu elektronischen Signaturen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Kann ich eine Frist für meine Prüfer festlegen?

### Antwort

Sie können bei der Erstellung des Testversands einen Termin für einen neuen Testversand oder eine neue Testversand-Version festlegen. Dies tun Sie im Abschnitt [!UICONTROL Workflow] Abschnitt [!UICONTROL Neuer Testversand] Seite. Wenn Sie [!UICONTROL Automatisierter Workflow]können Sie für jede Phase Ihrer Überprüfung einen anderen Termin festlegen.

Sie können auch einen Termin für einen vorhandenen Testversand festlegen oder aktualisieren, indem Sie [!UICONTROL Testversanddetails] Seite. Weitere Informationen finden Sie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Wie kann ich eine neue Version meines Testversands erstellen?

### Antwort

Überprüfer fordern häufig Änderungen in ihren Kommentaren zu einem Testversand an und möchten eine neue Version des Testversands sehen. Sie können neue Versionen eines Testversands erstellen. [!DNL Workfront Proof] speichert die Testversand-Einstellungen aus der vorherigen Version. Sie können diese Einstellungen weiterhin bearbeiten, wenn Sie beispielsweise Prüfer für den Testversand hinzufügen oder entfernen möchten.

Sie müssen jede Version für die jeweiligen Validierer freigeben, die sie anzeigen müssen. Wenn Sie beispielsweise nur Version 3 mit einem Validierer teilen, kann diese Person die Versionen 1 und 2 nicht sehen. Supervisoren und Administratoren in Ihrem Konto überwachen alle Projekte in dem Konto, damit sie alle Versionen des Testversands sehen und bearbeiten können.

Weitere Informationen finden Sie unter .

## Kann ich Dateien mit [!DNL Workfront Proof]?

### Antwort

Ja. Wenn Sie etwas mit anderen Personen teilen möchten, sie aber nicht als Testversand ansehen müssen (oder wenn es sich um einen Dateityp handelt, der von [!DNL Workfront Proof]), können Sie sie als Datei in Ihre [!DNL Workfront Proof] -Konto. Wie bei Testsendungen können Sie Ihre Dateien in Ordnern organisieren und Dateien taggen sowie eine benutzerdefinierte Nachricht zur Benachrichtigungs-E-Mail hinzufügen, wenn Sie die Datei freigeben. Weitere Informationen finden Sie unter [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Wenn Ihre Empfänger die E-Mail-Benachrichtigung über eine freigegebene Datei erhalten, können sie die Datei herunterladen, indem sie auf den in der Benachrichtigung enthaltenen Link klicken.

[!DNL Workfront Proof] -Benutzer können Dateien nach dem Speichern in ihrem Konto in Testsendungen konvertieren.

<!--Is there a limit-->
