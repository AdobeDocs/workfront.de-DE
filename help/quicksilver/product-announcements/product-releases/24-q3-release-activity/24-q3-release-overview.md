---
title: Versionsübersicht für das dritte Quartal 2024
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom dritten Quartal 2024 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 552e97c427e618f299b55a2eab5868c7b90a4156
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# Versionsübersicht für das dritte Quartal 2024

Diese Seite enthält Informationen zur Funktionalität, die in der Version vom dritten Quartal 2024 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.

Das Webinar zur Live-Version 24.7 wurde abgesagt, aber Sie können [hier eine Videodemonstration zu den Funktionen von 24.7 ansehen](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Off-Cycle-Funktionen (die vor dem Veröffentlichungsdatum des dritten Quartals 2024 in der Produktion veröffentlicht wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 enthielt die Option, Ihr Unternehmen auf monatliche Versionen umzustellen. Aus diesem Grund hat Workfront das Nummerierungsschema der Versionen geändert, um sowohl monatliche als auch vierteljährliche Veröffentlichungsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2024 lautet wie 24.4.
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Versionen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Version | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>24.5 (16. Mai 2024)</li><li>24.6 (13. Juni 2024)</li><li>24.7 (18. Juli 2024)</li></ul> | <ul><li>24.7 (18. Juli 2024)</li></ul> |
>
>Weitere Informationen zum Schnellfreigabeprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellfreigabeprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administrator-Verbesserungen](#administrator-enhancements)
* [Verbesserungen beim Finanzmanagement](#financial-management-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Proofing-Verbesserungen](#proofing-enhancements)
* [Verbesserungen beim Ressourcenmanagement](#resource-management-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administrator-Verbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Geschäftsregeln sind jetzt verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Administratoren können jetzt im Bereich „Setup“ von Workfront Geschäftsregeln hinzufügen.</p>
                        <p>Mit einer Geschäftsregel können Sie Validierungen auf Workfront-Objekte anwenden und Benutzer daran hindern, ein Objekt zu erstellen, zu bearbeiten oder zu löschen, wenn bestimmte Bedingungen erfüllt sind. Die Regeln werden mithilfe einer Formel erstellt, die den berechneten Feldern in benutzerdefinierten Formularen ähnelt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 4. Juli 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                        <p><i>Nur für Organisationen mit dem neuen Ultimate-Plan verfügbar.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Benutzerdefinierter Formular-Designer allgemein verfügbar in Adobe Workfront</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Ab Version 24.7 ist der Formular-Designer allgemein verfügbar und wird zum Standarderlebnis für das Erstellen und Bearbeiten benutzerdefinierter Formulare in Adobe Workfront. Wenn Sie ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen, wird der Arbeitsbereich im Arbeitsbereich-Stil des Formular-Designers angezeigt.</p>
                        <p>Nach dieser Version haben Sie keine Möglichkeit mehr, zum alten Formular-Builder zurückzukehren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 19. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Verschieben von Objekten zwischen Workfront-Umgebungen mit Umgebungs-Promotion</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Umgebungs-Promotion ermöglicht es Ihnen, Objekte von einer Workfront-Umgebung in eine andere zu verschieben, z. B. von einer Sandbox-Umgebung in eine Produktionsumgebung. Sie können Objekte ohne Risiko für die Daten und Datensätze Ihres Unternehmens konfigurieren und testen. Sie können diese Objekte dann in die Produktion verschieben, ohne sie neu konfigurieren zu müssen, was Zeit und Aufwand spart.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.6 (13. Juni 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Freigeben von benutzerdefinierten Formularen und Feldern im Designer für benutzerdefinierte Formulare</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Sie können jetzt sowohl benutzerdefinierte Formulare als auch benutzerdefinierte Felder im neuen Formular-Designer freigeben. Dies ermöglicht eine bessere Zusammenarbeit zwischen Benutzern in benutzerdefinierten Formularen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsfreigabe für alle Kunden: 13. Juni</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Ein neues benutzerdefiniertes Feld aus dem Bereich „Felder“ hinzufügen</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Sie können jetzt ein neues benutzerdefiniertes Feld oder Widget direkt aus dem Bereich Felder in Workfront hinzufügen, ohne ein benutzerdefiniertes Formular zu öffnen, um das Feld zu erstellen. Auf diese Weise können Sie schnell wiederverwendbare benutzerdefinierte Felder erstellen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Mehrfachauswahl-Dropdown-Feldtyp im Formular-Designer verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um Ihnen die Definition von Dropdown-Feldern zu erleichtern, haben wir das Dropdown-Feld Mehrfachauswahl zum benutzerdefinierten Formular-Designer hinzugefügt. Bei diesem Feldtyp können Benutzer mehr als eine Option aus einer Dropdown-Liste auswählen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 4. Juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 4. Juni 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbesserungen beim Finanzmanagement

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Abrechenbare und nicht abrechenbare Ausgaben für Projekte und Aufgaben</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Damit Sie Ausgabentypen leichter anzeigen können, wurden Ausgaben für Projekte und Aufgaben in fakturierbare und nicht fakturierbare Ausgaben unterteilt. Die folgenden Felder können zu Ansichten und Berichten hinzugefügt werden:</p>
                        <ul>
                            <li><p>Geplante abrechenbare Ausgabenkosten</p></li>
                            <li><p>Geplante nicht fakturierbare Kosten</p></li>
                            <li><p>Tatsächliche nicht fakturierbare Kosten</p></li>
                            <li><p>Tatsächliche nicht fakturierbare Kosten</p></li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 10. Mai 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 10. Mai 2024</span></p>
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen bei Workfront für Experience Manager Assets und Assets Essentials</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Für die Integration von Workfront mit Experience Manager Assets und Assets Essentials haben wir die folgenden Verbesserungen vorgenommen:</p>
                        <ul>
                            <li><p>Die Integration unterstützt jetzt GCP als Cloud Service Provider. AWS und Azure wurden zuvor unterstützt.</p></li>
                            <li><p>Die Größenbeschränkung für Dateien, die über die Integration an den Experience Manager gesendet werden, wurde auf 30 GB erhöht. Zuvor lag der Grenzwert bei 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 27. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Bearbeiten Sie das Commit-Datum und die Commit-Bedingung für Aufgabe und Problem in der Kopfzeile oder im Abschnitt Details</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um Ihnen das Aktualisieren von Aufgaben und Problemen zu erleichtern, haben wir jetzt die Felder „Übertragungsdatum“ und „Bedingung“ als Optionen hinzugefügt, die Sie den Kopfzeilen und Details von Aufgaben und Problemen in einer Layout-Vorlage hinzufügen können. Benutzer können diese Felder jetzt über den Kopfzeilen- oder Detailabschnitt einer Seite aktualisieren, wenn sie der geänderten Layout-Vorlage zugewiesen werden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 30. Mai 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.6 (13. Juni 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Relevantere Zuweisungen zum Workflow Neue Aufgabe hinzugefügt</a></p>
                        [!BADGE In Production for Fast Release ]{type=Positive}
                        <p>Wir haben dem Feld Zuweisungen im Feld Neue Aufgabe dieselbe Funktion für relevantere Smart-Zuweisungen hinzugefügt, wenn eine Aufgabe zu einem Projekt und in einer Projektaufgabenliste hinzugefügt wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 13. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                        </ul>
                    <p><i>Diese Funktion wurde aus der Vorschau- und Schnellveröffentlichungsproduktion entfernt.</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Relevantere Smart-Zuweisungen</a></p>
                        [!BADGE In Production for Fast Release ]{type=Positive}
                        <p>Wir haben den Algorithmus geändert, den Workfront verwendet, um smarte Zuweisungen für Aufgaben zu berechnen und vorzuschlagen. Der neue Algorithmus wird auf die folgenden Bereiche in Workfront angewendet, in denen Sie eine Aufgabe zuweisen: Aufgabenlisten, der Bereich „Zuweisungen“ in der Aufgabenkopfzeile, Startseite und das Bedienfeld „Zusammenfassung“.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. Dezember 2023</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                        </ul>
                    <p><i>Diese Funktion wurde aus der Vorschau- und Schnellveröffentlichungsproduktion entfernt.</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### Proofing-Verbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Sicherheitsaktualisierungen für den Desktop Proofing Viewer</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Das Sicherheitsupdate Workfront Proof Desktop Proofing Viewer 2.1.35 bietet Sicherheitsfehlerbehebungen für Sicherheitslücken, die in früheren Versionen identifiziert wurden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 4. Juli 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 4. Juli 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Verbesserungen beim Ressourcenmanagement

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Ausfallzeiten werden jetzt im Workload-Balancer angezeigt</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um die Arbeit nahtlos anzupassen, wenn der primäre Zugewiesene für eine Aufgabe Ausfallzeiten geplant hat, weist der Workload Balancer jetzt beim Neuberechnen der Projekt-Zeitleiste sowohl dem primären als auch dem sekundären Benutzer Stunden neu zu.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Backend-Änderung an produktinternen Handbüchern</a></p>
                        <p>Wir implementieren in den nächsten Wochen einen Technologiewechsel für unsere produktinternen Handbücher. Obwohl wir versucht haben, die Auswirkungen dieser Umstellung zu minimieren, können einige Benutzer auf Anleitungen stoßen, die sie zuvor gesehen haben.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Produktion für alle Kunden: Inkrementell bis Mitte August 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Einheitliches Erlebnis für Adobe jetzt für weitere Workfront-Organisationen verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um Unternehmen den Zugriff auf die Vorteile des einheitlichen Adobe-Erlebnisses zu ermöglichen, haben wir begonnen, dieses für bestehende Workfront-Kunden verfügbar zu machen. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 20. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktion für bestimmte Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Die Adobe Unified Shell wird in einem schrittweisen Rollout zur Verfügung gestellt. Weitere Unternehmen werden mit den Versionen 24.10 und 25.1 in die Adobe Unified Shell integriert. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Schaltfläche „Hilfe“ wurde aus der Hauptnavigationsleiste entfernt</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um das Erlebnis für Benutzende, die nicht in Unified Shell arbeiten, zu vereinheitlichen, wurde die Schaltfläche Hilfe in der Hauptnavigationsleiste entfernt. Diese Schaltfläche, die für Benutzende von Unified Shell nicht vorhanden, mit der Workfront-Dokumentation verknüpft und mit einer ähnlichen Schaltfläche „Hilfe“ redundant war, die für alle Benutzenden im Hauptmenü verfügbar ist.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserte Benutzeroberfläche für Benutzer mit eingeschränktem Objektzugriff</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Wenn ein(e) Benutzende(r) keinen Zugriff auf ein Objekt hat, wird „Kein Zugriff“ überall dort angezeigt, wo der Objektname in Workfront angezeigt wird. Dieses verbesserte Erlebnis gilt auch für die Workfront-API.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 27. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.5 (16. Mai 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Updates im dritten Quartal 2024</a></p>
                        <p>Innerhalb des Zeitrahmens des dritten Quartals 2024 werden kleinere Aktualisierungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Lesen Sie die einzelnen Versionshinweise für bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: Im gesamten Zeitrahmen der Version für das dritte Quartal 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Lesen Sie die Versionshinweise für bestimmte Daten</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## Ankündigungen

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind außerhalb des Veröffentlichungszeitplans für das dritte Quartal 2024 in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Verbesserungen am Workfront-Szenarioplaner

Es gibt derzeit keine Szenario-Planer-Aktualisierungen in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### Workfront-Zielverbesserungen

Es gibt derzeit keine Updates zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

### API-Version 18

Für API-Version 18 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die im dritten Quartal 2024 durchgeführt wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt Neue Funktionen auf der Seite [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
