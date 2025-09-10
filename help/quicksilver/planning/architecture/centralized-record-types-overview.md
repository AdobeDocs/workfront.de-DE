---
title: Übersicht über zentralisierte Datensatztypen
description: Zentralisierte Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.
hidefromtoc: true
hide: true
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1019'
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

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

In einem solchen Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während Sie die Team-übergreifende Sichtbarkeit erschließen, ohne dass alles zu einem Arbeitsbereich oder alle Personen in der Organisation zu jedem Arbeitsbereich hinzugefügt werden müssen. Hierfür können Sie zentralisierte Datensatztypen verwenden.

Gehen Sie wie folgt vor, um zentralisierte Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der in einem bestimmten Arbeitsbereich zentralisiert werden soll.

   Ein Workspace-Manager kann Benutzer mit einer Standardlizenz, Teams, Gruppen, Rollen oder Unternehmen auswählen, um einen ausgewählten Datensatztyp zu einem von ihnen verwalteten Arbeitsbereich hinzuzufügen.

   Der ursprüngliche Datensatztyp ist in seinem ursprünglichen Arbeitsbereich vorhanden, wird jedoch von allen anderen Arbeitsbereichen sichtbar gemacht.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Fügen Sie dem Arbeitsbereich eines Teams einen vorhandenen Datensatztyp aus einem vorhandenen Datensatztyp, der als zentralisierter Typ konfiguriert wurde, hinzu.

   Der Datensatztyp ist in den folgenden Arbeitsbereichen vorhanden:

   * Der ursprüngliche Arbeitsbereich, in dem er als zentralisierter Datensatztyp angegeben war.
   * Der Arbeitsbereich des Teams.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   In den folgenden Abschnitten werden Überlegungen zu zentralisierten Datensatztypen entweder in ihren ursprünglichen Arbeitsbereichen oder nach dem Hinzufügen zu den Arbeitsbereichen eines Teams beschrieben.

## Überlegungen zu den zentralisierten Datensatztypen in ihrem ursprünglichen Arbeitsbereich

Der für die Zentralisierung konfigurierte Datensatztyp weist die folgenden Eigenschaften auf:

* Alle zugehörigen Informationen können nur im ursprünglichen Arbeitsbereich bearbeitet werden.

* Sie können die folgenden Aktionen für den zentralisierten Datensatztyp aus dem ursprünglichen Arbeitsbereich eines zentralisierten Datensatztyps ausführen:

   * Bearbeiten

     Die Bearbeitung eines zentralisierten Datensatztyps umfasst die Bearbeitung des Erscheinungsbilds, der arbeitsbereichsübergreifenden Funktionen und aller im ursprünglichen Arbeitsbereich erstellten Felder.
   * Anfrageformulare erstellen
   * Anfrageformulare verwalten

* Ein zentralisierter Datensatztyp kann nur gelöscht werden, wenn er nicht zu einem Team-Arbeitsbereich hinzugefügt wurde. Nachdem er zum Arbeitsbereich eines Teams hinzugefügt wurde, führt der Versuch, ihn aus dem ursprünglichen Arbeitsbereich zu löschen, zu einem Fehler.

  Dies geschieht, damit der zentralisierte Datensatztyp in den Arbeitsbereichen verbleiben kann, in denen er bereits hinzugefügt wurde.
* Die Datensätze, die Sie einem zentralen Datensatztyp hinzufügen, sind nur für Benutzer sichtbar, die über Anzeigeberechtigungen für den ursprünglichen Arbeitsbereich verfügen.
* Die Datensätze, die Sie aus dem Arbeitsbereich des Teams hinzufügen, werden aggregiert und im ursprünglichen Arbeitsbereich angezeigt. Alle Mitglieder des ursprünglichen Arbeitsbereichs erhalten Ansichtsberechtigungen für ihn.

* Die verbundenen Datensatztypen eines zentralisierten Datensatztyps werden für die Verbindung in den Arbeitsbereichen verfügbar, in denen dieser Datensatztyp hinzugefügt wird.

* Felder, die für einen zentralen Datensatztyp aus dem ursprünglichen Arbeitsbereich erstellt wurden, sind in allen Arbeitsbereichen sichtbar, in denen der Datensatztyp hinzugefügt wird.

## Überlegungen zu zentralisierten Datensatztypen nach dem Hinzufügen zum Arbeitsbereich eines Teams

* Teamarbeitsbereich-Mitwirkende erhalten die Berechtigung Beitragen für den zentralisierten Datensatztyp im Teamarbeitsbereich. Sie können Datensätze darin hinzufügen und verwalten.

* Team Workspace-Betrachter erhalten die Berechtigung zum Anzeigen des zentralisierten Datensatztyps in Team Workspace. Es können keine Datensätze hinzugefügt und darin verwaltet werden.

* Team Workspace-Manager können die folgenden Aktionen für den Datensatztyp ausführen, der aus einem zentralisierten Datensatztyp im Arbeitsbereich eines Teams hinzugefügt wurde:

   * Neue Felder hinzufügen

     Felder, die einem zentralen Datensatz aus einem Team-Arbeitsbereich hinzugefügt werden, sind nur aus dem Arbeitsbereich des Teams sichtbar.
   * Freigeben
   * Löschen.

     Wenn Sie den Datensatztyp aus dem Arbeitsbereich eines Teams löschen, wird er nur aus dem Arbeitsbereich des Teams entfernt. Die Datensätze, die ihm aus dem Arbeitsbereich des Teams hinzugefügt wurden, werden ebenfalls gelöscht. Dadurch wird der Datensatztyp nicht aus seinem ursprünglichen Arbeitsbereich oder aus anderen Team-Arbeitsbereichen gelöscht, in denen er hinzugefügt wurde.

     Dies geschieht, damit es möglich ist, den bereits hinzugefügten zentralisierten Datensatztyp in Arbeitsbereichen, die ihn bereits verwenden, beizubehalten.

* Sie können die folgenden Aktionen nicht für den Datensatztyp ausführen, der aus einem zentralisierten Datensatztyp im Arbeitsbereich eines Teams hinzugefügt wurde:

   * Bearbeiten

     Sie können weder sein Erscheinungsbild noch seine Workspace-übergreifenden Funktionen oder die Felder bearbeiten, die aus dem ursprünglichen Workspace hinzugefügt wurden.
   * Anfrageformulare erstellen
   * Anfrageformulare verwalten

* In den Arbeitsbereichen eines Teams hinzugefügte Datensätze sind in den folgenden Arbeitsbereichen sichtbar, wenn Sie über Ansichts- oder höhere Berechtigungen für diese Arbeitsbereiche verfügen:

   * Der Arbeitsbereich des Teams, in dem sie hinzugefügt werden.
   * Der ursprüngliche Arbeitsbereich des zentralisierten Datensatztyps.
   * Alle anderen Arbeitsbereiche, bei denen der zentrale Arbeitsbereich hinzugefügt wird.

* Die folgenden Szenarien existieren für Datensätze, die in den Arbeitsbereichen der Teams erstellt wurden:

   * Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Arbeitsbereich und keine Berechtigungen für die Arbeitsbereiche der Teams verfügen, können Sie Datensätze anzeigen, die aus den Arbeitsbereichen des Teams im ursprünglichen Arbeitsbereich hinzugefügt wurden, Sie können sie jedoch nicht über den ursprünglichen Arbeitsbereich verwalten.
   * Wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich des Teams verfügen, können Sie die Datensätze im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps oder in dem Arbeitsbereich verwalten, in dem sie hinzugefügt wurden.

     Sie können die Datensätze in zusätzlichen Team-Arbeitsbereichen anzeigen, in denen der zentralisierte Datensatztyp nur hinzugefügt wird, wenn Sie über Anzeigeberechtigungen für diese Arbeitsbereiche verfügen.

## Zugriff auf Verbindungen

Datensatztypen, die mit dem zentralisierten Datensatztyp im ursprünglichen Arbeitsbereich verbunden sind, werden für Team-Arbeitsbereiche sichtbar, in denen der zentralisierte Datensatztyp hinzugefügt wird.

## API-Verhalten

Beim Hinzufügen von Datensätzen zu einem zentralisierten Datensatztyp aus einem Team-Arbeitsbereich mithilfe der Workfront Planning-API prüft das System, ob die Benutzenden Zugriff haben, um Datensätze im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps zu erstellen.

Die folgenden Fälle liegen vor:

* Wenn der/die Benutzende Zugriff hat, wird der Datensatz im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps erstellt.

* Wenn der/die Benutzende keinen Zugriff hat, erhält der/die Benutzende die Fehlermeldung, dass er/sie keinen Zugriff auf den ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps hat und er/sie die Arbeitsbereich-ID angeben muss, unter der er/sie Zugriff zum Erstellen von Datensätzen hat.