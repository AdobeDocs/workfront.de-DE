---
title: Übersicht über arbeitsbereichsübergreifende Datensatztypen
description: Zentralisierte Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.
hidefromtoc: true
hide: true
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '1356'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Übersicht über arbeitsbereichsübergreifende Datensatztypen

In Adobe Workfront Planning können Sie Workspace-übergreifende Funktionen für einen Datensatztyp aktivieren, mit dem Sie auf einen Datensatztyp in mehr als einem Workspace verweisen können.

Im Folgenden finden Sie arbeitsbereichsübergreifende Funktionen von Datensatztypen:

* Sie können einen Datensatztyp als zentralisiert festlegen. Benutzer können zentralisierte Datensatztypen zu anderen Arbeitsbereichen hinzufügen, die sie verwalten können.

  >[!IMPORTANT]
  >
  >Sie müssen über ein Workfront Planning Plus-Paket zusätzlich zu einem Workfront-Paket verfügen, um zentralisierte Datensatztypen verwenden zu können.
  >
  >Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront Account Manager.

* Sie können einen Datensatztyp als „verbindbar“ festlegen. Benutzer können von anderen Arbeitsbereichen aus eine Verbindung zu diesem Datensatztyp herstellen.

In diesem Artikel erhalten Sie einen Überblick über arbeitsbereichsübergreifende Datensatztypen. Informationen zum Definieren der arbeitsbereichsübergreifenden Funktionen eines Datensatztyps finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Übersicht über zentralisierte Datensatztypen

Zentralisierte Datensatztypen können in Adobe Workfront Planning über einen zentralen oder primären Arbeitsbereich zu mehreren Arbeitsbereichen hinzugefügt werden.

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

In einem solchen Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während Sie die Team-übergreifende Sichtbarkeit erschließen, ohne dass alles zu einem Arbeitsbereich oder alle Personen in der Organisation zu jedem Arbeitsbereich hinzugefügt werden müssen. Hierfür können Sie zentralisierte Datensatztypen verwenden.

Gehen Sie wie folgt vor, um zentralisierte Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der in einem bestimmten Arbeitsbereich zentralisiert werden soll.

   Ein Workspace-Manager kann Benutzer mit einer Standardlizenz, Teams, Gruppen, Rollen oder Unternehmen auswählen, um einen ausgewählten Datensatztyp zu einem von ihnen verwalteten Arbeitsbereich hinzuzufügen.

   Der ursprüngliche Datensatztyp ist in seinem ursprünglichen Arbeitsbereich vorhanden, wird jedoch von allen anderen Arbeitsbereichen sichtbar gemacht.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Hinzufügen eines Datensatztyps aus einem vorhandenen, der als zentralisierter Datensatztyp konfiguriert wurde, zu einem sekundären Arbeitsbereich.

   Der Datensatztyp ist in den folgenden Arbeitsbereichen vorhanden:

   * Der ursprüngliche Arbeitsbereich, in dem er als zentralisierter Datensatztyp angegeben war.
   * Ein sekundärer Arbeitsbereich.

   Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   In den folgenden Abschnitten werden Überlegungen zu zentralisierten Datensatztypen und deren Funktionsweise in ihren ursprünglichen oder sekundären Arbeitsbereichen beschrieben.

### Überlegungen zu den zentralisierten Datensatztypen in ihrem ursprünglichen Arbeitsbereich

Der für die Zentralisierung konfigurierte Datensatztyp weist die folgenden Eigenschaften auf:

* Alle zugehörigen Informationen können nur im ursprünglichen Arbeitsbereich bearbeitet werden.

* Sie können die folgenden Aktionen für den zentralisierten Datensatztyp aus dem ursprünglichen Arbeitsbereich eines zentralisierten Datensatztyps ausführen:

   * Bearbeiten

     Die Bearbeitung eines zentralisierten Datensatztyps umfasst die Bearbeitung des Erscheinungsbilds, der arbeitsbereichsübergreifenden Funktionen und aller im ursprünglichen Arbeitsbereich erstellten Felder.
   * Anfrageformulare erstellen
   * Anfrageformulare verwalten

* Ein zentralisierter Datensatztyp kann nur gelöscht werden, wenn er nicht zu einem sekundären Arbeitsbereich hinzugefügt wurde. Nachdem er einem anderen Arbeitsbereich hinzugefügt wurde, führt der Versuch, ihn aus dem ursprünglichen Arbeitsbereich zu löschen, zu einem Fehler.

  Dies geschieht, damit der zentralisierte Datensatztyp in den Arbeitsbereichen verbleiben kann, in denen er bereits hinzugefügt wurde.
* Die Datensätze, die Sie einem zentralen Datensatztyp hinzufügen, sind nur für Benutzer sichtbar, die über Anzeigeberechtigungen für den Arbeitsbereich verfügen, in dem sie hinzugefügt wurden.
* Die Datensätze, die Sie aus einem sekundären Arbeitsbereich hinzufügen, werden aggregiert und im ursprünglichen Arbeitsbereich angezeigt. Alle Mitglieder des ursprünglichen Arbeitsbereichs erhalten Ansichtsberechtigungen für ihn.

* Die verbundenen Datensatztypen eines zentralisierten Datensatztyps werden für die Verbindung in den Arbeitsbereichen verfügbar, in denen dieser Datensatztyp hinzugefügt wird.

  Wenn Sie beispielsweise einen Kampagnen-Datensatztyp haben, der eine Verbindung mit dem Datensatztyp Regionen aufweist, und Sie den Kampagnen-Datensatztyp einem sekundären Arbeitsbereich hinzufügen, werden Regionen für den sekundären Arbeitsbereich arbeitsbereichsübergreifend verbindbar. Die Mitglieder des sekundären Arbeitsbereichs können jetzt Kampagnen erstellen und sie mit Regionen verknüpfen.

* Felder, die für einen zentralen Datensatztyp aus dem ursprünglichen Arbeitsbereich erstellt wurden, sind in allen Arbeitsbereichen sichtbar, in denen der Datensatztyp hinzugefügt wird. Felder aus einem ursprünglichen Arbeitsbereich sind in den sekundären Arbeitsbereichen schreibgeschützt.

### Überlegungen zu zentralisierten Datensatztypen nach dem Hinzufügen zu einem sekundären Arbeitsbereich

* Sekundäre Arbeitsbereich-Mitwirkende erhalten die Berechtigung Beitragen für den zentralisierten Datensatztyp im Arbeitsbereich ihres Teams. Sie können Datensätze darin hinzufügen und verwalten.

* Sekundäre Arbeitsbereich-Betrachter erhalten die Berechtigung zum Anzeigen des zentralisierten Datensatztyps im Arbeitsbereich ihres Teams. Es können keine Datensätze hinzugefügt und darin verwaltet werden.

* Sekundär Workspace-Manager können die folgenden Aktionen für den Datensatztyp ausführen, der aus einem zentralisierten Datensatztyp in einem sekundären Workspace hinzugefügt wurde:

   * Löschen.

     Wenn Sie den Datensatztyp aus einem sekundären Arbeitsbereich löschen, wird er nur aus dem sekundären Arbeitsbereich entfernt. Die Datensätze, die ihm aus dem sekundären Arbeitsbereich hinzugefügt wurden, werden ebenfalls gelöscht. Dadurch wird der Datensatztyp nicht aus seinem ursprünglichen Arbeitsbereich oder aus anderen sekundären Arbeitsbereichen, in denen er hinzugefügt wurde, gelöscht.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Die folgenden Aktionen können nicht für den Datensatztyp ausgeführt werden, der aus einem zentralisierten Datensatztyp in einem sekundären Arbeitsbereich hinzugefügt wurde:

   * Bearbeiten

     Sie können weder sein Erscheinungsbild noch seine Workspace-übergreifenden Funktionen oder die Felder bearbeiten, die aus dem ursprünglichen Workspace hinzugefügt wurden.
   * Anfrageformulare erstellen und verwalten
   * Erstellen und Verwalten von Anfrageformularen

* In sekundären Arbeitsbereichen hinzugefügte Datensätze sind in den folgenden Arbeitsbereichen sichtbar, wenn Sie über Anzeigen- oder höhere Berechtigungen für diese Arbeitsbereiche verfügen:

   * Der sekundäre Arbeitsbereich, in dem sie hinzugefügt werden.
   * Der ursprüngliche Arbeitsbereich des zentralisierten Datensatztyps.
   * Alle anderen Arbeitsbereiche, bei denen der zentrale Arbeitsbereich hinzugefügt wird.

* Die folgenden Szenarien existieren für Datensätze, die in den Arbeitsbereichen der Teams erstellt wurden:

   * Wenn Sie über Verwaltungsberechtigungen für den ursprünglichen Arbeitsbereich und keine Berechtigungen für sekundäre Arbeitsbereiche verfügen, können Sie Datensätze anzeigen, die von den sekundären Arbeitsbereichen im ursprünglichen Arbeitsbereich hinzugefügt wurden. Sie können diese jedoch nicht über den ursprünglichen Arbeitsbereich verwalten.
   * Wenn Sie über Verwaltungsberechtigungen für den sekundären Arbeitsbereich verfügen, können Sie die Datensätze im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps oder in dem Arbeitsbereich verwalten, in dem sie hinzugefügt wurden.

     Sie können die Datensätze in zusätzlichen sekundären Arbeitsbereichen anzeigen, in denen der zentralisierte Datensatztyp nur hinzugefügt wird, wenn Sie über Anzeigeberechtigungen für diese Arbeitsbereiche verfügen.

### Zugriff auf die Verbindungen eines zentralisierten Datensatztyps

Datensatztypen, die mit dem zentralisierten Datensatztyp im ursprünglichen Arbeitsbereich verbunden sind, werden von anderen Arbeitsbereichen sichtbar, in denen der zentralisierte Datensatztyp hinzugefügt wird.

### API-Zugriff eines zentralisierten Datensatztyps

Beim Hinzufügen von Datensätzen zu einem zentralisierten Datensatztyp aus einem sekundären Arbeitsbereich mithilfe der Workfront Planning-API prüft das System, ob die Benutzenden Zugriff haben, um Datensätze im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps zu erstellen.

Die folgenden Fälle liegen vor:

* Wenn der/die Benutzende Zugriff hat, wird der Datensatz im ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps erstellt.

* Wenn der/die Benutzende keinen Zugriff hat, erhält der/die Benutzende die Fehlermeldung, dass er/sie keinen Zugriff auf den ursprünglichen Arbeitsbereich des zentralisierten Datensatztyps hat und er/sie die Arbeitsbereich-ID angeben muss, unter der er/sie Zugriff zum Erstellen von Datensätzen hat.

## Übersicht über verbindbare Datensatztypen

Sie können eine Verbindung zu einem Datensatztyp herstellen, der als von jedem von Ihnen verwalteten Arbeitsbereich aus verbindbar definiert wurde.

Möglicherweise müssen Ihre Teams ihre Datensätze mit Datensatztypen aus anderen Arbeitsbereichen verknüpfen oder Informationen anzeigen, die in Datensätzen erfasst wurden, die zu Datensätzen in anderen Arbeitsbereichen gehören. Sie können diese Konfiguration erreichen, indem Sie einen Datensatztyp als „verbindbar“ festlegen.

Gehen Sie wie folgt vor, um verbindbare Datensatztypen zu verwenden:

1. Konfigurieren Sie einen Datensatztyp, der in einem bestimmten Arbeitsbereich verbunden werden kann.

   Ein Workspace-Manager kann auswählen, mit welchen Arbeitsbereichen ein bestimmter Datensatztyp verbunden werden kann.

   Der ursprüngliche Datensatztyp ist in seinem ursprünglichen Arbeitsbereich vorhanden und wird als verbundener Datensatztyp zu einem anderen Arbeitsbereich hinzugefügt.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Stellen Sie eine Verbindung zu einem Datensatztyp her, der als von einem anderen von Ihnen verwalteten Arbeitsbereich aus verbindbar gekennzeichnet ist.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

   In den folgenden Abschnitten werden Überlegungen zu zentralisierten Datensatztypen und deren Funktionsweise in ihren ursprünglichen oder sekundären Arbeitsbereichen beschrieben.