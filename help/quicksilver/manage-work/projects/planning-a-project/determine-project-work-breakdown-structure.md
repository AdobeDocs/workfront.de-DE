---
product-area: projects
navigation-topic: plan-a-project
title: Bestimmen der Projektstrukturaufschlüsselung in einem Projekt
description: Die Definition einer Projektstrukturplan-Aktivität (Work Breakdown Structure, PSP) für ein Projekt ist eine Reihe von Aktivitäten, die letztendlich den Projektplan umreißen. Der Projektstrukturplan unterteilt das Projektergebnis in überschaubare Arbeitselemente, mit denen Meilensteine definiert und Arbeitszuweisungen organisiert werden können.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 1%

---

# Bestimmen der Projektstrukturaufschlüsselung in einem Projekt

Die Definition einer Projektstrukturplan-Aktivität (Work Breakdown Structure, PSP) für ein Projekt ist eine Reihe von Aktivitäten, die letztendlich den Projektplan umreißen. Der Projektstrukturplan unterteilt das Projektergebnis in überschaubare Arbeitselemente, mit denen Meilensteine definiert und Arbeitszuweisungen organisiert werden können.

Sie müssen über eine Planlizenz mit Bearbeitungszugriff auf Projekte verfügen, um die Projektaufschlüsselungsstruktur zu erstellen. Abhängig von der Anzahl der Aktivitäten, die Sie während des Erstellens des PSPs ausführen, ist möglicherweise zusätzlicher Zugriff auf andere Bereiche von Adobe Workfront erforderlich.

Es wird empfohlen, den Planungsstatus für das Projekt beizubehalten, während Sie die Projektaufteilungsstruktur ändern, um Benachrichtigungen an Trigger im Projektteam zu vermeiden.

## Projektlieferungen definieren

Der Zweck eines Projekts besteht darin, internen und externen Stakeholdern greifbare Ergebnisse bereitzustellen. Die Ergebnisse eines Projekts sind die Ergebnisse, die Sie durch den Abschluss des Projekts erreichen möchten. Ergebnisse sind fast immer mit mindestens einem Ergebnis verknüpft. Alle Ergebnisse sollten mit einem Projekt verknüpft werden.

Bei den Projektleistungen kann es sich um Verbrauchsgüter, geistige Produkte (z. B. Berichte) oder Dienstleistungen handeln. Wenn Ihr Projektumfang beispielsweise den Bau eines Hauses umfasst, können einige der Ergebnisse Folgendes umfassen:

* Erstellen von Architekturplänen
* Rohrleitung fertig stellen
* Elektroarbeit
* Gießen des Fundaments
* Rahmenwerk
* Schließt den Verkauf des Hauses ab.

Je nach Größe und Umfang kann ein Projekt aus mehreren Ergebnissen bestehen.

Sobald Sie Ihre Ergebnisse identifiziert haben, können Sie damit beginnen, sie in Aufgaben aufzuteilen. Aufgaben sind die Ergebnisse, die Sie erzielen, um Ihr Gesamtergebnis für das Projekt zu liefern. Bei der Definition Ihrer Aufgaben berücksichtigen Sie die folgenden Parameter:

* Dauer bis zum Abschluss.
* Für den Abschluss der Arbeiten erforderliches Budget.
* Erforderliche Ressourcen, um die Arbeit abzuschließen.
* Planung der Ressourcen basierend auf der logischen Zeitleiste der Aufgaben.

Stellen Sie bei der Aufgabendefinition sicher, dass Sie nicht zu viel Arbeit für eine einzelne Aufgabe planen. Wenn die für eine Aufgabe erforderliche Arbeit mehr als 40 Stunden beträgt (eine typische Arbeitswoche), müssen Sie diesen Arbeitsaufwand möglicherweise in Teilaufgaben aufschlüsseln. Mit dem Abschluss aller Teilaufgaben wird dann die Hauptaufgabe abgeschlossen.

Um PSP-Ergebnisse und -Ergebnisse in Workfront zu definieren, empfehlen wir die folgenden Aktivitäten, um eine hierarchische Ansicht von Projektaufgaben zu erstellen:

* Wenn Sie dies noch nicht getan haben, erstellen Sie ein neues Projekt.\
  Informationen zum Erstellen eines Projekts finden Sie im Artikel [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

* Erstellen Sie Aufgaben für alle Aktionselemente, die zum Abschließen der einzelnen Ergebnisse und Ergebnisse erforderlich sind.\
  Informationen zum Erstellen von Aufgaben finden Sie im Artikel [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* Identifizieren Sie aus den soeben erstellten Aufgaben, welche die wichtigsten Ergebnisse sind, und verknüpfen Sie sie mit Meilensteinen.\
  Informationen zum Erstellen von Meilensteinaufgaben finden Sie in den Artikeln [Erstellen eines Meilensteinpfads](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) und [Zuordnen von Meilensteinen zu Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Schlüsseln Sie die Aufgaben mit einem zu großen Bereich in Teilaufgaben auf. Verknüpfen Sie sie mit dem übergeordneten Element, das Ihre Leistung definiert .\
  Informationen zum Erstellen von Teilaufgaben finden Sie im Artikel [Erstellen von &#x200B;](../../../manage-work/tasks/create-tasks/create-subtasks.md)&quot;.

* Identifizieren Sie Abhängigkeitsbeziehungen zwischen Teilaufgaben und zwischen Meilensteinen.\
  In einer Abhängigkeitsbeziehung hängt der Beginn einer Aufgabe vom Abschluss einer anderen Aufgabe oder einer Gruppe von Aufgaben ab.\
  Informationen zu Aufgabenabhängigkeiten finden Sie in den Artikeln [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) und [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Stellen Sie fest, ob während der Lebensdauer des Projekts Genehmigungen und Überprüfungen erforderlich sind. Erstellen Sie Genehmigungsprozesse, um dieser Anforderung gerecht zu werden.\
  Informationen zu Validierungen finden Sie im Artikel [Erstellen eines Validierungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Kalkulation des Arbeitszeitplans und der Zeitplaneinschränkungen

Nachdem Sie die grundlegende Meilenstein- und Aufgabenstruktur des Projekts erstellt haben, können Sie die Zeit schätzen, die zum Abschluss des gesamten Projekts benötigt wird, indem Sie Aufgabenbeschränkungen und -dauern definieren.

Beachten Sie Folgendes:

* Aufgabenbeschränkungen definieren, wann die Arbeit an einer Aufgabe beginnen oder enden muss.

  Informationen zum Definieren von Aufgabenbeschränkungen finden Sie im Artikel [Übersicht über Aufgabenbeschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Die Dauer einer Aufgabe ist der Zeitraum, der zum Abschließen einer Aufgabe zur Verfügung steht. Bei der Schätzung der Dauer sollten Sie einen Wert eingeben, der die Möglichkeit einer Verzögerung berücksichtigt. Wenn ähnliche Projekte in der Vergangenheit abgeschlossen wurden, können Sie eine gute Idee haben, wo Sie diesen Wert festlegen können.

  Da es sich bei der Dauer um eine Schätzung handelt, stellen Sie sicher, dass Sie optimistische Zeitwerte festlegen, um Faktoren zu berücksichtigen, die sich auf die Aufgabe auswirken können, z. B. Wetter, Stromausfälle, Lieferantenschwierigkeiten oder andere unvorhergesehene Ereignisse. Überlegen Sie außerdem, ob es Vorgänger- oder Abhängigkeitsaufgaben gibt und wie diese Einschränkungen für die Arbeit verursachen und sich auf den Abschluss von Aufgaben auswirken können.

  Je nach Dauertyp der Aufgabe können Sie die Dauer einer Aufgabe während der Lebensdauer eines Projekts ändern. Dies wirkt sich jedoch auch auf die Zeitleiste des Projekts aus. Informationen zur Dauer einer Aufgabe finden Sie im Artikel [Übersicht über die Aufgabendauer und den &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Aufgaben zuweisen

Nachdem Sie die Dauer und Einschränkungen jeder Aufgabe definiert haben, können Sie festlegen, wer über die Zeit und die Fähigkeiten verfügt, um die Arbeit zu erledigen. In Workfront können Sie folgenden Entitäten Aufgaben zuweisen:

* Benutzende\
  Nur Benutzer mit der Zugriffsebene „Planer“ oder „Arbeitskraft“ können Aufgaben zugewiesen werden. Obwohl Sie Anfordernden und Prüfenden Aufgaben zuweisen können, können diese sie nicht abschließen. Aus diesem Grund empfehlen wir, ihnen keine Aufgaben zuzuweisen.

  Informationen zu den Zugriffsebenen und dazu, wie sie definieren, was Benutzende mit Workfront-Objekten tun können, finden Sie unter [Zugriffsebenen - Übersicht](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Aufgabengebiete
* Teams

Informationen zum Zuweisen von Aufgaben finden Sie in den Artikeln im Abschnitt [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md).

## Verwalten von Ressourcen

Mit der Ressourcenverwaltung in Workfront können Sie feststellen, ob ausreichend Personal vorhanden ist, um das Projekt abzuschließen. Wenn Benutzende zu einem Projekt hinzugefügt werden, zeigt Workfront die Auslastung der einzelnen Benutzenden an. Ressourcenmanager können die Gesamtzahl der Stunden sehen, die die Person während des Zeitrahmens des Projekts anderen Projekten zugewiesen wurde.

>[!NOTE]
>
>Solange das Projekt den Status Planung hat, werden den Benutzern zugewiesene Aufgaben nicht in ihren Aufgabenlisten angezeigt.

Zu Beginn eines Geschäftsjahres oder Quartals möchten Sie möglicherweise Ihre Ressourcen auf einer höheren Ebene und über mehrere Projekte hinweg verwalten, ohne dass Sie über die Kenntnisse einer bestimmten Arbeitsaufschlüsselungsstruktur verfügen.\
Informationen zur Planung der Verwendung Ihrer Ressourcen auf einer höheren Ebene finden Sie im Artikel [Erste Schritte mit der Ressourcenplanung](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Wenn Sie Ihre Ressourcen im Zusammenhang mit dem Aufbau der Projektaufteilungsstruktur verwalten und sicherstellen, dass jede Aufgabe der richtigen Ressource zugewiesen ist, können Sie die Ressourcen für die zu erledigenden Arbeiten planen.\
Informationen zur Planung Ihrer Ressourcen finden Sie in den Artikeln im Abschnitt [Der Workload Balancer: Artikelindex](../../../resource-mgmt/workload-balancer/workload-balancer.md) .

## Projektfinanzen schätzen

Workfront berechnet die geplanten Kosten für jede Aufgabe und die Gesamtkosten für ein Projekt. Geplante Kosten für eine Aufgabe umfassen alle Kosten der Aufgabe zuzüglich der Kosten für den Mitarbeiter oder die Funktion, der bzw. die der Aufgabe zugewiesen wurde. Stundensätze für die Aufgabe, die Funktion und den Mitarbeiter werden während der Aufgaben-, Funktions- und Benutzererstellung zugewiesen.

Informationen zu den Projektfinanzen finden Sie im Abschnitt [Projektfinanzen: Artikelindex](../../../manage-work/projects/project-finances/project-finances-overview.md).

## Festlegen von Genehmigungspunkten für das Projekt

Durch die Erstellung von Genehmigungsprozessen in Workfront können Sie Prüfpunkte für das Projekt festlegen, um den Fortschritt und potenzielle Problembereiche zu überwachen. Durch den Genehmigungsprozess können Projektbesitzer erkennen, welche Aufgaben zu spät oder zu früh durchgeführt wurden, Audit-Protokolle anzeigen, die auflisten, wer einen Aufgabenstatus geändert hat, und einen Verlauf von Problemen einsehen, einschließlich der Art und Weise, wie Probleme behoben wurden und wann sie geschlossen wurden. Nach der Überprüfung eines Projekts können Projektbesitzer festlegen, welche Schritte unternommen werden sollen, und den Projektplan bei Bedarf aktualisieren.

Informationen zu Validierungen finden Sie im Artikel [Erstellen eines Validierungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## PSP anzeigen

Um den PSP eines Projekts zu verstehen, sollten Sie die folgenden Aufgabenelemente anzeigen:

* Aufgabensequenz und Zeitleiste (geplante Start- und Abschlussdaten und Aufgabendauer)
* Vorgängerabhängigkeiten
* Beziehung zwischen untergeordnetem und übergeordnetem Element
* Arbeitsaufträge

Sobald Sie Ihren PSP abgeschlossen haben, können Sie ihn in einer Aufgabenliste auf Projektebene oder in einem Bericht anzeigen.

* [PSP in einer Aufgabenliste anzeigen](#view-the-wbs-in-a-task-list)
* [PSP in einem Aufgabenbericht anzeigen](#view-the-wbs-in-a-task-report)

### PSP in einer Aufgabenliste anzeigen {#view-the-wbs-in-a-task-list}

Sie können die Aufgabenliste auf Projektebene anzeigen.

1. Wechseln Sie zu dem Projekt, für das Sie die Projektaufschlüsselungsstruktur anzeigen möchten.
1. Wählen Sie die **Aufgaben** aus.
1. (Optional) Wählen Sie **Keine** im Dropdown-Menü **Gruppierung** aus.

   Die Projektstrukturplan-Struktur zeigt nicht die Einrückung der Aufgaben im PSP an.

1. Wählen Sie aus **Dropdown** Menü „Ansicht“ die Ansicht **Arbeitsaufwand** aus.

   Die Struktur für die Arbeitsaufschlüsselung wird in der zweiten Spalte der ausgewählten Ansicht angezeigt.

   ![Struktur der Arbeitsaufschlüsselung in einer Aufgabenliste](assets/work-breakdown-structure.png)

### PSP in einem Aufgabenbericht anzeigen {#view-the-wbs-in-a-task-report}

Sie können einen Aufgabenbericht erstellen und den PSP der Aufgaben anzeigen, indem Sie einen der folgenden Schritte ausführen:

* Wenden Sie die vorhandene Ansicht Arbeitsaufschlüsselungsstruktur auf den Bericht an.
* Fügen Sie die Spalte Arbeitsaufschlüsselungsstruktur zu einem benutzerdefinierten Bericht hinzu.

>[!TIP]
>
>Es wird empfohlen, eine Projektgruppierung hinzuzufügen, um Klarheit darüber zu schaffen, zu welchen Projekten die Aufgaben gehören. Die Einrückung der Aufgaben wird nicht in einem Aufgabenbericht angezeigt.

Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Speichern des PSP eines Projekts als Vorlage

Wenn Sie an anderen Projekten arbeiten, die Arbeitszeitplänen ähnlich der soeben erstellten PSP folgen, können Sie das Projekt als Vorlage speichern. Eine Vorlage spart Zeit und Mühe bei der Erstellung zukünftiger verwandter Projekte.

Wenn Ihre Organisation nur über eine geringe Fluktuation verfügt, sollten Sie warten, bis Benutzerzuweisungen vorgenommen wurden, um die Vorlage zu speichern. Unabhängig davon, wann ein Projekt als Vorlage gespeichert wird, können Benutzerzuweisungen oder bestimmte Aufgaben beim Anhängen der Vorlage an ein neues Projekt entfernt werden.

Die folgenden Elemente einer Projektstrukturplan-Struktur können in einer Vorlage gespeichert werden, um sie später mit einem anderen Projekt zu verwenden:

* Vorgängerabhängigkeiten
* Zuweisungen (einschließlich Projektbesitzer, Sponsor und Ressourcen-Manager)
* Genehmigungsprozesse
* Aufgabenbeschränkungen
* Dokumente
* Ausgaben und sonstige Finanzinformationen
* Ziele
* Stundentypen
* Warteschlangenstruktur anfordern
* Erinnerungsnachrichten
* Risiken
* Abrechnungssätze
* Freigeben von Informationen
* Benutzerdefinierte Formulare

Informationen zum Speichern von Projekten als Vorlagen finden Sie im Artikel [Erstellen einer Vorlage aus einem Projekt](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
