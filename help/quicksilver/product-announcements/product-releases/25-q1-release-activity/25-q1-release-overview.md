---
title: Übersicht über die Version des ersten Quartals 2025
description: Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom ersten Quartal 2025 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: cea70727aaaa867b55ce999f68a675c453840d41
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---

# Übersicht über die Version des ersten Quartals 2025

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom ersten Quartal 2025 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.

<span class="preview">Off-Cycle-Funktionen (diejenigen, die vor dem Ersten Quartal 2025 veröffentlicht wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 beinhaltet die Option, Ihr Unternehmen auf monatliche Releases umzustellen. Daher hat Workfront das Nummerierungsschema der Veröffentlichungen geändert, um sowohl die monatlichen als auch die vierteljährlichen Versionsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2025 lautet 25.4.
>
>Die monatlichen und vierteljährlichen Versionen sollen am Donnerstag der zweiten vollen Woche des Monats verfügbar sein, sofern nichts anderes angegeben ist.
>
>| Monatliche Version | Quartalsversion |
>|----|----|
>| <ul><li>24.11 (14. November 2024)</li><li>24.12 (12. Dezember 2024)</li><li>25.1 (15. Januar 2025)</li></ul> | <ul><li>25.1 (16. Januar 2025)</li></ul> |
>
>Beachten Sie, dass für die endgültige Version jedes Quartals (25.1 in diesem Quartal) die Benutzer des Zeitplans für die schnelle Veröffentlichung die Version einen Tag früher erhalten.
>
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Aktivieren oder Deaktivieren des Prozesses der schnellen Veröffentlichung](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Verbesserungen für Administratoren](#administrator-enhancements)<!--* [Boards enhancements](#boards-enhancements)-->
* [Verbesserungen bei der Dokumentenverwaltung](#document-management-enhancements)
* [Verbesserungen der Startseite](#home-enhancements)
* [Verbesserungen bei der Überprüfung](#proofing-enhancements)
* [Verbesserungen bei Berichten und Dashboards](#report-and-dashboard-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administratorverbesserungen

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungsdaten</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Verwendung des Projekt- oder Benutzerzeitplans für Einzelzuweisungsaufgaben</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Als System- oder Gruppenadministrator haben Sie jetzt eine neue Voreinstellung, um anzugeben, ob Workfront den Zeitplan des Projekts oder des Benutzers verwenden sollte, um die Timeline des Projekts zu berechnen, wenn Sie einer Aufgabe einen Benutzer zuweisen und sowohl das Projekt als auch der Benutzer einem Zeitplan zugeordnet sind.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Geschäftsregeln unterstützen jetzt Hyperlinks</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Sie können jetzt Hyperlinks in die benutzerdefinierte Fehlermeldung einer Geschäftsregel einfügen, um den Benutzer darauf hinzuweisen, wie er seine Aktion innerhalb der Beschränkung der Regel ändern kann. Die statische URL kann mit der Dokumentation oder anderen Seiten verknüpft werden, die für den Benutzer hilfreich sind.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Filtern nach nativen Typeahead-Feldern ist jetzt verfügbar</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Wenn Sie einen nativen Feldverweis zu einem benutzerdefinierten Formular hinzufügen und auf ein Typeahead-Feld verweisen (z. B. Portfolio, Firma oder Eigentümer), ist jetzt eine Filteroption verfügbar. Mit dem Filter können Sie die Objekte einschränken, die Benutzer bei der Verwendung des Felds auswählen können. Dieser benutzerdefinierte Filter funktioniert genauso wie ein Filter für ein benutzerdefiniertes typeahead-Feld, wobei der Textmodus zum Definieren des Filters verwendet wird.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Symbol "Verschieben nach"zu benutzerdefinierten Feldern hinzugefügt</a></p>
            [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
            <p>Wenn ein benutzerdefiniertes Formular mehrere Abschnitte mit vielen Feldern enthält, kann es schwierig sein, ein Feld durch Ziehen und Ablegen von einem Abschnitt in einen anderen zu verschieben. Jedem Feld wurde das Symbol "Verschieben nach"hinzugefügt, über das Sie den Bereich auswählen können, in dem das Feld platziert wird.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 29. Oktober 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

<!--### Boards enhancements

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Feature</span></p>
        </td>
        <td>
            <p><span class="bold">Release dates</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Change the owner of a board</a></p>
            <p>The creator of a board is the owner by default. The board owner is the only person who can delete that board or update its filters in the Configure panel. Functionality has been added to allow Workfront system administrators to change the owner of a board. The current owner of a board can also change the owner of that specific board.</p>
        </td>
        <td>
            <p><b>Available on these dates:</b></p>
            <ul>
                <li>Preview release: October 31, 2024</li>
                <li>Production for fast release: With the 24.11 release (November 14, 2024)</li>
                <li>Production release for all customers: With the 25.1 release (January 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>-->

### Verbesserungen bei der Dokumentenverwaltung

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungsdaten</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mehrere Dokumente gleichzeitig bearbeiten</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Sie können jetzt mehrere Dokumente gleichzeitig bearbeiten. Sie können die Beschreibungen bearbeiten und benutzerdefinierte Formulare aktualisieren.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Neuer Status "Entzogen"für Genehmigungen von Dokumentversionen verfügbar</a></p>
            [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
            <p>Wenn einem Dokument eine neue Version mit ausstehenden Genehmigungen hinzugefügt wird, wird die Genehmigung für die vorherige Version jetzt als "Zurückgezogen"angezeigt, was bedeutet, dass der vorherige Genehmigungsprozess aufgrund der neuen Version abgeschlossen wurde.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 7. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
            <p><i>Diese Funktion ist Teil einer stufenweisen Veröffentlichung und steht nur bestimmten Kunden zur Verfügung.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Verbesserungen der Startseite

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungsdaten</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aktualisierte Optionen in der Spalte Mein Fokus in Prioritäten</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Wir haben die Optionen in der Spalte Mein Fokus aktualisiert, damit Sie Ihre Arbeit intuitiver priorisieren und sortieren können. Die neuen Beschriftungen enthalten</p>
            <ul>
                <li>Dringend</li>
                <li>Hoch</li>
                <li>Normal</li>
                <li>Niedrig</li>
            </ul>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 14. November 2024</li>
                <li><span class="preview">Produktionsversion für alle Kunden: 14. November 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Anzeigen von Projektdetails in Prioritäten</a></p>
            [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
            <p>Sie können jetzt Projektdetails und Kommentare aus der Arbeitsliste in Prioritäten anzeigen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 6. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Verbesserungen bei der Überprüfung

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungsdaten</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Neue Browsererweiterung für interaktive Überprüfung in der Beta-Version</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Wir führen eine neue Browsererweiterung ein, das Adobe Workfront-Überprüfungstool, um die veraltete Browsererweiterung für die Überprüfung interaktiver ZIP-Inhalte zu ersetzen. Das neue Adobe Workfront-Überprüfungstool unterstützt die Überprüfung von ZIP-Inhalten in allen gängigen Browsern.</p>
            <p>Die ältere Browsererweiterung wird am 28. Februar 2025 entfernt.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 7. November 2024</li>
                <li><span class="preview">Produktionsversion für alle Kunden: 7. November 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Verbesserungen bei Berichten und Dashboards

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungsdaten</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Schaltfläche zur ersten Erstellung von Leserkonten für Data Connect</a></p>
            <p>Administratoren, die erstmals auf Data Connect zugreifen, haben jetzt die Möglichkeit, ein neues Snowflake-Leserkonto zu erstellen, indem sie auf eine Schaltfläche klicken. Der Vorgang dauert einige Minuten, erfordert jedoch keine weiteren Maßnahmen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 14. November 2024</li>
                <li><span class="preview">Produktionsversion für alle Kunden: 14. November 2024</span></li>
            </ul>
        </td>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aktualisierung der Verwaltung von verschobenen oder gelöschten Assets in verknüpften Ordnern</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Die Handhabung von verschobenen und gelöschten Assets bei der Verwendung der Adobe Workfront-Integration mit Experience Manager Assets und Assets Essentials wurde geändert:</p>
            <ul>
                <li>Gelöschte Assets: Wenn ein Asset innerhalb eines verknüpften Ordners in Assets oder Assets Essentials gelöscht wird, wird das gelöschte Asset im Bereich Projektdokumente beibehalten.</li>
                <li>Verschiebte Assets: Wenn ein Asset in Assets- oder Assets-Grundlagen aus einem verknüpften Ordner verschoben wird, wird das verschobene Asset im Bereich "Projekte - Dokumente"beibehalten.</li>
            </ul>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li><span class="preview">Produktionsversion für alle Kunden: 5. Dezember 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Abschnitte in einem benutzerdefinierten Formular sind jetzt ausblendbar und erweiterbar</a></p>
            <p>Wenn ein benutzerdefiniertes Formular mit mehreren Abschnitten an ein Objekt angehängt wird, können Sie jetzt alle Abschnitte mit Ausnahme des Standardabschnitts oben im Formular ausblenden und erweitern. Der Administrator kann diese Funktion auch bei der Vorschau des Formulars im Formularentwickler sehen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 11. November 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Der KI-Assistent kann jetzt mit Projekten, Aufgaben und Problemen arbeiten</a></p>
            [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
            <p>Um die Verwaltung Ihrer Arbeitselemente in Workfront zu vereinfachen, haben wir den KI-Assistenten aktualisiert, um mit Projekten, Aufgaben und Problemen zu arbeiten. Jetzt kann AI Assistant Projekte, Aufgaben und Probleme basierend auf von Ihnen festgelegten Kriterien finden.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Version: 31. Oktober 2024</li>
                <li>Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit der Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Look-and-Feel-Aktualisierungen während des Zeitrahmens für das erste Quartal 2025</a></p>
            <p>Im ersten Quartal 2025 werden geringfügige Änderungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Terminen:</b></p>
            <ul>
                <li>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des ersten Quartals 2025</li>
                <li><span class="preview">Produktionsversion: Versionshinweise zu bestimmten Daten lesen</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Ankündigungen

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung ab einem Zeitpunkt verfügbar, der außerhalb des Veröffentlichungszeitplans für das erste Quartal 2025 liegt. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen der Workfront-Planung

Neue Funktionen in der Workfront-Planung sind in der Produktion verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Planning First Quarter 2025 release activity](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Verbesserungen bei Workfront-Zielen

Es gibt derzeit keine Aktualisierungen zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### API-Version 19

Für API Version 19 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Weitere Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API-Version 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version vom ersten Quartal 2025 vorgenommen wurden, finden Sie unter [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;auf der Seite [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
