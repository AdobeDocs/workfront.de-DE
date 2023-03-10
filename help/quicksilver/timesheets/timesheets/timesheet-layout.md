---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: Grundlegendes zum Layout des Zeitplans
description: In diesem Artikel wird das Layout von Timesheets in Adobe Workfront beschrieben, sodass Sie besser verstehen können, wie Sie Timesheets zur Aufzeichnung der Zeit anpassen und nutzen können.
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: ca552b80e9d78fd09068d72479e1b2bddc596c70
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 1%

---

# Grundlegendes zum Layout des Zeitplans

In diesem Artikel wird das Layout von Timesheets in Adobe Workfront beschrieben, sodass Sie besser verstehen können, wie Sie Timesheets zur Aufzeichnung der Zeit anpassen und nutzen können.

Das Timesheet und die Voreinstellungen zur Stunde steuern, was auf einem Timesheet angezeigt wird. Dieser Artikel bietet einen Überblick über alle verfügbaren Optionen. Weitere Informationen finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen zum Protokollieren der Zeit in einem Zeitblatt finden Sie unter [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md).

![Datenblatt-Layout](assets/timesheet-layout-unshimmed.png)

Im Folgenden finden Sie die Bereiche eines Zeitplans:

* [Header des Datenblatts](#timesheet-header)
* [Das linke Bedienfeld](#the-left-panel)
* [Arbeitselemente](#work-items)
* [Symbolleiste](#toolbar)
* [Fußzeile des Datenblatts](#timesheet-footer)
* [Auftragsrolle](#job-role)
* [Stundentyp](#hour-type)
* [Aktualisierungsbereich im linken Bereich](#updates-area-in-the-left-panel)
* [Zusammenfassungsbereich](#summary-panel)
* [Zeitrahmen und Einstiegsbereich für Stunde](#time-frame-and-hour-entry-area)
* [Kommentare zu stündlichen Einträgen](#hour-entry-comments)
* [Stunden](#hours)
* [Gesamtwerte](#totals)

## Header des Datenblatts

![](assets/timesheet-title-unshimmed-redesign.png)

Der Header des Zeitplans enthält folgende Informationen:

* Der Zeitrahmen des Zeitplans.
* Der Bereich Aktionen , der Folgendes umfasst:
   * Ein Sternsymbol, mit dem Sie die Timesheets zu Ihrer Favoritenliste hinzufügen können.
   * Klicken Sie auf das Symbol Mehr mit der Option Löschen , über das Sie das Zeitblatt löschen können.
* Der Name des Eigentümers des Zeitblatts.
* Die Gesamtzahl der Stunden für die protokollierten Elemente, die im Timesheet angezeigt werden.
* Die Anzahl der Überstunden. Dies ist ein manueller Eintrag und nur sichtbar, wenn die Variable **Überstunden** -Einstellung auf einem Timesheet aktiviert ist. Weitere Informationen finden Sie unter [Timesheet-Informationen bearbeiten](../create-and-manage-timesheets/edit-timesheets.md).

>[!TIP]
>
>Es ist nicht möglich, eine größere Anzahl von Überstunden als die aktuellen Gesamtstunden auf dem Zeitblatt zu protokollieren. Wenn Sie beispielsweise bisher 7 Stunden auf dem Timesheet angemeldet haben, können Sie keine 8 Stunden Überstunden protokollieren.


* Der Status des Zeitplans.

## Das linke Bedienfeld

![](assets/timesheet-left-panel-unshimmed-redesign.png)

Sie können auf die folgenden Abschnitte im linken Bereich zugreifen:

* **Datenblatt**: Zeigt das tatsächliche Timesheet an.
* **Updates**: Zeigt Kommentare und Systemaktualisierungen zum Timesheet an. Weitere Informationen finden Sie unter [Aktualisierungsbereich im linken Bereich](#updates-area-in-the-left-panel) in diesem Artikel.

## Arbeitselemente

![](assets/timesheet-object-names-unshimmed-redesign.png)

Die Arbeitselemente sind die Projekte, Aufgaben und Probleme, für die Sie die Zeit protokollieren möchten. Durch Klicken auf den nach unten zeigenden Pfeil in der Kopfzeile werden die Projekte sowie die darunter aufgeführten Aufgaben und Probleme ausgeblendet. Durch Klicken auf den nach unten zeigenden Pfeil neben dem Namen eines Projekts werden die Arbeitselemente für dieses Projekt ausgeblendet.

Aufgaben, Probleme und Projekte, bei denen die Zeit außerhalb des Zeitplans aufgezeichnet wird, oder im Zeitrahmen des Zeitplans geplante Elemente werden hier automatisch angezeigt.

## Symbolleiste

![](assets/timesheet-toolbar-unshimmed-redesign.png)

Die Symbolleiste enthält die folgenden Optionen:

* Schaltfläche Element hinzufügen , über die Sie Projekte, Aufgaben oder Probleme hinzufügen können.
* Über das Schnellfiltersymbol können Sie nach Aufgaben oder Problemen im Timesheet suchen.
* Die **Kommentare anzeigen** -Einstellung, mit der Sie Stundenkommentare anzeigen oder ausblenden können, die für Projekt-, Aufgaben- oder Problemstundeneinträge protokolliert werden.
* Vollbildsymbol, über das Sie das Timesheet im Vollbildmodus anzeigen können.
* **Zusammenfassung öffnen** (oder **Zusammenfassung schließen**), über die Sie das Bedienfeld &quot;Zusammenfassung&quot;öffnen oder schließen können, um zusätzliche Informationen zu Aufgaben oder Problemen anzuzeigen. Dies ist nicht für Projekte verfügbar.

Weitere Informationen finden Sie unter [Protokollzeit](../create-and-manage-timesheets/log-time.md).

## Fußzeile des Datenblatts

![](assets/timesheet-footer-unshimmed-redesign.png)

Sie können in diesem Bereich auf die Schaltflächen Zur Genehmigung senden, Schließen, Genehmigen und Ablehnen klicken, um die Genehmigung eines Zeitblatts zu schließen oder abzulehnen.

Dieser Bereich enthält auch Informationen darüber, wann das Timesheet zuletzt gespeichert wurde. Alle Änderungen, die Sie an den Informationen im Timesheet vornehmen, werden automatisch gespeichert.

## Aufgabengebiet

![](assets/timesheet-job-role-area-unshimmed-redesign.png)

Sie können eine andere Auftragsrolle auswählen, um sie den Stundeneinträgen zuzuordnen. Ihr Workfront-Administrator muss die manuelle Einstellung &quot;Auftragsrollen für Stundeneinträge zuweisen&quot;aktivieren. Die bei der Zuweisung zur Aufgabe angegebene Auftragrolle bzw. das Problem wird standardmäßig angezeigt. Wenn Ihnen für die Aufgabe oder das Problem keine Rolle zugewiesen wurde, wird Ihre Primäre Rolle als Standard angezeigt. Weitere Informationen finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Sie können mehrere Stundeneinträge für dasselbe Arbeitselement für verschiedene Rollen protokollieren. Weitere Informationen finden Sie unter [Protokollzeit](../create-and-manage-timesheets/log-time.md).

## Stundentyp

![](assets/timesheet-hour-type-unshimmed-redesign.png)

Sie können für jedes Element verschiedene Stundentypen auswählen, die mit Ihren Stundeneinträgen verknüpft werden sollen. Dieses Feld wird nur angezeigt, wenn der Workfront-Administrator es für Ihre Umgebung aktiviert hat. Weitere Informationen finden Sie im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Sie können mehrere Stundeneinträge für dasselbe Arbeitselement für verschiedene Stundentypen protokollieren. Weitere Informationen finden Sie unter [Protokollzeit](../create-and-manage-timesheets/log-time.md).

## Aktualisierungsbereich im linken Bereich

![](assets/timesheet-updates-section-unshimmed-redesign.png)

Im Abschnitt Updates im linken Bereich können Sie Kommentare zu einem Timesheet abgeben, um mit Ihren Timesheet-Genehmigern oder anderen Benutzern zu kommunizieren.

Alle auf dem Zeitblatt abgegebenen Kommentare werden in diesem Bereich am Ende des Zeitplans angezeigt. Dieser Bereich wird unter dem Timesheet und über der Fußzeile des Zeitblatts angezeigt. Weitere Informationen finden Sie unter [Anzeigen und Verwalten von Kommentaren auf einem Timesheet](../create-and-manage-timesheets/view-and-manage-comments-timesheets.md).

## Zusammenfassungsbereich

![](assets/timesheet-summary-panel-for-task-unshimmed-redesign.png)

Sie können Kommentare zum Zugriff auf das Bedienfeld &quot;Zusammenfassung&quot;für Aufgaben oder Probleme in einem Timesheet erstellen. Hier können Sie sich zu Aufgaben und Problemen äußern oder deren Informationen aktualisieren. Weitere Informationen finden Sie unter [Zusammenfassungsübersicht](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Die Kommentare, die Sie für Arbeitselemente im Bereich &quot;Zeitblatt-Zusammenfassung&quot;eingeben, werden im Bereich &quot;Updates&quot;der Aufgabe oder des Problems angezeigt. Das Bedienfeld Zusammenfassung ist nicht für Projekte verfügbar.

## Zeitrahmen und Einstiegsbereich für Stunde

![](assets/timesheet-time-frame-log-time-area.png)

Der Zeitrahmen des Zeitplans wird rechts neben den Arbeitselementen angezeigt.

Sie können Timesheets für eine, zwei oder vier Wochen erstellen.

Der Zeitrahmen wird in vollen Wochenschritten angezeigt. Tage außerhalb des angegebenen Zeitrahmens werden abgeblendet angezeigt. Sie können die Zeit nicht für Tage protokollieren, die außerhalb des Zeitrahmens des Zeitblatts liegen.

Weitere Informationen finden Sie unter [Einmaliges Erstellen eines Timesheets](../create-and-manage-timesheets/create-tmshts.md) oder [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../create-and-manage-timesheets/create-timesheet-profiles.md).

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## Kommentare zu stündlichen Einträgen

![](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

Sie können einen Kommentar für jeden Stundeneintrag hinzufügen, den Sie zu Ihrem Timesheet hinzufügen.

Die Kommentare, die Sie in das Kommentarfeld für die Stundeneingabe eingeben, werden im Timesheet unter jedem Arbeitselement angezeigt, bei dem Sie die Uhrzeit der **Kommentare anzeigen** in der Symbolleiste aktiviert ist.

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## Stunden

![](assets/timesheet-hours-area-unshimmed-redesign.png)

Das Timesheet enthält Eingabefelder für jedes Arbeitselement und jeden Tag des Zeitblattes, um die mit der Bearbeitung des Artikels verbrachte Zeit aufzuzeichnen. Während Sie die Zeit protokollieren, wird das Element, das Sie die Zeit für Highlights in hellblau protokollieren, und das Stundenfeld in dunkelblau dargestellt.

## Gesamtwerte

![](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

Überprüfen Sie die Summe aller Stunden, die auf dem Timesheet eingegeben wurden, zusammengefasst nach Tag (in der Kopfzeile des Timesheets) sowie nach Objekt (in der letzten Spalte).
