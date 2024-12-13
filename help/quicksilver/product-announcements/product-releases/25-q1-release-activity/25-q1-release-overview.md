---
title: Übersicht über die Version im ersten Quartal 2025
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom ersten Quartal 2025 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 8b0c40d6fa5898581c50d6257bc2b2f2a4838b06
workflow-type: tm+mt
source-wordcount: '1728'
ht-degree: 0%

---

# Übersicht über die Version im ersten Quartal 2025

Diese Seite enthält Informationen zur Funktionalität, die in der Version vom ersten Quartal 2025 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.

<span class="preview">Off-Cycle-Funktionen (die vor dem Veröffentlichungsdatum des ersten Quartals 2025 in der Produktion veröffentlicht wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 enthielt die Option, Ihr Unternehmen auf monatliche Versionen umzustellen. Aus diesem Grund hat Workfront das Nummerierungsschema der Versionen geändert, um sowohl monatliche als auch vierteljährliche Veröffentlichungsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2025 lautet wie 25.4.
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Versionen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Version | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>24.11 (14. November 2024)</li><li>24.12 (12. Dezember 2024)</li><li>25.1 (15. Januar 2025)</li></ul> | <ul><li>25.1 (16. Januar 2025)</li></ul> |
>
>Beachten Sie, dass die Benutzer des Zeitplans für die schnelle Veröffentlichung jedes Quartals (25.1 in diesem Quartal) die Veröffentlichung einen Tag früher erhalten werden.
>
>Weitere Informationen zum Schnellfreigabeprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellfreigabeprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Verbesserungen für Administratoren](#administrator-enhancements)<!--* [Boards enhancements](#boards-enhancements)-->
* [Verbesserungen beim Dokumentenmanagement](#document-management-enhancements)
* [Home-Verbesserungen](#home-enhancements)
* [Proofing-Verbesserungen](#proofing-enhancements)
* [Verbesserungen an Berichten und Dashboards](#report-and-dashboard-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administrator-Verbesserungen

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungstermine</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Voreinstellung zur Verwendung von Projekt- oder Benutzerzeitplänen für Aufgaben mit einfacher Zuweisung</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Als System- oder Gruppenadministrator haben Sie jetzt eine neue Einstellung, um anzugeben, ob Workfront den Zeitplan des Projekts oder des Benutzers verwenden soll, um den Zeitplan des Projekts zu berechnen, wenn Sie einer Aufgabe einen Benutzer zuweisen und sowohl das Projekt als auch der Benutzer einem Zeitplan zugeordnet sind.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Geschäftsregeln unterstützen jetzt Hyperlinks</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Sie können jetzt Hyperlinks in die benutzerdefinierte Fehlermeldung einer Geschäftsregel einfügen, um Benutzende dabei zu unterstützen, ihre Aktion innerhalb der Beschränkung der Regel zu ändern. Die statische URL könnte eine Verknüpfung zu Dokumentationen oder anderen Seiten aufweisen, die für den Benutzer hilfreich wären.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Filtern von Feldern mit nativer automatischer Textvervollständigung ist jetzt verfügbar</a></p>
            <p>Wenn Sie einem benutzerdefinierten Formular einen nativen Feldverweis hinzufügen und es auf ein Feld mit automatischer Textvervollständigung verweist (z. B. Portfolio, Unternehmen oder Inhaber), ist jetzt eine Filteroption verfügbar. Mit dem Filter können Sie die Objekte einschränken, die Benutzerinnen und Benutzer bei der Verwendung des Felds auswählen können. Dieser benutzerdefinierte Filter funktioniert genauso wie ein Filter für ein benutzerdefiniertes Feld mit automatischer Textvervollständigung, wobei der Textmodus zum Definieren des Filters verwendet wird.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Symbol „Verschieben nach“ zu benutzerdefinierten Feldern hinzugefügt</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Wenn ein benutzerdefiniertes Formular mehrere Abschnitte mit vielen Feldern enthält, kann es schwierig sein, ein Feld durch Ziehen und Ablegen von einem Abschnitt in einen anderen zu verschieben. Zu jedem Feld wurde das Symbol „Verschieben nach“ hinzugefügt, über das Sie den Bereich auswählen können, in dem das Feld platziert werden soll.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau der Version: 29. Oktober 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
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

### Verbesserungen beim Dokumentenmanagement

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungstermine</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Gleichzeitiges Bearbeiten mehrerer Dokumente</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Sie können jetzt mehrere Dokumente gleichzeitig bearbeiten. Sie können die Beschreibungen bearbeiten und benutzerdefinierte Formulare aktualisieren.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 21. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Neuer zurückgezogener Status für Genehmigungen der Dokumentversion verfügbar</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Wenn eine neue Version zu einem Dokument mit ausstehenden Genehmigungen hinzugefügt wird, wird die Genehmigung für die vorherige Version jetzt als „Zurückgezogen“ angezeigt, was anzeigt, dass der vorherige Genehmigungsprozess aufgrund des Hinzufügens der neuen Version geschlossen wurde.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 7. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
            <p><i>Diese Funktion ist Teil einer stufenweisen Veröffentlichung und nur für bestimmte Kunden verfügbar.</i></p>
        </td>
    </tr>
</tbody>
</table>

### Home-Verbesserungen

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungstermine</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aktualisierungen der Arbeitsliste „Prioritäten“</a></p>
            [!BADGE New in Preview ]{type=Negative}
            <p>Wir haben die Prioritätenarbeitsliste aktualisiert, um die Funktionen zu verbessern und sie an andere Anwendungsbereiche anzupassen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 12. Dezember 2024</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Gehen Sie von „Prioritäten“ zur Detailseite eines Projekts.</a></p>
            <p>Sie können jetzt direkt von der Prioritätenarbeitsliste zu einem Projekt in Workfront gehen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau der Version: 5. Dezember 2024</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Aktualisierte Optionen in der Spalte Mein Fokus in Prioritäten</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Die Optionen in der Spalte Mein Fokus wurden aktualisiert, damit Sie Ihre Arbeit auf intuitivere Weise priorisieren und sortieren können. Zu den neuen Kennzeichnungen gehören</p>
            <ul>
                <li>Dringend</li>
                <li>Hoch</li>
                <li>Normal</li>
                <li>Niedrig</li>
            </ul>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
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
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Sie können jetzt Projektdetails und Kommentare aus der Arbeitsliste in Prioritäten anzeigen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau der Version: 6. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Proofing-Verbesserungen

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungstermine</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Neue Browser-Erweiterung für interaktive Überprüfung in der Beta-Version verfügbar</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Wir führen eine neue Browser-Erweiterung ein, das Adobe Workfront Review Tool, um die veraltete Browser-Erweiterung zur Überprüfung interaktiver ZIP-Inhalte zu ersetzen. Das neue Adobe Workfront-Überprüfungs-Tool unterstützt die Überprüfung von ZIP-Inhalten in allen gängigen Browsern.</p>
            <p>Die alte Browser-Erweiterung wird am 28. Februar 2025 entfernt.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 7. November 2024</li>
                <li><span class="preview">Produktionsversion für alle Kunden: 7. November 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

## Verbesserungen an Berichten und Dashboards

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Funktion</span></p>
        </td>
        <td>
            <p><span class="bold">Veröffentlichungstermine</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Schaltfläche zur Erstellung des erstmaligen Leserkontos für Data Connect</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Admins, die zum ersten Mal auf Data Connect zugreifen, haben jetzt die Möglichkeit, durch Anklicken einer einzigen Schaltfläche ein neues Snowflake-Leserkonto zu erstellen. Der Vorgang dauert einige Minuten, erfordert jedoch keine weiteren Maßnahmen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
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
            Aktualisierung zur Verwaltung von verschobenen oder gelöschten Assets in verknüpften Ordnern</a></p>
            [!BADGE In Production ]{type=Informative}
            <p>Wir haben die Art und Weise geändert, wie verschobene und gelöschte Assets bei Verwendung der Adobe Workfront-Integration mit Experience Manager Assets und Assets Essentials gehandhabt werden:</p>
            <ul>
                <li>Gelöschte Assets: Wenn ein Asset in einem verknüpften Ordner in Assets oder Assets Essentials gelöscht wird, bleibt das gelöschte Asset im Bereich der Projektdokumente erhalten.</li>
                <li>Verschobene Assets: Wenn ein Asset aus einem verknüpften Ordner in Assets oder Assets Essentials verschoben wird, bleibt das verschobene Asset im Bereich Projektdokumente erhalten.</li>
            </ul>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
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
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Wenn ein benutzerdefiniertes Formular mit mehreren Abschnitten an ein Objekt angehängt wird, können Sie jetzt alle Abschnitte mit Ausnahme des Standardabschnitts am oberen Rand des Formulars reduzieren und erweitern. Administratoren können diese Funktion auch in der Vorschau des Formulars im Formular-Designer sehen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau-Version: 11. November 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Der KI-Assistent kann jetzt mit Projekten, Aufgaben und Problemen arbeiten</a></p>
            [!BADGE In Production for Fast Release ]{type=Positive}
            <p>Um die Verwaltung Ihrer Arbeitselemente in Workfront zu vereinfachen, haben wir den KI-Assistenten für die Arbeit mit Projekten, Aufgaben und Problemen aktualisiert. Jetzt kann der KI-Assistent Projekte, Aufgaben und Probleme basierend auf von Ihnen angegebenen Kriterien suchen.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau der Version: 31. Oktober 2024</li>
                <li>Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024)</li>
                <li>Produktionsversion für alle Kunden: Mit Version 25.1 (Januar 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Lookand-Feel-Updates im ersten Quartal 2025</a></p>
            <p>Im ersten Quartal 2025 werden kleinere Aktualisierungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Lesen Sie die einzelnen Versionshinweise für bestimmte Veröffentlichungstermine.</p>
        </td>
        <td>
            <p><b>Verfügbar zu diesen Daten:</b></p>
            <ul>
                <li>Vorschau der Version: Im gesamten Zeitrahmen der Version für das erste Quartal 2025</li>
                <li><span class="preview">Produktionsversion: Lesen Sie die Versionshinweise für bestimmte Daten</span></li>
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

Neue Funktionen in Workfront Fusion sind außerhalb des Veröffentlichungszeitplans für das erste Quartal 2025 in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Workfront-Planungsverbesserungen

Neue Funktionen in Workfront Planning sind in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Planning-Aktivität für das erste Quartal 2025](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

### Verbesserungen am Workfront-Szenarioplaner

Es gibt derzeit keine Szenario-Planer-Aktualisierungen in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### Workfront-Zielverbesserungen

Es gibt derzeit keine Updates zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### API-Version 19

Für API-Version 19 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 19](/help/quicksilver/wf-api/api/new-api-version-19.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die im ersten Quartal 2025 durchgeführt wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt Neue Funktionen auf der Seite [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
