---
title: Übersicht über zentralisierte Datensatztypen
description: Zentralisierte Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.
hidefromtoc: true
hide: true
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Übersicht über zentralisierte Datensatztypen


Zentralisierte Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.

## Übersicht über zentralisierte Datensatztypen

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um auf eine zentrale, globalere Ebene zu gelangen.

Mit diesem Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während sie gleichzeitig eine Team-übergreifende Sichtbarkeit ermöglichen, ohne dass alle Personen in der Organisation zu einem Arbeitsbereich hinzugefügt werden müssen.

Gehen Sie wie folgt vor, um zentralisierte Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der zentralisiert werden soll.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Einen vorhandenen Datensatztyp aus einem zentralisierten hinzufügen.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).




・ Die neue Einstellung „Zulassen, dass der Datensatztyp in anderen Arbeitsbereichen hinzugefügt wird“ ist in den erweiterten Einstellungen für Datensatztypen verfügbar.

・ Wenn diese Option aktiviert ist, kann der Workspace-Manager Benutzer mit Standardlizenz, Teams, Gruppen, Rollen oder Unternehmen auswählen, die den Datensatztyp in den von ihnen verwalteten Workspaces hinzufügen können.

・ Der Workspace-Manager, der die Einstellung bearbeitet, wird standardmäßig automatisch zur Liste der ausgewählten Benutzer hinzugefügt

o Der Workspace-Manager kann seinen eigenen Namen entfernen, nachdem er mindestens 1 andere Entität hinzugefügt hat

o Es muss mindestens 1 Benutzer/Team/… ausgewählt sein, um die Einstellung zu speichern

o Sobald der Datensatztyp in mindestens 1 anderen Arbeitsbereich hinzugefügt wurde, können alle ausgewählten Benutzer entfernt werden

§ Dies geschieht, damit verhindert werden kann, dass der globale Datensatztyp in neuen Arbeitsbereichen hinzugefügt wird, während er in Arbeitsbereichen beibehalten wird, in denen er bereits verwendet wird.

・ In Phase 1 werden alle Datensätze der verbundenen Datensatztypen automatisch für alle Arbeitsbereiche freigegeben, in denen der Datensatztyp hinzugefügt wurde.

・ Sobald der Datensatztyp als arbeitsbereichsübergreifend aktiviert ist, wird dem Datensatztyp ein systemgeneriertes &quot;Workspace&quot;-Feld hinzugefügt

So wird der Arbeitsbereich angezeigt, aus dem jeder Datensatz erstellt wurde.

o Dieses Feld ist schreibgeschützt und kann nicht gelöscht werden.

So kann es aus den Ansichtsfeldern ausgeblendet werden.

o Das Arbeitsbereich -Feld kann zum Filtern, Gruppieren und Sortieren sowie in allen Anzeigeeinstellungen wie anderen Feldern verwendet werden.


Workspace-übergreifende Datensatztypen in lokalen Arbeitsbereichen

・ Beim Versuch, einen neuen Datensatztyp zu ihrem Arbeitsbereich hinzuzufügen, sehen lokale Arbeitsbereich-Manager eine Option, um aus der Liste der globalen Datensatztypen auszuwählen, die für sie verfügbar sind

・ Wenn ein globaler Datensatztyp ausgewählt wird, wird er sofort zum Arbeitsbereich hinzugefügt

・ Es ist möglich, den globalen Datensatztyp in einen beliebigen Bereich und an eine beliebige Position im lokalen Arbeitsbereich zu verschieben


Berechtigungen für den globalen Datensatztyp in lokalen Arbeitsbereichen

In lokalen Arbeitsbereichen erhalten die Mitglieder folgenden Zugriff auf den globalen Datensatztyp:

・ In Phase 1 erhalten lokale Workspace-Manager die Berechtigung Beitragen . Dies bedeutet:

So können lokale Arbeitsbereichsmanager:

§ Globalen Datensatztyp hinzufügen

§ Hinzufügen/Bearbeiten/Löschen von Datensätzen im globalen Datensatztyp, unabhängig davon, aus welchem Arbeitsbereich der Datensatz hinzugefügt wurde.

§ Löschen des globalen Datensatztyps aus dem lokalen Arbeitsbereich

o Lokale Workspace-Manager können:

§ Hinzufügen, Bearbeiten und Löschen von Feldern

§ Aktualisieren des Erscheinungsbilds und der Kennzeichnung des Datensatztyps

§ Siehe die erweiterten Einstellungen für den Datensatztyp

§ Automatisierungen verwalten

§ Anfrageformulare verwalten

§ Anpassen der Freigabe des Datensatztyps für den Umfang des Arbeitsbereichs

§ Deaktivieren Sie in den erweiterten Einstellungen die Einstellung Globaler Datensatztyp .

・ Mitwirkende am lokalen Arbeitsbereich erhalten die Berechtigung Beitragen zum globalen Datensatztyp und können darin Datensätze hinzufügen und verwalten

・ Lokale Workspace-Viewer erhalten die Berechtigung zum Anzeigen des globalen Datensatztyps

・ Sobald ein Datensatz zum globalen Datensatztyp aus einem der lokalen Arbeitsbereiche hinzugefügt wird, wird dieser Arbeitsbereichsname im Workspace-Feld angezeigt

o Im Moment ist es nicht möglich, das Feld Arbeitsbereich zu bearbeiten oder zu ändern

・ Datensätze, die zu lokalen Arbeitsbereichen hinzugefügt werden, werden aggregiert und im primären Arbeitsbereich angezeigt, und alle Mitglieder des primären Arbeitsbereichs erhalten Ansichtszugriff darauf.

・ In lokalen Arbeitsbereichen hinzugefügte Datensätze werden in anderen lokalen Arbeitsbereichen mit demselben globalen Datensatztyp nicht angezeigt und ihre Mitglieder erhalten keinen Zugriff auf die Datensätze.



Zugriff auf Verbindungen:

・ MVP-Umfang

o Die mit dem globalen Datensatztyp verbundenen Datensatztypen werden für lokale Arbeitsbereiche sichtbar, in denen der globale Datensatztyp hinzugefügt wird, damit sie die Verbindungsfelder zum Taggen verwenden können


API-Verhalten

Wenn Benutzende versuchen, über die API Datensätze in einem globalen Datensatztyp zu erstellen, ohne die Workspace-ID anzugeben, prüft das System, ob die Benutzenden Zugriff haben, um Datensätze im primären Arbeitsbereich zu erstellen (wo der globale Datensatztyp erstellt wird)

・ Wenn ja, wird der Datensatz im primären Arbeitsbereich erstellt

・ Wenn nicht, erhält der Benutzer einen Validierungsfehler, dass er keinen Zugriff auf den primären Arbeitsbereich hat und die Arbeitsbereich-ID angeben muss, in der er Zugriff zum Erstellen hat.