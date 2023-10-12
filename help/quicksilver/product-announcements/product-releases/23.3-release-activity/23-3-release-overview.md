---
title: Übersicht über die Version 23.3
description: Übersicht über die Version 23.3
author: Becky
feature: Product Announcements
exl-id: 441d84d6-6c40-4a03-967e-836cf78c8fc1
source-git-commit: 46d0a392875f24a55ebddaa7ff123bca0289a0bf
workflow-type: tm+mt
source-wordcount: '2737'
ht-degree: 0%

---

# Übersicht über die Version 23.3

Auf dieser Seite finden Sie Informationen zu den Funktionen der Version 23.3. Diese Verbesserungen wurden mit der Version 23.3 vom 20. und 21. Juli 2023 in der Produktionsumgebung verfügbar gemacht.

Das Webinar zur Version 23.3 wurde am 29. Juni 2023 veröffentlicht. Sie können [Registrieren Sie sich für das Webinar, um eine On-Demand-Aufzeichnung hier anzuzeigen.](https://webinars.on24.com/adobe_workfront/whatsnewin233?partnerref=exlreleaseoverview).

<span class="preview">Funktionen außerhalb des Kreislaufs (Funktionen, die vor dem Veröffentlichungsdatum 23.3 für die Produktion freigegeben wurden) sind gelb hervorgehoben.</span>

>[!IMPORTANT]
>
>Version 23.3 bietet die Möglichkeit, Ihr Unternehmen auf monatliche Releases umzustellen. Daher ändert Workfront das Nummerierungsschema der Versionen, um sowohl die monatlichen als auch die vierteljährlichen Releasedateien zu berücksichtigen.
>
>* Wenn Sie auf der **fast release (monatlich)** track, wird die Version nach 23.3 **23,8**, am 31. August 2023.
> * Wenn Sie auf der **vierteljährlich** Release-Track, wird die Version nach 23.3 **23,10**, in der Woche vom 26. Oktober 2023.
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
* [Agile Verbesserungen](#agile-enhancements)
* [Verbesserungen bei der Finanzverwaltung](#financial-management-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Mobile Verbesserungen](#mobile-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Schnellere Workfront-Veröffentlichungszyklen aktivieren</a></p>
                        <p>Damit Sie neue Workfront-Produktfunktionen und -Updates schneller erhalten können, haben wir die Möglichkeit hinzugefügt, schnellere Versionszyklen zu ermöglichen. Jetzt können Sie festlegen, dass Ihr Unternehmen Workfront-Versionen häufiger als einmal pro Quartal erhält. Der vierteljährliche Versionszyklus steht weiterhin für Organisationen zur Verfügung, die weniger häufige Versionen bevorzugen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Steuerung auf Gruppenebene, verfügbar für Timesheet- und Stundenvoreinstellung "Wo Benutzer Zeit protokollieren können"</a></p>
                        <p>Der Systemadministrator kann jetzt das Timesheet und die Voreinstellung "Wo Benutzer Zeit protokollieren können"sperren und entsperren. Wenn diese Voreinstellung entsperrt ist, können Gruppenadministratoren die Einstellungen "Wo Benutzer die Zeit protokollieren können"für jede Gruppe separat konfigurieren.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 4. Mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 18. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Logik anzeigen und Logikindikatoren und Regeln überspringen, die in der Beta-Version des Formulardesigners angezeigt werden</a></p>
                        <p>Die öffentliche Beta-Version des Formulardesigners wurde am 21. Juli 2023 in der Vorschau und Produktion wieder aktiviert. Darüber hinaus können Sie jetzt die vorhandenen Logikregeln anzeigen, die in älteren benutzerdefinierten Formularen im Formularentwickler erstellt wurden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 21. Juli 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion: 21. Juli 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Agile Verbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Agile Ansicht eines Projekts zeigt ein Kanban-Board an</a></p>
                        <p>Die Agile-Ansicht eines Projekts enthält jetzt zusätzliche Funktionen zum Filtern, Gruppieren und Sortieren von Arbeiten in einem Kanban-Board. Das neue, flexible Design der Ansicht beinhaltet eine robuste Suchfunktion und die Möglichkeit, dem Projekt direkt aus der Pinnwand neue Aufgaben hinzuzufügen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Nach Pinnwandspalten sortieren</a></p>
                        <p>Wir haben die Möglichkeit hinzugefügt, die Karten in den Spalten auf einer Pinnwand zu sortieren. Wenn Sie eine Sortieroption auswählen, werden alle Spalten sortiert. Eine einzelne Spalte kann nicht sortiert werden und der Rückstand oder die Annahmespalte sind nicht sortiert.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                             
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Dunkelmodus jetzt auf Adobe Workfront-Pinnwänden verfügbar</a></p>
                        <p>Sie können jetzt alle Foren und Workflows im Dunkelmodus anzeigen. Die neue Einstellung ist über die Voreinstellungen im Dashboard der Foren verfügbar.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Juni 2023<span style="color: #ff0000;"> Diese Funktion wurde aus der Vorschau entfernt und wird nicht mit Version 23.3 veröffentlicht.</span></p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: nicht verfügbar</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ziele, die bei Workstream-Iterationen in Adobe Workfront-Foren verfügbar sind</a></p>
                        <p>Wir haben die Möglichkeit hinzugefügt, einer Iteration Ziele hinzuzufügen, ohne die Ziele auf einer Karte auflisten zu müssen. Ziele werden in einem Checklisten-Format hinzugefügt und können als abgeschlossen markiert werden. Im Metrikbereich oben rechts in der Iteration wird angezeigt, wie viele Ziele vorhanden sind und wie viele erreicht wurden.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Juni 2023<span style="color: #ff0000;"> Diese Funktion wurde aus der Vorschau entfernt und wird nicht mit Version 23.3 veröffentlicht.</span></p>
                            </li>
                            <li>
                                <p>Produktionsversion für alle Kunden: nicht verfügbar</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Hinzufügen von Kommentaren zu Karten auf Pinnwänden</a></p>
                        <p>Sie können jetzt Kommentare zu Ad-hoc- und verbundenen Karten auf Pinnwänden hinzufügen und andere Benutzer mit den Kommentaren versehen. Kommentare sind in den Kartendetails verfügbar. Die Kommentarfunktion für Pinnwände verwendet das neue Adobe Workfront-Kommentarerlebnis.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau: 15. Juni 2023</p>
                            </li>
                            <li>
                                 <p>Produktionsversion für frühe Anmeldung: 22. Juni 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</span></p>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbesserungen beim Tag-Manager für Foren</a></p>
                        <p>Die Benutzeroberfläche des Tag-Managers wurde verbessert, sodass Sie schnell neue Tags erstellen und sie auf Karten anwenden können. Sie können auch Tags für Workflows erstellen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 19. Mai 2023</p>
                            </li>
                            <li>
                                 <p><span class="preview">Produktionsversion: 19. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Einfache Filter, die in Aufnahmespalten an Bord verfügbar sind</a></p>
                        <p>Vereinfachte Filter wurden zur Einrichtung der Ansaugspalte hinzugefügt, damit Sie die Ansauspalte schneller definieren können. Die verfügbaren Filter sind Workfront-Projekte und -Zuweisungen nach Team oder Benutzer. Sie können bei Bedarf zu den erweiterten Filtern wechseln.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 10. Mai 2023<br /></p>
                            </li>
                            <li>
                                 <p>Produktionsversion für frühe Anmeldung: 10. Mai 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</span></p>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Einfache Filter zur Vorlage der dynamischen Pinnwand hinzugefügt</a></p>
                        <p>Die Filter auf der Vorlage für dynamische Pinnwände wurden vereinfacht, sodass Sie Pinnwände schneller erstellen können.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 27. April 2023<br /></p>
                            </li>
                            <li>
                                 <p>Produktionsversion für frühe Anmeldung: 28. April 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</span></p>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Vorlage für dynamische Pinnwände</a></p>
                        <p>Eine neue Vorlage, dynamische Pinnwand, ist jetzt für eigenständige Pinnwände verfügbar. Diese Vorlage ist nicht für Pinnwände innerhalb eines Workflows verfügbar.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 20. April 2023<br /></p>
                            </li>
                            <li>
                                 <p>Produktionsversion für frühe Anmeldung: 28. April 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</span></p>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Migrieren von agilen Teams Kanban-Karten zu Foren</a></p>
                        <p>Eine neue <b>Hinzufügen zu Pinnwänden</b> Button in der agile Team Kanban Boards können Sie alle Karten aus dem Kanban-Board zu einer Workfront-Pinnwand hinzufügen. Sie können eine neue Workfront-Pinnwand erstellen oder die Karten einer vorhandenen Pinnwand hinzufügen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 20. April 2023<br /></p>
                            </li>
                            <li>
                                 <s><p>Produktionsversion für frühe Anmeldung: 28. April 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</span></p></s>
                                 </li>
                                 <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 18. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Linke Navigation zu Kartendetails auf Pinnwänden hinzugefügt</a></p>
                        <p>Je mehr Feldoptionen zu Karten auf Workfront-Pinnwänden hinzugefügt werden, desto länger sind die Kartendetails. In einem neuen Navigationsfenster links neben den Kartendetails können Sie einen Abschnitt auswählen und automatisch zu dieser Feldergruppe wechseln.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 20. April 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion für alle Kunden: 27. April 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">E-Mail-Benachrichtigungen und Voreinstellungen in Foren</a></p>
                        <p>E-Mail-Benachrichtigungen sind jetzt für Adobe Workfront-Pinnwände verfügbar. Die Benachrichtigungen sind standardmäßig aktiviert und Sie können in Ihren Voreinstellungen auswählen, welche E-Mails Sie erhalten möchten. Sie erhalten eine E-Mail, wenn Sie einer Pinnwand hinzugefügt und Ihnen eine Karte zugewiesen wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 13. April 2023<br /></p>
                            </li>
                            <li>
                                 <p>Produktionsversion für frühe Anmeldung: 13. April 2023 <span style="color: #ff0000;"> Diese Funktion ist zu diesem Zeitpunkt in der Produktion nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.</p>
                                <p>Produktionsversion für alle Kunden: Mit Version 23.3</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-finance-enhancements.md" class="MCXref xref" xrefformat="{para}">Datum der tatsächlichen Kosten- und Abrechnungskurse</a></p>
                        <p>Auf den Unternehmens-, Benutzer- und Jobrollenobjekten in Workfront sind jetzt datumswirksame Kosten- und Abrechnungskurse verfügbar. Wenn auf ein Projekt Datumswerte angewendet werden und Stunden für Projektaufgaben protokolliert werden, werden die Kosten und Einnahmen anhand der für jeden Zeitraum festgelegten Beträge berechnet.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 29. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion für Fast-Release-Kunden: Nach der Produktionsversion 23.3 anzukündigen.</p>
                                <p>Produktionsversion für alle Kunden: Ankündigung<br>
                                Die Funktion zum Außerkraftsetzen der Zuweisungsrate wurde in der Vorschau vom 30. Juni bis 13. Juli 2023 vorübergehend deaktiviert.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue G Suite-Integration verfügbar</a></p> 
                        <p>Eine neue G Suite-Integration ist jetzt im Google Marketplace verfügbar. Die neue Integration authentifiziert sich mit OAuth2 und ersetzt die vorherige Integration.</p><p>Die vorherige G Suite-Integration wird jetzt nicht mehr unterstützt und automatisch deinstalliert.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschauversion: nicht verfügbar</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 27. Juni 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Creative Cloud-Integrationen unterstützen jetzt mehrere zugewiesene Benutzer</a></p> 
                        <p>Die Adobe Creative Cloud-Integration unterstützt jetzt die Möglichkeit, zwischen "Fertig mit meinem Teil" und "Fertig"(oder "gelöst") zu wählen, wenn einer Aufgabe oder einem Problem mehrere Benutzer zugewiesen sind.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschauversion: nicht verfügbar</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 22. Juni 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Anzeigen und Verwalten von Workfront-Benachrichtigungen über Workfront für Creative Cloud-Plug-ins</a></p> 
                        <p>Um Ihnen den Empfang der benötigten Benachrichtigungen zu erleichtern, haben wir es ermöglicht, Workfront-Benachrichtigungen anzuzeigen und zu verwalten, ohne die Adobe Creative Cloud verlassen zu müssen. Jetzt können Sie Benachrichtigungen sowie die damit verbundenen Arbeitselemente und Kommentare direkt im Workfront-Plug-in-Fenster in der Creative Cloud-Anwendung anzeigen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschauversion: nicht verfügbar</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 22. Juni 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
 <!--               <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Improved experience when moving a document to a linked folder with drag and drop</a></p> 
                        <p>We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder. </p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: June 7, 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: June 15, 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>-->
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Automatisch verknüpfte Ordner mit Adobe Experience Manager Assets erstellen, wenn ein Projekt erstellt wird</a></p>
                        <p>Mit dem neuen Workflow Verknüpften Ordner für die Adobe Experience Manager-Integration erstellen können Sie die Integration mit einem Pfad zu einem Adobe Experience Manager Assets-Ordner konfigurieren. Wenn die Integration zu einer Projektvorlage hinzugefügt wird, erstellen alle aus der Vorlage erstellten Projekte automatisch einen verknüpften Unterordner in Experience Manager Assets im angegebenen Ordner. </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 11. Mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 24. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Zuordnen von Workfront-Feldwerten zu Tags in Experience Manager Assets</a></p>
                        <p>Jetzt können Sie Assets basierend auf Daten aus Workfront kategorisieren und schnell finden. Sie können diese Daten als Teil Ihrer Metadatenkonfiguration in der Workfront für Experience Manager Assets-Integration zuordnen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 10. Mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 10. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront-Felder benutzerdefinierten Experience Manager Assets-Metadatenfeldern zuordnen</a></p>
                        <p>Mit der nativen Integration können Sie jetzt sowohl native als auch integrierte Workfront-Felder benutzerdefinierten Metadatenschema-Feldern in Experience Manager Assets as a Cloud Service zuordnen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 10. Mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 10. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Anpassen der Workflow-Vorlageneinstellungen für automatisierte Testsendungen mit Adobe Workfront für Creative Cloud</a></p>
                        <p>Sie können die vorhandenen automatisierten Workflow-Vorlageneinstellungen jetzt direkt im Creative Cloud anpassen.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 27. April 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 27. April 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Dokumentgenehmigungen</a> </p>
                        <p>Dokumentgenehmigungen werden in einem schrittweisen Rollout neu gestaltet, das mit jeder Version mehr Benutzern zur Verfügung gestellt wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 31. Mai 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 14. Juni 2023</span></p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Diese Funktion ist Teil einer stufenweisen Veröffentlichung und steht derzeit nur bestimmten Kunden zur Verfügung.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Schaltfläche "Neue Freigabe"</a> </p>
                        <p>Die Option Freigeben wurde aus dem Menü Mehr für Projekte, Aufgaben und Probleme abgerufen, um die Freigabe intuitiver zu gestalten.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 22. Juni 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktionsversion: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Mobile Verbesserungen

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Testversandfunktion in der mobilen Workfront-App</a> </p>
                        <p>Da die eigenständige Workfront-Testversand-App in der Version 23.10 (Oktober 2023) eingestellt wurde, wurden der primären mobilen Workfront-App Testfunktionen hinzugefügt, mit denen die Weiterverfolgung von Testsendungen auf Mobilgeräten ermöglicht wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschauversion: nicht verfügbar</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Verfügbar im Apple App Store und Google Play Store am 21. Juni 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Starterlebnis</a></p>
                        <p>Um es Benutzern aller Typen zu ermöglichen, Workfront für ihre spezifischen Anforderungen zu nutzen, hat Home ein umfangreiches Update erhalten! Das neue Starterlebnis bietet visuelle und inhaltliche Anpassungen für Ihre Startseite und bietet die Flexibilität, nur die Informationen anzuzeigen, die für Ihre Arbeit am relevantesten sind.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 23. Juni 2023</p>
                            </li>
                            <li>
                                <p>Produktionsversion: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                                 
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Kommentierungserlebnis für zusätzliche Objekte</a> </p>
                        <p>Die neue Kommentarfunktion steht für die folgenden Objekte kurz nach der Version 23.3 in der Produktion zur Verfügung: Vorlagenaufgaben, Vorlagen, Timesheets, Teams, Benutzer, Programme, Portfolios.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Nach der Produktionsversion 23.3 anzukündigen.</p>
                            </li>
                            <li>
                                <p>Produktionsversion für Fast-Release-Kunden: Nach der Produktionsversion 23.3 anzukündigen. </p>
                                <p>Produktionsversion für alle Kunden: Mit der Version 23.10 (Oktober 2023)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                
            <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Kommentierungserlebnis für Beta für Projekte, Aufgaben und Dokumente</a> </p>
                        <p>Das neue Beta-Kommentarerlebnis ist jetzt für Projekte, Aufgaben und Dokumente verfügbar. Vor dieser Aktualisierung war das Beta-Kommentarerlebnis nur für Probleme und Ziele verfügbar.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 1. Juni 2023<br /></p>
                            </li>
                            <li>
                                <p>Produktionsversion: Mit Version 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Benutzerinitialen werden jetzt in Profilen ohne Avatare angezeigt</a></p>
                        <p>Um das Auffinden bestimmter Benutzer in großen Listen zu vereinfachen, werden die Benutzerinitialen in Profilen ohne benutzerdefinierte Avatare jetzt in Listen und Legacy-Berichten farbig hinterlegt. Dies ist eine geringfügige kosmetische Änderung und gilt nicht, wenn bereits ein Avatar-Foto verwendet oder der Benutzer deaktiviert wird.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 20. April 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 4. Mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Neue Verbesserungen beim kommentierenden Beta-Erlebnis</a></p>
                        <p>Verbesserungen am Abschnitt Aktualisierungen werden innerhalb des Zeitrahmens der Version 23.3 für das neue Kommentar-Beta-Erlebnis bereitgestellt. Sofern nicht anders angegeben, werden diese Verbesserungen in der Produktionsumgebung mit Version 23.3 bereitgestellt.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Während des Veröffentlichungszeitrahmens 23.3<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Mit Version 23.3 (sofern nicht anders angegeben)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Neue Verbesserungen beim Canvas-Dashboard</a></p>
                        <p>Verbesserungen am Canvas-Dashboard werden innerhalb des Veröffentlichungszeitrahmens von 23.3 bereitgestellt. Sofern nicht anders angegeben, werden diese Verbesserungen in der Produktionsumgebung mit Version 23.3 bereitgestellt. 
 </p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Version: 5. Juni 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: 5. Juni 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen während des Zeitrahmens der Version 23.3</a></p>
                        <p>Kleinere Aktualisierungen des Erscheinungsbilds verschiedener Bereiche der Adobe Workfront-Anwendung werden innerhalb des Veröffentlichungszeitrahmens von 23.3 vorgenommen. Diese Verbesserungen werden in der Produktionsumgebung mindestens 2 Wochen nach Veröffentlichung in der Vorschau verfügbar gemacht.</p>
                    </td>
                    <td><p><b>Verfügbar zu diesen Terminen:</b></p>
                        <ul>
                            <li>
                                <p>Vorschau-Veröffentlichung: Während des Veröffentlichungszeitrahmens 23.3</p>
                            </li>
                            <li>
                                <p><span class="preview">Produktionsversion: Mindestens 2 Wochen nach Veröffentlichung in der Vorschau (sofern nicht anders angegeben)</span></p>
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

Neue Funktionen in Workfront Fusion sind in der Produktion ab einem Zeitpunkt verfügbar, der außerhalb des Veröffentlichungszeitplans für 23.3 liegt. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbesserungen am Workfront-Szenario-Planer

Zu diesem Zeitpunkt der Version gibt es keine Aktualisierungen des Szenario-Players. Dieser Bereich wird aktualisiert, sobald Updates verfügbar sind.

### Workfront-Testverbesserungen

Neue Funktionen in der Workfront-Testversion innerhalb des Veröffentlichungszeitrahmens 23.3. Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront-Testversand mit Version 23.3](/help/quicksilver/product-announcements/product-releases/workfront-proof-release-activity/proof-23-3-release/proof-23-3-overview.md).

### Verbesserungen bei Workfront-Zielen

Neue Funktionen im Zusammenhang mit der Veröffentlichung der Workfront-Ziele innerhalb des Zeitrahmens der Version 23.3. Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront-Ziele mit Version 23.3](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-3-release/goals-23-3-release.md).

### API-Version 16

Für API Version 16 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere vereinfachen die Verwendung der über die API verfügbaren Informationen.

Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API Version 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version 22.3 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Informieren Sie sich über die neuesten Updates zu Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt &quot;Neue Funktionen&quot;im [Workfront Tutorials-Seite](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Funktion wird bald aus Workfront entfernt

Die folgende Funktion wird in Kürze aus Workfront entfernt:

#### Einstellung der mobilen Testversand-App mit Version 23.10 (Oktober 2023)

Mit der Version 23.10 (Oktober 2023) werden wir die mobile Proof-App offiziell als veraltet einstufen. Die allgemeine mobile Workfront-App wurde um eine neue Testversandfunktion erweitert (weitere Informationen finden Sie in der Versionshinweise unter Workfront Mobile-Verbesserungen ). Den Benutzern wird empfohlen, die Anwendung so bald wie möglich für Testsendungen zu verwenden.

Beachten Sie, dass für die mobile Workfront-App eine Workfront-Anmeldung erforderlich ist. Externe Benutzer und Gäste können die Proof-App weiterhin für Testsendungen verwenden. Sie wird jedoch nicht mehr unterstützt und ab Version 23.10 (Oktober 2023) nicht mehr verfügbar sein.


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


Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
