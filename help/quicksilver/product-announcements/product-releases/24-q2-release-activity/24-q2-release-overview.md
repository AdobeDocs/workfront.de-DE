---
title: Übersicht über die Version 2024 im zweiten Quartal
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom zweiten Quartal 2024 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bdcfed70-1999-4c40-a38f-12c762c8c1c4
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 0%

---

# Übersicht über die Version 2024 im zweiten Quartal

Diese Seite enthält Informationen zur Funktionalität, die in der Version vom zweiten Quartal 2024 enthalten ist. Diese Verbesserungen wurden mit der Version 24.4 vom 10. und 11. April 2024 in der Produktionsumgebung für alle Kunden verfügbar gemacht.

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview).-->
Anstelle eines Veröffentlichungs-Webinars laden wir Sie ein, sich für [ Adobe Summit zu registrieren](https://summit.adobe.com/na/) um die folgenden Workfront-Sitzungen anzusehen:

[Die Zukunft von Adobe Workfront](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=S302) am 26. März 2024, um eine Vorschau auf die Zukunft der strategischen Planung und des Workflows zu erhalten. Erfahren Sie, wie das Workfront-Team Geschäftsfunktionen über den gesamten Marketing-Lebenszyklus hinweg mit einem KI-First-Ansatz zur Automatisierung der Arbeit, zur Vereinfachung von Anwendererlebnissen und zur Steigerung der Produktivität ansprechen möchte.

[Vorstellung von Marketing-Kalendern und Tools für die End-to-End](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=s304)Kampagnenplanung am 28. März 2024, um mehr über neue Produktfunktionen zu erfahren, mit denen Ihr Unternehmen End-to-End-Betriebszyklen verwalten und visualisieren kann.

Sie können auch [eine PDF-Datei anzeigen](https://acrobat.adobe.com/id/urn:aaid:sc:US:1754831a-dbfe-471d-bca7-386264d90352){target="_blank"} mit den Highlights der Version 24.4.

<span class="preview">Off-Cycle-Funktionen (die vor dem Veröffentlichungsdatum des zweiten Quartals 2024 in der Produktion veröffentlicht wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 enthielt die Option, Ihr Unternehmen auf monatliche Versionen umzustellen. Aus diesem Grund hat Workfront das Nummerierungsschema der Versionen geändert, um sowohl monatliche als auch vierteljährliche Veröffentlichungsspuren zu berücksichtigen. Die erste Zahl bezeichnet das Jahr und die zweite Zahl den Monat der Veröffentlichung. Beispiel: Die Version für April 2024 lautet wie 24.4.
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Versionen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Version | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>24.2 (15. Februar 2024)</li><li>24.3 (14. März 2024)</li><li>24.4 (11. April 2024)</li></ul> | <ul><li>24.4 (11. April 2024)</li></ul> |
>
>Weitere Informationen zum Schnellfreigabeprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellfreigabeprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administrator-Verbesserungen](#administrator-enhancements)
* [Verbesserungen beim Dokumentenmanagement](#document-management-enhancements)
* [Home-Verbesserungen](#home-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen beim Ressourcenmanagement](#resource-management-enhancements)
* [Verbesserungen bei Aktualisierungs-Streams und Benachrichtigungen](#update-stream-and-notification-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Anzeigelogik und Überspringen-Logik sind jetzt im Vorschaumodus des Formular-Designers verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Mit dem benutzerdefinierten Beta-Formular-Designer können Sie jetzt Ihre Anzeigelogik testen und im Vorschaumodus die Logik überspringen . Zuvor wurden alle Felder in der Vorschau angezeigt, selbst wenn Logik angewendet wurde.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 28. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Unternehmen und Benutzer unterstützen jetzt erweiterte benutzerdefinierte Formularfelder</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind jetzt verfügbar, wenn Sie ein benutzerdefiniertes Formular an ein Unternehmen oder einen Benutzer anhängen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 14. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Die JumpSeat-Integration ist jetzt für neue Pakettypen verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Die bestehende JumpSeat-Integration ist jetzt für Konten verfügbar, die einen der neuen Pakettypen verwenden (d. h. Select, Prime oder Ultimate). Sie müssen weiterhin über ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 26. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Native Workfront-Felder sind in der Beta-Version von Form Designer verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Die in Workfront nativen Felder können jetzt zu Ihren benutzerdefinierten Formularen hinzugefügt werden. Mit diesem neuen Feldtyp können Sie Daten logisch organisieren und den Benutzern präsentieren, ohne vorhandene Daten in benutzerdefinierten Feldern neu erstellen zu müssen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 29. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Attributzuordnung jetzt für Organisationen verfügbar, die zu Adobe IMS migriert haben</a></p>
                        <p>[!BADGE In Production &#x200B;]{type=Informative}</p><p>Workfront-Systemadministratoren können jetzt die Benutzerattributzuordnung für Unternehmen einrichten, die zu Adobe IMS migriert sind. Auf diese Weise können Benutzerinformationen vom SSO-Provider (Single Sign-on) des Unternehmens an Workfront weitergeleitet werden, sodass die Daten des Benutzers nicht sowohl in Workfront als auch beim SSO-Provider eingegeben werden müssen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 22. Februar 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Überspringen-Logik und Anzeigelogik sind jetzt in der Beta-Version von Form Designer verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Sie können jetzt in der Beta-Version von Form Designer vorhandene Anzeigen- und Überspringen-Logik bearbeiten und benutzerdefinierten Formularen eine neue Logik hinzufügen. Ein benutzerfreundlicher Logik-Builder hilft Ihnen dabei, basierend auf einer Auswahl im Formular zu definieren, welche Felder angezeigt oder übersprungen werden sollen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 8. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Verbesserungen beim Dokumentenmanagement

>[!IMPORTANT]
>
>Die in **Document Management-Verbesserungen** aufgelisteten Funktionen sind Teil einer stufenweisen Veröffentlichung und nur für bestimmte Kundinnen und Kunden verfügbar.

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Fügen Sie einem Dokument eine Frist für Überprüfungen und Genehmigungen hinzu</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Sie können jetzt eine Frist für Benutzer oder Teams festlegen, die zur Überprüfung oder Genehmigung eines Dokuments zugewiesen sind. Validierungsverantwortliche und genehmigende Personen erhalten E-Mail-Benachrichtigungen 72 Stunden und anschließend 24 Stunden vor Ablauf der festgelegten Frist. Die Frist wird auch im Widget Genehmigungen im Bereich Neue Startseite angezeigt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 28. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Erstellen und Verwenden von Genehmigungsvorlagen</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Sie können jetzt im Bereich Setup Validierungsvorlagen erstellen, um den Prüfungs- und Validierungsprozess zu optimieren. Mit Validierungsvorlagen können Sie den Überprüfungs- und Validierungsprozess wie folgt wiederholbarer gestalten
                        <ul>
                            <li>
                                <p>Validierungsverantwortliche und genehmigende Personen hinzufügen</p>
                            </li>
                            <li>
                                <p>Festlegen eines Zeitrahmens</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 28. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Informationen zu allen Genehmigungen an einem Ort anzeigen</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Damit Sie Ihre Genehmigungsanfragen auf einen Blick verwalten und analysieren können, haben wir die folgenden wichtigen Leistungsindikatoren zum Widget Alle Genehmigungen hinzugefügt:
                        <ul>
                            <li>
                                <p>Genehmigungen nach Entscheidung</p>
                            </li>
                            <li>
                                <p>Durchschnittliche Genehmigungszeit</p>
                            </li>
                            <li>
                                <p>Ausstehende Genehmigungen</p>
                            </li>
                            <li>
                                <p>Überfällige Genehmigungen</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 28. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Spaltenoptionen wurden zu Administratorsteuerelementen für eine neue Startseite mithilfe von Layout-Vorlagen hinzugefügt</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Admins können jetzt mithilfe von Layout-Vorlagen anpassen, welche Spalten in bestimmten neuen Startseiten-Widgets für Benutzende verfügbar sind. Zu den Optionen gehören das Ausblenden oder Anzeigen von Standardspalten und das Hinzufügen vorhandener Felder als neue Spalten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 2. Januar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen des Workflows für die automatisierte Ordnererstellung in der Adobe Experience Manager-Integration</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Um sicherzustellen, dass Ihre Adobe Experience Manager-Ordner Ihre Anforderungen genauer widerspiegeln, haben wir einige Aktualisierungen am Workflow für verknüpfte Ordner in Adobe Experience Manager vorgenommen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 11. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für alle Kunden: 14. März 2024</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Relevantere Zuweisungen zum Workflow Neue Aufgabe hinzugefügt</a></p>
                        <p>[!BADGE In Production for Fast Release &#x200B;]{type=Positive}</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Relevantere Smart-Zuweisungen</a></p>
                        <p>[!BADGE In Production for Fast Release &#x200B;]{type=Positive}</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-resource-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Indikator für manuell angepasste Zuweisungen im Workload Balancer</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p><p>Um mehr Klarheit über manuelle Anpassungen oder die Konturierung im Workload Balancer zu schaffen, wird bei manuell angepassten stündlichen Zuordnungen jetzt ein Stiftsymbol angezeigt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 12. Oktober 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.2 (15. Februar 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Verbesserungen bei Aktualisierungs-Streams und Benachrichtigungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Iterationen wurden neue Kommentierungserlebnisse hinzugefügt</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Um Ihnen während der gesamten Anwendung ein konsistentes Erlebnis zu bieten, haben wir zu Iterationen das neue Kommentierungserlebnis hinzugefügt. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 11. April 2024</p>
                            </li>
                            <li>
                                <p>Produktion für alle Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Der Zugriff auf den alten Kommentarbereich wurde entfernt</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Der Umschalter „Neue Kommentare“ im Bereich „Aktualisierungen“ für Projekte, Aufgaben, Probleme und Dokumente wurde entfernt. Der neue Kommentar ist jetzt die Standard- und einzige Option für diese Objekte. Mit dieser Änderung können Sie nicht mehr zum alten Kommentierungserlebnis zurückkehren. Darüber hinaus haben wir die Einstellung „Prozentuale Fertigstellung bei Aktualisierungsstatus anzeigen“ im Profil eines Benutzers entfernt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 1. April 2024</p>
                            </li>
                            <li>
                                <p>Produktion für alle Kunden: Mit Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neuer Kommentar-Stream jetzt in Schnellaktionen für neue Startseiten-Widgets verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Wir haben nun in der neuen Startseite die neue Kommentierungsfunktion zur Schnellaktionsschaltfläche „Neues Update hinzufügen“ in den Widgets Meine Arbeit, Meine Projekte, Meine Aufgaben und Meine Probleme hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 1. März 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">In der neuen Kommentarerfahrung stehen zusätzliche Kommentar-Informationen zur Verfügung</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>In der neuen Kommentar-Funktion wurden folgende Verbesserungen vorgenommen:</p>
                        <ul>
                            <li>
                                <p>Sie können auf den Namen eines Kommentators klicken, um dessen Namen, Rolle und E-Mail-Adresse in einem Informationsfeld anzuzeigen. Diese Informationen können Ihnen dabei helfen, den richtigen Benutzer zu identifizieren, wenn mehrere Benutzer mit demselben Namen vorhanden sind. Wenn Sie im Informationsfeld auf den Namen des Kommentators klicken, wird sein Benutzerprofil geöffnet.</p>
                            </li>
                            <li>
                                <p>Ihr Benutzername wird in Kommentaren, mit denen Sie getaggt sind, hervorgehoben, wenn Sie im Kommentartext erwähnt werden.</p>
                            </li>
                        </ul>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 29. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Die Registerkarte „Systemaktivität“ im neuen Kommentarerlebnis unterstützt schreibgeschützte Kommentare</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Kommentare zu den Systemaktivitätsdatensätzen im alten Kommentar-Erlebnis werden jetzt auf der Registerkarte Systemaktivität im neuen Kommentar-Erlebnis als schreibgeschützt ausgefüllt. Sie können in der neuen Kommentar-Version nicht auf Systemaktivitätsdatensätze antworten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Registerkarte Aktualisierungsstrom , um sowohl Kommentare als auch Systemaktivitätseinträge zu erfassen</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Um Ihnen eine chronologisch einheitliche Ansicht von Kommentaren und Systemaktivitätsprotokollen zu geben, führen wir eine dritte Registerkarte im Bereich Aktualisierungen aller Objekte ein. Die Registerkarte „Alle“ erfasst sowohl Benutzerkommentare als auch Systemaktivitätskommentare in einem kohärenten Stream.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Neuer Kommentar-Stream jetzt im Bedienfeld Zusammenfassung verfügbar</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Wir haben dem Bedienfeld Zusammenfassung für Aufgaben- und Problemlisten nun die neue Kommentierungsfunktion hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: 22. Februar 2024</p>
                            </li>
                            <li>
                                <p>Produktion für die schnelle Veröffentlichung: Mit der Version 24.3 (14. März 2024)</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 24.4 (11. April 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Updates im zweiten Quartal 2024</a></p><p>[!BADGE In Production &#x200B;]{type=Informative}</p>
                        <p>Im zweiten Quartal 2024 werden kleinere Aktualisierungen des Erscheinungsbilds verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Lesen Sie die einzelnen Versionshinweise für bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Daten:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau der Version: Im gesamten Zeitraum der Version für das zweite Quartal 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Lesen Sie die Versionshinweise für bestimmte Daten</span></p>
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

Neue Funktionen in Workfront Fusion sind außerhalb des Veröffentlichungszeitplans für das zweite Quartal 2024 in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

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

Informationen zu den Wartungs-Updates, die im zweiten Quartal 2024 durchgeführt wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt Neue Funktionen auf der Seite [Workfront-Tutorials](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

