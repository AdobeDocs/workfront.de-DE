---
content-type: reference
navigation-topic: notifications
title: "Mitteilungen: Kommunikation"
description: Die folgenden Benachrichtigungen informieren Sie über die Kommunikation, z. B. über einen Aktualisierungskommentar, der für ein Arbeitselement erfolgt, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 4%

---

# Mitteilungen: Kommunikation

Die folgenden Benachrichtigungen informieren Sie über die Kommunikation, z. B. über einen Aktualisierungskommentar, der für ein Arbeitselement erfolgt, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Diese Benachrichtigungen informieren Sie über alle Kommentare, die zu einem bestimmten Artikel veröffentlicht wurden. Aus diesem Grund müssen Sie alle Benachrichtigungen gleichzeitig auswählen oder deaktivieren, um sie in einer täglichen Digest-E-Mail versenden zu können. Wenn Sie nur über bestimmte Kommentare benachrichtigt werden möchten, während diese auftreten, können Sie die einzelnen Benachrichtigungen für einen sofortigen Versand festlegen.

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>Einbezogene Felder </p> <p> *Nur tägliche Digest-Felder</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Jemand bezieht mich in eine gezielte Aktualisierung ein</strong> </p> <p>Eine gezielte Aktualisierung ist der Fall, wenn ein Benutzer einen anderen Benutzer in eine Aktualisierung einbezieht, wie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Aktualisierungen für [!UICONTROL Andere über Tags]</a>.</p> <p>In diesem Fall erhält der Benutzer, der in der empfohlenen Aktualisierung enthalten ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur gesendet, wenn der Benutzer über Zugriffsrechte für das Objekt verfügt.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL wollte wissen]</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist: <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Objektname, an dem die Aktualisierung vorgenommen wurde<br>Übergeordneter Objektname<br>Objektverweisnummer<br>Namen aller Benutzer und Teams, die in der direkten Aktualisierung enthalten sind<br>Datum und Uhrzeit der Aktualisierung<br>Text der direkten Aktualisierung<br><strong>[!UICONTROL Kommentar]</strong> button<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jedes Objekt erhaltenen Kommentare<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn Benutzer auf einen Arbeitsauftrag antworten, die Person, die den Auftrag erteilt hat, per E-Mail benachrichtigen</strong> </p> <p>Nachdem ein Benutzer eine Arbeitsanfrage sendet und ein anderer Benutzer auf diese Arbeitsanfrage antwortet, erhält der Benutzer, der die Anforderung gesendet hat, eine E-Mail-Benachrichtigung.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn:</p> 
    <ul> 
     <li> <p>Der Benutzer, der antwortet, ist derselbe Benutzer, der die Anfrage gestellt hat</p> </li> 
     <li> <p>Der Benutzer hat keinen Zugriff auf die Notiz.</p> </li> 
    </ul><strong>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Kommentar zu] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Anforderungsname<br>Projektname<br>Referenznummer<br>Name des Benutzers, der auf Ihre Anfrage geantwortet hat<br>Datum und Uhrzeit des Kommentars<br>Text des Kommentars zu Ihrer Anfrage<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jede Anfrage erhaltenen Kommentare<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Es wurde ein Kommentar zu meiner Anfrage gepostet</strong> </p> <p>Der primäre Ansprechpartner für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar in einer [!UICONTROL Help Desk]-Anfrage veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der primäre Ansprechpartner für das Problem.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Kommentar zu] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Anforderungsname<br>Projektname<br>Referenznummer<br>Name des Benutzers, der auf Ihre Anfrage geantwortet hat<br>Datum und Uhrzeit des Kommentars<br>Text des Kommentars zu Ihrer Anfrage<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jede Anfrage erhaltenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Es wird ein Kommentar zu meinem Dokument gepostet</strong> </p> <p>Der Eigentümer eines Dokuments in [!DNL Adobe Workfront] empfängt eine E-Mail-Benachrichtigung, wenn ein Kommentar im Dokument veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der Dokumenteigentümer.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet. </p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Kommentar zu] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Dokumentname<br>Projekt-, Aufgaben- oder Problemname<br>Referenznummer<br>Name des Benutzers, der auf Ihre Anfrage geantwortet hat<br>Datum und Uhrzeit des Kommentars<br>Text des Kommentars zum Dokument</td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand hat einen Thread kommentiert, an dem ich teilnehme</strong> </p> <p>Teilnehmer im Thread und Benutzer, die in einer Direktnachricht enthalten sind, erhalten eine E-Mail-Benachrichtigung, wenn ein Benutzer einen Kommentar im Thread abgibt.</p> <p>Benutzer müssen Zugriff auf die [!UICONTROL Ansicht] haben, um eine Benachrichtigung zu erhalten.</p> <p>Die folgenden Benutzer erhalten keine Benachrichtigung:</p> 
    <ul> 
     <li>In einer Direktnachricht enthaltene Teams</li> 
     <li>Der Eigentümer der Notiz</li> 
     <li>Der Primäre Kontakt</li> 
    </ul> <p><strong>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL RE: Kommentar zu] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Objektname<br>Übergeordneter Objektname<br>Name des Benutzers, der den Thread kommentiert hat<br>Text des Kommentars zum Thread<br>Datum und Uhrzeit des Kommentars<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jedes Objekt erhaltenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>[!UICONTROL Täglich]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand kommentiert eines meiner Arbeitselemente</strong> </p> <p>Der Verantwortliche des Arbeitselements erhält jedes Mal, wenn ein Benutzer ein Update zu einem Arbeitselement hinzufügt, eine E-Mail-Benachrichtigung, es sei denn, der Benutzer, der die Aktualisierung hinzufügt, ist auch der Verantwortliche. </p> <p>Wenn ein Kommentar zu einer Anfrage gepostet wird, senden Sie eine E-Mail an den Hauptkontakt des Problems.</p> <p>Der Hauptkontakt für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar auf einer Anfrage veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der primäre Ansprechpartner für das Problem.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Kommentar zu] &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Arbeitselementname<br>Projektname<br>Referenz für Arbeitselemente<br>Name des Benutzers, der das Arbeitselement kommentiert hat<br>Text des Kommentars zum Arbeitselement<br>Datum und Uhrzeit des Kommentars<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jedes Objekt erhaltenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand bezieht mein Team in eine gezielte Aktualisierung ein</strong> </p> <p>Eine gezielte Aktualisierung ist der Fall, wenn ein Benutzer einen anderen Benutzer in eine Aktualisierung einbezieht, wie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagging anderer Benutzer auf Updates</a>.</p> <p>In diesem Fall erhält jedes Mitglied des Teams, das in der empfohlenen Aktualisierung enthalten ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur an Benutzer gesendet, die über Zugriffsberechtigungen für das Objekt verfügen.</p> <p>Wenn der Benutzer, der die gezielte Aktualisierung sendet, Mitglied des Teams ist, das eingeschlossen ist, erhält der Benutzer, der die Aktualisierung sendet, keine E-Mail-Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: [!UICONTROL Kommentar] &lt;object name=""&gt; on &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Objektname<br>Übergeordneter Objektname<br>Objektverweisnummer<br>Name des Benutzers, der die gezielte Aktualisierung vorgenommen hat<br>Name aller Teams und Benutzer, die in der direkten Aktualisierung enthalten sind<br>Datum und Uhrzeit der gezielten Aktualisierung<br>Text der gezielten Aktualisierung<br><strong>[!UICONTROL Kommentar]</strong> button<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jedes Objekt erhaltenen Kommentare<br>*Projektname<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung </p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn Kommentar zu Benutzer hinzugefügt wird</strong> </p> <p>Sie können einen Benutzer auf der Registerkarte [!UICONTROL Updates] des Benutzerobjekts kommentieren. Sie können einen Benutzer auch kommentieren, wenn Sie die Einstellungen des Benutzers bearbeiten. Der Benutzer, gegen den der Kommentar abgegeben wird, erhält eine E-Mail, um ihn über diesen Kommentar zu benachrichtigen. </p> <p>Sie müssen über Berechtigungen für mindestens [!UICONTROL Ansicht] des Benutzers verfügen, um eine Aktualisierung auf der Registerkarte [!UICONTROL Updates] des Benutzers vornehmen zu können. Sie müssen über [!UICONTROL Bearbeitungsberechtigungen] für den Benutzer verfügen, um die Einstellungen des Benutzers bearbeiten zu können. </p> <p>Weitere Informationen zum Hinzufügen von Kommentaren zu Benutzern auf der Registerkarte Updates finden Sie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update der Arbeit</a>.</p> <p>Weitere Informationen zum Eingeben eines Kommentars für einen Benutzer beim Bearbeiten der Benutzereinstellungen finden Sie unter <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Meine Einstellungen konfigurieren</a>.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;user name=""&gt; [!UICONTROL wollte wissen]</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Ihr Benutzername<br>Name des Benutzers, der den Kommentar hinzugefügt hat<br>Text des Kommentars<br>Datum und Uhrzeit des Kommentars<br>*Gesamtzahl der eingegangenen Stellungnahmen<br>*Anzahl der für jedes Objekt erhaltenen Kommentare<br>*<strong>[!UICONTROL Alle Benachrichtigungen anzeigen]</strong> button<br>*Datum der täglichen Zusammenfassung </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
