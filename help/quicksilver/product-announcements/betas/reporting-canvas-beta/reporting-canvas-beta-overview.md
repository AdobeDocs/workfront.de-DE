---
content-type: reference
navigation-topic: betas
title: '"Reporting Canvas beta: overview'''
description: Informationen zum Betaprogramm für das bevorstehende Tool zur Berichtsarbeitsfläche für Adobe Workfront
author: Nolan
feature: Product Announcements
exl-id: cc0adf28-08ab-4330-b901-219ab687f02f
source-git-commit: d738ef3f6642d5b1a646f58896575a2971bbc06a
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# Reporting-Arbeitsfläche - Beta: Übersicht

## Berichtsarbeitsfläche

Eine komplette Neuerung der Berichterstellung in Workfront, dem neuen Tool für die Berichtsarbeitsfläche, befindet sich derzeit in der Entwicklung. Bei der Erstellung von Reporting-Arbeitsflächen haben wir hart daran gearbeitet, ein Erlebnis zu bieten, das maximale Flexibilität bietet, verbunden mit einem intuitiven, modularen Design, sodass Benutzer wie Sie Ihre eigenen Daten am effektivsten für die Erstellung und Freigabe von Berichten nutzen können. Durch einen neuen, einheitlichen Berichtstyp, mit dem Sie nahezu jedes Element auf eine grenzenlose Arbeitsfläche ziehen und ablegen können, wird die Erstellung eines visuellen Daten-Master-Elements bald einfacher denn je sein.

Dieser Artikel enthält Informationen zur aktuellen privaten Beta-Version, die auf bestimmte Kunden beschränkt ist. Neue Reporting-Arbeitsflächenfunktionen werden jetzt über Canvas-Dashboards bereitgestellt. Siehe **Entwicklungsplan** unten finden Sie weitere Informationen.

### Entwicklungsplan

Wir befinden uns in der letzten Phase der Lösung eines Problems mit der Datenqualität, das wir frühzeitig in der Beta-Phase der Reporting-Arbeitsfläche beobachtet haben. Wir werden in Kürze die Arbeit fortsetzen, um neue Visualisierungen bereitzustellen, die Auswahl der berichtspflichtigen Workfront-Objekte zu erweitern und die Erlebnisse bei der Berichterstellung und -verteilung zu verbessern, die allesamt von zentraler Bedeutung für die Erreichung unserer Ziele für die Reporting-Arbeitsfläche sind.

Wir werden diese neuen Erlebnisse schrittweise bereitstellen, beginnend mit Version 23.2, über die neue Seite &quot;Canvas-Dashboards&quot;, die jetzt in Ihrer Vorschau-Umgebung verfügbar ist. Mit Leinwanddashboards können Sie neben den neuen, von uns erstellten Berichtsfunktionen vorhandene Berichte anzeigen. Diese Funktion dient als primäre Umgebung für die Bereitstellung und Prüfung neuer Funktionen für die Berichtarbeitsfläche. Weitere Informationen zum Aktivieren und Verwenden von Canvas-Dashboards finden Sie unter [Übersicht über Canvas-Dashboards](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Beta-Teilnahme

>[!IMPORTANT]
>
>Die unten stehenden Beta-Informationen richten sich an Administratoren, die bereits in der Beta-Version der Reporting-Arbeitsfläche enthalten waren und keine neuen Teilnehmer mehr akzeptieren. Wenn Sie neue Funktionen der Reporting-Arbeitsfläche testen möchten, während sie hinzugefügt werden, lesen Sie **Entwicklungsplan** Informationen zum Aktivieren von Canvas-Dashboards.

### Verfügbarkeit

Die Beta-Version der Reporting-Arbeitsfläche steht allen Unternehmen in AWS zur Verfügung, unabhängig von der Region.

### Betaversion

Die Beta-Version der Reporting-Arbeitsfläche ist vollständig optional, kann jedoch nur von einem Workfront-Administrator aktiviert werden. So melden Sie sich als Systemadministrator an:

1. Wählen Sie die **Berichterstellung (Beta)** im Hauptmenü Ihrer Workfront-Instanz.
1. Klicken **Accept** um die Bedingungen zu akzeptieren.
1. Lassen Sie zu, dass die Daten Ihres Unternehmens der Berichtsarbeitsfläche hinzugefügt werden (dies kann bis zu einigen Stunden dauern).
1. Verwendung der Berichtsarbeitsfläche.

Nachdem die Daten Ihres Unternehmens der Arbeitsfläche für die Berichterstellung hinzugefügt wurden, können andere Systemadministratoren auf die gleiche Weise individuelle Zugriffe auswählen (ohne darauf zu warten, dass die Daten erneut hinzugefügt werden).

So aktivieren Sie andere Benutzer, die keine Workfront-Administratoren sind:

1. Wählen Sie die **Berichterstellung (Beta)** im Hauptmenü Ihrer Workfront-Instanz.
1. Klicken Sie auf **Berechtigungen für die Berichterstellung**.
1. Suchen Sie nach bestimmten Benutzern, die Sie teilnehmen möchten, und wählen Sie sie aus.

   >[!IMPORTANT]
   >
   >Benutzer, denen Sie Zugriff auf die Berichtarbeitsfläche gewähren, haben Zugriff auf **all** -Daten im System schreibgeschützt sind, unabhängig von den Standardberechtigungen zur Anzeige dieser Daten.

1. Klicken Sie auf **Speichern**.
1. Fügen Sie die **Berichterstellung (Beta)** in die Vorlage für das Hauptlayout jedes ausgewählten Benutzers ein. Weitere Informationen finden Sie unter [Hauptmenü mithilfe einer Layoutvorlage anpassen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Jeder Benutzer muss dann einzeln zur **Berichterstellung (Beta)** in ihrem Hauptmenü und akzeptieren Sie die Bedingungen.

### Feedback senden

So senden Sie Feedback zur Beta:

1. Klicken Sie auf der Reporting-Arbeitsfläche in Workfront auf die **Feedback senden** Schaltfläche.
1. Füllen Sie das Formular aus und klicken Sie auf **Einsenden**.

## Häufig gestellte Fragen zu Beta

++ Kann ich meine alten Berichte auf die Berichtarbeitsfläche migrieren?

Kurz gesagt, die Migration von Legacy-Berichten ist während der Beta-Phase nicht verfügbar. Es handelt sich jedoch um eine geplante Funktion (mit einigen unten beschriebenen Einschränkungen) für den offiziellen Start.

Die Hürde zum Erstellen neuer Berichte wurde mit der Berichtsarbeitsfläche zwar erheblich verringert, wir wissen jedoch, dass die Übernahme einiger Ihrer vorhandenen Berichte und Dashboards den Adoptionsvorgang beschleunigen wird. Daher möchten wir die erforderlichen Tools und Ressourcen bereitstellen, um sicherzustellen, dass Sie alle relevanten Legacy-Elemente übernehmen können, um sicherzustellen, dass Sie in der Reporting-Arbeitsfläche auf dem richtigen Fuß beginnen. Da die Berichtsarbeitsfläche eine derart radikale Änderung an der Funktionsweise der aktuellen Berichterstellung darstellt, wäre es jedoch nicht möglich, jeden Bericht oder jedes Dashboard genau so zu migrieren, wie es heute der Fall ist.

Unsere aktuelle Migrationsstrategie in der offiziellen Version ermöglicht Ihnen Folgendes:

1. Relevante Berichte und Dashboards identifizieren

   1. Sie erhalten die Möglichkeit, eine CSV-Datei mit allen Berichten und Dashboards im System zusammen mit allen relevanten Tracking-Informationen zu exportieren (Anzahl der Ansichten, wann und von wem).
   1. Erstellen Sie einen Export von Berichten, die mit geplanten Sendungen mit den Empfängern eingerichtet wurden.

1. Wählen Sie die Berichte und Dashboards aus, die Sie migrieren möchten, und klicken Sie dann auf **Migrieren**

   Dies ist eine einmalige Migration. Es wird eine Kopie der ausgewählten Berichte und Dashboards auf die Berichtsarbeitsfläche erstellt, sodass der alte Bericht oder das Dashboard im aktuellen Reporting-Tool intakt bleiben.

   Sie können denselben Bericht oder dasselbe Dashboard beliebig oft migrieren.

1. Stellen Sie sicher, dass in der Berichtsarbeitsfläche alle ausgewählten Berichte und Dashboards migriert wurden.
+++

+++ Warum kann ich nicht alle Objekte sehen, die ich normalerweise mache?

Um unseren Kunden die Beta so früh wie möglich bereitzustellen, haben wir sie nur mit einer Untergruppe der vielen Objekttypen veröffentlicht, die heute in Workfront verfügbar sind. Nachfolgend finden Sie die Objekttypen, die derzeit in der Beta-Version unterstützt werden:

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

+++ Wenn während der Beta-Phase in der Arbeitsfläche für die Berichterstellung etwas schiefgeht, werden dann die Daten meiner Organisation betroffen sein?

Nein. Die Beta-Version verwendet eine Kopie der Daten Ihres Unternehmens, die in die Arbeitsfläche für die Berichterstellung eingetragen sind. Dies bedeutet zwar, dass Sie während der Beta-Phase sicher experimentieren können, ohne dass die Gefahr besteht, dass wichtige Daten beeinträchtigt werden. Gleichzeitig bedeutet dies, dass die Inline-Bearbeitung von Daten in der Reporting-Arbeitsfläche bis zum offiziellen Start nicht verfügbar sein wird.
+++

+++ Kann ich mich von der Beta-Version abmelden, nachdem ich beigetreten bin?

Ein Workfront-Administrator kann die Beta-Version nicht abwählen. Nicht-systembasierte Administratoren können jedoch wie folgt entfernt werden:

1. Melden Sie sich als Systemadministrator an.
1. Navigieren Sie zur Berichtsarbeitsfläche.
1. Klicken Sie auf Berichtsarbeitsfläche . **Berechtigungen**.
1. Entfernen Sie die Benutzer, die Sie aus der Beta-Liste ausschließen möchten, aus der Liste, für die Sie sich angemeldet haben.
1. Klicken Sie auf **Speichern**.
+++
