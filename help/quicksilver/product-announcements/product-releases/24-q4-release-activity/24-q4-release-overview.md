---
title: Übersicht über die Version 2024 im vierten Quartal
description: Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom vierten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '1606'
ht-degree: 0%

---

# Übersicht über die Version 2024 im vierten Quartal

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom vierten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.

<span class="preview">Off-Cycle-Funktionen (diejenigen, die vor dem Veröffentlichungsdatum des vierten Quartals 2024 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 beinhaltet die Option, Ihr Unternehmen auf monatliche Releases umzustellen. Daher hat Workfront das Nummerierungsschema der Veröffentlichungen geändert, um sowohl die monatlichen als auch die vierteljährlichen Versionsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2024 lautet 24.4.
>
>Die monatlichen und vierteljährlichen Versionen sollen am Donnerstag der zweiten vollen Woche des Monats verfügbar sein, sofern nichts anderes angegeben ist.
>
>| Monatliche Version | Quartalsversion |
>|----|----|
>| <ul><li>24.8 (15. August 2024)</li><li>24.9 (12. September 2024)</li><li>24.10 Uhr (Oktober 2024)</li></ul> | <ul><li>24.10 Uhr (Oktober 2024)</li></ul> |
>
>Beachten Sie, dass für die endgültige Version jedes Quartals (24.10 in diesem Quartal) die Benutzer des Zeitplans für die schnelle Veröffentlichung die Version einen Tag früher erhalten.
>
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Aktivieren oder Deaktivieren des Prozesses der schnellen Veröffentlichung](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen bei der Überprüfung](#proofing-enhancements)
* [Verbesserungen bei Berichten und Dashboards](#report-and-dashboard-enhancements)
* [Weitere Verbesserungen](#other-enhancements)
* [Funktion wird bald aus Workfront entfernt](#functionality-soon-to-be-removed-from-workfront)

### Administratorverbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">In Layoutvorlagen ist jetzt die Option "Alle auswählen"verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um das Anzeigen und Ausblenden von Feldern mit Layoutvorlagen zu vereinfachen, wurde den Bereichen Übersicht und Finanzen in der Detailansicht in einer Layoutvorlage das Kontrollkästchen "Alle auswählen"hinzugefügt. Diese Option ist verfügbar, wenn Sie Projekt, Aufgabe, Problem, Portfolio oder Programm unter "Anpassen, was Benutzer sehen"ausgewählt haben.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. August 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 29. August 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Weiterleiten von Umgebungs-Promotion-Paketen</a></p>
                        [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
                        <p>Um die Umgebungsförderung flexibler und benutzerfreundlicher zu gestalten, haben wir die Rollback-Funktion aktiviert. Jetzt können Sie Pakete innerhalb von 24 Stunden zurücksetzen, um frühere Konfigurationen, die von einem Umgebungs-Promotionpaket betroffen sind, leichter wiederherzustellen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. August 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.9 (12. September 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.10 (Oktober 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Layout-Schaltfläche im benutzerdefinierten Formularentwickler erlaubt zwei oder drei Spalten</a></p>
                        <p>Mit der Schaltfläche "Layout"im benutzerdefinierten Formularentwickler können Sie aus einem zweispaltigen oder dreiseitigen Arbeitsbereich wählen. Der ursprüngliche Formularentwickler verwendet drei Spalten und die Feldeinstellungen werden in der Spalte ganz rechts angezeigt. Wenn Sie zwei Spalten auswählen, werden die Feldeinstellungen in der Spalte ganz links neben der Feldbibliothek angezeigt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. August 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.9 (12. September 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: TBD</p>
                            </li>
                        </ul>
                        <p><i>Diese Funktion ist Teil einer stufenweisen Veröffentlichung und wird im September für eine begrenzte Anzahl von Kunden verfügbar sein.</i></p>
                    </td>
                </tr>
           </tbody>
        </table>

### Integrationsverbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen bei der Anmeldung bei Outlook-Integrationen</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Die Anmeldeerfahrung für die Outlook-Integration wurde optimiert, sodass alle Kunden dieselbe Schaltfläche sehen, um sich bei Workfront anzumelden, unabhängig davon, ob sie IMS-fähig sind oder nicht. Die nachfolgenden Anmeldeschritte bleiben für IMS- und Nicht-IMS-Instanzen unterschiedlich, die Anfangsseite ist jedoch für alle Benutzer gleich.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 6. August 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 6. August 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Projektverbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Weitere relevante Zuweisungen wurden dem Workflow "Neue Aufgabe"hinzugefügt</a></p>
                        [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
                        <p>Dieselbe Funktionalität für relevantere Smart-Zuweisungen wurde dem Feld Zuweisungen im Feld Neue Aufgabe hinzugefügt, wenn eine Aufgabe zu einem Projekt und in einer Projektaufgabenliste hinzugefügt wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 13. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.10 (Oktober 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> Weitere relevante Smart-Zuweisungen</a></p>
                        [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
                        <p>Wir haben den Algorithmus geändert, den Workfront zum Berechnen und Vorschlagen von intelligenten Zuweisungen für Aufgaben verwendet. Der neue Algorithmus wird in den folgenden Bereichen in Workfront angewendet, in denen Sie eine Aufgabe zuweisen: Aufgabenlisten, Zuweisungsbereich in der Aufgabenkopf, Startseite und Zusammenfassungsbereich.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. Dezember 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.10 (Oktober 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbesserungen bei der Überprüfung

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Leere Bildschirmkorrektur für Benutzer von Windows mit Desktop Proofing für Windows-Desktop-Computer</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Es wurde ein Problem mit der neuen Version 2.1.36 des Desktop Proofing-Viewers behoben, bei dem einige Windows-Benutzer nach dem Öffnen des Viewers einen leeren Bildschirm angezeigt haben. </p>
                        <p>Neue Version für Windows-Benutzer: 2.1.37</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 30. August 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 30. August 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Chromium-Update für den Desktop Proofing Viewer</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Wir aktualisieren den Desktop Proofing Viewer, um Chromium 126.0.6478.127 zu unterstützen, das Probleme mit UI-Elementen in interaktiven Testsendungen behebt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. August 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 29. August 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbesserungen bei Berichten und Dashboards

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect ist für neue Pläne verfügbar</a></p>
                        <p>Workfront Data Connect steht Unternehmen für einen der neuen Workfront-Pläne zur Verfügung. Data Connect ermöglicht Unternehmen den Zugriff auf ihre Daten als sicheren und skalierbaren Data Lake, der mithilfe von Business Intelligence-Tools analysiert und visualisiert oder extern gespeichert werden kann. Darüber hinaus können Unternehmen Data Connect verwenden, um Datenanalysen anzuzeigen, die zuvor nicht verfügbar waren, z. B. zeitbasierte Trendanalyse, Variablenzuordnung und Analyse externer Systemdaten in Kombination mit Workfront-Daten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: Mit der Version 24.10 (Oktober 2024)</span></p>
                            </li>
                        </ul>
                        <p><i>Nur für Unternehmen verfügbar, die an einem der neuen Adobe Workfront-Pläne teilnehmen. Data Connect ist im Ultimate-Plan enthalten oder kann als Add-on zu den Prime- und Select-Plänen erworben werden.</i></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}">Allgemeine Verfügbarkeit der Adobe Workfront-Planung</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Workfront Planning steht allen Kunden zur Verfügung, die zusätzlich zu ihrer Workfront-Lizenz eine Workfront Planning-Lizenz erworben haben. Weitere Informationen zur Workfront-Planung erhalten Sie von Ihrem Kundenbetreuer.</p>
                        <p>Die neuesten Informationen zur Workfront Planning-Version pro Quartal finden Sie unten im Abschnitt <a href="#workfront-planning-enhancements">Verbesserungen der Workfront-Planung</a> .</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 28. August 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe AI-Assistent in Workfront verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um Ihnen die Arbeit zu erleichtern, haben wir Adobe I Assistant zu Workfront hinzugefügt. Der KI-Assistent kann Sie bei Folgendem unterstützen:</p>
                        <ul>
                            <li>Zusammenfassung von Arbeitselementen und Dokumenten, sodass Sie schnell ein allgemeines Verständnis von Aufgaben, Projekten und Assets gewinnen können.</li>
                            <li>Bereitstellung von Informationen aus der Experience League-Dokumentation, Einbringen von Anweisungen und Referenzmaterial in Workfront und Verknüpfung zu einer ausführlicheren Dokumentation.</li>
                            <li>Erstellen und Verfeinern von Formeln für berechnete benutzerdefinierte Formularfelder, Generieren von Formeln aus Textaufforderungen oder Auffinden von Fehlern in vorhandenen Formeln.</li>
                            </ul>
                            <p>Ihr Workfront-Administrator kann den KI-Assistenten für Ihr Unternehmen aktivieren oder deaktivieren. Der KI-Assistent steht für Instanzen mit Select-, Prime- und Ultimate-Plänen zur Verfügung.</p>
                        </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 28. August 2024</p>
                            </li>
                            <li>
                                <p class="preview">Produktionsversion: 28. August 2024</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen im vierten Quartal 2024-Zeitrahmen</a></p>
                        <p>Im vierten Quartal 2024 wurden kleinere Änderungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des vierten Quartals 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Versionshinweise zu bestimmten Daten lesen</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                            
           </tbody>
        </table>

### Funktion wird bald aus Workfront entfernt

Die folgende Funktion wird in Kürze aus Workfront entfernt:

#### Veraltetes Home-Erlebnis mit Version 24.10

Mit der Version 24.10 werden wir offiziell das alte Home-Erlebnis einstellen. Es wird empfohlen, dass Benutzer mit der Verwendung des neuen Home beginnen, das vor der Einstellung weiter um zusätzliche Funktionen erweitert wird. Weitere Informationen zur Umstellung, einschließlich Hinweise dazu, was Benutzer und Administratoren zur Vorbereitung tun können, finden Sie im [Handbuch zur veralteten Home-Version](/help/quicksilver/product-announcements/announcements/legacy-home-deprecation.md).

## Ankündigungen

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung außerhalb des Veröffentlichungszeitplans für das vierte Quartal 2024 verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen der Workfront-Planung

Neue Funktionen in der Workfront-Planung sind in der Produktion verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront-Planungs-Aktivität für das vierte Quartal 2024](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Verbesserungen bei Workfront-Zielen

Es gibt derzeit keine Aktualisierungen zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### API-Version 18

Für API Version 18 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Weitere Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API-Version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die in der Version vom 4. Quartal 2024 vorgenommen wurden, finden Sie unter [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;auf der Seite [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
