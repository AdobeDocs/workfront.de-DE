---
title: Übersicht über die Version 2024 im zweiten Quartal
description: Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom zweiten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1e103c41d225c3bcc2699da24b0c6733c09b6637
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 0%

---

# Übersicht über die Version 2024 im zweiten Quartal

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom zweiten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview). -->

<span class="preview">Funktionen außerhalb des Kreislaufs (Funktionen, die vor dem Veröffentlichungsdatum des zweiten Quartals 2024 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 beinhaltet die Option, Ihr Unternehmen auf monatliche Releases umzustellen. Daher hat Workfront das Nummerierungsschema der Veröffentlichungen geändert, um sowohl die monatlichen als auch die vierteljährlichen Versionsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2024 lautet 24.4.
>
>Die monatlichen und vierteljährlichen Versionen sollen am Donnerstag der zweiten vollen Woche des Monats verfügbar sein, sofern nichts anderes angegeben ist.
>
>| Monatliche Version | Quartalsversion |
>|----|----|
>| <ul><li>24.2 (15. Februar 2024)</li><li>24.3 (14. März 2024)</li><li>24.4 (11. April 2024)</li></ul> | <ul><li>24.4 (April 2024)</li></ul> |
>
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Schnellveröffentlichungsprozess aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Verbesserungen der Startseite](#home-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen bei der Ressourcenverwaltung](#resource-management-enhancements)
* [Aktualisierung von Stream- und Benachrichtigungsverbesserungen](#update-stream-and-notification-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

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
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">JumpSeat-Integration jetzt für neue Pakettypen verfügbar</a></p>
                        <p>Die vorhandene JumpSeat-Integration ist jetzt für Konten verfügbar, die einen der neuen Pakettypen verwenden (d. h. Select, Prime oder Ultimate). Sie müssen weiterhin über ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 26. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Native Workfront-Felder sind in der Beta-Version des Formulardesigners verfügbar.</a></p>
                        <p>In Workfront native Felder können jetzt zu benutzerdefinierten Formularen hinzugefügt werden. Mit diesem neuen Feldtyp können Sie Daten logisch organisieren und darstellen, ohne vorhandene Daten in benutzerdefinierten Feldern neu erstellen zu müssen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Die Attributzuordnung ist jetzt für Organisationen verfügbar, die zu Adobe IMS migriert haben</a></p>
                        <p>[!BADGE In Production ]{type=Informative}</p><p>Workfront-Systemadministratoren können jetzt die Zuordnung von Benutzerattributen für Organisationen einrichten, die zu Adobe IMS migriert wurden. Auf diese Weise können Benutzerinformationen vom SSO-Provider (Single Sign-on) des Unternehmens an Workfront weitergegeben werden, sodass die Benutzerdaten nicht sowohl in Workfront als auch im SSO-Provider eingegeben werden müssen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 22. Februar 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Logik und Anzeigenlogik überspringen sind jetzt in der Beta-Version des Formulardesigners verfügbar</a></p><p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Sie können jetzt die vorhandene Anzeige bearbeiten und die Logik überspringen und benutzerdefinierte Formulare in der Beta-Version des Formulardesigners um eine neue Logik erweitern. Mit einem benutzerfreundlichen Logikaufbau können Sie festlegen, welche Felder je nach Auswahl im Formular angezeigt oder übersprungen werden sollen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 8. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: TBD</p>
                            </li>
                        </ul>
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
                        <p><span class="bold">Funktion</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                 </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Zu Administratorsteuerelementen hinzugefügte Spaltenoptionen mit Layoutvorlagen für neues Startseiten</a></p><p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p><p>Administratoren können jetzt mithilfe von Layoutvorlagen anpassen, welche Spalten für Benutzer in bestimmten neuen Home-Widgets verfügbar sind. Zu den Optionen gehören das Ausblenden oder Anzeigen von Standardspalten und das Hinzufügen vorhandener Felder als neue Spalten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 2. Januar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
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
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen am Workflow für die automatische Ordnererstellung in der Adobe Experience Manager-Integration</a></p><p>[!BADGE In Production ]{type=Informative}</p><p>Um sicherzustellen, dass Ihre Adobe Experience Manager-Ordner Ihren Anforderungen besser entsprechen, haben wir verschachtelte Ordnerbäume zum Workflow für verknüpfte Ordner mit Adobe Experience Manager hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 11. März 2024</p>
                            </li>
                             <li> <p><span class="preview">Produktionsversion für alle Kunden: 14. März 2024</span></p>
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
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Dem Workflow "Neue Aufgabe"hinzugefügte relevantere Zuweisungen</a></p><p>Dieselbe Funktionalität für relevantere Smart-Zuweisungen wurde dem Feld Zuweisungen im Feld Neue Aufgabe hinzugefügt, wenn eine Aufgabe zu einem Projekt und in einer Projektaufgabenliste hinzugefügt wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 13. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Wichtigere intelligente Zuweisungen</a></p><p>Wir haben den Algorithmus geändert, den Workfront zum Berechnen und Vorschlagen von intelligenten Zuweisungen für Aufgaben verwendet. Der neue Algorithmus wird in den folgenden Bereichen in Workfront angewendet, in denen Sie eine Aufgabe zuweisen: Aufgabenlisten, Zuweisungsbereich in der Aufgabenkopf, Startseite und Zusammenfassungsbereich.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. Dezember 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Verbesserungen bei der Ressourcenverwaltung

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
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-resource-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Indikator für manuell angepasste Zuordnungen im Arbeitslastausgleich</a></p><p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p><p>Um mehr Klarheit über manuelle Anpassungen oder die Konfiguration im Arbeitslastausgleich zu schaffen, zeigen manuell angepasste stündliche Zuordnungen jetzt ein Stiftsymbol an.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Aktualisierung von Stream- und Benachrichtigungsverbesserungen

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
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neuer Kommentar-Stream jetzt in Schnellaktionen für neue Home-Widgets verfügbar</a></p>
                        <p>Die neue Kommentarfunktion wurde jetzt der Schnellaktion-Schaltfläche "Neues Update hinzufügen"in den Widgets "Meine Arbeit", "Meine Projekte", "Meine Aufgaben"und "Meine Probleme"in der neuen Startseite hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 1. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Zusätzliche Kommentar-Informationen, die im neuen Kommentierungserlebnis verfügbar sind</a></p><p>Wir haben die folgenden Verbesserungen an der neuen Kommentarfunktion vorgenommen:</p>
                        <ul>
                            <li>
                                <p>Sie können auf den Namen eines Kommentars klicken, um dessen Namen, Rolle und E-Mail-Adresse in einem Informationsfeld anzuzeigen. Diese Informationen können Ihnen dabei helfen, den richtigen Benutzer zu identifizieren, wenn Sie mehr als einen Benutzer mit demselben Namen haben. Wenn Sie im Informationsfeld auf den Namen des Kommentars klicken, wird sein Benutzerprofil geöffnet.</p>
                            </li>
                            <li>
                                <p>Ihr Benutzername wird in Kommentaren hervorgehoben, die Sie mit Tags versehen haben, wenn Sie im Kommentartext erwähnt werden.</p>
                            </li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Die Registerkarte Systemaktivität im neuen Kommentarerlebnis unterstützt schreibgeschützte Kommentare</a></p><p>Kommentare zu den Datensätzen der Systemaktivität im alten Kommentierungserlebnis werden jetzt auf der Registerkarte Systemaktivität in der neuen Kommentierungserfahrung als schreibgeschützt ausgefüllt. Sie können im neuen Kommentar-Erlebnis nicht auf Systemaktivitätsdatensätze antworten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Registerkarte für den Aktualisierungsstream, um sowohl Kommentare als auch Systemaktivitätseinträge zu erfassen</a></p><p>Um Ihnen eine chronologisch zusammenhängende Ansicht der Kommentare und Systemaktivitätsprotokolle zu ermöglichen, führen wir einen dritten Tab in den Bereich Updates aller Objekte ein. Die Registerkarte "Alle"erfasst sowohl Benutzerkommentare als auch Systemaktivitätskommentare in einem zusammenhängenden Stream.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neuer Kommentar-Stream jetzt im Bedienfeld "Zusammenfassung"verfügbar</a></p><p>Jetzt wurde die neue Kommentarfunktion zum Bedienfeld "Zusammenfassung"für Aufgaben- und Problemlisten hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (April 2024)</p>
                            </li>
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
                        <p><span class="bold">Funktion</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen im zweiten Quartal 2024-Zeitrahmen</a></p><p>Im zweiten Quartal 2024 werden geringfügige Änderungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: Im gesamten Veröffentlichungszeitrahmen des zweiten Quartals 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Versionshinweise zu bestimmten Daten lesen</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>   
           </tbody>
        </table>

## Ankündigungen

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung ab einem Zeitpunkt verfügbar, der außerhalb des Ersten Quartal 2023 liegt. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront-Testverbesserungen

Es gibt derzeit keine Workfront Testversandaktualisierungen in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Verbesserungen bei Workfront-Zielen

Es gibt derzeit keine Aktualisierungen zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### API-Version 16

Für API Version 16 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API Version 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version 22.3 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;im [Workfront Tutorials-Seite](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
