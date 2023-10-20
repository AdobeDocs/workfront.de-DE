---
title: Übersicht über die Version 2023 im vierten Quartal
description: Übersicht über die Version 2023 im vierten Quartal
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: 803c03845b834757b4643d8fd5c88f185ad6c32e
workflow-type: tm+mt
source-wordcount: '2606'
ht-degree: 0%

---

# Übersicht über die Version 2023 im vierten Quartal

Auf dieser Seite finden Sie Informationen zu den Funktionen, die in der Version vom vierten Quartal 2023 enthalten sind. Diese Verbesserungen sollen in der Produktionsumgebung für alle Kunden mit der Version 23.10 vom 26. und 27. Oktober 2023 verfügbar sein.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

Das Webinar zur Version 23.10 wurde am 5. Oktober 2023 veröffentlicht. Sie können [Registrieren Sie sich für das Webinar, um eine On-Demand-Aufzeichnung hier anzuzeigen.](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Funktionen außerhalb des Kreislaufs (Funktionen, die vor dem Veröffentlichungsdatum des vierten Quartals 2023 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Die Version 23.3 beinhaltet die Option, Ihr Unternehmen auf monatliche Releases umzustellen. Daher ändert Workfront das Nummerierungsschema der Versionen, um sowohl die monatlichen als auch die vierteljährlichen Releasedateien zu berücksichtigen.
>
>* Wenn Sie auf der **fast release (monatlich)** track: Die Version nach 23.3 ist **23,8**, am 31. August 2023.
> * Wenn Sie auf der **vierteljährlich** Release-Track, die Version nach 23.3 ist **23,10**, in der Woche vom 26. Oktober 2023.
> 
> Vierteljährliche Versionen enthalten Funktionen aus drei monatlichen Versionen. Die vierteljährliche Version 23.10 umfasst beispielsweise Funktionen, die in den monatlichen Versionen 23.8, 23.9 und 23.10 veröffentlicht wurden.
>
>Die monatlichen und vierteljährlichen Versionen sollen am letzten Donnerstag des Monats verfügbar sein.
>
>| Monatliche Version | Quartalsversion |
>|----|----|
>| <ul><li>23.8 (31. August 2023)</li><li>23.9 (28. September 2023)</li><li>23.10 (26. Oktober 2023)</li></ul> | <ul><li>23.10 Uhr (Woche vom 26. Oktober 2023)</li></ul> |
>| <ul><li>Keine Veröffentlichung (November 2023)</li><li>Keine Veröffentlichung (Dezember 2023)</li><li>24.1 (Januar 2024)</li></ul> | <ul><li>24.1 (Januar 2024)</li></ul> |
>
>Weitere Informationen zum Prozess der schnellen Veröffentlichung finden Sie unter [Schnellveröffentlichungsprozess aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Erweiterungen für Foren](#boards-enhancements)
* [Verbesserungen bei der Finanzverwaltung](#financial-management-enhancements)
* [Verbesserungen der Startseite](#home-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Berechnete Felder in benutzerdefinierten Formularen können jetzt den Platzhalter $$USER verwenden</a></p>
                        <p>Der Platzhalter $$USER ist jetzt in berechneten benutzerdefinierten Feldern und externen Suchfeldern im neuen Formularentwickler verfügbar.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 5. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Hinzufügen von Wertoptionen aus einer externen API zu einem benutzerdefinierten Formular</a></p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Ein neuer Feldtyp, <strong>Externe Suche</strong>, ist jetzt im benutzerdefinierten Formularentwickler verfügbar. Wenn Daten in einem externen System gespeichert sind, können Sie mit diesem Feldtyp Optionen aus einer externen API laden und basierend auf anderen Feldwerten im benutzerdefinierten Formular filtern.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 14. September 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Erweiterungen für Foren

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Auf Adobe Workfront-Pinnwänden jetzt verfügbare Unteraufgaben</a><span style="color: #ff0000;"> Neu in der Vorschau!</span></p><p>Wenn Sie einer Pinnwand für eine Workfront-Aufgabe eine verbundene Karte hinzufügen, werden alle vorhandenen Unteraufgaben auf die Karte importiert. Wenn Sie eine Unteraufgabe auf einer verbundenen Karte erstellen, wird der Workfront-Aufgabe eine Unteraufgabe hinzugefügt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für Foren - frühzeitiger Zugriff: nicht zutreffend</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: nicht zutreffend</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen bei der Benutzerzuweisung auf Pinnwänden und Karten</a></p><p>[!BADGE In Production ]{type=Informative}</p><p>Es gibt jetzt Verbesserungen, die beim Hinzufügen von Benutzern zu Pinnwänden und Karten in Adobe Workfront-Pinnwänden mehr Flexibilität bieten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. August 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 24. August 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Hinzufügen von Dokumenten zu verbundenen Karten</a></p><p>Sie können jetzt Dokumente auf verbundenen Karten auf Adobe Workfront-Pinnwänden anhängen. Alle Dokumente, die Sie auf der Karte hinzufügen, stehen auf der Registerkarte Dokumente der verbundenen Aufgabe oder Ausgabe zur Verfügung. Dieselben Dateitypen werden in beiden Bereichen unterstützt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für Foren frühzeitiger Zugriff: 24. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: nicht zutreffend</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Dokumente, die auf verbundenen Karten nur als Ansicht verfügbar sind</a></p><p>Für verbundene Karten auf Adobe Workfront-Pinnwänden können Sie jetzt Dokumente wie Bilder und PDF anzeigen. Sie können entweder eine Vorschau eines Dokuments im Browser anzeigen oder es auf Ihren Computer herunterladen. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 3. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für Foren frühzeitiger Zugriff: 10. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: nicht zutreffend</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Überblick über ein Projekt jetzt für Probleme verfügbar</a></p><p>Sie können jetzt auf eine Pinnwandansicht einer Projektfehlerliste zugreifen. Das Kanban-Board kann Ihnen dabei helfen, den Fortschritt der Probleme visueller zu verfolgen, als sie in der Liste anzuzeigen. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 3. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für Foren - frühzeitiger Zugriff: nicht zutreffend</p>
                            </li>
                             <li>
                                <p>Produktion für schnelle Veröffentlichung: nicht zutreffend</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Datum der tatsächlichen Kosten- und Abrechnungskurse</a></p>
                        <p>Auf den Unternehmens-, Benutzer- und Jobrollenobjekten in Workfront sind jetzt datumswirksame Kosten- und Abrechnungskurse verfügbar. Wenn auf ein Projekt Datumswerte angewendet werden und Stunden für Projektaufgaben protokolliert werden, werden die Kosten und Einnahmen anhand der für jeden Zeitraum festgelegten Beträge berechnet.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Schaltfläche "Arbeit delegieren"für Projekt-, Aufgaben- und Problem-Widgets</a> <span style="color: #ff0000;"> Neu in der Vorschau!</span></p>
                        <p>Als häufig angeforderte Funktion der alten Startseite haben wir jetzt eine Delegierungsschaltfläche zu den Widgets "Meine Arbeit", "Meine Aufgaben"und "Meine Probleme"hinzugefügt, damit Sie Ihre Arbeit einfach delegieren können, wenn Sie nicht im Büro sind.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Widget "Pinnwände"für neues Zuhause</a> <span style="color: #ff0000;"> Neu in der Vorschau!</span></p>
                        <p>In einer wichtigen neuen Ergänzung zu den Arbeitsverwaltungsoptionen, die in New Home verfügbar sind, können Sie jetzt eine Pinnwand auf Ihrer Homepage anzeigen!</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Mitarbeiter-Standard-Landingpage: Neue Startseite</a> <span style="color: #ff0000;"> Neu in der Vorschau!</span> </p>
                        <p>Die neue Startseite ist jetzt die Standard-Landingpage für Mitarbeiter-/Anforderungskonten. Diese neue Standard-Startseite enthält eine Reihe von Widgets, die speziell ausgewählt wurden, damit Mitarbeiter ihre Arbeit am besten sofort verwalten können.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Änderungen an der Arbeitsverfolgung in der neuen Startseite </a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Basierend auf dem Benutzer-Feedback haben wir den seitenweiten Zeitbereichsfilter und die Zusammenfassungsleiste entfernt, in denen Aufgaben aufgelistet wurden, die fällig und abgeschlossen waren. Projekt-, Aufgaben- und Problem-Widgets verfügen jeweils über integrierte Filterfunktionen, mit denen Sie ihren Umfang individuell anpassen können.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 13. September 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Schnellzugriffsschaltflächen für Projekt-, Aufgaben- und Problemverfolgungswidgets</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Die Tracking-Widgets "Projekt", "Aufgabe"und "Problem"wurden um neue Schnellzugriffsschaltflächen erweitert, sodass Sie Ihre Arbeit direkt über die neue Startseite verwalten können.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 13. September 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.9</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Filteroptionen für neue Startseite</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Neue Filteroptionen sind jetzt für das Widget "Meine Arbeit"in "Neue Startseite"verfügbar. Zu den Optionen gehören Filter für Objekttypen (Aufgaben, Probleme und Anforderungen) und Status (nicht bereit, startbereit, arbeiten und fertig gestellt).</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Benutzerdefinierte Terminologieunterstützung für die neue Startseite</a> </p><p>[!BADGE In Production ]{type=Informative}</p>
                        <p>Um die besonderen Anforderungen von Unternehmen besser zu erfüllen, verwendet das neue Home jetzt benutzerdefinierte Terminologie für Objekte, die in den Layoutvorlagen einer Instanz definiert sind. Wenn beispielsweise die Objekte "Projekt"in Ihrer Workfront-Instanz in "Kampagnen"umbenannt wurden, wird das Widget "Meine Projekte"stattdessen als "Meine Kampagnen"auf der neuen Startseite angezeigt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 31. August 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Die Schaltfläche Neue Startseite ausprobieren wurde für Konten entfernt, die "Neue Startseite"deaktiviert haben</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Die Schaltfläche Neue Startseite ausprobieren ist nicht mehr für Konten vorhanden, für die die Option Neue Startseite deaktiviert wurde. Die neue Startseite muss vom Systemadministrator erneut aktiviert werden, bevor einzelne Benutzer die Schaltfläche zum Testen der neuen Startseite verwenden können.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Standard-Widget "Neue Startseite"ändern</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Das To-dos-Widget, das die Berechtigung zum Erstellen von Aufgaben erfordert, ist jetzt nur im standardmäßigen Widget-Satz für Benutzer mit den Lizenztypen Standard, Plan oder Arbeit vorhanden. Darüber hinaus wurde das Widget automatisch aus den Startseiten von Benutzern mit allen anderen Lizenztypen entfernt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: 17. August 2023</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: 17. August 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen beim Senden von Dokumenten an SharePoint (GraphAPI)</a></p><p>[!BADGE In Production ]{type=Informative}</p><p>Wir haben einige Änderungen vorgenommen, um das Auffinden von Ordnern beim Senden von Dokumenten an Ihre SharePoint (GraphAPI)-Ordner zu vereinfachen</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 24. August 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 31. August 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Aktualisierungen zum Drag &amp; Drop für Dokumentintegrationen</a></p><p>[!BADGE In Production ]{type=Informative}</p><p>Wir haben einige Verbesserungen vorgenommen, um Klarheit zu schaffen und Benutzerfehler beim Ziehen und Ablegen einer Datei in einen verknüpften Ordner zu entfernen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 24. August 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: 31. August 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Dokumentgenehmigungen</a> <span style="color: #ff0000;"> Neu in der Vorschau!</span></p>
                        <p>In dieser Version wurde der Genehmigungsprozess optimiert, um neben neuen Funktionen sowohl Genehmigungen zu erstellen als auch Dokumente zu genehmigen/zu überprüfen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Diese Funktion ist Teil einer stufenweisen Veröffentlichung und steht derzeit nur bestimmten Kunden zur Verfügung.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Echtzeitaktualisierungen auf der Aufgabenliste</a> </p>
                        <p>[!BADGE In Produktion]{type=Informative}</p>
                        <p>Aufgabenlisten werden jetzt in Echtzeit aktualisiert. Änderungen, die an einer Aufgabe vorgenommen werden, werden in der Aufgabenliste aktualisiert, sodass ein Benutzer, der die Aufgabenliste anzeigt, die Änderung sehen kann, ohne die Seite zu aktualisieren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschauversion: nicht verfügbar<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktion für alle Kunden: stufenweise Einführung, abgeschlossen am 19. Oktober 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Entwurf beim Hinzufügen eines neuen Problems zu einem Projekt aktualisiert</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Dieses Update wurde mit Version 23.3 angekündigt.</p>
                        <p>Wir haben das Feld Neues Problem aktualisiert, das beim Senden eines neuen Problems an ein Projekt angezeigt wird. Jetzt stimmt die Benutzeroberfläche mit dem Feld Neue Anforderung überein, das beim Senden einer neuen Anforderung an eine Anforderungswarteschlange angezeigt wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 26. Juli 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Dynamische Neuberechnung berechneter Felder in Formularen</a></p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Berechnete Felder in einem Formular, das an ein Objekt angehängt ist, werden jetzt dynamisch in Echtzeit neu berechnet, wenn die abhängigen Werte in einem Formular auf der Seite geändert werden. Auf diese Weise können Sie die aktualisierten Ergebnisse anzeigen, ohne das Formular zu speichern.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Geplante Stunden für untergeordnete wiederkehrende Aufgaben mit einfacher Dauer ohne Zuweisung festlegen</a></p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Die Art und Weise, wie geplante Stunden wiederkehrenden Aufgaben ohne Zuweisung und einfache Dauer zugeordnet werden, wurde geändert. Wenn Sie jetzt "Geplante Stunden"für eine neue wiederkehrende Aufgabe mit dem Typ Einfache Dauer und ohne Zuweisung festlegen, werden die Stunden auch den einzelnen Wiederholungen zugeordnet. Vor dieser Änderung wurden die Stunden nicht für einzelne Wiederholungen gespeichert, wenn die Zuordnung der übergeordneten Aufgaben aufgehoben wurde.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 17. August 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Änderungen am Hauptmenü des Beitragenden</a> <span style="color: #ff0000;"> Neu in der Vorschau!</span></p>
                        <p>Um Mitarbeiter/Antragsteller besser über die Funktionen zu informieren, die mit einem gebührenpflichtigen Workfront-Lizenztyp verfügbar sind, können sie jetzt alle verfügbaren Optionen im Hauptmenü sehen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 12. Oktober 2023</p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit der Version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Neue Verbesserungen der Beta-Version für Kommentierungserlebnisse</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Verbesserungen am Abschnitt Updates werden innerhalb des Zeitrahmens der Veröffentlichung für das kommentierende Erlebnis-Beta für das vierte Quartal 2023 bereitgestellt. Diese Verbesserungen werden in der Produktionsumgebung allen Kunden mit der Version vom vierten Quartal 2023 (Oktober 2023) zur Verfügung gestellt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des vierten Quartals 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Ab Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit Version 23.10 (sofern nicht anders angegeben)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Neue Beta-Verbesserungen für Canvas Dashboards</a> </p>
                        <p>[!BADGE In Produktion für schnelle Veröffentlichung ]{type=Positive}</p>
                        <p>Verbesserungen an den Canvas-Dashboards werden im Rahmen der laufenden Beta-Phase im Veröffentlichungszeitrahmen des vierten Quartals 2023 bereitgestellt. Diese Verbesserungen werden in der Produktionsumgebung allen Kunden mit der Version vom vierten Quartal 2023 (Oktober 2023) zur Verfügung gestellt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des vierten Quartals 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktion für schnelle Veröffentlichung: Ab Version 23.8</p>
                            </li>
                            <li>
                                <p>Produktion für die vierteljährliche Veröffentlichung: Mit Version 23.10 (sofern nicht anders angegeben)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen im vierten Quartal 2023</a></p><p>Im vierten Quartal 2023 werden kleinere Aktualisierungen des Erscheinungsbilds verschiedener Bereiche der Adobe Workfront-Anwendung vorgenommen. Prüfen Sie die einzelnen Versionshinweise auf bestimmte Veröffentlichungstermine.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Im gesamten Veröffentlichungszeitrahmen des vierten Quartals 2023</p>
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

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung außerhalb des Veröffentlichungszeitplans für das vierte Quartal 2023 verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront-Testverbesserungen

Es gibt derzeit keine Workfront Testversandaktualisierungen in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Verbesserungen bei Workfront-Zielen

Es gibt derzeit keine Aktualisierungen zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### API-Version 17

API-Version 17 wurde am 12. Oktober 2023 veröffentlicht. Für API Version 17 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API Version 17](/help/quicksilver/wf-api/api/new-api-version-17.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version 22.3 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;im [Workfront Tutorials-Seite](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funktion wird bald aus Workfront entfernt

Die folgende Funktion wird in Kürze aus Workfront entfernt:

#### Einstellung der mobilen Testversand-App mit Version 23.10

Mit Version 23.10 werden wir die mobile Proof-App offiziell als veraltet einstufen. Die allgemeine mobile Workfront-App wurde um eine neue Testversandfunktion erweitert (weitere Informationen finden Sie in der Versionshinweise unter Workfront Mobile-Verbesserungen ). Den Benutzern wird empfohlen, die Anwendung so bald wie möglich für Testsendungen zu verwenden.

Beachten Sie, dass für die mobile Workfront-App eine Workfront-Anmeldung erforderlich ist. Externe Benutzer und Gäste können die Proof-App weiterhin für Testsendungen verwenden. Sie wird jedoch nicht mehr unterstützt und ab Version 23.10 nicht mehr verfügbar sein.

#### Workflows wurden für Konten entfernt, die sie nicht verwenden

Bei Konten, die noch nie einen Workstream in Adobe Workfront-Pinnwänden erstellt haben, wurde der Bereich Workflows ab dem 11. Oktober 2023 aus dem Dashboard der Pinnwände entfernt. Konten, die Workflows verwenden, haben weiterhin Zugriff darauf. In zukünftigen Versionen werden verbesserte Funktionen für die Bildbearbeitung behoben.

<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
