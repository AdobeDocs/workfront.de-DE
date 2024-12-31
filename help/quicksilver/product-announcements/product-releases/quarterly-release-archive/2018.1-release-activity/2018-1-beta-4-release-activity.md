---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 4 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2018.1 verfügbar waren. Die Funktion wurde am 24. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# Versionsaktivität von Beta 4 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2018.1 verfügbar waren. Die Funktion wurde am 24. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.1 finden Sie unter  Übersicht über die Versionsaktivität [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Version 2018.1 4 enthält Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Zeitpläne, die von Gruppenadministratoren verwaltet werden](#schedules-managed-by-group-administrators)

**Für alle Benutzer**

* [Proofing-Verbesserungen in Workfront](#proofing-improvements-within-workfront)
* [Erstellung von Korrekturabzügen in Workfront Proof - Verbessertes Benutzererlebnis und zusätzliche Funktionen](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Proofing-Verbesserungen in Workfront und Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Aktualisiertes Look-and-Feel mit Basecamp-Integration in Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Einfügen von Bildern in Workfront aus der Zwischenablage](#paste-images-to-workfront-from-the-clipboard)
* [Verbesserungen am Auslastungsbericht](#utilization-report-improvements)
* [Entfernen des Objekts „Ressource budgetiert Stunde“ aus Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Nutzungsstatistiken von Berichten](#report-usage-statistics)
* [Gantt-Diagramm - Aktualisierungen](#gantt-chart-updates)
* [Neuer Portfolio-Optimizer](#new-portfolio-optimizer)
* [Option „Budgetdatumsanpassung“ im Ressourcenplaner](#budget-date-adjustment-option-in-the-resource-planner)
* [Ressourcenplanung: Beschränken Sie Zuweisungen an Benutzer auf Grundlage der Gruppenmitgliedschaft](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Ressourcenplanung: Zuweisungen an Benutzer unabhängig von deren Rolle zulassen](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Emoji-Unterstützung](#emoji-support)

## Proofing-Verbesserungen in Workfront {#proofing-improvements-within-workfront}

Die folgenden Verbesserungen wurden an der Dokumentliste in Workfront vorgenommen: 

* [Testversandstatus in der Dokumentliste anzeigen](#view-proof-progress-from-the-document-list)
* [Neue Option zum Anzeigen der Druckzusammenfassung in der Dokumentliste](#new-option-to-view-the-print-summary-from-the-document-list)
* [Das Erscheinungsbild zum Erzeugen oder Öffnen des Korrekturabzugs über die Dokumentliste wurde aktualisiert](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Verschiedene Links wurden aus Dokumenten in der Dokumentliste entfernt](#various-links-removed-from-documents-on-the-document-list)
* [Dateinamen auf kombinierten Korrekturabzügen anzeigen](#view-file-names-on-combined-proofs)
* [Anzeigen der aktuellen aktiven Phase eines Korrekturabzugs in der Dokumentliste](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Anzeigen des Korrekturstatus in der Dokumentliste {#view-proof-progress-from-the-document-list}

In der Dokumentliste werden jetzt für alle Korrekturabzüge Fortschrittsanzeigen angezeigt. (Dazu gehören „Gesendet“, „Geöffnet“, „Kommentare abgegeben“ und „Entscheidung“.)

Vor dieser Änderung mussten Sie einen Korrekturabzug in der Dokumentliste auswählen, um den Fortschritt des Korrekturabzugs im rechten Bedienfeld anzuzeigen. 

Weitere Informationen finden Sie unter [Testversand-Fortschritt und Statusübersicht](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Neue Option zum Anzeigen der Druckzusammenfassung in der Dokumentliste {#new-option-to-view-the-print-summary-from-the-document-list}

Sie können jetzt die Druckzusammenfassung für einen Korrekturabzug direkt in der Dokumentliste anzeigen.

Vor dieser Änderung konnten Sie die Druckzusammenfassung nur über die Proofing-Anzeige anzeigen. 

Weitere Informationen zum Anzeigen der Druckzusammenfassung in der Dokumentliste finden Sie unter [Drucken einer Zusammenfassung eines Korrekturabzugs in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Das Erscheinungsbild zum Erzeugen oder Öffnen des Korrekturabzugs über die Dokumentliste wurde aktualisiert {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Wenn Sie nun den Mauszeiger über ein Dokument in der Dokumentliste bewegen, wurden die Optionen zum Generieren des Korrekturabzugs oder zum Öffnen des Korrekturabzugs aktualisiert. Diese Optionen sind jetzt auffälliger und werden als Schaltflächen angezeigt.

Vor dieser Änderung waren diese Optionen als Links unter dem Dokumentnamen verfügbar.

Weitere Informationen finden Sie in den folgenden Abschnitten:

* .
* in .

### Verschiedene Links wurden aus Dokumenten in der Dokumentliste entfernt {#various-links-removed-from-documents-on-the-document-list}

Die folgenden Aktionen sind nicht mehr als Links zu einzelnen Dokumenten in der Dokumentliste verfügbar:

* Korrekturabzug generieren
* Korrekturabzug
* Details
* Freigeben
* Auschecken/Einchecken

Die folgenden Aktionen sind jetzt als Schaltfläche für das Dokument in der Dokumentliste verfügbar:

* Korrekturabzug öffnen (verfügbar, nachdem der Korrekturabzug erstellt wurde) 
* Korrekturabzug erstellen (verfügbar, wenn der Korrekturabzug noch nicht generiert wurde)

Die folgenden Aktionen sind jetzt im Dropdown-Menü neben der Schaltfläche Korrekturabzug öffnen oder Korrekturabzug erstellen verfügbar:

* Korrekturabzug-Details
* Dokumentdetails
* Zusammenfassung drucken

Weitere Informationen finden Sie in den folgenden Abschnitten:

* .
* in .

### Anzeigen von Dateinamen bei kombinierten Korrekturabzügen {#view-file-names-on-combined-proofs}

Sie können jetzt die einzelnen Dateinamen anzeigen, aus denen ein kombinierter Korrekturabzug besteht. Diese Informationen werden auf der Registerkarte Details angezeigt, wenn der Korrekturabzug in der Dokumentliste ausgewählt wird.

Weitere Informationen finden Sie unter Anzeigen aller in einem kombinierten Korrekturabzug enthaltenen Dateien. 

### Anzeigen der aktuellen aktiven Phase eines Korrekturabzugs in der Dokumentliste {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Wenn Sie nun einen Korrekturabzug in der Dokumentliste auswählen, werden die aktuell aktiven Phasen in der rechten Spalte auf der Registerkarte Details angezeigt. 

Weitere Informationen finden Sie unter [Anzeigen aktiver Phasen eines Korrekturabzugs](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Erstellung von Korrekturabzügen in Workfront Proof - Verbessertes Benutzererlebnis und zusätzliche Funktionen {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Zusätzlich zu einem verbesserten Benutzererlebnis beim Erstellen von Korrekturabzügen in Workfront Proof sind jetzt die folgenden zusätzlichen Funktionen verfügbar:

* Zusammenführen mehrerer Bilder zu einem einzigen Korrekturabzug.
* Korrekturabzugs-Websites in mehreren Auflösungen (mehrere Auflösungen können als einzelne Korrekturabzüge erstellt oder zu einem einzigen Korrekturabzug kombiniert werden).
* Bearbeiten Sie den Dateinamen während des Upload-Vorgangs.
* Fügen Sie benutzerdefinierte Felder in das Formular zur Erstellung von Korrekturabzügen ein.
* Hinzufügen einer benutzerdefinierten Nachricht zu Korrekturabzugs-E-Mail-Benachrichtigungen.
* Zusätzliche Korrekturabzugseinstellungen 
* Echtzeit-Fehlervalidierung beim Proofing einer URL (zuvor mussten Sie mehrere Minuten warten, bevor ein Fehler angezeigt wurde)

>[!NOTE]
>
>Diese neue Seite zur Erstellung von Korrekturabzügen in Workfront Proof entspricht jetzt der Seite zur Erstellung von Korrekturabzügen, die kürzlich in Workfront bei der Erstellung von Korrekturabzügen zur Verfügung gestellt wurde. 

Weitere Informationen finden Sie unter  [Erstellen von Testsendungen in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Proofing-Verbesserungen in Workfront und Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Beim Hinzufügen von Dokumenten zu Workfront und Workfront Proof gelten die folgenden Änderungen:

* [Ändern der Größe der Kommentarliste bei der Überprüfung von Korrekturabzügen](#resize-the-comment-list-when-reviewing-proofs)
* [Hyperlinks sind bei der Überprüfung statischer Korrekturabzüge aktiv](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Verbesserungen beim Hinzufügen von Korrekturabzügen](#improvements-when-adding-proofs)

### Größe der Kommentarliste bei der Überprüfung von Korrekturabzügen ändern {#resize-the-comment-list-when-reviewing-proofs}

Jetzt können Sie bei der Überprüfung von Korrekturabzügen in der Korrekturabzugsansicht die Größe der Kommentarliste ändern.

Weitere Informationen finden Sie unter in .

### Hyperlinks sind bei der Überprüfung statischer Korrekturabzüge aktiv {#hyperlinks-are-active-when-reviewing-static-proofs}

Hyperlinks sind jetzt aktiv, wenn Sie einen statischen Korrekturabzug in der Korrekturabzugsansicht prüfen. Klicken Sie auf einen Hyperlink, um zur verknüpften Seite zu gelangen.

Diese Funktion wird in allen Dateitypen mit Text unterstützt, z. B. PDF, DOC usw. Bilddateien werden nicht unterstützt.

### Verbesserungen beim Hinzufügen von Korrekturabzügen {#improvements-when-adding-proofs}

Beim Hinzufügen von zu prüfenden Dokumenten stehen die folgenden Verbesserungen zur Verfügung. 

* Die Informationen in der Empfängerliste sind jetzt in einer 3-spaltigen Ansicht verfügbar, sodass die Informationen leichter angezeigt und geändert werden können. 

  Zuvor wurden die Informationen in einer einspaltigen Ansicht angezeigt, sodass mehr Klicks erforderlich waren, wenn Änderungen erforderlich waren. 

  Weitere Informationen finden Sie unter in .

* Ziehen Sie bei Verwendung des automatisierten Workflows einen oder mehrere Empfänger von einem Workflow-Schritt in einen anderen. Sie können direkt zu einem Schritt ziehen oder zu einem Schritt im Diagramm oben auf der Seite ziehen.

  Weitere Informationen finden Sie unter in .

* Das Workflow-Diagramm bleibt auch beim Scrollen oben auf der Seite sichtbar. Das Diagramm ist standardmäßig reduziert. Erweitern Sie das Diagramm, um das vollständige Diagramm anzuzeigen.

  Weitere Informationen finden Sie unter in .

* Beim Hinzufügen einer Vorlage zu einem automatisierten Workflow in einem Korrekturabzug wird eine Ladeanimation angezeigt, was angibt, dass die Vorlage geladen wird.

  Weitere Informationen finden Sie unter in .

* Die folgenden Einstellungen wurden aus dem Abschnitt Korrekturabzugseinstellungen in den Abschnitt Workflow auf der Seite Neuer Korrekturabzug verschoben:

   * Primärer Entscheidungsträger
   * Nur eine Entscheidung verlangen

## Das Erscheinungsbild mit der Basecamp-Integration in Workfront Proof wurde aktualisiert {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Das Erscheinungsbild der Basecamp-Integration mit Workfront Proof wurde aktualisiert. Die Funktionalität bleibt gleich.

## Einfügen von Bildern in Workfront aus der Zwischenablage {#paste-images-to-workfront-from-the-clipboard}

Sie können jetzt Bilddateien zu Workfront hinzufügen, indem Sie ein Bild aus Ihrer Systemzwischenablage einfügen.

Die Möglichkeit zum Einfügen aus der Zwischenablage wurde in einer früheren Version von Workfront entfernt; sie wird mit dieser Version wieder eingeführt. Die neue Methode ist schlanker und intuitiver.

Weitere Informationen finden Sie unter [Einfügen von Bildern aus der Zwischenablage](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Verbesserungen beim Auslastungsbericht {#utilization-report-improvements}

Der Auslastungsbericht enthält die folgenden Verbesserungen:

* Umsatz im Auslastungsbericht für ein Projekt anzeigen

  Ermöglicht die Anzeige der budgetierten Einnahmen, der geplanten Einnahmen, der tatsächlichen Einnahmen, der budgetierten Abweichung und der geplanten Abweichung.

* Einnahmen mit geplanten Kosten und Istkosten vergleichen

  Ermöglicht die Anzeige der geplanten Kosten oder Ist-Kosten zusammen mit dem geplanten Umsatz. Die Spanne (%) wird ebenfalls angezeigt (die Spanne wird als Umsatz - Kosten/Umsatz berechnet).

* Der Umsatz wird beim Anzeigen des Diagramms angezeigt.
* Kopfzeilen bleiben beim Scrollen sichtbar.

  Wenn Sie nun durch die Informationen im Auslastungsbericht scrollen, ist die Kopfzeile oben im Auslastungsbericht immer sichtbar, sodass Sie die Daten im Bericht leichter verstehen können.

  Zuvor war die Kopfzeile am oberen Rand des Auslastungsberichts beim Scrollen nicht mehr sichtbar.

* Auslastungsbericht für ein einzelnes Projekt wird automatisch geladen

  Beim Anzeigen des Auslastungsberichts für ein Projekt wird der Bericht automatisch geladen.

  Vor dieser Änderung mussten Sie auf „Ausführen“ klicken, bevor der Bericht ausgeführt wurde.

* Verbesserte Leistung

Weitere Informationen zum Auslastungsbericht finden Sie unter [Übersicht über den Ressourcenauslastungsbericht](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Entfernen des Objekts „Ressource budgetiert Stunde“ aus Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Um Leistungsprobleme zu beheben, wurde das Feld Ressource - budgetierte Stunde vorübergehend aus Workfront entfernt.

Zur Erinnerung: Die von der Ressource budgetierten Stunden sind die Stunden, die Sie für Ihre Ressourcen oder Projekte im Ressourcenplaner budgetieren. Derzeit können Sie in der Web-Anwendung oder über die API keinen Bericht mehr zu diesem Feld erstellen. Das Feld wird in einer zukünftigen Version wieder aktiviert, wenn die Leistungsprobleme behoben wurden.

Weitere Informationen zur Budgetierung von Stunden im Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Nutzungsstatistiken von Berichten {#report-usage-statistics}

Sie können jetzt die folgenden Nutzungsinformationen für Ihre Workfront-Berichte in einer Liste von Berichten anzeigen:

* Zuletzt angezeigt von
* Datum der letzten Ansicht
* Letzten 10 anzeigenden Benutzer
* Anzeigen in diesem Monat/Quartal/Jahr
* Aufrufe letzten Monat/letztes Quartal/Jahr
* Alle Ansichten

Vor diesem Update gab es nur eingeschränkte Informationen zur Verwendung in Ihren Berichten.

Weitere Informationen zur Verwendung von Berichten finden Sie unter [Berichtsnutzung anzeigen](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Zeitpläne, die von Gruppenadministratoren verwaltet werden {#schedules-managed-by-group-administrators}

Als Gruppenadministrator können Sie Zeitpläne erstellen und bearbeiten, die mit den von Ihnen verwalteten Gruppen oder deren Untergruppen verknüpft sind. Vor dieser Änderung konnten nur Workfront-Administratoren Zeitpläne erstellen und bearbeiten.

Weitere Informationen zum Verwalten von Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Gantt-Diagramm-Aktualisierungen {#gantt-chart-updates}

Das Gantt-Diagramm kann jetzt bearbeitet werden. Mithilfe des Gantt-Diagramms können Sie die folgenden Aktualisierungen an Ihren Aufgaben vornehmen:

* Erstellen von Vorgängerbeziehungen
* Aufgabendauer bearbeiten
* Aufgabe in Prozent abgeschlossen aktualisieren
* Ressourcenabgleich anwenden

Vor dieser Änderung konnten Sie nur Vorgängerbeziehungen im Gantt-Diagramm entfernen und Vorgänge nur in der Aufgabenliste bearbeiten.

Weitere Informationen zum Gantt-Diagramm finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## Neuer Portfolio Optimizer {#new-portfolio-optimizer}

Der Bereich Portfolio-Optimizer von Workfront wurde nun mit einem neuen Look-and-Feel aktualisiert. Die Funktionalität hat sich nicht geändert.

Weitere Informationen zum Portfolio-Optimizer finden Sie unter Übersicht über den [Portfolio-Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Budgetdatumsanpassungsoption im Ressourcenplaner {#budget-date-adjustment-option-in-the-resource-planner}

Wir haben eine Option hinzugefügt, um Ihnen einen schnellen Einblick in Zeitrahmen zu geben, ohne Budgetkonflikte zu vermeiden. Nachdem Sie angezeigt haben, wann die Zeitrahmen ohne Budgetierungskonflikte auftreten, können Sie Ihre budgetierten Stunden manuell in diese Zeiten verschieben. Dadurch werden auch die budgetierten Daten der Stunden angepasst. Vor diesem Update war das Anzeigen von Budgetierungskonflikten für ein Projekt auf einen Blick nicht möglich.

Weitere Informationen zum Anpassen budgetierter Termine im Ressourcenplaner finden Sie im Abschnitt „Anpassen von Budgetierungsterminen“ in der Übersicht [Ressourcenplaner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Ressourcenplanung: Beschränken Sie Zuweisungen auf Benutzer basierend auf der Gruppenmitgliedschaft {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Bei Benutzerzuweisungen im Planungsbereich (wie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen“ beschrieben) können Sie jetzt Workfront so konfigurieren, dass die Zuweisung von Aufgaben und Problemen nur auf die Benutzer beschränkt wird, die Mitglieder der Gruppe sind, die in dem Projekt definiert ist, aus dem die Aufgabe oder das Problem stammt. 

Dies gilt, wenn Zuweisungen wie folgt vorgenommen werden:

* Beim Zuweisen eines Benutzers zu allen Aufgaben und Problemen für eine bestimmte Rolle, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung konnte eine Aufgabe oder ein Problem immer jedem Benutzer zugewiesen werden, unabhängig von seiner Gruppenmitgliedschaft. 

* Beim Austauschen von Zuweisungen gegen einen anderen Benutzer, wie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung konnte eine Aufgabe oder ein Problem immer jedem Benutzer zugewiesen werden, unabhängig von seiner Gruppenmitgliedschaft. 

* Beim manuellen Zuweisen einer Aufgabe oder eines Problems über die Zeitleiste für die Planung, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung konnte eine Aufgabe oder ein Problem immer jedem Benutzer zugewiesen werden, unabhängig von seiner Gruppenmitgliedschaft. 

* Wenn Workfront die automatische Zuweisung von Benutzern erlaubt, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung würde Workfront Benutzenden Aufgaben und Probleme zuweisen, unabhängig von der Gruppenmitgliedschaft.

Weitere Informationen zum Konfigurieren dieser Option finden Sie unter „Erste Schritte mit der Ressourcenplanung“.

## Ressourcenplanung: Zulassen von Zuweisungen an Benutzer unabhängig von deren Rolle {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Bei Benutzerzuweisungen im Planungsbereich (wie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen“ beschrieben) können Sie jetzt Workfront so konfigurieren, dass Aufgaben und Probleme jedem Benutzer zugewiesen werden können, unabhängig davon, ob dieser Benutzer in seinem Benutzerprofil eine Rolle definiert hat, die der Rollenzuweisung der ihm zugewiesenen Aufgabe oder des Problems entspricht.

Dies gilt, wenn Zuweisungen wie folgt vorgenommen werden:

* Beim Zuweisen eines Benutzers zu allen Aufgaben und Problemen für eine bestimmte Rolle, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen“ in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen“ beschrieben.

  Vor dieser Änderung musste die primäre Rolle des Benutzers, den Sie zuweisen, mit der bereits im Feld Rolle auswählen definierten Rolle übereinstimmen.

* Beim Austauschen von Zuweisungen gegen einen anderen Benutzer, wie unter „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung musste die primäre Rolle des Benutzers, den Sie zuweisen, mit der bereits im Feld Rolle auswählen definierten Rolle übereinstimmen.

* Beim manuellen Zuweisen einer Aufgabe oder eines Problems über die Zeitleiste für die Planung, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

  Vor dieser Änderung wurden in der Zeitplanleiste nur Benutzer angezeigt, deren Rolle mit der Rolle der Aufgabe oder des Problems übereinstimmt, die bzw. das Sie zugewiesen haben.

>[!NOTE]
>
>Dies gilt nicht, wenn Workfront die automatische Zuweisung von Benutzern ermöglicht, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben. Beim automatischen Zuweisen von Benutzern können Aufgaben und Probleme nur Benutzern mit einer entsprechenden Rolle zugewiesen werden.

Weitere Informationen zum Konfigurieren dieser Option finden Sie unter „Erste Schritte mit der Ressourcenplanung“.

## Emoji-Unterstützung {#emoji-support}

Jetzt können Sie den Ton für Kommentare und Aktualisierungen festlegen, die Sie in Workfront vornehmen, indem Sie Emojis einfügen. Alle Emojis, die zu Kommentaren auf der Registerkarte Aktualisierungen hinzugefügt wurden, werden auch in der E-Mail-Benachrichtigung zur Aktualisierung angezeigt. 

Weitere Informationen finden Sie unter [Arbeit aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
