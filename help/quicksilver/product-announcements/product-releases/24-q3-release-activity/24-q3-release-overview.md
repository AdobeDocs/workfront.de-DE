---
title: Übersicht über die Version 2024 im dritten Quartal
description: Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom dritten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 21ad93a3438962fd45a6b348960c37402c71a18a
workflow-type: tm+mt
source-wordcount: '1830'
ht-degree: 0%

---

# Übersicht über die Version 2024 im dritten Quartal

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom dritten Quartal 2024 enthalten sind. Diese Verbesserungen sollen während des gesamten Quartals in der Produktionsumgebung verfügbar sein.

Das Live-Webinar der Version 24.7 wurde abgebrochen, Sie können sich aber trotzdem [eine Videodemonstration zu Funktionen der Version 24.7 hier ansehen](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Off-Cycle-Funktionen (diejenigen, die vor dem Veröffentlichungsdatum des dritten Quartals 2024 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

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
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Aktivieren oder Deaktivieren des Prozesses der schnellen Veröffentlichung](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Verbesserungen bei der Finanzverwaltung](#financial-management-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen bei der Überprüfung](#proofing-enhancements)
* [Verbesserungen bei der Ressourcenverwaltung](#resource-management-enhancements)
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Geschäftsregeln sind jetzt verfügbar </a></p>
                        [!BADGE In Production ]{type=Informative}
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
                        <p><i>Nur für Organisationen mit dem neuen Ultimate-Plan verfügbar.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Benutzerdefinierter Formularentwickler allgemein in Adobe Workfront verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Mit Version 24.7 ist der Formularentwickler allgemein verfügbar und wird zum Standarderlebnis beim Erstellen und Bearbeiten benutzerdefinierter Formulare in Adobe Workfront. Wenn Sie ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen, wird der Arbeitsbereich im Arbeitsbereich des Formulardesigners angezeigt.</p>
                        <p>Nach dieser Version haben Sie nicht mehr die Möglichkeit, zum alten Formular-Builder zurückzukehren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau: 19. Juni 2024</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Objekte zwischen Workfront-Umgebungen mit Umgebungsförderung verschieben</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Freigeben von benutzerdefinierten Formularen und benutzerdefinierten Feldern im benutzerdefinierten Formularentwickler</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Sie können jetzt sowohl benutzerdefinierte Formulare als auch benutzerdefinierte Felder im neuen Formularentwickler freigeben. Dies ermöglicht eine bessere Zusammenarbeit zwischen Benutzern bei benutzerdefinierten Formularen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 6. Juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 13. Juni</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Fügen Sie ein neues benutzerdefiniertes Feld aus dem Felderbereich hinzu</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Sie können jetzt ein neues benutzerdefiniertes Feld oder Widget direkt aus dem Bereich Felder in Workfront hinzufügen, ohne ein benutzerdefiniertes Formular zum Erstellen des Felds zu öffnen. Auf diese Weise können Sie schnell wiederverwendbare benutzerdefinierte Felder erstellen.</p>
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
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Dropdown-Feldtyp für mehrere Auswahlen, der im Formularentwickler verfügbar ist</a></p>
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Abrechenbare und nicht abrechnungsfähige Ausgabenfelder, die für Projekte und Aufgaben verfügbar sind</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen für Workfront für Experience Manager Assets und Assets Essentials</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Wir haben die folgenden Verbesserungen an der Workfront für Experience Manager Assets- und Assets Essentials-Integrationen vorgenommen:</p>
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Bearbeiten Sie die Aufgabe und geben Sie das Datum und die Bedingung für die Übermittlung aus der Kopfzeile oder dem Detailabschnitt aus.</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um die Aktualisierung von Aufgaben und Problemen zu vereinfachen, haben wir jetzt die Felder "Datum und Bedingung für die Übermittlung"als Optionen hinzugefügt, die in einer Layout-Vorlage zum Abschnitt "Aufgaben- und Problemkopfzeilen und Details"hinzugefügt werden können. Benutzer können diese Felder jetzt über die Kopfzeile oder den Detailabschnitt einer Seite aktualisieren, wenn sie der geänderten Layoutvorlage zugewiesen sind.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 30. Mai 2024</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 24.6 (13. Juni 2024)</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit der Version 24.7 (18. Juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Weitere relevante Zuweisungen wurden dem Workflow "Neue Aufgabe"hinzugefügt</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> Weitere relevante Smart-Zuweisungen</a></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Sicherheitsupdates für den Desktop Proofing Viewer</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Das Sicherheitsupdate für Workfront Proof Desktop Proofing Viewer 2.1.35 enthält Sicherheitsfehlerbehebungen für Sicherheitslücken, die in früheren Versionen identifiziert wurden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 4. Juli 2024</p>
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Zeitlimit, die jetzt im Lastenausgleich angezeigt wird</a></p>
                        [!BADGE In Production ]{type=Informative}
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
                        <p><span class="bold">Veröffentlichungstermine</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Backend-Änderung an In-Produkt-Handbüchern</a></p>
                        <p>In den nächsten Wochen führen wir für unsere produktinternen Leitfäden eine Technologieänderung durch. Während wir versucht haben, die Auswirkungen dieser Transition zu minimieren, können einige Benutzer auf Leitfäden stoßen, die sie zuvor gesehen haben.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Produktion für alle Kunden: schrittweise bis Mitte August 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience ist jetzt für weitere Workfront-Organisationen verfügbar</a></p>
                        [!BADGE In Production ]{type=Informative}
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
                         <span style="color: #ff0000;">Die Adobe Unified Shell wird in einem schrittweisen Rollout zur Verfügung gestellt. Weitere Organisationen werden mit den Versionen 24.10 und 25.1 in die Adobe Unified Shell integriert. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Schaltfläche "Hilfe"aus der Hauptnavigationsleiste entfernt</a></p>
                        [!BADGE In Production ]{type=Informative}
                        <p>Um das Erlebnis für Benutzer zu vereinheitlichen, die nicht Unified Shell verwenden, wurde die Schaltfläche Hilfe in der Hauptnavigationsleiste entfernt. Diese Schaltfläche, die nicht für Unified Shell-Benutzer vorhanden ist und mit der Workfront-Dokumentation verknüpft ist, war redundant und mit einer ähnlichen Schaltfläche für alle Benutzer im Hauptmenü verfügbar.</p>
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
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbessertes Benutzeroberflächenerlebnis für Benutzer mit eingeschränktem Objektzugriff</a></p>
                        [!BADGE In Production ]{type=Informative}
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen im dritten Quartal 2024-Zeitrahmen</a></p>
                        <p>Im dritten Quartal 2024 werden geringfügige Änderungen am Erscheinungsbild verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des dritten Quartals 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Versionshinweise zu bestimmten Daten lesen</span></p>
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

Für API Version 18 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Weitere Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API-Version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die in der Version vom 3. Quartal 2024 vorgenommen wurden, finden Sie unter [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;auf der Seite [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
