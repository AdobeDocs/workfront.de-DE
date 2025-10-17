---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Kommunikation'
description: Die folgenden Benachrichtigungen informieren Sie über Kommunikationsvorgänge, z. B. einen Aktualisierungskommentar, die bei einem von Ihnen verwendeten Arbeitselement erfolgen. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen .
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# Benachrichtigungen: Kommunikation

Die folgenden Benachrichtigungen informieren Sie über Kommunikationsvorgänge, z. B. einen Aktualisierungskommentar, die bei einem von Ihnen verwendeten Arbeitselement erfolgen. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Diese Benachrichtigungen informieren Sie über alle Kommentare, die zu einem bestimmten Element gepostet wurden. Aus diesem Grund müssen Sie alle Benachrichtigungen gleichzeitig auswählen oder abwählen, um sie in einer Daily Digest-E-Mail zu erhalten. Wenn Sie über bestimmte Kommentare nur direkt benachrichtigt werden möchten, können Sie die einzelnen Benachrichtigungen für den sofortigen Versand angeben.

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>Enthaltene Felder </p> <p> *Nur Tägliche Digest-Felder</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Jemand bezieht mich in eine gezielte Aktualisierung ein</strong> </p> <p>Ein direktes Update liegt vor, wenn ein Benutzer einen anderen Benutzer explizit in ein Update einbezieht, wie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag other on] Updates beschrieben</a>.</p> <p>In diesem Fall erhält der Benutzer, der an der weitergeleiteten Aktualisierung beteiligt ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur gesendet, wenn der Benutzer über Zugriffsrechte für das Objekt verfügt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>&lt;Name des Benutzers, der Sie in das Update eingebunden hat&gt; [!UICONTROL wollte Sie wissen]</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em>[!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> Objektname, an dem die Aktualisierung vorgenommen wurde<br>Übergeordneter Objektname<br>Objektverweisnummer<br>Namen aller Benutzer und Teams, die in der gerichteten Aktualisierung enthalten waren<br>Datum und Uhrzeit, an dem die Aktualisierung vorgenommen wurde<br>Text der gerichteten Aktualisierung<br><strong>[!UICONTROL Comment]</strong><br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jedes Objekt empfangenen Kommentare<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong>-Schaltfläche<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand antwortet auf meine Anfrage</strong> </p> <p>Nachdem ein(e) Benutzende(r) eine Arbeitsanfrage gesendet hat und ein(e) andere(r) Benutzende(r) auf diese Arbeitsanfrage antwortet, erhält der/die Benutzende, der/die die Anfrage gesendet hat, eine E-Mail-Benachrichtigung.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn:</p> 
    <ul> 
     <li> <p>Der Benutzer, der antwortet, ist derselbe Benutzer, der die Anfrage gestellt hat</p> </li> 
     <li> <p>Der/die Benutzende hat keinen Zugriff, um die Anmerkung anzuzeigen</p> </li> 
    </ul><strong>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Comment on] &lt;Request Name&gt; on &lt;Projektname&gt; (ref# &lt;Referenznummer der Anfrage&gt;)</em></strong> Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></td> 
   <td> Anfragename<br>Projektname<br>Referenznummer<br>Name des Benutzers, der auf Ihre Anfrage geantwortet hat<br>Datum und Uhrzeit, zu der der Kommentar abgegeben wurde<br>Text des Kommentars zu Ihrer Anfrage<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jede Anfrage empfangenen Kommentare<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> Schaltfläche<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Kommentar zu meiner Anfrage wurde veröffentlicht</strong> </p> <p>Der primäre Kontakt für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar zu einer [!UICONTROL Helpdesk]-Anfrage gepostet wird, es sei denn, der Benutzer, der den Kommentar gepostet hat, ist auch der primäre Kontakt für das Problem.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Kommentar zu] &lt;Anfragename&gt; auf &lt;Projektname&gt; (ref# &lt;Anfragenummer&gt;)</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> Anfragename<br>Projektname<br>Referenznummer<br>Name des Benutzers, der auf Ihre Anfrage geantwortet hat<br>Datum und Uhrzeit, zu der der Kommentar abgegeben wurde<br>Text des Kommentars zu Ihrer Anfrage<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jede Anfrage erhaltenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong>-Schaltfläche<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Kommentar zu meinem Dokument wird hinzugefügt</strong> </p> <p>Der Inhaber eines Dokuments in [!DNL Adobe Workfront] erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar zu dem Dokument veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der Dokumentbesitzer.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist. </p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Kommentar zu] &lt;Anfragename&gt; auf &lt;Projektname&gt; (ref# &lt;Anfragenummer&gt;)</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td>Dokumentname<br>Projekt, Aufgabe oder Problemname/<br>/<br>/Name des Benutzers, der auf Ihre Anfrage geantwortet hat <br>/Datum und Uhrzeit, zu der der Kommentar <br> wurde/Text des Kommentars zum Dokument</td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand kommentiert einen Thread, an dem ich teilnehme</strong> </p> <p>Teilnehmer am Thread und Benutzer, die in einer Direktnachricht enthalten sind, erhalten eine E-Mail-Benachrichtigung, wenn ein Benutzer einen Kommentar im Thread abgibt.</p> <p>Benutzer müssen über Zugriff auf [!UICONTROL View] verfügen, um eine Benachrichtigung zu erhalten.</p> <p>Die folgenden Benutzer erhalten keine Benachrichtigung:</p> 
    <ul> 
     <li>Teams, die in einer Direktnachricht enthalten sind</li> 
     <li>Der Besitzer der Notiz</li> 
     <li>Der Primäre Ansprechpartner</li> 
    </ul> <p><strong>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL RE: Kommentar zu] &lt;Objektname&gt;&lt;Objekttyp&gt; auf &lt;Projektname&gt;(ref# &lt;Objektreferenznummer&gt;</em>)</strong> </p> <p><strong> Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Datum der täglichen Digest&gt;</em></strong> </p> </td> 
   <td> Objektname<br>übergeordnetes ObjektName<br>Name des Benutzers, der den Thread kommentiert hat<br>Text des Kommentars zum Thread<br>Datum und Uhrzeit des Kommentars<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jedes Objekt empfangenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong>-Schaltfläche<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand kommentiert eines meiner Arbeitselemente</strong> </p> <p>Der Bevollmächtigte des Arbeitselements erhält jedes Mal eine E-Mail-Benachrichtigung, wenn ein Benutzer ein Update zu einem Arbeitselement hinzufügt, es sei denn, der Benutzer, der das Update hinzufügt, ist auch der Bevollmächtigte. </p> <p>Wenn ein Kommentar zu einer Anfrage gepostet wird, senden Sie eine E-Mail an den primären Kontakt für das Problem.</p> <p>Der primäre Kontakt für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar zu einer Anfrage gepostet wird, es sei denn, der Benutzer, der den Kommentar gepostet hat, ist auch der primäre Kontakt für das Problem.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Kommentar zu] &lt;Name des Arbeitselements&gt; auf &lt;Projektname (ref# &lt;Referenznummer des Arbeitselements&gt;)</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> Name des Arbeitselements<br> Projektname<br>Referenznummer des Arbeitselements<br>Name des Benutzers, der das Arbeitselement kommentiert hat<br>Text des Kommentars zum Arbeitselement<br>Datum und Uhrzeit, zu der der Kommentar abgegeben wurde<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jedes Objekt empfangenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand schließt mein Team in eine direkte Aktualisierung ein</strong> </p> <p>Eine direkte Aktualisierung liegt vor, wenn ein Benutzer einen anderen Benutzer explizit in eine Aktualisierung einbezieht, wie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere bei Aktualisierungen </a>.</p> <p>In diesem Fall erhält jedes Teammitglied, das an der weitergeleiteten Aktualisierung beteiligt ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur an Benutzer gesendet, die über Zugriffsrechte für das Objekt verfügen.</p> <p>Wenn der Benutzer, der die direkte Aktualisierung sendet, Mitglied des Teams ist, das die Aktualisierung sendet, erhält der Benutzer, der die Aktualisierung sendet, keine E-Mail-Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: [!UICONTROL Kommentar zu] &lt;Objektname&gt; auf &lt;Name des übergeordneten Objekts&gt; (ref# &lt;Objektreferenznummer&gt;)</p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> <p>Objektname<br>übergeordneter Objektname<br>Objektreferenz-Nummer<br>Name des Benutzers, der die direkte Aktualisierung vorgenommen hat<br>Name aller Teams und Benutzer, die in der direkten Aktualisierung enthalten sind<br>Datum und Uhrzeit, an der die direkte Aktualisierung vorgenommen wurde<br>Text der direkten Aktualisierung<br><strong>[!UICONTROL Comment]</strong> button<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der für jedes Objekt empfangenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong>Schaltfläche<br>*Datum der täglichen Zusammenfassung </p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn Kommentar zu Benutzer hinzugefügt wird</strong> </p> <p>Auf der Registerkarte [!UICONTROL Updates] des Benutzerobjekts können Sie einen Kommentar zu einem Benutzer abgeben. Sie können auch einen Kommentar zu einem Benutzer abgeben, wenn Sie die Einstellungen des Benutzers bearbeiten. Der Benutzer, zu dem der Kommentar gesendet wird, erhält eine E-Mail, um ihn über diesen Kommentar zu informieren. </p> <p>Sie müssen über Berechtigungen für mindestens [!UICONTROL View] den Benutzer verfügen, um eine Aktualisierung auf der Registerkarte [!UICONTROL Updates] des Benutzers eingeben zu können. Sie müssen über [!UICONTROL Bearbeiten]-Berechtigungen für den Benutzer verfügen, um die Einstellungen des Benutzers bearbeiten zu können. </p> <p>Weitere Informationen über Benutzerkommentare auf der Registerkarte Aktualisierungen finden Sie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a>.</p> <p>Weitere Informationen zur Eingabe eines Kommentars zu einem Benutzer, wenn Sie die Einstellungen des Benutzers bearbeiten, finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Konfigurieren meiner Einstellungen</a>.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Benutzername&gt; [!UICONTROL wollte Sie wissen]</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> Benutzername<br>Name des Benutzers, der den Kommentar hinzugefügt hat<br>Text des Kommentars<br>Datum und Uhrzeit des Kommentars<br>*Gesamtzahl der eingegangenen Kommentare<br>*Anzahl der eingegangenen Kommentare für jedes Objekt<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong>-Schaltfläche<br>*Datum der täglichen Zusammenfassung </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
