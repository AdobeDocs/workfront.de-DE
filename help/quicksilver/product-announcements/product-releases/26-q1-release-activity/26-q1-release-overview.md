---
title: Übersicht über die Version im ersten Quartal 2026
description: Diese Seite enthält Informationen zur Funktionalität, die in der Version vom ersten Quartal 2026 enthalten ist. Diese Verbesserungen werden voraussichtlich im gesamten Quartal in der Produktionsumgebung verfügbar sein.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d66ff030bbc06436c9212352e53fbd9f8241d8c0
workflow-type: tm+mt
source-wordcount: '2885'
ht-degree: 5%

---

# Übersicht über die Version im ersten Quartal 2026

Diese Seite enthält Informationen zur Funktionalität, die in der für Januar 2026 geplanten Version vom ersten Quartal 2026 enthalten ist.

Die Verbesserungen auf dieser Seite sind in der Vorschau -Umgebung verfügbar. Diese Seite wird mit zusätzlichen Verbesserungen aktualisiert, sobald die Veröffentlichung im ersten Quartal 2026 der geplanten Produktionsversion nahekommt.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Sofern nicht anders angegeben, sind monatliche und vierteljährliche Versionen am Donnerstag der zweiten vollen Woche des Monats verfügbar.
>
>| Monatliche Version | Vierteljährliche Veröffentlichung |
>|----|----|
>| <ul><li>25.11 (13. November 2025)</li><li>25.12 (11. Dezember 2025)</li><li>26.1 (14. Januar 2026)</li></ul> | <ul><li>26.1 (15. Januar 2026)</li></ul> |
>
>Beachten Sie, dass Benutzer, die den Zeitplan für die schnelle Veröffentlichung im letzten Quartal (26.1 in diesem Quartal) einhalten, die Veröffentlichung einen Tag früher erhalten (14. Januar 2026).
>
>Weitere Informationen zum Schnellfreigabeprozess finden Sie unter [Aktivieren oder Deaktivieren des Schnellfreigabeprozesses](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront-Verbesserungen

* [Administrator-Verbesserungen](#administrator-enhancements)
* [Verbesserungen bei Dokumenten und Genehmigungen](#documents-and-approvals-enhancements)
* [Home-Verbesserungen](#home-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen beim Reporting](#reporting-enhancements)
* [Verbesserungen bei Anfragen](#requests-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administrator-Verbesserungen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Verwalten von Prioritäten in der Layout-Vorlage</a>
            <p><span class="preview">Vorübergehend nicht in der Vorschau-Umgebung verfügbar</span></p>
            <p>Sie können jetzt in der Layout-Vorlage Prioritäten für bestimmte Benutzer aktivieren oder deaktivieren. Wenn Sie zuvor Prioritäten für Ihre Organisation deaktiviert hatten, bleibt sie mit dieser Änderung in der Layout-Vorlage deaktiviert.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Mittwoch, 14. Januar 2025</td>
        <td>Donnerstag, 15. Januar 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Überprüfung auf Konflikte mit mehreren Formularen für berechnete benutzerdefinierte Felder</a>
            <p>Um bei der Bearbeitung eines Ausdrucks für benutzerdefinierte Felder die möglichen Auswirkungen auf Objekte sichtbar zu machen, wurde eine Option zur Konfliktprüfung hinzugefügt. In diesem Dialogfeld werden alle Objekte gruppiert nach Objekttyp angezeigt, die von einer Änderung der Formel betroffen sein könnten. Sie können zu den Details der einzelnen Objekte navigieren und die Felder überprüfen, um zu entscheiden, ob das Feld aus einem der Formulare entfernt werden soll oder der Ausdruck unverändert bleiben soll.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Mittwoch, 14. Januar 2025</td>
        <td>Donnerstag, 15. Januar 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Eingabedatum und „Eingegeben von ID“ in benutzerdefinierten Objekten</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Das Eingabedatum und die von der ID eingegebenen Daten werden jetzt in benutzerdefinierten Formularen, Feldern und Abschnitten gespeichert. Sie können diese Datenoptionen in Berichten als Filter, Ansichten oder Gruppierungen verwenden. Um sie in der Liste der benutzerdefinierten Formulare, Felder oder Abschnitte im Setup anzuzeigen, fügen Sie „Eingabedatum“ hinzu und geben Sie „Nach Name“ als Spalten in einer neuen oder vorhandenen Ansicht ein.</p>
        </td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 13. November 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Aktualisierungen der Schaltflächennamen beim Bearbeiten einer Layout-Vorlage</a>
            <p>Um für mehr Konsistenz mit anderen Bereichen von Setup zu sorgen, z. B. mit dem benutzerdefinierten Formular-Designer, wurden die Schaltflächen, die Sie beim Bearbeiten einer Layout-Vorlage sehen, in Anwenden, Speichern und schließen und Abbrechen geändert. Mit der neuen Option Übernehmen können Sie Ihre Änderungen an der Layout-Vorlage speichern und mit der Bearbeitung fortfahren. Zuvor waren die verfügbaren Optionen Speichern und Abbrechen. </p>
        </td>
        <td>Freitag, 30. Oktober 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Verbesserte Feldverwaltung mit Markierung „Aktiv“ für benutzerdefinierte Felder</a>
            <p>Wenn das System eine große Anzahl benutzerdefinierter Felder enthält, kann die Verwaltung dieser Felder in benutzerdefinierten Formularen und Berichten schwierig sein. Sie können jetzt benutzerdefinierte Felder mit der neuen Markierung „Aktiv<b> als inaktiv </b>. Diese Markierung ist verfügbar, wenn Sie mit einem Feld in einem benutzerdefinierten Formular arbeiten oder ein Feld aus der Liste Felder hinzufügen oder bearbeiten. </p>
        </td>
        <td>Freitag, 30. Oktober 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
  </tbody>
</table>

### Verbesserungen bei Dokumenten und Genehmigungen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
        </tr>
       <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Set up brands for the AI reviewer in Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>You can now set up brands for the AI reviewer in the Workfront Setup area. This allows you to customize the AI review process based on your organization's branding guidelines.</p>
            <p>The AI reviewer is currently in beta.</p>
        </td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
    </tr> -->
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Wählen Sie ein Workfront-Projekt, wenn Sie eine Überprüfung in Adobe Express senden<p>[!BADGE OFF SCHEDULE]{type=neutral}</p> </a>
            <p>Sie können ein Workfront-Projekt auswählen, an das ein Testversand gesendet werden soll. Auf diese Weise bleiben alle zugehörigen Assets und Testsendungen innerhalb desselben Projekts organisiert.</p>
        </td>
        <td>Dienstag, 15. Dezember 2025</td>
        <td>Dienstag, 15. Dezember 2025</td>
        <td>Dienstag, 15. Dezember 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Organisationsübergreifende Unterstützung für Adobe Express mit Workfront Proofing<p>[!BADGE OFF SCHEDULE]{type=neutral}</p> </a>
            <p>Mit Workfront Proofing führen wir organisationsübergreifenden Support für Adobe Express ein. Diese Verbesserung ermöglicht es Kunden, die in mehreren IMS-Organisationen tätig sind, Proofing-Workflows nahtlos zu verwenden und zu verwalten.</p>
        </td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 13. November 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager ist jetzt mit der Frame.io-Integration verfügbar <p>[!BADGE OFF SCHEDULE]{type=neutral}</p> </a>
            <p>Jetzt können Sie Experience Manager Assets verwenden, ​ Ihre digitalen Assets zu verwalten und zu speichern, die den Überprüfungs- und Genehmigungszyklus durchlaufen haben. Durch diese Integration können Sie die Funktionen von Adobe Experience Manager, Frame.io und Workfront nutzen, um Ihr Content-Management und Ihre Kollaborationsprozesse zu optimieren. </p>
        </td>
        <td>Freitag, 30. Oktober 2025</td>
        <td>Freitag, 30. Oktober 2025</td>
        <td>Freitag, 30. Oktober 2025</td>
    </tr>   
  </tbody>
</table>



### Home-Verbesserungen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">Aktualisieren des Widgets Erwähnungen auf der Startseite</a>
            <p>Wir haben folgende Verbesserungen am Mentions-Widget auf der Startseite vorgenommen: <ul><li>Das gleiche Erlebnis im Bereich Aktualisierungen der meisten Workfront-Objekte ist jetzt auch im Erwähnungen -Widget auf der Startseite verfügbar. </li><li>Das Widget Erwähnungen enthält jetzt die Kommentare, die der Benutzer in den letzten zwei Wochen gemacht hat oder getaggt wurde</li><ul></p>
        </td>
        <td>Donnerstag, 17. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
  </tbody>
</table>

### Integrationsverbesserungen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Wählen Sie ein Workfront-Projekt aus, wenn Sie eine Überprüfung in Creative Cloud Express senden</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Sie können ein Workfront-Projekt auswählen, an das ein Testversand gesendet werden soll. Auf diese Weise bleiben alle zugehörigen Assets und Testsendungen innerhalb desselben Projekts organisiert. </p>
        </td>
        <td>Dienstag, 15. Dezember 2025</td>
        <td>Dienstag, 15. Dezember 2025</td>
        <td>Dienstag, 15. Dezember 2025</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Aktualisierter Asset-Wähler für die native Integration von Adobe Workfront für Experience Manager Assets </a>
            <p>Wir haben den Asset-Wähler in der Integration von Adobe Workfront für Experience Manager Assets aktualisiert. Mit diesem Upgrade können Sie jetzt AEM-Sammlungen direkt in Workfront auswählen und abrufen. </p>
        </td>
        <td>Freitag, 20. November 2025</td>
        <td>Freitag, 11. Dezember 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
    <!-- <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>   -->
  </tbody>
</table>

### Projektverbesserungen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Light-Benutzer können die Zeit in Projekten protokollieren</a>
            <p>Leichte Benutzer können jetzt die Zeit direkt in Projekten protokollieren. Zuvor konnten nur Benutzer von Standardlizenzen Stunden an Projekten protokollieren.</p>
        </td>
        <td>Freitag, 11. Dezember 2025</td>
        <td>Freitag, 15. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
  </tbody>
</table>

### Verbesserungen beim Reporting

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Währungs-Updates in Arbeitsflächen-Dashboards</a>
            <p>Für Währungsfelder haben wir die folgenden Aktualisierungen vorgenommen:<ul><li>Wenn mehrere Währungen in Workfront definiert sind, können Sie jetzt während der Erstellung eine Standardwährung für das Dashboard auswählen. </li><li>Beim Erstellen eines Berichts können Sie ein Währungsfeld sperren. Dadurch wird sichergestellt, dass die Währungsvoreinstellung auf Dashboard-Ebene keine Auswirkungen auf die Anzeige dieser Werte hat.</li><li>Beim Anzeigen eines Dashboards können Benutzer in Workfront zwischen beliebigen definierten Währungen wechseln. Diese Änderungen gelten für das gesamte Dashboard mit Ausnahme gesperrter Währungsfelder</li></ul></p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}"> Ergebnisse der Schnellsuch-Tabelle in Canvas-Dashboards</a>
            <p>Wir haben eine Schnellsuche zu Tabellenberichten hinzugefügt. Diese Suche funktioniert über alle Seiten hinweg, sodass Sie Daten finden können, auch wenn sie derzeit nicht sichtbar sind.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Neue Option „Gesamtsumme anzeigen“ für Tortendiagramme</a>
            <p>Wir haben eine neue Option Gesamt anzeigen eingeführt, die Tortendiagramme in Ringdiagramme konvertiert. Mit dieser Funktion können Benutzer einen zentralen Wert anzeigen, der die Summe aller Segmente im Diagramm darstellt.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Neue Konfigurationsoptionen für Tortendiagramme in Leinwand-Dashboards</a>
            <p>Wir haben zwei neue Konfigurationsoptionen für Tortendiagramme eingeführt: <ul><li>Segmentbeschriftungen ausblenden: Sie können jetzt festlegen, dass Segmentbeschriftungen in einem Tortendiagramm ausgeblendet werden, wenn sie zu lang sind und die Lesbarkeit des Diagramms beeinträchtigen.</li><li>Diagrammlegende ausblenden und neu positionieren: Sie können jetzt eine Tortendiagramm-Legende ausblenden. Sie können die Position der Legende auch rechts (Standard), links, oben oder unten im Diagramm festlegen. </li></ul></p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Verbesserungen bei der Gruppierungsanzahl in Arbeitsflächen-Dashboards</a>
            <p>Die Gruppierungsleiste in den Dashboards der Arbeitsfläche wurde aktualisiert, um die Datensatzanzahl für die aktuelle Seite und die Gesamtdatensatzanzahl für die Gruppierung über alle Seiten hinweg anzuzeigen. </p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Neue Referenzzeilenfunktion in Berichten in Arbeitsflächen-Dashboards</a>
            <p>Sie können jetzt eine Referenzlinie in Balken-, Spalten- und Liniendiagrammen definieren, um einen Ziel- oder Schwellenwert für Ihre serienbasierten Berichte festzulegen. </p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Anpassen von Achsenbeschriftungen in Diagrammberichten in Arbeitsflächen-Dashboards</a>
            <p>Sie können jetzt die Achsenbeschriftungen in Diagrammberichten anpassen. Mit dieser neuen Funktion können Sie eine Beschriftung für die Ersatzachse eingeben, die anstelle des Standardobjekts und des Feldpfads angezeigt werden soll. Darüber hinaus können Sie festlegen, dass die Achsenbeschriftungen vollständig ausgeblendet werden.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Duplizieren eines Berichts in einem Arbeitsflächen-Dashboard</a><p>[!BADGE OFF SCHEDULE]{type=neutral}</p>
            <p>Sie können jetzt einen KPI-, Tabellen- oder Diagrammbericht in einem Arbeitsflächen-Dashboard duplizieren, nachdem er erstellt wurde. Nach dem Duplizieren können Sie den Bericht nach Bedarf bearbeiten, bevor Sie ihn speichern.</p>
        </td>
        <td>Freitag, 23. Oktober 2025</td>
        <td>Freitag, 23. Oktober 2025</td>
        <td>Freitag, 23. Oktober 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Entfernen von Feldoptionen aus Berichtsfiltern</a>
            <p>Wir haben die folgenden Feldoptionen entfernt, die zuvor beim Anwenden eines Filters auf einen Bericht verfügbar waren:
            <ul>
            <li>Andere Gruppen-IDs</li>
            <li>Andere Rollen-IDs</li>
            <li>Andere Team-IDs</li>
            </ul>
            </p>
        </td>
        <td>Freitag, 6. November 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Neue Leitplanken zur Verbesserung der Ladezeiten in Arbeitsflächen-Dashboards</a>
            <p>Um Ladezeitverzögerungen zu vermeiden und die Gesamtleistung in Arbeitsflächen-Dashboards zu verbessern, haben wir Grenzwerte für die Anzahl der Dashboard-Komponenten angewendet, die einem Dashboard hinzugefügt werden können:
            <ul>
            <li>Berichte pro Dashboard: maximal 25</li>
            <li>Gruppierungen in Tabellenansichten: maximal 5</li>
            <li>Entfernung vom Basisobjekt des Berichts: 10 Grenze</li>
            <li>Spalten in einer Tabellenansicht: maximal 25</li>
            <li>Filter auf Dashboard-Ebene - Eingabeaufforderungen: 10 Grenze</li>
            </ul></p>
        </td>
       <td>Freitag, 6. November 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
  </tbody>
</table>

### Verbesserungen bei Anfragen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Erstellte Objektverknüpfungen sind jetzt im Bereich Anfragen und im Widget Meine Anfragen verfügbar</a>
            <p>Um Ihnen den Zugriff auf das von einer bestimmten Anfrage erstellte Objekt zu erleichtern, haben wir Links zur Spalte Erstelltes Objekt hinzugefügt. Jetzt können Sie auf den Link in dieser Spalte klicken, um direkt zur Seite des erstellten Objekts zu gelangen.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr> 
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Benutzerdefinierte Felder zur Anfragenliste und zum Widget „Meine Anfragen“ hinzufügen</a>
            <p>Um Ihnen die Anzeige der benötigten Informationen zu erleichtern, haben wir die Möglichkeit hinzugefügt, benutzerdefinierte Felder als Spalten zur Anfragenliste und zum Widget Meine Anfragen auf der Startseite hinzuzufügen. Jetzt können Sie Felder aus benutzerdefinierten Formularen als Spalte hinzufügen. Anfragen, die Informationen in diesem Feld enthalten, zeigen diese Informationen in der Liste oder im Widget an.</p><p>Diese Funktion ist nur in der neuen Anfrageerfahrung verfügbar.</p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Der Platzhalter für aktuelle Benutzer ist jetzt im Anforderungsfilter verfügbar</a>
            <p>Um das Filtern nach für Sie relevanten Anfragen zu vereinfachen, haben wir einen Platzhalter für aktuelle Benutzer erstellt. Jetzt können Sie beim Filtern „Ich (angemeldeter Benutzer)“ auswählen. Der Filter gilt dann für den Benutzer, der die Anfrageliste anzeigt.   </p>
        </td>
        <td>Freitag, 18. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Formularausfüllen mit KI ist jetzt für Anfragen verfügbar</a>
            <p>Um das Erstellen von Anfragen zu vereinfachen, haben wir das Formularausfüllen mit KI erstellt. Jetzt können Sie eine Eingabeaufforderung einfügen oder ein Dokument in ein Anfrageformular hochladen, und AI ruft die relevanten Informationen ab und füllt das Formular aus.  </p>
        </td>
        <td>Freitag, 11. Dezember 2025</td>
        <td>Freitag, 11. Dezember 2025</td>
        <td>Freitag, 11. Dezember 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Freigeben von Ansichten im Bereich „Anfragen“ und im Widget „Meine Anfragen“</a>
            <p>Um die Anzeige der benötigten Informationen zu vereinfachen, haben wir die Möglichkeit hinzugefügt, Ansichten zu dem neuen anfordernden Erlebnis auszutauschen. Jetzt können Sie Ansichten mit anderen Benutzern, Teams oder Gruppen teilen. </p>
        </td>
        <td>Freitag, 4. Dezember 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Speichern von Anfrageentwürfen in der neuen anfragenden -Version</a>
            <p>Um das Erstellen und Senden von Anfragen zu vereinfachen, haben wir die Möglichkeit hinzugefügt, Entwürfe zu speichern. Wenn Sie jetzt mit dem Ausfüllen und Schließen einer Anfrage beginnen, wird die Anfrage im Status Entwurf gespeichert und ist im Anfrageformular zu finden, das zum Erstellen des Entwurfs verwendet wird. Sie können den Entwurf dann jederzeit erneut öffnen, aktualisieren und senden. </p>
        </td>
        <td>Freitag, 20. November 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Gelöschte Anfragen in der neuen anfordernden Version löschen</a>
            <p>Um die Organisation Ihrer Anfragen zu vereinfachen und die Übersichtlichkeit zu verbessern, haben wir die Möglichkeit hinzugefügt, Anfragen zu löschen. Jetzt können Sie von Ihnen gesendete Anfragen löschen. Workfront-Administratoren und Workfront Planning Workspace-Administratoren können Anfragen auch löschen.</p>
        </td>
        <td>Freitag, 20. November 2025</td>
        <td>Donnerstag, 14. Januar 2026</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Erstellen neuer Anfragen durch Kopieren zuvor gesendeter Anfragen in das neue anfragende Erlebnis</a>
            <p>Um das Senden von Anfragen zu vereinfachen, haben wir die Möglichkeit hinzugefügt, Anfragen in das neue anfordernde Erlebnis zu kopieren. Jetzt können Sie eine Anfrage kopieren, alle Felder bearbeiten und als neue Anfrage senden. </p>
        </td>
        <td>Freitag, 20. November 2025</td>
        <td>Freitag, 11. Dezember 2025</td>
        <td>Freitag, 15. Januar 2026</td>
    </tr>    
  </tbody>
</table>

### Weitere Verbesserungen

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Funktion</strong>
        </td>
        <td><strong>Vorschau</strong></td>
        <td><strong>Schnelle Veröffentlichung</strong></td>
        <td><strong>Vierteljährlich</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Updates im ersten Quartal 2026</a>
                        <p>Geringfügige Aktualisierungen des Erscheinungsbilds verschiedener Bereiche der Adobe Workfront-Anwendung werden innerhalb des Zeitrahmens der Version vom ersten Quartal 2026 vorgenommen. </p>
                    </td>
                    <td><p>Im gesamten Zeitrahmen des ersten Quartals 2026<br /></p>
                    <td colspan="2"><p>Schnellfreigabe: Mindestens 1 Woche nach der Freigabe für die Vorschau (sofern nicht anders angegeben)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Auswahlbeschränkungen für Felder mit Mehrfachauswahl</a>
              <p>Felder, die mehrere Auswahlmöglichkeiten zulassen, z. B. Kontrollkästchen und Mehrfachauswahl-Dropdown-Listen, sind jetzt auf 5.000 Auswahlmöglichkeiten beschränkt, wenn ein Benutzer das Formular ausfüllt.</p>
             </td>
        <td>Freitag, 30. Oktober 2025</td>
        <td>Freitag, 13. November 2025</td>
        <td>Freitag, 15. Januar 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Einheitliches Adobe-Erlebnis jetzt für mehr Workfront-Organisationen verfügbar</a><p></p>
            <p>Um Unternehmen den Zugriff auf die Vorteile von Adobe Unified Experience zu ermöglichen, stellen wir es bestehenden Workfront-Kunden weiterhin zur Verfügung.</p>
        </td>
        <td><p>Freitag, 11. Dezember 2025</p></td>
        <td><p>Donnerstag, 11. Februar 2026</p></td>
        <td><p>Donnerstag, 11. Februar 2026</p></td>
    <tr>
            </tbody>
        </table>


### Funktion wird bald aus Workfront entfernt

#### Abwertung der Überschreibungswährung für Aufgabengebiete mit der Version 25.11

Im Rahmen der Vereinfachung des Finanzmodells werden wir die Überschreibungswährung für Aufgabengebiete in der Vorschau am 30. Oktober und in der Produktion für alle Kunden mit der Version 25.11 einstellen. Diese Änderung wirkt sich darauf aus, wie Währungen und Kurse für Aufgabengebiete im Bereich „Setup“ konfiguriert werden.

* Die **Währung überschreiben** Felder in einem Aufgabengebiet sind nicht mehr verfügbar.
* Jedes Aufgabengebiet hat eine einzige Währung mit den zugehörigen Kosten und dem zugehörigen Abrechnungssatz.
* Alle vorhandenen Überschreibungswährungen und ihre Kurswerte werden automatisch migriert, um die einzige Währung und Kurse für dieses Aufgabengebiet zu werden.

## Modernisierung der Benutzeroberfläche

Wir aktualisieren die Benutzeroberfläche in Adobe Workfront, um das Benutzererlebnis zu verbessern und es mit anderen Adobe-Programmen zu vereinheitlichen. Diese Änderungen werden außerhalb des standardmäßigen Veröffentlichungszeitplans veröffentlicht. Eine Liste dieser Änderungen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Versionshinweise für andere Bereiche

### Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktionsumgebung in einem zeitlichen Abstand außerhalb des standardmäßigen Veröffentlichungszeitplans verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Workfront-Planungsverbesserungen

Neue Funktionen in Workfront Planning sind in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2026](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Für Folgendes gibt es derzeit keine Aktualisierungen in der Version:

* Szenarienplaner
* Korrekturabzug
* Ziele

## Aktualisierungen der Desktop Proofing Viewer

### Version 2.1.54

**Produktionsversion für alle Kunden: 11. Dezember 2025**

Desktop Proofing Viewer wurde von 2.1.52 auf 2.1.54 aktualisiert. Diese Aktualisierung umfasste interne Tooling-Aktualisierungen und hatte keine Auswirkungen auf die Endbenutzerfunktionalität.

Die Version 2.1.53 enthielt auch interne Werkzeugänderungen.

Dieses Update ist sowohl für Mac als auch für Windows.

### Version 2.1.52

**Produktionsversion für alle Kunden: 31. Juli 2025**

Der Desktop Proofing Viewer wurde auf Version 2.1.52 aktualisiert, welche Fehlerkorrekturen behandelt.

Die Aktualisierung vom 2.1.51 umfasste interne Tooling-Aktualisierungen und hatte keine Auswirkungen auf die Endbenutzerfunktionalität.

Dieses Update ist sowohl für Mac als auch für Windows.

## Ankündigungen

### API-Version 21

Workfront API Version 21 wurde am 23. Oktober 2025 veröffentlicht. Für API-Version 21 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

>[!IMPORTANT]
>
>Diese API-Versionsänderung beinhaltet eine grundlegende Änderung, die sich auf Ihre vorhandenen API-Aufrufe auswirken kann. Dies liegt daran, dass die API-Version 21 die Ereignisabonnements-Version 2 verwendet.
>
> Bei Feldern mit Mehrfachauswahl werden Ereignisabonnements in Version 2 immer als Array gesendet. Version 1 hat ein Array gesendet, wenn mehr als ein Wert ausgewählt ist. Wenn nur ein Wert ausgewählt war, wurde eine Zeichenfolge gesendet.

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 21](/help/quicksilver/wf-api/api/new-api-version-21.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Neue Version von Workfront für Microsoft Teams

Da [Microsoft auf den neuen Teams-Client umstellt](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) ist der Classic Teams-Client nach dem 1. Juli 2025 nicht mehr verfügbar. Um Microsoft Teams und integrierte Apps wie Workfront weiterhin verwenden zu können, müssen Kunden vor diesem Datum zum neuen Teams-Client wechseln.

Die aktualisierte Workfront-Integration ist jetzt verfügbar und vollständig mit der neuen Team-Erfahrung kompatibel. In den meisten Fällen wird Workfront automatisch angezeigt, sobald Benutzende den Wechsel vollzogen haben. Ist dies nicht der Fall, kann die Integration manuell über die Microsoft Teams App Store installiert werden. Informationen zum Installieren oder Überprüfen der Workfront-Integration im neuen Team-Client finden Sie unter [Installieren [!DNL Adobe Workfront]  für Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront für Microsoft Outlook

[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.

* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**

Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**

### Andere Workfront-Integrationsübergänge

Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses werden die folgenden Integrationen nach dem 28. **2026 nicht mehr**:

* Workfront für G Suite
* Workfront für Jira
* Workfront für Salesforce.

Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Google Workspace zu verwenden.
Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die im ersten Quartal 2025 durchgeführt wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie im Abschnitt Neue Funktionen auf der Seite [Workfront-Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=de).
