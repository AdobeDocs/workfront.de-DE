---
title: Übersicht über die Version 2024 im dritten Quartal
description: Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom dritten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 0965c9a02496127bbf9b562784ff06c295dc0cf1
workflow-type: tm+mt
source-wordcount: '1740'
ht-degree: 0%

---

# Übersicht über die Version 2024 im dritten Quartal

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom dritten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.

Das Live-Webinar der Version 24.7 wurde abgebrochen, Sie können jedoch weiterhin [Sehen Sie sich hier eine Videodemonstration zu Funktionen von 24.7 an.](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Funktionen außerhalb des Kreislaufs (Funktionen, die vor dem Veröffentlichungsdatum des dritten Quartals 2024 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 beinhaltet die Option, Ihr Unternehmen auf monatliche Releases umzustellen. Daher hat Workfront das Nummerierungsschema der Veröffentlichungen geändert, um sowohl die monatlichen als auch die vierteljährlichen Versionsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2024 lautet 24.4.
>
>Die monatlichen und vierteljährlichen Versionen sollen am Donnerstag der zweiten vollen Woche des Monats verfügbar sein, sofern nichts anderes angegeben ist.
>
>| Monatliche Version | Quartalsversion |
>|----|----|
>| <ul><li>24.5 (16. Mai 2024)</li><li>24.6 (13. Juni 2024)</li><li>24.7 (18. Juli 2024)</li></ul> | <ul><li>24.7 (18. Juli 2024)</li></ul> |
>
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Schnellveröffentlichungsprozess aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Verbesserungen des Finanzmanagements](#financial-management-enhancements)
* [Verbesserungen bei der Integration](#integration-enhancements)
* [Projekt Verbesserungen](#project-enhancements)
* [Verbesserungen bei der Korrekturfunktion](#proofing-enhancements)
* [Verbesserungen bei der Verwaltung Ressource](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Geschäftsregeln sind jetzt verfügbar</a></p>
                        <p>Administratoren können nun im Einrichtungsbereich von Workfront Geschäftsregeln hinzufügen.</p>
                        <p>Mit einer Geschäftsregel können Sie eine Validierung auf Workfront-Objekte anwenden und verhindern, dass Benutzer ein Objekt erstellen, bearbeiten oder löschen, wenn bestimmte Bedingungen erfüllt sind. Die Regeln werden mit einer Formel erstellt, die der berechneten Feldern in benutzerdefinierten Formularen ähnelt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 4. Juli 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Benutzerdefinierter Formularentwickler, der allgemein in Adobe Workfront verfügbar ist</a></p>
                        <p>Mit Version 24.7 ist der Formular-Designer allgemein verfügbar und wird zum Standard-Erlebnis zum Erstellen und Bearbeiten von benutzerdefinierten Formularen in Adobe Systems Workfront. Wenn Sie ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen, sehen Sie die Arbeitsfläche Arbeitsbereich des Formulardesigners.</p>
                        <p>Nach dieser Version haben Sie nicht mehr die Möglichkeit, zum alten Formular-Builder zurückzukehren.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau Veröffentlichung: 19. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsfreigabe für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Verschieben von Objekten zwischen Workfront-Umgebungen mit Umgebungsförderung</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Mit der Umgebungsförderung können Sie Objekte von einer Workfront-Umgebung in eine andere verschieben, z. B. von einer Sandbox-Umgebung in eine Produktionsumgebung. Sie können Objekte so konfigurieren und testen, dass die Daten und Datensätze Ihrer Organisation nicht gefährdet werden. Sie können diese Objekte dann in die Produktion verschieben, ohne sie neu konfigurieren zu müssen, was Zeit und Mühe spart.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.6 (13. Juni 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Benutzerdefinierte Formulare und benutzerdefinierte Felder im benutzerdefinierten Formularentwickler freigeben</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Sie können jetzt sowohl benutzerdefinierte Formulare als auch benutzerdefinierte Felder im neuen Formularentwickler freigeben. Dies ermöglicht eine bessere Zusammenarbeit zwischen Benutzern bei benutzerdefinierten Formularen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsfreigabe für alle Kunden: 13. Juni</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">hinzufügen ein neues benutzerdefiniertes Feld aus dem Bereich "Felder"</a></p>
                        <p>Sie können jetzt ein neues benutzerdefiniertes Feld oder Widget direkt aus dem Bereich "Felder" in Workfront hinzufügen, ohne ein benutzerdefiniertes Formular zum Erstellen des Felds zu öffnen. Auf diese Weise können Sie schnell wiederverwendbare benutzerdefinierte Felder erstellen.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Dropdown-Feldtyp mit Mehrfachauswahl, der im Formularentwickler verfügbar ist</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um Ihnen zu helfen, Dropdown-Felder einfacher zu definieren, haben wir das Dropdown-Feld Mehrfachauswahl zum benutzerdefinierten Formularentwickler hinzugefügt. Mit diesem Feldtyp können Benutzer aus einer Dropdown-Liste mehrere Optionen auswählen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 4. Juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 4. Juni 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbesserungen bei der Finanzverwaltung

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Abrechenbare und nicht abrechnungsfähige Ausgabenfelder für Projekte und Aufgaben</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Damit Sie die Ausgabetypen leichter erkennen können, wurden die Ausgaben in abrechenbare und nicht abrechnungsfähige Ausgaben für Projekte und Aufgaben unterteilt. Die folgenden Felder stehen Ihnen zum Hinzufügen zu Ansichten und Berichten zur Verfügung:</p>
                        <ul>
                            <li><p>Geplante abrechenbare Ausgabenkosten</p></li>
                            <li><p>Geplante nicht abrechnungsfähige Kosten</p></li>
                            <li><p>Tatsächliche nicht abrechnungsfähige Kosten</p></li>
                            <li><p>Tatsächliche nicht abrechnungsfähige Kosten</p></li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 10. Mai 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 10. Mai 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Verbesserungen bei der Integration

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Merkmal</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Versionstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen in Workfront for Experience Manager Assets und Assets Essentials</a></p>
                        [! BADGE Neu in Vorschau ]{type=Negative}
                        <p>Wir haben die folgenden Verbesserungen an den Integrationen von Workfront for Experience Manager Assets und Assets Essentials vorgenommen:</p>
                        <ul>
                            <li><p>Die Integration unterstützt nun GCP als Cloud Service-Provider. AWS und Azure wurden zuvor unterstützt.</p></li>
                            <li><p>Die Größenbeschränkung für Dateien, die über die Integration an Experience Manager gesendet werden, wurde auf 30 GB erhöht. Zuvor war der Grenzwert 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau: 27. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Bearbeiten Sie die Aufgabe und geben Sie das Datum und die Bedingung für die Übermittlung aus der Kopfzeile oder dem Detailabschnitt aus.</a></p>
                        [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
                        <p>Um Ihnen das Aktualisieren von Aufgaben und Problemen zu erleichtern, haben wir jetzt die Felder "Commits Datum" und "Bedingung" als Optionen hinzugefügt, die zu Aufgabe- und Issue-Headern und Details Abschnitten in einem Layout-Vorlage hinzugefügt werden können. Benutzer können diese Felder nun aus der Kopfzeile oder dem Details Abschnitt eines Seite aktualisieren, wenn sie dem geänderten Layout-Vorlage zugewiesen werden.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau Veröffentlichung: 30. Mai 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.6 (13. Juni 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsfreigabe für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Dem Workflow "Neue Aufgabe"hinzugefügte relevantere Zuweisungen</a></p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
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
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Wichtigere intelligente Zuweisungen</a></p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Wir haben den Algorithmus geändert, den Workfront zum Berechnen und Vorschlagen von intelligenten Zuweisungen für Aufgaben verwendet. Der neue Algorithmus wird in den folgenden Bereichen in Workfront angewendet, in denen Sie eine Aufgabe zuweisen: Aufgabenlisten, Zuweisungsbereich in der Aufgabenkopf, Startseite und Zusammenfassungsbereich.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau Veröffentlichung: 21. Dezember 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsfreigabe für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Verbesserungen bei der Korrekturfunktion

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Merkmal</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Veröffentlichungsdaten</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Sicherheitsupdates für den Desktop Proofing Viewer</a></p>
                        <p>Das Sicherheitsupdate für Workfront Proof Desktop Proofing Viewer 2.1.35 enthält Sicherheitsfehlerbehebungen für Sicherheitslücken, die in früheren Versionen identifiziert wurden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: Juli 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 4. Juli 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Die Auszeit wird jetzt im Lastenausgleich angezeigt.</a></p>
                        <p>Um die Arbeit nahtlos anzupassen, wenn der primäre Verantwortliche für eine Aufgabe eine geplante Zeitüberschreitung aufweist, weist der Arbeitslastausgleich jetzt sowohl den primären als auch den sekundären Benutzern Stunden zu, wenn die Projekt-Timeline neu berechnet wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ist jetzt für mehr Workfront-Organisationen verfügbar</a></p>
                        <p>Um Unternehmen den Zugriff auf die Vorteile des Adobe Unified Experience zu ermöglichen, haben wir begonnen, es bestehenden Workfront-Kunden zur Verfügung zu stellen. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 20. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion für bestimmte Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Die Adobe Systems Unified Shell wird schrittweise Rollout bereitgestellt. Mit den Versionen 24.10 und 25.1 werden weitere Organisationen in die Adobe Systems Unified Shell aufgenommen. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Hilfe Button aus der Haupt Navigation Leiste entfernt</a></p>
                        <p>Um die Erlebnis für Benutzer, die sich nicht auf Unified Shell befinden, zu vereinheitlichen, wurde der Hilfe Button in der Haupt Navigation Leiste entfernt. Diese Button, die für Benutzer auf Unified Shell nicht vorhanden ist, verlinkte auf die Workfront-Dokumentation und war redundant mit einer ähnlichen Hilfe Button, die für alle Benutzer im Hauptmenü verfügbar war.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserte Benutzeroberfläche für Benutzer mit eingeschränktem Objektzugriff</a></p>
                        [!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}
                        <p>Wenn ein Benutzer keinen Zugriff auf ein Objekt hat, wird ihm überall dort "Kein Zugriff"angezeigt, wo der Objektname in Workfront angezeigt wird. Dieses verbesserte Erlebnis gilt auch für die Workfront-API.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 27. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen im Zeitraum vom 3. Quartal 2024</a></p>
                        <p>Im dritten Quartal 2024 werden geringfügige Änderungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar an folgenden Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau Version: Die gesamte Version des dritten Quartals 2024 Zeitrahmen</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsfreigabe: prüfen die Versionshinweise für bestimmte Daten</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Ankündigungen

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung außerhalb des Veröffentlichungszeitplans für das dritte Quartal 2024 verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Verbesserungen bei Workfront-Zielen

Es gibt derzeit keine Aktualisierungen zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### API-Version 18

Für API Version 18 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

Informationen zu den Neuerungen und Aktualisierungen finden Sie unter [Neue Funktionen in API Version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und -supportzeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version des dritten Quartals 2024 vorgenommen wurden, finden Sie unter [Workfront-Wartungsupdates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsupdates

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;im [Workfront Tutorials-Seite](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
