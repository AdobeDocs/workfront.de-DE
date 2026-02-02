---
title: 'Die Bridge: Strategischen Intent mit Projekten verbinden'
description: Erfahren Sie, wie Sie einen „strategischen Thread“ zwischen Ihren allgemeinen Plänen in Adobe Workfront Planning und Ihrer täglichen Ausführung von Workflows in Adobe Workfront erstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# Die Brücke: Strategische Intention mit Projekten verbinden


## Ziel

Erfahren Sie, wie Sie im Workflow-Modul einen „strategischen Thread“ zwischen Ihren allgemeinen Plänen in Workfront Planning und Ihrer täglichen Ausführung erstellen.



## Übersicht

Die Verbindung Ihrer Strategie mit Ihrer täglichen Arbeit macht Vision zur Realität. Wenn Pläne auf hoher Ebene mit der Ausführung synchronisiert sind, erstellen Sie einen **strategischen Thread**, der sicherstellt, dass jedes Projekt und jede Aufgabe das Unternehmen voranbringt.



Um diese Ausrichtung zu erreichen, sind eine Reihe technischer Links und Prozessleitplanken erforderlich, die die Bemühungen im **Workflow-Modul** mit strategischen Datensätzen in **Workfront Planning (WFP) verbinden**. Durch die Überbrückung der Kluft zwischen Planung und Handeln stellen Sie sicher, dass sich die Energie Ihres Teams immer auf Ihre obersten Ziele konzentriert.



## Die Grundlage: Herstellen der Verbindung

Bevor Sie eine Verbindung zwischen Planung und Ausführung herstellen können, muss ein Workspace-Manager festlegen, welche Datensatztypen für eine Verbindung infrage kommen.



### Das Verbindungsfeld: Der technische Handshake

Die Brücke beginnt mit einem **Verbindungsfeld**. Dieser Feldtyp ist die Engine hinter allen Beziehungen in WFP. Sie ist ein Ausdruck der Absicht, da sie festlegt, dass ein bestimmter Datensatztyp (wie *Kanaltaktik*) mit anderen Objekten verknüpft werden darf, unabhängig davon, ob sie im Workflow-Modul oder in der Planung selbst leben.



### Entscheidung zur Verbindung

Die Festlegung dieser Zulage ist eine Entscheidung auf Konfigurationsebene, die normalerweise vor der Erstellung einer Arbeit erfolgt. Durch Hinzufügen eines Verbindungsfelds architektonisch gestalten Sie Ihre Umgebung so, dass ein „strategischer Thread“ unterstützt wird, unabhängig davon, wie die einzelnen Datensätze letztendlich erstellt werden.



## Strategie und Ausführung synchron

Um Ihre strategische Ebene fokussiert zu halten, empfehlen wir, Ihre Planungsdatensätze auf eine allgemeine Absicht zu konzentrieren, während Sie das Workflow-Modul für die taktische Ausführung verwenden. Dieser Ansatz nutzt die einzigartigen Stärken beider Module:



* **Workfront-Planung (Die strategische Ebene):** Bleibt auf hoher Ebene. Es verfolgt die *Kampagne* die *Channel-*) und das *Budget*. Es ist lärmfrei und für Führungskräfte geeignet.

* **Workflow-Modul (die Ausführungsebene):** Verwaltet die taktischen Details. Einzelne „Erlebnisse“ oder „Aktivitäten“ werden hier als **Projekte, Aufgaben und Probleme“**.



## Aktivieren der Brücke: Von Absicht zu Aktion

Nachdem die Verbindung konfiguriert wurde, müssen Sie entscheiden, wie Sie die Verknüpfung zwischen einem bestimmten strategischen Datensatz und einem Ausführungsprojekt aktivieren.



### Professionelle Triage: Der tabellengeführte Pfad

Strategen und Power-User nutzen oft die **Tabellenansicht** als ihre „Workbench“, um Pläne im Laufe der Zeit zu verfeinern.

* **Absichtliche Übergabe** Standardmäßig wird beim Erstellen eines Datensatzes in einer Tabelle keine Verknüpfung zum Workflow-Modul hergestellt. Die Verbindung zu einem Ausführungsprojekt wird hergestellt, wenn ein Benutzer den Link aktivieren möchte. Dies kann durch manuelles Erstellen eines nachgelagerten verbundenen Projekts direkt über das Verbindungsfeld in WFP oder durch eine optionale **Verbindungsansichtsseite** in der Detailansicht des Datensatzes erfolgen. Beachten Sie, dass die manuelle Erstellung zu einem leeren Projekt ohne spezifische benutzerdefinierte Formulare führt. Für komplexere Anforderungen können Sie eine **native WFP-Automatisierung“**. Diese Automatisierungen sind verfügbar, wenn Sie eine Zeile in einer Tabelle auswählen und als Schaltflächen in der blauen Aktionsleiste am unteren Bildschirmrand angezeigt werden. Dies ermöglicht eine menschliche Aufsicht oder die Erstellung von Platzhaltern und stellt sicher, dass Projekte nur dann in Ihrer Workflow-Umgebung generiert werden, wenn sie wirklich benötigt werden.



### Automatisierte Aktivierung

Für Organisationen mit Anfragen mit hohem Volumen oder erweiterten Automatisierungsanforderungen kann die Brücke automatisch basierend auf bestimmten Ereignissen oder Feldwerten aktiviert werden.

* Trigger **Übermittlungsereignisse:** Da Formulare ein einziges, sauberes „Übermittlungsereignis“ bereitstellen, können sie als Trigger für **Fusion-Automatisierungen“** werden. Ein Szenario kann eine Formularübermittlung erkennen und sofort ein verknüpftes Projekt im Workflow-Modul generieren.

* **Feldwert-Trigger:** Für eine tiefere Automatisierung können Sie **Fusion)** Überwachung bestimmter Felder konfigurieren. Beispielsweise kann ein einfaches Kontrollkästchen mit der Bezeichnung „Bereit zur Ausführung“ als Katalysator dienen, der die Brücke automatisch in dem Moment herstellt, in dem sie aktiviert wird.



## Sichtbarkeit: Suchfelder

Sobald ein Projekt verknüpft ist, können Sie Echtzeitdaten aus dem Workflow-Modul direkt im WFP-Datensatz einblenden.



Ein Workspace-Manager kann **Suchfelder“ einrichten** um jedes native oder benutzerdefinierte Feld aus dem verknüpften Projekt (z. B. *tatsächliches Abschlussdatum* oder *kreativer Lead*) in den WFP-Datensatztyp abzurufen. Nach der Erfassung können diese Daten über mehrere Ebenen Ihrer strategischen Hierarchie hinweg aggregiert werden - sogar bis hin zur Kampagnenebene. Dies bietet ein leistungsstarkes aggregiertes Reporting für Stakeholder über den gesamten Marketing-Lebenszyklus hinweg, sodass sie auf dem Laufenden bleiben, ohne die Planungsumgebung verlassen zu müssen.



## Sichtbarkeit von Strategie zu Aktion

Der ultimative Wert der Brücke ist **Echtzeit-Sichtbarkeit**. Durch die Verknüpfung von Absicht und Aktion können Sie wichtige geschäftliche Fragen auf einen Blick beantworten:



* „Liefert unsere Kampagne &#39;FY26 Brand Awareness&#39; gerade aktiv Ergebnisse?“

* „Wo brauchen wir mehr kreative Unterstützung, um planmäßig zu bleiben? &quot;

* „Wie bringen wir unsere Ressourcen mit unseren vorrangigen strategischen Säulen in Einklang?“



## Best Practices und Tipps



### Führen Sie Folgendes aus:

* **Verwenden Sie die Metapher des „strategischen Threads“.** Erinnere Teams daran, dass jedes Projekt eine „Perle“ auf einer strategischen Zeichenfolge sein sollte.

* **Automatisieren Sie die Übergabe.** Verwenden Sie Automatisierungen, um die Projekterstellung in Triggern zu halten und so Zeit und Aufwand zu sparen und gleichzeitig die Datenkonnektivität und Governance zu verbessern.

* **Link, nicht duplizieren.** Verwenden Sie Suchfelder, um Echtzeitausführungsdaten (wie Status- oder Abschlussdaten) in Ihren strategischen Datensätzen anzuzeigen. Dadurch wird sichergestellt, dass Ihre strategischen Ansichten immer korrekt sind, ohne dass manuelle Aktualisierungen durch Ihr Team erforderlich sind.



### Nicht:

* **Planungs-Datensätze nicht als Aufgabenlisten behandeln.** Die Brücke ist so konzipiert, dass sie strategische Absichten mit Ausführungsprojekten verbindet. Halten Sie Ihre Planungsunterlagen auf das „Was“ und „Warum“ fokussiert und überlassen Sie dem Workflow-Modul das granulare „Wie“ durch Aufgaben und Probleme.

* **Übersynchronisieren Sie nicht.** Sie müssen nicht alle Details auf Projektebene wieder mit der Planung synchronisieren. Halten Sie die strategische Schicht auf hohem Niveau und lärmfrei.

* **Fahr nicht an der Brücke vorbei!** Wenn die Arbeit im Workflow-Modul beginnt, ohne dass ein Link zur Planung vorhanden ist, haben Sie einen „Schattenplan“ erstellt, der für Führungskräfte unsichtbar ist.




