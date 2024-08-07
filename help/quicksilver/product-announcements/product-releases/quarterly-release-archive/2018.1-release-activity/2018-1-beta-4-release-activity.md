---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Version 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2018.1 von Beta 4 verfügbar waren. Die Funktion wurde am 24. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# Beta-Version 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Version 2018.1 von Beta 4 verfügbar waren. Die Funktion wurde am 24. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.1 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Version 2018.1 von Beta 4 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Von Gruppenadministratoren verwaltete Zeitpläne](#schedules-managed-by-group-administrators)

**Für alle Benutzer**

* [Verbesserungen beim Testen in Workfront](#proofing-improvements-within-workfront)
* [Erstellung von Testsendungen in Workfront Proof - Verbessertes Benutzererlebnis und zusätzliche Funktionen](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Verbesserungen beim Testen in Workfront und Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Aktualisiertes Erscheinungsbild und Verhalten mit Basecamp-Integration in Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [ Bilder aus der Zwischenablage in Workfront einfügen](#paste-images-to-workfront-from-the-clipboard)
* [Verbesserungen beim Nutzungsbericht](#utilization-report-improvements)
* [Entfernen Sie das Ressourcenbudget aus Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Statistiken zur Berichtverwendung](#report-usage-statistics)
* [Aktualisierungen des Gantt-Diagramms](#gantt-chart-updates)
* [New Portfolio Optimizer](#new-portfolio-optimizer)
* [Option zur Anpassung des Budgetdatums im Ressourcenplaner](#budget-date-adjustment-option-in-the-resource-planner)
* [Ressourcenplanung: Beschränken der Zuweisungen an Benutzer auf der Grundlage der Gruppenmitgliedschaft](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Ressourcenplanung: Zulassen von Zuweisungen an Benutzer unabhängig von Rolle](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Emoji-Unterstützung](#emoji-support)

## Verbesserungen bei der Überprüfung in Workfront {#proofing-improvements-within-workfront}

Die Dokumentliste in Workfront wurde wie folgt verbessert: 

* [Testversand-Fortschritt aus der Dokumentliste anzeigen](#view-proof-progress-from-the-document-list)
* [Neue Option zum Anzeigen der Druckzusammenfassung aus der Dokumentliste](#new-option-to-view-the-print-summary-from-the-document-list)
* [Aktualisierter Look and Feel für das Erstellen oder Öffnen des Testversands aus der Dokumentliste](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Verschiedene Links, die aus Dokumenten auf der Dokumentliste entfernt wurden](#various-links-removed-from-documents-on-the-document-list)
* [Dateinamen bei kombinierten Testsendungen anzeigen](#view-file-names-on-combined-proofs)
* [Anzeigen der aktuellen aktiven Phase eines Testversands aus der Dokumentliste](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Anzeigen des Testfortschritts über die Dokumentliste {#view-proof-progress-from-the-document-list}

Beim Anzeigen der Dokumentliste werden nun für alle Testsendungen Indikatoren zum Fortschritt angezeigt. (Dazu gehören Gesendet, Geöffnet, Kommentar und Beschluss.)

Vor dieser Änderung mussten Sie einen Testversand in der Dokumentliste auswählen, um den Testversand-Fortschritt im rechten Bereich anzuzeigen. 

Weitere Informationen finden Sie unter [Fortschrittsnachweis und Statusübersicht](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Neue Option zum Anzeigen der Druckzusammenfassung über die Dokumentliste {#new-option-to-view-the-print-summary-from-the-document-list}

Sie können die Druckzusammenfassung für einen Testversand jetzt direkt aus der Dokumentliste anzeigen.

Vor dieser Änderung konnten Sie die Druckzusammenfassung nur aus dem Testversand-Viewer anzeigen. 

Weitere Informationen zum Anzeigen der Druckzusammenfassung aus der Dokumentliste finden Sie unter [Drucken einer Testversand-Zusammenfassung in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Aktualisiertes Erscheinungsbild für das Erstellen oder Öffnen des Testversands aus der Dokumentliste {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Wenn Sie nun den Mauszeiger über ein Dokument in der Dokumentliste bewegen, wurden die Optionen zum Generieren des Testversands oder zum Öffnen des Testversands aktualisiert. Diese Optionen sind jetzt auffälliger und erscheinen als Schaltflächen.

Vor dieser Änderung waren diese Optionen als Links unter dem Dokumentnamen verfügbar.

Weitere Informationen finden Sie in den folgenden Abschnitten:

* .
* in .

### Verschiedene Links, die aus Dokumenten auf der Dokumentliste entfernt wurden {#various-links-removed-from-documents-on-the-document-list}

Die folgenden Aktionen sind nicht mehr als Links auf einzelnen Dokumenten in der Dokumentliste verfügbar:

* Korrekturabzug generieren
* Korrekturabzug
* Details
* Freigeben
* Auschecken/Einchecken

Die folgenden Aktionen sind jetzt als Schaltfläche im Dokument in der Dokumentliste verfügbar:

* Offener Testversand (verfügbar nach der Erstellung des Testversands) 
* Testversand generieren (verfügbar, wenn der Testversand noch nicht erstellt wurde)

Die folgenden Aktionen sind jetzt im Dropdown-Menü neben der Schaltfläche Testversand öffnen oder Testversand generieren verfügbar:

* Korrekturabzug-Details
* Dokumentdetails
* Zusammenfassung drucken

Weitere Informationen finden Sie in den folgenden Abschnitten:

* .
* in .

### Dateinamen bei kombinierten Testsendungen anzeigen {#view-file-names-on-combined-proofs}

Sie können nun die einzelnen Dateinamen anzeigen, aus denen sich ein kombinierter Testversand zusammensetzt. Diese Informationen werden im Tab Details angezeigt, wenn der Testversand in der Dokumentliste ausgewählt wird.

Weitere Informationen finden Sie unter Anzeigen aller Dateien, die in einem kombinierten Testversand enthalten sind. 

### Anzeigen der aktuellen aktiven Phase eines Testversands aus der Dokumentliste {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Wenn Sie nun einen Testversand in der Dokumentliste auswählen, werden die aktuellen aktiven Phasen in der rechten Spalte auf dem Tab Details angezeigt. 

Weitere Informationen finden Sie unter [Anzeigen aktiver Bühnen auf einem Testversand](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Erstellung von Testsendungen in Workfront Proof - Verbessertes Benutzererlebnis und zusätzliche Funktionen {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Zusätzlich zu einer verbesserten Benutzererfahrung beim Erstellen von Testsendungen in Workfront Proof stehen nun die folgenden zusätzlichen Funktionen zur Verfügung:

* Zusammenführen mehrerer Bilder zu einem Testversand.
* Testversand-Websites mit mehreren Auflösungen (mehrere Auflösungen können als einzelne Testsendungen erstellt oder zu einem Testversand kombiniert werden).
* Bearbeiten Sie den Dateinamen während des Upload-Prozesses.
* Fügen Sie benutzerdefinierte Felder in das Formular zur Testversand-Erstellung ein.
* Fügen Sie eine benutzerdefinierte Nachricht zum Testversand von E-Mail-Benachrichtigungen hinzu.
* Zusätzliche Testeinstellungen 
* Validierung von Echtzeitfehlern beim Testen einer URL (zuvor mussten Sie mehrere Minuten warten, bevor ein Fehler angezeigt wurde)

>[!NOTE]
>
>Diese neue Seite zur Erstellung von Testsendungen in Workfront Proof entspricht jetzt der Seite zur Erstellung von Testsendungen, die kürzlich bei der Erstellung von Testsendungen in Workfront zur Verfügung gestellt wurde. 

Weitere Informationen finden Sie unter  [Generieren von Testsendungen in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Verbesserungen bei der Überprüfung in Workfront und Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Die folgenden Änderungen gelten für das Hinzufügen von Dokumenten zu Workfront und Workfront Proof:

* [Größe der Kommentarliste bei der Überprüfung von Testsendungen ändern](#resize-the-comment-list-when-reviewing-proofs)
* [Hyperlinks sind aktiv bei der Überprüfung statischer Testsendungen](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Verbesserungen beim Hinzufügen von Testsendungen](#improvements-when-adding-proofs)

### Anpassen der Kommentarliste bei der Überprüfung von Testsendungen {#resize-the-comment-list-when-reviewing-proofs}

Jetzt können Sie die Größe der Kommentarliste ändern, wenn Sie Testsendungen im Testversand-Viewer überprüfen.

Weitere Informationen finden Sie unter .

### Hyperlinks sind aktiv bei der Überprüfung statischer Testsendungen {#hyperlinks-are-active-when-reviewing-static-proofs}

Hyperlinks sind jetzt aktiv, wenn ein statischer Testversand im Testversand-Viewer überprüft wird. Klicken Sie auf einen Hyperlink, um zur verknüpften Seite zu gelangen.

Diese Funktion wird in allen Dateitypen unterstützt, die Text enthalten, z. B. PDF, DOC usw. Bilddateien werden nicht unterstützt.

### Verbesserungen beim Hinzufügen von Testsendungen {#improvements-when-adding-proofs}

Die folgenden Verbesserungen sind verfügbar, wenn zu prüfende Dokumente hinzugefügt werden. 

* Informationen in der Empfängerliste sind jetzt in einer 3-Spalten-Ansicht verfügbar, was die Anzeige und Änderung der Informationen erleichtert. 

  Zuvor wurden die Informationen in einer Einzelspaltenansicht angezeigt, sodass bei Bedarf mehr Klicks erforderlich waren. 

  Weitere Informationen finden Sie unter .

* Ziehen Sie bei Verwendung des automatisierten Workflows einen oder mehrere Empfänger aus einer Workflow-Phase in eine andere. Sie können direkt auf eine Bühne ziehen oder auf eine Bühne im Diagramm ziehen, die sich oben auf der Seite befindet.

  Weitere Informationen finden Sie unter .

* Das Workflow-Diagramm bleibt auch beim Scrollen am oberen Seitenrand sichtbar. Das Diagramm ist standardmäßig ausgeblendet. Erweitern Sie das Diagramm, um das vollständige Diagramm anzuzeigen.

  Weitere Informationen finden Sie unter .

* Beim Hinzufügen einer Vorlage zu einem automatisierten Workflow in einem Testversand wird eine Animation zum Laden angezeigt, die angibt, dass die Vorlage geladen wird.

  Weitere Informationen finden Sie unter .

* Die folgenden Einstellungen wurden aus dem Abschnitt Testversandeinstellungen in den Abschnitt Workflow auf der Seite Neuer Testversand verschoben:

   * Primärer Entscheidungsträger
   * Nur eine Entscheidung erforderlich

## Aktualisierte Look-and-Feel-Integration mit Basecamp in Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Das Erscheinungsbild der Basecamp-Integration mit Workfront Proof wurde aktualisiert. Die Funktionalität bleibt gleich.

## Bilder aus der Zwischenablage in Workfront einfügen {#paste-images-to-workfront-from-the-clipboard}

Sie können jetzt Bilddateien zu Workfront hinzufügen, indem Sie ein Bild aus der Zwischenablage des Systems einfügen.

Die Möglichkeit, aus der Zwischenablage einzufügen, wurde in einer früheren Version aus Workfront entfernt. Sie wird mit dieser Version wieder eingeführt. Die neue Methode ist schlanker und intuitiver.

Weitere Informationen finden Sie unter [Bilder aus der Zwischenablage einfügen](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Verbesserungen beim Nutzungsbericht {#utilization-report-improvements}

Der Nutzungsbericht enthält die folgenden Verbesserungen:

* Anzeigen des Umsatzes im Bericht &quot;Nutzung&quot;zu einem Projekt

  Ermöglicht Ihnen die Anzeige von budgetiertem Umsatz, geplantem Umsatz, tatsächlichem Umsatz, budgetierter Varianz und geplanter Varianz.

* Vergleich des Umsatzes mit den geplanten und tatsächlichen Kosten

  Ermöglicht die Anzeige der geplanten oder tatsächlichen Kosten neben dem geplanten Umsatz. Die Marge (%) wird ebenfalls angezeigt (die Marge wird als Umsatz - Kosten/Umsatz berechnet).

* Der Umsatz wird beim Anzeigen der Grafik angezeigt.
* Die Kopfzeilen bleiben beim Scrollen sichtbar.

  Wenn Sie jetzt durch die Informationen im Bericht &quot;Nutzung&quot;scrollen, wird immer die Kopfzeile oben im Bericht &quot;Nutzung&quot;angezeigt, sodass Sie die Daten im Bericht leichter verstehen können.

  Zuvor wurde die Kopfzeile oben im Nutzungsbericht beim Scrollen nicht mehr angezeigt.

* Der Nutzungsbericht eines einzelnen Projekts wird automatisch geladen

  Beim Anzeigen des Nutzungs berichts für ein Projekt wird der Bericht automatisch geladen.

  Vor dieser Änderung mussten Sie auf &quot;Ausführen&quot;klicken, bevor der Bericht ausgeführt wurde.

* Verbesserte Leistung

Weitere Informationen zum Bericht &quot;Nutzung&quot;finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Entfernen Sie das Ressourcenbudget aus Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Zur Behebung von Leistungsproblemen wurde das Feld Resource Budgeted Hour vorübergehend aus Workfront entfernt.

Zur Erinnerung: Die Resource Budgeted Hours sind die Stunden, die Sie für Ihre Ressourcen oder Projekte im Resource Planer einplanen. Derzeit können Sie in der Webanwendung oder über die API keinen Bericht mehr zu diesem Feld erstellen. Das Feld wird in einer zukünftigen Version erneut aktiviert, wenn die Leistungsprobleme behoben wurden.

Weitere Informationen zu Budgeteinsätzen im Ressourcenplaner finden Sie unter [Ressourcenplanerübersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Nutzungsstatistiken von Berichten {#report-usage-statistics}

Sie können jetzt die folgenden Nutzungsinformationen für Ihre Workfront-Berichte in einer Liste von Berichten anzeigen:

* Zuletzt angezeigt von
* Letztes Ansichtsdatum
* Letzten 10 anzeigenden Benutzer
* Ansichten in diesem Monat/Quartal/Jahr
* Ansichten im letzten Monat/Quartal/Jahr
* Alle Ansichten

Vor dieser Aktualisierung war die Anzeige der Nutzungsinformationen in den Berichten eingeschränkt.

Weitere Informationen zur Verwendung von Berichten finden Sie unter [Nutzung von Berichten anzeigen](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Von Gruppenadministratoren verwaltete Zeitpläne {#schedules-managed-by-group-administrators}

Als Gruppenadministrator können Sie Zeitpläne erstellen und bearbeiten, die mit den von Ihnen verwalteten Gruppen sowie deren Untergruppen verknüpft sind. Vor dieser Änderung konnten nur Workfront-Administratoren Zeitpläne erstellen und bearbeiten.

Weitere Informationen zum Verwalten von Zeitplänen finden Sie unter [Zeitplan erstellen](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Gantt-Diagramm-Aktualisierungen {#gantt-chart-updates}

Das Gantt-Diagramm kann jetzt bearbeitet werden. Mithilfe des Gantt-Diagramms können Sie Ihre Aufgaben wie folgt aktualisieren:

* Erstellen von Vorgängerbeziehungen
* Dauer der Aufgabe bearbeiten
* Aktualisierung des Prozentsatzes der Aufgabe
* Anwenden der Ressourcenebene

Vor dieser Änderung konnten Sie nur Vorgängerbeziehungen im Gantt-Diagramm entfernen und Aufgaben nur in der Aufgabenliste bearbeiten.

Weitere Informationen zum Gantt-Diagramm finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## New Portfolio Optimizer {#new-portfolio-optimizer}

Das Portfolio Optimizer-Gebiet von Workfront wird jetzt mit einem neuen Erscheinungsbild aktualisiert. Die Funktionalität wurde nicht geändert.

Weitere Informationen zum Portfolio Optimizer finden Sie unter [Übersicht über Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Option zur Anpassung des Budgetdatums im Ressourcenplaner {#budget-date-adjustment-option-in-the-resource-planner}

Wir haben eine Option hinzugefügt, mit der Sie schnell Einblicke in Zeitrahmen erhalten können, ohne dass es zu Budgetkonflikten kommt. Nachdem Sie gesehen haben, wann die Zeitrahmen ohne Budgetkonflikte eintreten, können Sie Ihre Budgetzeit manuell zu diesen Zeiten verschieben. Dadurch werden auch die Budgetzeiten der Stunden angepasst. Vor dieser Aktualisierung war es nicht möglich, Budgetierungskonflikte für ein Projekt auf einen Blick zu betrachten.

Weitere Informationen zum Anpassen von geplanten Datumsangaben im Ressourcenplaner finden Sie im Abschnitt &quot;Anpassen der Budgetierungsdaten&quot;in der [Ressourcenplanerübersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Ressourcenplanung: Beschränken der Zuweisungen an Benutzer auf der Grundlage der Gruppenmitgliedschaft {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Bei der Benutzerzuweisung im Planungsbereich (wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben) können Sie Workfront jetzt so konfigurieren, dass nur die Zuweisung von Aufgaben und Problemen auf die Benutzer beschränkt wird, die Mitglieder der Gruppe sind, die für das Projekt definiert ist, von dem die Aufgabe oder das Problem stammt. 

Dies gilt für Zuweisungen auf folgende Weise:

* Beim Zuweisen eines Benutzers zu allen Aufgaben und Problemen für eine bestimmte Rolle, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung konnte jedem Benutzer unabhängig von der Gruppenmitgliedschaft des Benutzers immer eine Aufgabe oder ein Problem zugewiesen werden. 

* Beim Austausch von Zuweisungen mit einem anderen Benutzer, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung konnte jedem Benutzer unabhängig von der Gruppenmitgliedschaft des Benutzers immer eine Aufgabe oder ein Problem zugewiesen werden. 

* Beim manuellen Zuweisen einer Aufgabe oder eines Problems über die Planung, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung konnte jedem Benutzer unabhängig von der Gruppenmitgliedschaft des Benutzers immer eine Aufgabe oder ein Problem zugewiesen werden. 

* Wenn es Workfront ermöglicht, automatisch Benutzer zuzuweisen, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung ordnete Workfront Benutzern unabhängig von der Gruppenmitgliedschaft Aufgaben und Probleme zu.

Weitere Informationen zum Konfigurieren dieser Option finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Ressourcenplanung: Zuweisung an Benutzer unabhängig von Rolle zulassen {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Bei Benutzerzuweisungen im Planungsbereich (wie unter &quot;Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Planungsbereichen&quot;beschrieben) können Sie Workfront jetzt so konfigurieren, dass Aufgaben und Probleme jedem Benutzer zugewiesen werden können, unabhängig davon, ob für diesen Benutzer in seinem Benutzerprofil eine Rolle definiert ist, die mit der Rollenzuweisung der Aufgabe oder des Problems übereinstimmt, die ihm zugewiesen wurde.

Dies gilt für Zuweisungen auf folgende Weise:

* Beim Zuweisen eines Benutzers zu allen Aufgaben und Problemen für eine bestimmte Rolle, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;in &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung musste die primäre Rolle des Benutzers, den Sie zuweisen, mit der bereits im Feld Rolle auswählen definierten Rolle übereinstimmen.

* Beim Austausch von Zuweisungen mit einem anderen Benutzer, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung musste die primäre Rolle des Benutzers, den Sie zuweisen, mit der bereits im Feld Rolle auswählen definierten Rolle übereinstimmen.

* Beim manuellen Zuweisen einer Aufgabe oder eines Problems über die Planung, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

  Vor dieser Änderung wurden nur Benutzer in der Planung angezeigt, deren Rolle mit der Rolle der von Ihnen zugewiesenen Aufgabe oder des Problems übereinstimmte.

>[!NOTE]
>
>Dies gilt nicht, wenn Workfront automatisch Benutzer zuweisen kann, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben. Beim automatischen Zuweisen von Benutzern können Aufgaben und Probleme nur Benutzern mit der entsprechenden Rolle zugewiesen werden.

Weitere Informationen zum Konfigurieren dieser Option finden Sie unter &quot;Erste Schritte mit der Ressourcenplanung&quot;.

## Emoji-Unterstützung {#emoji-support}

Jetzt können Sie den Ton für Kommentare und Aktualisierungen festlegen, die Sie in Workfront vornehmen, indem Sie Emojis einfügen. Alle Emojis, die zu Kommentaren hinzugefügt wurden, die auf der Registerkarte Aktualisierungen erstellt wurden, werden auch in der E-Mail-Benachrichtigung zum Aktualisieren angezeigt. 

Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
