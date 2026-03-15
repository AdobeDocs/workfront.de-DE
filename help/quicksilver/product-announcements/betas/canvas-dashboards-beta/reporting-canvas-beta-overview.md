---
content-type: reference
navigation-topic: betas
title: 'Reporting-Arbeitsfläche - Betaversion: Übersicht'
description: Informationen zum Beta-Programm des kommenden Reporting-Canvas-Tools für Adobe Workfront
author: Courtney
feature: Product Announcements
hidefromtoc: true
hide: true
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 3%

---

# Reporting-Arbeitsfläche - Betaversion: Übersicht

## Reporting-Arbeitsfläche

Das neue Arbeitsflächen-Tool für Berichte in Workfront befindet sich derzeit in der Entwicklung. Bei der Gestaltung der Reporting-Arbeitsfläche haben wir uns sehr darum bemüht, ein Erlebnis bereitzustellen, das maximale Flexibilität in Kombination mit einem intuitiven, modularen Design bietet, sodass Benutzer wie Sie Ihre eigenen Daten am effektivsten bei der Erstellung und Freigabe von Berichten nutzen können. Durch einen neuen, einheitlichen Berichtstyp, mit dem Sie nahezu jedes Element auf eine unbegrenzte Arbeitsfläche ziehen und ablegen können, wird die Erstellung eines visuellen Daten-Meisterwerks bald einfacher sein als je zuvor.

Dieser Artikel enthält Informationen zur aktuellen privaten Beta-Version, die auf bestimmte Kunden beschränkt ist. Neue Funktionen der Reporting-Arbeitsfläche werden jetzt über Arbeitsflächen-Dashboards bereitgestellt. Weitere Informationen finden **im** „Entwicklungsplan“.

### Entwicklungsplan

Wir befinden uns in der letzten Phase der Behebung eines Datenqualitätsproblems, das wir am Anfang der Beta-Phase der Reporting-Arbeitsfläche beobachtet haben. Wir werden bald unsere Arbeit fortsetzen, um neue Visualisierungen bereitzustellen, die Auswahl an berichtspflichtigen Workfront-Objekten zu erweitern und die Berichterstellung und -verteilung zu verbessern, die alle von entscheidender Bedeutung für die Verwirklichung unserer Ziele für die Reporting-Arbeitsfläche sind.

Wir stellen diese neuen Erlebnisse schrittweise bereit, beginnend mit Version 23.2, über die neue Seite „Canvas-Dashboards“, die jetzt in Ihrer Vorschau-Umgebung verfügbar ist. Mit Canvas-Dashboards können Sie vorhandene Berichte neben den neuen Berichtsfunktionen anzeigen, die wir gerade erstellen. Sie dienen als primäre Umgebung für die Bereitstellung und das Testen neuer Funktionen für Reporting Canvas. Weitere Informationen zur Aktivierung und Verwendung von Arbeitsflächen-Dashboards finden Sie unter [Arbeitsflächen-Dashboards - Übersicht](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Beta-Version testen

>[!IMPORTANT]
>
>Die unten stehenden Beta-Informationen gelten für Administratoren, die bereits in die Beta-Version der Berichtscanvas aufgenommen wurden, in der keine neuen Teilnehmer mehr akzeptiert werden. Wenn Sie neue Funktionen von Reporting Canvas testen möchten, während diese hinzugefügt werden, finden Sie unter **Entwicklungsplan** oben weitere Informationen zum Aktivieren von Canvas-Dashboards.

### Verfügbarkeit

Die Beta-Version der Reporting-Arbeitsfläche steht allen Organisationen zur Verfügung, die sich in AWS befinden, unabhängig von der Region.

### Beta-Version

Die Beta-Version der Reporting-Arbeitsfläche ist vollständig optional, kann jedoch nur von einem Workfront-Administrator aktiviert werden. So melden Sie sich als Systemadministrator an:

1. Wählen Sie **Hauptmenü Ihrer Workfront-Instanz das Symbol** Reporting (Betaversion) aus.
1. Klicken Sie **Akzeptieren**, um die Nutzungsbedingungen zu akzeptieren.
1. Zulassen, dass die Daten Ihres Unternehmens zur Reporting-Arbeitsfläche hinzugefügt werden (dies kann bis zu einigen Stunden dauern).
1. Beginnen Sie mit der Verwendung der Reporting-Arbeitsfläche.

Nachdem die Daten Ihrer Organisation zur Reporting-Arbeitsfläche hinzugefügt wurden, können andere Systemadministratoren auf die gleiche Weise einzeln beitreten (ohne darauf zu warten, dass die Daten erneut hinzugefügt werden).

Opt-in für andere Benutzende, die keine Workfront-Administratoren sind:

1. Wählen Sie **Hauptmenü Ihrer Workfront-Instanz das Symbol** Reporting (Betaversion) aus.
1. Klicken Sie auf **Berichterstellungs-Arbeitsfläche - Berechtigungen**.
1. Suchen Sie nach den Benutzern, an denen Sie teilnehmen möchten, und wählen Sie sie aus.

   >[!IMPORTANT]
   >
   >Benutzer, denen Sie Zugriff auf die Reporting-Arbeitsfläche gewähren, haben unabhängig von ihren Standardberechtigungen zum Anzeigen **Daten** schreibgeschützt Zugriff auf alle Daten im System.

1. Klicken Sie auf **Speichern**.
1. Fügen Sie das Symbol **Reporting (Betaversion** in die Haupt-Layout-Vorlage jedes ausgewählten Benutzers ein. Weitere Informationen finden Sie unter [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Jeder Benutzer muss dann einzeln zum Symbol **Reporting (Betaversion)** im Hauptmenü navigieren und die Nutzungsbedingungen akzeptieren.

### Feedback senden

So senden Sie Feedback zur Beta-Version:

1. Klicken Sie auf der Berichtsarbeitsfläche in Workfront auf die Schaltfläche **Feedback senden**.
1. Füllen Sie das Formular aus, und klicken Sie dann auf **Senden**.

## Häufige Fragen zu Beta

+++Kann ich meine alten Berichte zur Reporting-Arbeitsfläche migrieren?

Kurz gesagt: Die Migration veralteter Berichte wird während der Beta-Phase nicht verfügbar sein. Es ist jedoch eine geplante Funktion (mit einigen Einschränkungen, die unten beschrieben werden) für den offiziellen Launch.

Auch wenn die Barriere für die Erstellung neuer Berichte durch die Reporting-Arbeitsfläche erheblich gesenkt wurde, wissen wir, dass die Übertragung einiger Ihrer vorhandenen Berichte und Dashboards dazu beitragen wird, den Annahmeprozess zu beschleunigen. Daher möchten wir die Tools und Ressourcen bereitstellen, die erforderlich sind, um sicherzustellen, dass Sie alle relevanten Legacy-Elemente übernehmen können, um sicherzustellen, dass Sie auf der Reporting-Arbeitsfläche mit dem richtigen Fuß beginnen. Da die Reporting-Arbeitsfläche eine so radikale Änderung der Funktionsweise des aktuellen Reportings darstellt, wäre es jedoch unmöglich, jeden Bericht oder jedes Dashboard genau so zu migrieren, wie es heute ist.

Unsere aktuelle Migrationsstrategie in den offiziellen -Versionen ermöglicht Ihnen Folgendes:

1. Relevante Berichte und Dashboards identifizieren

   1. Ermöglicht den Export einer CSV-Datei aller Berichte und Dashboards im System zusammen mit allen relevanten Tracking-Informationen (Anzahl der Ansichten, Zeitpunkt und von wem).
   1. Export von Berichten, die mit terminierten Sendungen eingerichtet wurden, zusammen mit den Empfängern bereitstellen

1. Wählen Sie die zu migrierenden Berichte und Dashboards aus und klicken Sie auf **Migrieren**

   Dies ist eine Einwegmigration. Dadurch wird eine Kopie der ausgewählten Berichte und Dashboards in die Reporting-Arbeitsfläche erstellt, sodass der alte Bericht oder das alte Dashboard im aktuellen Reporting-Tool intakt bleibt.

   Sie können denselben Bericht oder dasselbe Dashboard beliebig oft migrieren.

1. Stellen Sie in Reporting Canvas sicher, dass alle ausgewählten Berichte und Dashboards migriert wurden.
+++

+++Warum kann ich nicht alle Objekte sehen, die ich normalerweise mache?

Um unseren Kunden die Beta-Version so früh wie möglich zur Verfügung zu stellen, haben wir sie nur mit einer Untergruppe der vielen Objekttypen veröffentlicht, die heute in Workfront verfügbar sind. Im Folgenden sind die derzeit in der Beta-Version unterstützten Objekttypen aufgeführt:

* Zuweisung
* Dokument
* Dokumentengenehmigung
* Ausgabe
* Stunde
* Problem
* Notiz
* Portfolio
* Projekt
* Programm
* Aufgabe
* Arbeitszeittabelle
* Arbeitselement
+++

+++Wenn während der Beta-Phase auf der Reporting-Arbeitsfläche ein Fehler auftritt, sind dann die Daten meiner Organisation betroffen?

Nein. Die Beta-Version verwendet eine Kopie der Daten Ihrer Organisation, die in die Reporting-Arbeitsfläche eingefügt wird. Das bedeutet, dass Sie zwar während der Beta-Phase sicher experimentieren können, ohne das Risiko, dass sich dies auf wichtige Daten auswirkt, es bedeutet aber auch, dass die Inline-Bearbeitung von Daten auf der Reporting-Arbeitsfläche bis zum offiziellen Start nicht verfügbar ist.
+++

+++Kann ich die Beta-Version deaktivieren, sobald ich Mitglied bin?

Ein Workfront-Administrator kann die Beta-Version nicht deaktivieren. Dagegen können Nicht-Systemadministratoren wie folgt entfernt werden:

1. Melden Sie sich als Systemadministrator an.
1. Navigieren Sie zu Berichtsarbeitsfläche.
1. Klicken Sie auf Berichtsarbeitsfläche **Berechtigungen**.
1. Entfernen Sie die Benutzer, die Sie aus der Beta-Version ausschließen möchten, aus der Liste, die angemeldet wurden.
1. Klicken Sie auf **Speichern**.
+++
