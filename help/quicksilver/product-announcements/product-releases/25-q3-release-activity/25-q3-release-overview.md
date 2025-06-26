---
title: Versionsübersicht für das dritte Quartal 2025
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom dritten Quartal 2025 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9342f393-a404-44b4-aad6-2c4cf634dfd5
source-git-commit: e3fa5f6fd86f0fe9ba221fb7c20f46f966437a42
workflow-type: tm+mt
source-wordcount: '1627'
ht-degree: 3%

---

# Versionsübersicht für das dritte Quartal 2025

Diese Seite enthält Informationen zur Funktionalität, die in der für Juli 2025 geplanten Version vom dritten Quartal 2025 enthalten ist.

Die Verbesserungen auf dieser Seite sind in der Vorschau -Umgebung verfügbar. Diese Seite wird mit zusätzlichen Verbesserungen aktualisiert, sobald die geplante Produktionsversion des dritten Quartals 2025 näher rückt.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Versionen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Version | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>25.5 (Mai 2025)</li><li>25.6 (Juni 2025)</li><li>25.7 (Juli 2025)</li></ul> | <ul><li>25.7 (Juli 2025)</li></ul> |
>
>Beachten Sie, dass die Benutzer des Zeitplans für die schnelle Veröffentlichung jedes Quartals (25.7 in diesem Quartal) die Veröffentlichung einen Tag früher erhalten werden.
>
>Weitere Informationen zum Schnellfreigabeprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellfreigabeprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).



## Adobe Workfront-Verbesserungen

* [Verbesserungen beim Dokumentenmanagement](#document-management-enhancements)
* [Home-Verbesserungen](#home-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen beim Reporting](#reporting-enhancements)
* [Verbesserungen bei Aktualisierungen und Benachrichtigungen](#update-and-notification-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Verbesserungen beim Proofing und Dokumentenmanagement

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Desktop Proofing Viewer-Update</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Der Desktop Proofing Viewer wurde auf Version 2.1.50 aktualisiert. Diese Aktualisierung umfasst Aktualisierungen der internen Tools und wirkt sich nicht auf die Endbenutzerfunktionen aus.</p>
        </td>
        <td>Samstag, 13. Juni 2025</td>
        <td>Samstag, 13. Juni 2025</td>
        <td>Samstag, 13. Juni 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Proofing- und GenStudio for Performance Marketing-Integration</a>
            <p>Wir freuen uns, eine neue Integration zwischen Proofing und GenStudio for Performance Marketing einführen zu können. Mit dieser Integration können Sie 
            <ul>
            <li>Verwenden von Workfront-Genehmigungsvorlagen zum Definieren von Genehmigungs-Workflows
            </li>
             <li>Überprüfen von GenStudio-Entwurfsinhalten im Proofing Viewer
            </li>
             <li>Siehe Entscheidungen zur endgültigen Genehmigung und Veröffentlichung in GenStudio überprüfen 
            </li>
            </ul>
            </p>
        </td>
        <td>Freitag, 12. Juni 2025</td>
        <td>Freitag, 12. Juni 2025</td>
        <td>Freitag, 12. Juni 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Desktop Proofing Viewer-Update</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Dieses Update ist eine Fehlerbehebung, um die Kompatibilität des Desktop Viewers mit Mac-Betriebssystemen sicherzustellen. Elektronen wurde auf 34,4,0 herabgestuft und Chrom auf 132.</p>
        </td>
        <td>Donnerstag, 7. Mai 2025</td>
        <td>Donnerstag, 7. Mai 2025</td>
        <td>Donnerstag, 7. Mai 2025</td>
    </tr> 
      <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Assets in einem verknüpften Google-Ordner muss einzeln hinzugefügt werden, damit es in Workfront angezeigt wird</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Google <a href="https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps">verbessert die Sicherheitskontrollen</a>
            für Anwendungen von Drittanbietern, die auf Google Drive zugreifen, sodass Anwendungen ein Einverständnismodell pro Benutzer anwenden müssen. Daher müssen einzelne Assets einzeln verknüpft werden, damit sie in Workfront sichtbar sind. Siehe <a href="/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md">Konfigurieren von Dokumentenintegrationen</a>
             für weitere Informationen. </p>
        </td>
        <td>29. Mai 2025</td>
        <td>29. Mai 2025</td>
        <td>29. Mai 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Entscheidungsschaltflächen für Dokumentgenehmigungen in der Proofing-Anzeige verfügbar</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Die neuen Schaltflächen für die Entscheidung zur Dokumentgenehmigung werden jetzt in der Proofing-Anzeige angezeigt. Wenn Sie jetzt einen einfachen Korrekturabzug erstellen und genehmigende Personen und Prüfende aus der Dokumentzusammenfassung hinzufügen, können diese ihre Entscheidung direkt in der Korrekturabzugsansicht treffen.</p>
        </td>
        <td>Freitag, 10. April 2025</td>
        <td>17. April 2025</td>
        <td>17. April 2025</td>
    </tr>     
  </tbody>
</table>

### Home-Verbesserungen

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
       <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity//25-q3-home-enhancements.md" class="MCXref xref" xrefformat="{para}">All Approvals widget renamed to Document approval metrics</a><p></p>
            <p>We've renamed the All Approvals widget to Document Approval Metrics to more accurately reflect the information it displays. The Document Approval Metrics widget provides high-level insights into document approvals for the projects you own.</p>
        </td>
        <td>TBD</td>
        <td>TBD</td>
        <td>TBD</td>
    </tr> -->   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity//25-q3-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Aktualisiertes Kommentierungserlebnis im Abschnitt „Erwähnungen“ im Bereich „Meine Aktualisierungen“</a><p></p>
            <p>Die Kommentierungserfahrung im Abschnitt „Erwähnungen“ im Bereich „Meine Aktualisierungen“ wird aktualisiert. Dasselbe Erlebnis im Bereich „Updates“ für die meisten Workfront-Objekte ist jetzt auch im Abschnitt „Erwähnungen“ von „Meine Updates“ verfügbar.</p>
        </td>
        <td>Freitag, 19. Dezember 2024</td>
        <td>Freitag, 19. Juni 2025</td>
        <td>Freitag, 19. Juni 2025</td>
    </tr>     
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity//25-q3-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Das Widget Meine Genehmigungen wird jetzt automatisch nach </a> sortiert<p></p>
            <p>Das Widget Meine Genehmigungen auf der Startseite wurde aktualisiert, sodass standardmäßig nach Frist (absteigend) sortiert wird. Dadurch können die dringendsten Genehmigungen oben in der Liste angezeigt werden. </p><p><b>Hinweis</b> Derzeit können im Widget Meine Genehmigungen nur Korrekturabzugsgenehmigungen nach Frist sortiert werden.</p>
        </td>
        <td>29. Mai 2025</td>
        <td>Freitag, 12. Juni 2025</td>
        <td>Freitag, 17. Juli 2025</td>
    </tr>     
  </tbody>
</table>

### Projektverbesserungen

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Vorhandenes Feld „Tatsächliche Stunden“ wurde durch das Feld „Alte tatsächliche Stunden“ ersetzt und neues Feld „Tatsächliche Stunden“ wurde erstellt</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Das vorhandene Feld „Tatsächliche Stunden“ wurde in „Frühere Tatsächliche Stunden“ umbenannt. In diesem Feld wird die für Projekte, Aufgaben und Probleme protokollierte Zeit in Minuten gespeichert. Das Feld wird in der Workfront-Datenbank als actualWorkRequired gespeichert. </p>
            <p>Wir haben ein neues Feld Tatsächliche Stunden hinzugefügt, das die für Projekte, Aufgaben und Probleme protokollierte Zeit mit Dezimalpräzision in Stunden speichert. Das Feld wird in der Workfront-Datenbank als actualWorkRequiredDouble gespeichert.</p>
        </td>
        <td>Mittwoch, 24. Juni 2025</td>
        <td>Mittwoch, 24. Juni 2025</td>
        <td>Mittwoch, 24. Juni 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Änderung der Art und Weise, wie die tatsächlichen Stunden für API-Aufrufe in der Datenbank gespeichert werden</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Diese Aktualisierung führt zu einer Änderung der Art und Weise, wie die tatsächlichen Stunden für Projekte, Aufgaben und Probleme in der Datenbank gespeichert werden. Ab dieser Aktualisierung verwenden die tatsächlichen Stunden ein <code>actualWorkRequiredDouble</code> (mit einem Wert in Stunden).</p>
        </td>
        <td>Mit der nächsten API-Version, die für Ende 2025 geplant ist</td>
        <td>Mit der nächsten API-Version, die für Ende 2025 geplant ist</td>
        <td>Mit der nächsten API-Version, die für Ende 2025 geplant ist</td>
    </tr>     
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Aktualisieren Sie in mithilfe des Schiebereglers Prozent abgeschlossen in einer Aufgaben- oder Problem-Kopfzeile</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Die Funktionsweise des Schiebereglers Prozent abgeschlossen für Aufgaben und Probleme wurde aktualisiert. Wenn Sie die blaue Blase Prozent abgeschlossen in die Kopfzeile einer Aufgabe oder eines Problems schieben, wird der Prozentsatz der Fertigstellung der Aufgabe oder des Problems jetzt in Schritten von fünf Punkten aktualisiert. Vor diesem Update wurden durch Schieben der blauen Blase Prozent abgeschlossen die Aufgaben oder Probleme in Schritten von einem Punkt aktualisiert.</p>
        </td>
        <td>Mittwoch, 27. Mai 2025</td>
        <td>Mittwoch, 27. Mai 2025</td>
        <td>Mittwoch, 27. Mai 2025</td>
    </tr>     
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mehr Transparenz bei der Verwendung des KI-Assistenten für Projekte, Aufgaben und Probleme</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Um klarer zu machen, wie der KI-Assistent Antworten auf Fragen zu Workfront-Projekten, -Aufgaben und -Problemen findet, haben wir diese Informationen zur Frageantwort hinzugefügt. Jetzt fügt der KI-Assistent seine Suchinformationen in die Ausgabe ein. Sie können diese Informationen verwenden, um zu überprüfen, ob der KI-Assistent die von Ihnen gestellte Frage korrekt identifiziert hat, und um den Kontext der Antwort zu verstehen.</p>
        </td>
        <td>Dienstag, 19. Mai 2025</td>
        <td>Dienstag, 19. Mai 2025</td>
        <td>Dienstag, 19. Mai 2025</td>
    </tr>     
  </tbody>
</table>



### Verbesserungen beim Reporting

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
      <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Erweiterte </a> für die Berichtbereitstellung<p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Wir haben die geplante Bereitstellung von Berichten verbessert, um sicherzustellen, dass Workfront-Benachrichtigungen nur an E-Mail-Domains gesendet werden, die in der -Zulassungsliste genehmigt wurden.</p>
            <p></p>
        </td>
        <td>Freitag, 26. Juni 2025</td>
        <td>(Schrittweiser Rollout): 26. Juni bis 9. Juli 2025</td>
        <td>(Schrittweiser Rollout): 26. Juni bis 9. Juli 2025</td>
    </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Benutzer-Platzhalter geben beim Filtern von </a> keine Ergebnisse mehr mit einem Nullwert zurück<p></p>
            <p>Das Verhalten der Benutzer-Platzhalter wurde aktualisiert, um beim Filtern eines Berichts einen Nullwert auszuschließen. Diese Änderung hilft dem Filter, genauere Ergebnisse zu erzielen, anstatt Ergebnisse zurückzugeben, bei denen ein Benutzer nicht richtig konfiguriert ist (ein Nullergebnis). </p>
        </td>
        <td>Donnerstag, 30. April 2025</td>
        <td>Freitag, 15. Mai 2025</td>
        <td>Freitag, 17. Juli 2025</td>
    </tr>     
  </tbody>
</table>

### Verbesserungen bei Aktualisierungen und Benachrichtigungen

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-update-and-notification-enhancements.md" class="MCXref xref" xrefformat="{para}">Geändertes Erlebnis beim Hinzufügen von Personen zu Kommentaren</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Um eine verbesserte Leistung zu erzielen, haben wir ein geändertes Erlebnis eingeführt, wenn Personen zu Kommentaren hinzugefügt werden. Jetzt bleibt der Link „Personen oder Teams taggen“ im Kommentarfeld bestehen, nachdem Sie Benutzer oder Teams zum Kommentar hinzugefügt haben. </p>
        </td>
        <td>Donnerstag, 30. April 2025</td>
        <td>(Schrittweiser Rollout): 8. Mai bis 15. Mai 2025</td>
        <td>(Schrittweiser Rollout): 8. Mai bis 15. Mai 2025</td>
    </tr>     
  </tbody>
</table>

### Weitere Verbesserungen

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Funktion</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Updates im dritten Quartal 2025</a></p>
                        <p>Geringfügige Aktualisierungen des Erscheinungsbilds verschiedener Bereiche des Adobe Workfront-Programms werden innerhalb des Zeitrahmens des dritten Quartals 2025 vorgenommen. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: Im gesamten Zeitrahmen der Version für das dritte Quartal 2025<br /></p>
                            </li>
                            <li>
                                <p>Produktionsfreigabe: Mindestens 2 Wochen nach der Freigabe für die Vorschau (sofern nicht anders angegeben)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernisierung der Benutzeroberfläche

Wir aktualisieren die Benutzeroberfläche in Adobe Workfront, um das Benutzererlebnis zu verbessern und es mit anderen Adobe-Programmen zu vereinheitlichen. Diese Änderungen werden außerhalb des standardmäßigen Veröffentlichungszeitplans veröffentlicht. Eine Liste dieser Änderungen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Versionshinweise für andere Bereiche

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung in einem zeitlichen Abstand außerhalb des standardmäßigen Veröffentlichungszeitplans verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Workfront-Planungsverbesserungen

Neue Funktionen in Workfront Planning sind in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront-Planungs-Aktivität für das dritte Quartal 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q3.md).

Für Folgendes gibt es derzeit keine Aktualisierungen in der Version:

* Szenarienplaner
* Korrekturabzug
* Ziele

## Ankündigungen

### Neue Version von Workfront für Microsoft Teams

Da [Microsoft auf den neuen Teams-Client umstellt](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) ist der Classic Teams-Client nach dem 1. Juli 2025 nicht mehr verfügbar. Um Microsoft Teams und integrierte Apps wie Workfront weiterhin verwenden zu können, müssen Kunden vor diesem Datum zum neuen Teams-Client wechseln.

Die aktualisierte Workfront-Integration ist jetzt verfügbar und vollständig mit der neuen Team-Erfahrung kompatibel. In den meisten Fällen wird Workfront automatisch angezeigt, sobald Benutzende den Wechsel vollzogen haben. Ist dies nicht der Fall, kann die Integration manuell über die Microsoft Teams App Store installiert werden. Informationen zum Installieren oder Überprüfen der Workfront-Integration im neuen Team-Client finden Sie unter [Installieren [!DNL Adobe Workfront]  für Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront für Microsoft Outlook

[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.

* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**

Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**

### API-Version 20

Workfront API Version 20 wurde am 4. Mai 2024 veröffentlicht. Für die API-Version 20 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 20](/help/quicksilver/wf-api/api/new-api-version-19.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die im ersten Quartal 2025 durchgeführt wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=de).

### Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt Neue Funktionen auf der Seite [Workfront-Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).



<!-- HTML you might need

New table

### add product area name

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    </tr>
    <tr>
        <td>
            <p>Title</p>
            <p>Body</p>
        </td>
        <td>Date</td>
        <td>Date</td>
        <td>Date</td>
    </tr>     
  </tbody>
</table> 

New row for table 

<tr>
    <td>
        <p>Title</p>
        <p>Body</p>
    </td>
        <td>Date</td>
        <td>Date</td>
        <td>Date</td>
    </tr>   



-->

